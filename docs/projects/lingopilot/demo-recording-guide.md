# LingoPilot — Demo Recording Guide

**Purpose:** Record a 60–90 second screen capture showing the full end-to-end LingoPilot flow, then export it as a GIF for embedding in both GitHub READMEs.  
**Target format:** GIF, ≤10 MB, 1280×800  
**Tool (recommended):** [Kap](https://getkap.co) (free, Mac-native, exports GIF directly)

---

## The Story to Tell in 60 Seconds

```
Engineer edits a locale file
    → git push
        → Bot receives webhook (Railway)
            → Run appears in dashboard (live)
                → PR opens on GitHub with Puppeteer screenshots
```

That's it. Everything else in the recording is context for that arc.

---

## Before You Hit Record — Setup Checklist

### 1. Prepare your screen layout

Tile 4 windows so all four are visible simultaneously (or use a 2-screen layout):

| Window | What to show |
|---|---|
| **Editor** | `next-i18next-sample/public/locales/en/home.json` open, cursor on a line ready to edit |
| **Terminal** | In the `next-i18next-sample` repo directory, ready to run `git commit && git push` |
| **Dashboard tab** | `localhost:3000` (or `lingopilot.app`) — logged in, project card visible |
| **GitHub tab** | `github.com/heyitschien/next-i18next-sample/pulls` — PRs list, ready to refresh |

> **Tip:** Use Mission Control or a window manager like Magnet to snap windows into quadrants for a clean screen layout.

### 2. Clean up state before recording

- [ ] Dashboard shows the project card (`heyitschien/next-i18next-sample`) and existing run history
- [ ] Close or merge any old open PRs on the demo repo so a fresh PR will be PR #N+1
- [ ] Railway logs for `lingopilot-bot` are tailing live (open in browser or Railway dashboard)
- [ ] `lingopilot-worker` is healthy on Railway (check Railway dashboard)
- [ ] You are logged into `lingopilot.app` (or localhost:3000) — no auth prompts mid-recording

### 3. Prepare your edit

Open `public/locales/en/home.json` in `next-i18next-sample`. Pick a simple, visible string — for example:

```json
// Before
"hero": "Welcome to our store"

// After (what you'll change during the recording)
"hero": "Welcome back to our store"
```

Have it ready to type — you don't want to be hunting for the right line mid-recording.

---

## Recording Script — Shot by Shot

| Timestamp | Action | What It Demonstrates |
|---|---|---|
| **0:00 – 0:05** | Show the LingoPilot dashboard. Pan to show: "GitHub connected ✓ — 74 installations active", the project card for `heyitschien/next-i18next-sample`, and the runs table below. | The system is live and connected to GitHub. |
| **0:05 – 0:12** | Switch to your editor. Show the file `public/locales/en/home.json`. Make a small change to one string value. Save. | The trigger: a real engineer editing real copy. |
| **0:12 – 0:20** | Switch to terminal. Run: `git add . && git commit -m "update hero copy" && git push` | One push. That's the entire human action required. |
| **0:20 – 0:28** | Switch to Railway bot logs (or the Railway dashboard). Show the log line confirming the webhook was received and the job was enqueued to Upstash Redis. | The GitHub App received the event. The pipeline is running. |
| **0:28 – 0:45** | Switch back to the LingoPilot dashboard. Wait. Within 10 seconds a new row appears in "All runs" — first as `running`, then transitions to `Succeeded`. The PR number column populates. | Live update. No page refresh. The pipeline ran automatically. |
| **0:45 – 1:00** | Click the PR link (#N). GitHub PR opens — show the PR title, the list of changed files (`public/locales/zz-pseudo/`), and the embedded Puppeteer screenshots of each route. | The deliverable: a visual PR a team can review before merging. |
| **1:00 – 1:10** (optional) | Pan back to the dashboard "Runs" view. Show the full run history — multiple entries, timestamps, branches, durations. | Repeatability and run history. |

---

## Screen Recording Tool Options

### Option A — Kap (Recommended, free)

1. Download from [getkap.co](https://getkap.co)
2. Open Kap → drag the crop handles to cover your 4-window layout (or go full screen)
3. Set FPS to **10** in Kap preferences (adequate for a demo, keeps file size down)
4. Click record
5. After stopping: Kap shows the export panel → select **GIF** → set quality to **Medium** → click Export
6. Done — Kap outputs a `.gif` directly

> Kap can also trim the clip before export. Cut any dead time where the worker is running (the ~25 second processing window) down to 5–10 seconds to keep the GIF under 10 MB.

### Option B — OBS + FFmpeg (more control, higher quality)

**Record with OBS:**
1. Install OBS ([obsproject.com](https://obsproject.com)) — free
2. Add a "Display Capture" or "Window Capture" source for each window
3. Record to `.mp4` (H.264)

**Convert to GIF with FFmpeg:**
```bash
brew install ffmpeg gifsicle

# Step 1: Convert to GIF (scale to 1280px wide, 10 fps)
ffmpeg -i demo.mp4 \
  -vf "fps=10,scale=1280:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" \
  demo-raw.gif

# Step 2: Optimize file size (critical — keep under 10 MB for GitHub README)
gifsicle --optimize=3 --lossy=80 --colors 256 demo-raw.gif -o demo.gif

# Check the output file size
du -sh demo.gif
```

> The two-pass `palettegen`/`paletteuse` approach produces much better color quality than a basic FFmpeg GIF conversion.

**Trimming with FFmpeg (if needed):**
```bash
# -ss = start time, -t = duration (in seconds)
ffmpeg -ss 00:00:02 -t 00:01:05 -i demo.mp4 -c copy demo-trimmed.mp4
```

### Option B — QuickTime + Gifox

1. Open QuickTime → File → New Screen Recording → select crop area → record
2. Save as `.mov`
3. Open in [Gifox](https://gifox.io) (paid, ~$15) → drag `.mov` in → export as GIF
4. Gifox handles compression automatically

---

## File Size Targets

| Length | Target size | Notes |
|---|---|---|
| Under 30s | < 3 MB | Easy to achieve at 10fps/1280px |
| 30–60s | 3–7 MB | Trim aggressively; reduce to 8fps if needed |
| 60–90s | 7–10 MB | Upper limit for GitHub README inline display |

> GitHub READMEs will display GIFs inline up to ~10 MB. Above that they render as a broken link. Always check `du -sh demo.gif` before committing.

---

## Where to Save and Embed

### Save the GIF

```
lingopilot-dashboard/
  docs/
    assets/
      demo.gif        ← commit here
```

```bash
# From lingopilot-dashboard root:
mkdir -p docs/assets
cp ~/path/to/demo.gif docs/assets/demo.gif
git add docs/assets/demo.gif
git commit -m "docs: add demo GIF for README"
git push
```

### Embed in dashboard README

Place immediately after the one-line value proposition — above the fold:

```markdown
# LingoPilot

> Autonomous localization QA pipeline — push English copy, get a visual PR.

![LingoPilot end-to-end demo](docs/assets/demo.gif)

**Live demo:** [lingopilot.app](https://www.lingopilot.app) · **Engine:** [lingopilot-engine](https://github.com/heyitschien/lingopilot-phrase0)
```

### Embed in engine README

Reference the same GIF via the dashboard repo's raw GitHub URL (no need to commit twice):

```markdown
![LingoPilot demo](https://github.com/heyitschien/lingopilot-dashboard/raw/main/docs/assets/demo.gif)
```

---

## Optional Polish — Recording Tips

- **Slow your mouse movements.** Fast cursor motion creates visual noise in GIFs.
- **Use a dark terminal theme.** High contrast reads better when compressed to GIF colors.
- **Hide your bookmarks bar** (View → Always Show Bookmarks Bar → off) for a cleaner browser look.
- **Turn off notifications.** Cmd+Option+Do Not Disturb, or switch to a dedicated macOS user account.
- **Zoom the browser to 90%** if the dashboard layout looks too dense at 1280px.
- **Use the deployed app** (`lingopilot.app`) rather than localhost if possible — shows the real deployment, not a dev server.

---

## After Recording — Reference Checklist

- [ ] GIF exported and under 10 MB
- [ ] GIF committed to `lingopilot-dashboard/docs/assets/demo.gif`
- [ ] Dashboard README updated: GIF embedded above the fold
- [ ] Engine README updated: links to dashboard GIF via raw GitHub URL
- [ ] Both READMEs pushed to main

---

*Part of the LingoPilot job readiness sprint. See [`job-readiness-analysis.md`](./job-readiness-analysis.md) for the full execution order.*
