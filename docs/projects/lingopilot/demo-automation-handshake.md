# LingoPilot Demo Execution Plan (Human + Agent Handshake)

This plan outlines the division of labor for our next session to successfully record, optimize, and embed the LingoPilot demo GIF without running into authentication blockers.

## Phase 1: Environment Prep (Agent)
*When you are ready, you will tell me to "Act on Phase 1".*
1. **Repository Check**: I will ensure `next-i18next-sample` is on a clean branch (e.g., `demo-run`).
2. **Setup Verification**: I will check that `lingopilot-dashboard` and `lingopilot-engine` are up to date and ready to receive the README updates.

## Phase 2: The Live Recording (User)
*This is the manual step to bypass the GitHub 2FA/Auth limitations.*
1. **Tile Your Windows**: Arrange your screen into 4 quadrants as per the recording guide (Editor, Terminal, LingoPilot Dashboard, GitHub PRs).
2. **Record**: Start recording with **Kap** (or QuickTime/OBS).
3. **Action**: 
   - Make a small text change in `public/locales/en/home.json`.
   - Run `git commit -am "update copy" && git push`.
   - Watch the Dashboard update live.
   - Click the newly created PR on GitHub to show the visual screenshots.
4. **Save**: Save the raw recording (e.g., `demo-raw.mp4` or `demo-raw.mov`) into your `lingopilot-dashboard/docs/assets/` folder.

## Phase 3: Post-Processing & Integration (Agent)
*Once you've saved the raw recording, tell me to "Act on Phase 3".*
1. **Optimization**: I will run the multi-pass `ffmpeg` and `gifsicle` commands locally on your machine to convert your raw video into a highly optimized, `<10MB` GIF.
2. **README Integration**: I will embed the final `demo.gif` above the fold in both the `lingopilot-dashboard` and `lingopilot-engine` README files.
3. **Checklist Update**: I will mark the Recruiter Readiness checklists as fully complete, crossing off the final demo requirements.

---
**Next Steps:**
When we resume this in our next session, simply reference this plan or ask me to **"Start Phase 1"** and make sure you have your screen recording tool ready!
