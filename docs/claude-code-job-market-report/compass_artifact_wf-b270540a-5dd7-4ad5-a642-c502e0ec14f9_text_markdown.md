# Agentic-AI frontend job market and portfolio playbook, April 2026

**You are entering a market that has re-organized itself around your exact profile in the last 18 months.** Roughly 90+ publicly live job listings surveyed across 14 boards explicitly require both an agentic AI coding tool (Cursor, Claude Code, Codex, GitHub Copilot, Windsurf, v0, Bolt, Lovable, Replit Agent) *and* a React/Next.js/TypeScript/Tailwind stack — the two halves of your resume. Entry-level paths are real but narrow: of the listings surveyed, roughly **10–12 are genuinely open to 0–2 YOE candidates** who can substitute a shipped portfolio for tenure. The highest-density hunting grounds are the niche vibe-coding boards (**goodvibecode.com**, **remotevibecodingjobs.com**, **vibecoding.work**) plus **YC Work at a Startup** and the **Hacker News "Who is hiring"** monthly thread. Your Meta Frontend certificate is a credibility signal at best; shipped, deployed, AI-native projects will carry 10× its weight with the companies that matter. Three specific new builds — a RAG SaaS, a custom MCP server, and an "AI digital twin" portfolio site — will move you from "one of many AI-curious juniors" to "rare AI-native product engineer" inside 6–8 weeks of focused work.

The rest of this report is organized as: market structure and tool frequencies, a curated table of tier-1 target listings, board-by-board recommendations, the mindset/language decoder that will tune your resume, the disqualifier list, a full portfolio criteria document, and three build specs.

## What the 90+ listings actually say

The market has consolidated around a remarkably narrow toolchain. **Cursor is mentioned by name in roughly 63% of qualifying listings**, **Claude Code in 46%**, and **GitHub Copilot in 43%**. Windsurf, Codex, v0, Bolt, and Lovable each appear in 10–17%, while Replit Agent, Aider, and Cline show up sporadically. An important second-order signal is emerging: **Model Context Protocol (MCP) awareness** now appears in JDs from Life360, Modern Amenities, Mercedes-Benz Tech, Knack, and Lumimeds — often phrased as "integrates MCP servers" or "builds agentic workflows," which is table-stakes for the 2026 cohort but almost absent from the 2024 cohort.

On the frontend side, the "new LAMP stack" is effectively one thing: **Next.js App Router + TypeScript + Tailwind + shadcn/ui + Supabase-or-Neon + Drizzle-or-Prisma + Vercel deploy + Vercel AI SDK**. You already use every component of this stack. React appears in 30+ of 35 listings surveyed on major boards, TypeScript in 22, Next.js in 18, Tailwind in 14, Node.js in 12, and Supabase explicitly in at least 8 across all boards. shadcn/ui is the fastest-rising component library mention.

The pattern across boards diverges by seniority: **YC and AI-native company pages (Vercel, Anthropic, Anysphere/Cursor, Supabase, Replit, Lovable) skew senior and staff+**, with bars of 3–5+ years dominant, while **niche vibe-coding boards and HN "Who is hiring"** contain the majority of genuinely entry-friendly roles. General boards (Indeed, LinkedIn, ZipRecruiter) sit in between but are heavily padded with recruiter-reposted enterprise "AI engineer" generic roles that are not actually AI-native in culture.

## Tier-1 target listings with live URLs

These are the listings most precisely matched to a Meta-cert + 2-year-Cursor/Claude-Code + 60-repo + TS/React/Next.js/Tailwind/Supabase/Neon/Drizzle profile, entry-level accepted, remote or LA-compatible. Apply to the top 10 this week.

| Rank | Company | Role | Location | Comp | AI tools named | Stack | Level | URL |
|---|---|---|---|---|---|---|---|---|
| 🥇 1 | **Stardex** (YC) | Forward Deployed Engineer | Remote US/CA/EU | $60–90K + 0.10–0.75% | Claude Code, Cursor | React, Supabase, TS, SQL, AWS Lambda | New grads OK | workatastartup.com/jobs/90537 |
| 🥇 2 | **Adaptify SEO** | Vibe Coder (Full-Stack AI/SEO) | Remote Worldwide | $40K–100K | Claude Code, Cursor | TS, Next.js, React, Node.js, Firebase, PostgreSQL | 0–2 yrs OK | remotevibecodingjobs.com / adaptify.ai/jobs/vibe-coder |
| 🥇 3 | **Jobhire** | Vibe Coder (freelance, 5–15 hrs/wk) | Remote / Cyprus | Hourly | Cursor, Claude, v0, Copilot, Replit, Bolt | Next.js, React, Tailwind, Node.js | 0–2 yrs | goodvibecode.com/jobs/vibe-coder-freelance-part-time-jobhire-472631 |
| 🥇 4 | **Tradeify** | Vibe Coder | Remote Worldwide | Not listed | Cursor, Claude, Bolt, Windsurf, v0 | Next.js, React, TS, Tailwind, Node.js, Supabase, Vercel | Portfolio-driven | goodvibecode.com/jobs/vibe-coder-tradeify-705833 |
| 🥇 5 | **Reforged Labs** (YC W22) | Junior Frontend Engineer | Hybrid (SF-area) | Not listed | Agentic AI pipelines | React, Next.js, TS | Junior/entry | workatastartup.com/jobs/81227 |
| ⭐ 6 | **Breezy** (HN hiring) | AI Product Engineer | Remote US | $120–150K + equity | Claude Code, Codex, Cursor | TS, React, Node.js, PostgreSQL | Mid (stretch) | HN item 47219668 |
| ⭐ 7 | **Reacher** (YC) | SWE Intern → Full-Stack | SF / **LA** / NY / Remote US | $90–130K FT | LLMs, AI agents | React, Tailwind, shadcn/ui, Python | Intern / 1+ yr | workatastartup.com/jobs/80430 |
| ⭐ 8 | **RINSE** (HN Apr 2026) | Software Engineer | Remote / **LA**/SF/NYC | $80–200K | "AI to automate" | React, RN, Python, Django, Postgres | New grads OK this cycle | HN item 47601859 |
| ⭐ 9 | **Presence** | Product Engineering Intern, Summer 2026 | Remote US | $15–20/hr | Claude Code, Lovable | Prototyping, Figma → code | 0–2 yrs / intern | goodvibecode.com/jobs/product-engineering-intern-summer-2026-presence-987067 |
| ⭐ 10 | **Modern Amenities (AIMS)** | Junior Agentic Engineer | Remote US | Not listed | Claude Code, Cursor | MCP, RAG, agentic systems | Junior | vibecoding.work |
| ⭐ 11 | **FurtherAI** (YC) | Forward Deployed Engineer | SF / Remote US | Comp + meaningful equity | Agentic AI systems | Python, React, TS | New grads OK | workatastartup.com/jobs/77473 |
| ⭐ 12 | **Blaze** (YC) | Junior Software Engineer | Mexico City | Not listed | Cursor, Windsurf, Copilot | React, RN, Next.js, Node, TS, Postgres | New grad | workatastartup.com/jobs/77590 |
| ⭐ 13 | **OakNorth** | Junior SWE (AI-native) | London onsite / Singapore remote | Not listed | Claude Code, Cursor, Copilot, Codex | Python, APIs, general SWE | 0–2 yrs / grad | vibecoding.work |
| ⭐ 14 | **DataCamp** | Full Stack Engineer Intern | Leuven / EU remote | Not listed | Cursor, Claude Code | TS, React, Node | Intern | be.indeed.com |
| ⭐ 15 | **Redfin** | Software Developer I | Seattle, WA | Not listed | Copilot, Claude Code, Cursor | General SWE | Entry (Dev I) | indeed.com |
| ⭐ 16 | **Real HR Hero / Thompson HR** | SWE I–II (AI-Enhanced) | Remote | Not listed | Cursor, Windsurf, Copilot, ChatGPT | React, Django, .NET, JS/Node | 1+ yr | remotive.com/.../software-engineer-i-ii-ai-enhanced-1473509 |
| ⭐ 17 | **Sealed Security** | Entry-Level SWE, Rust UX/DX | Remote US | Not listed | Cursor, Claude | Rust, WASM (stretch) | 0–2 yrs | goodvibecode.com |
| ⭐ 18 | **Wonder Dog** | Vibe Coder / Founding Engineer | Remote US | Salary + equity | Claude, Supabase, Inngest | RN, React, TS, Next.js | Pre-seed, flexible | weworkremotely.com |
| ⭐ 19 | **Lumimeds** | AI-First Frontend Engineer | Remote LATAM/E.Europe | Not listed | Cursor, Copilot, Claude Code, Claude Agent SDK | Next.js, React, Tailwind, Framer Motion, TanStack Query, Zustand | 3+ yrs (stretch) | greenhouse.io/lumimeds/jobs/4205821009 |
| ⭐ 20 | **Capsule** | Senior Frontend Engineer | **Los Angeles** | Series A | AI-native culture | React, Next.js, Figma | Senior (stretch) | indeed.com |

**LA-specific additional targets** that surfaced: Ghost (ghst.io) Senior SWE at $180–220K in LA; Red 6 Senior Frontend in Santa Monica; First Resonance Senior Frontend in LA; NETA Full-Stack React Native in Van Nuys; Whatnot Software Engineer, Early Career in LA. Most are senior but the Whatnot Early Career track and any Capsule/Ghost referral path deserve direct outreach, since LA's AI-native startup density is meaningfully thinner than SF's.

**Higher-bar aspirational targets** to monitor and build toward (not apply today): Vercel DX Engineer Next.js ($115–170K), Vercel AI Engineer v0 team ($192–288K), Supabase Frontend Engineer (Remote Worldwide), Anysphere/Cursor Design Engineer, Anthropic Product Engineer. These are gold-standard AI-native employers and represent where your portfolio should aim within 12–18 months.

## Where to hunt, in priority order

The board landscape splits cleanly into three tiers. **Spend 60% of applications on tier 1, 30% on tier 2, 10% on tier 3.**

**Tier 1 — the niche vibe-coding boards.** goodvibecode.com is the single highest signal-to-noise board found: 367 curated listings, each tagged with the specific AI tools required and a "Why this is a good vibe coding job" note, with an explicit 0–2 YOE filter. Listings are 3–14 days old and the $99 posting fee keeps spam low. remotevibecodingjobs.com is the volume play at ~1,575 aggregated roles with excellent filters (junior level, Cursor/Claude Code tool filters, "no-leetcode" culture tags, async-first). vibecoding.work is smaller (67 roles) but carries full JD text and named Fortune-500 compensation ranges. Set up email alerts on all three with filters: React + Next.js + TypeScript + Junior/Intern/0–2 + Remote.

**Tier 2 — YC Work at a Startup and HN "Who is hiring".** workatastartup.com is the richest single source for genuine AI-native culture at companies small enough to hire new grads. Filter by "AI" industry + "frontend" role + "New grads OK". Hacker News's monthly "Who is hiring" thread (search for the latest thread ID each month on news.ycombinator.com) is where smaller AI startups post without recruiter polish — read the raw text and grep for "Cursor," "Claude Code," "React," "Next.js." Also use hnhiring.com as a searchable UI over the same data.

**Tier 3 — general boards.** Indeed, LinkedIn, and ZipRecruiter work best for LA-local onsite/hybrid roles and for enterprise AI-enhanced postings that are less glamorous but offer stable comp. Their AI-native coverage is padded with recruiter reposts; filter aggressively by keyword "Cursor" or "Claude Code" rather than browsing. Remotive.com sits between tier 2 and 3 — a small but legitimate remote-first pipeline. Wellfound/AngelList is currently thinner than expected for AI-native roles; use it only for backup.

**Freelance/contract pipeline.** vibecodejobs.io ($1 post, $1 apply) is a niche marketplace explicitly designed for "vibe-coded MVPs needing a real developer to finish the last 20%" — an ideal fit for a 60-GitHub-project junior who can charge by deliverable. Use this to build paid references while salaried interviews are in flight.

## The mindset and language decoder

AI-native job descriptions have developed a recognizable dialect, and your resume and cover letter should mirror it. The recurring phrases are not clichés — they are filter keywords. Rewrite your resume summary to include at least five of these verbatim or near-verbatim.

The most frequent phrases across surveyed JDs were **"AI-native" and "AI-first"** (appearing in more than half of qualifying listings), **"ship fast / ship quickly / you can just ship things"** (Vercel's internal tagline now echoed everywhere), **"high agency / extreme ownership / operates like a founder,"** and **"product engineer / design engineer"** as the preferred title replacing "frontend developer." Augment Code's public hiring framework, widely copied in early 2026, names six dimensions: **product taste, system judgment, agent leverage, communication, ownership, and learning velocity** — with learning velocity explicitly highlighted as the top trait for "AI-Native Early Professionals," which is Augment's term for the entry-level archetype you occupy.

More specific phrases worth internalizing: **"slope over y-intercept"** (Mintlify — value growth rate over starting level), **"talent density"** (Anysphere/Cursor), **"cracked engineers"** (FurtherAI), **"embraces new AI-powered dev tools the moment they drop"** (Lingo.dev), **"10x development speed / multiplies output through AI tooling"** (Blaze, Life360), **"forward deployed engineer / FDE"** (becoming standard title for customer-facing AI product engineers at Stardex, FurtherAI, Hyperspell), **"you instinctively reach for AI tools to automate repetitive work"** (Stardex, near-verbatim usable in a cover letter), and **"first value in under 3 minutes / p75 FCP <1s"** (Lingo.dev performance obsession). The Life360 phrasing is the single most useful to mirror: *"You don't just use AI — you rely on it to scale your impact."*

Avoid, conversely, phrases that signal AI-generated-by-default résumés: **delve, realm, intricate, pivotal, showcasing, strategic thinker, passionate developer who loves problem-solving**. TopResume data indicates 33.5% of hiring managers claim they can spot AI-written résumés in under 20 seconds and 19.6% would reject outright. The irony of an AI-native role screening out AI-written résumés is real; personalize every submission.

## Red flags, disqualifiers, and filter traps

Thirteen recurring disqualifiers surface across the listing corpus. The hard gates are **years-of-experience minimums** (65% of surfaced AI-native roles required 3+ years, so you must over-weight the 0–2-YOE-explicit roles), **location-locked onsite requirements** at some LA roles (NETA Van Nuys onsite, Red 6 Santa Monica, Fuerte LLC LA 35-hr onsite), **US citizenship or clearance** at federal contractors (iAdeptive, BigBear.ai), **geographic eligibility bands** like Lumimeds' LATAM/Eastern-Europe-only restriction, and **stack mismatches** where "agentic" wraps a Python/Django/Go/.NET/Ruby core rather than React/Next.js.

The softer but more dangerous gates are around portfolio quality, since they determine whether you clear screening at the entry-friendly roles. Listings surveyed repeatedly warned against: tutorial clones (Netflix/Spotify/weather apps), uncurated repo dumps (a hiring-manager review of 200 portfolios on dev.to flagged "dozens of repos signal nothing if they're all tutorial clones"), projects with no live deployed URL, README text that reads AI-generated, inability to explain technical decisions behind claimed projects (utkrusht.ai cites ~70% of developers failing this), and "scope inflation" where a Lovable/v0 export is presented as authored work. Ed Mangini at GlobalLogic summarized it in IEEE-USA: *"Overusing AI when inappropriate is more likely to demonstrate ignorance and distract from someone's actual skill set."*

The single most dangerous trap for your specific profile is **your 60+ GitHub projects being read as noise rather than prolific output**. Hiring managers will not browse 60 repos — they will skim the 4–6 pinned. Curation is not optional.

## Portfolio criteria document

This is the target state your public footprint should reach before heavy application push. Treat it as a checklist.

### What an ideal AI-native portfolio looks like

The ideal portfolio is a personal website on a custom domain (yourname.dev beats yourname.vercel.app on recruiter perception), mobile-responsive (60% of recruiters browse on phone per markaicode Feb 2026), with a hero section that answers "what do you ship and how fast" in one sentence, followed by 5–6 case-study project cards each linking to a live demo and a GitHub repo. A green contribution graph over the last 6 months is expected; a blog with 3–5 posts documenting your build journeys is a strong positive signal; a visible "built in public" presence on X/Twitter is a further multiplier that Lee Robinson of Vercel has repeatedly endorsed.

Your GitHub profile itself should have exactly **4–6 pinned repos**, each demonstrating a distinct capability. All other repos should be archived or left un-pinned. Each pinned repo should hit star counts opportunistically (50–100 stars is "good profile" signal per Kula 2026 recruiting data) by being shared on Show HN, Product Hunt, r/nextjs, and X — but stars are supporting, not primary. What matters more is deployment, README quality, and visible evidence of the AI-native workflow: a committed `.cursorrules` file, an `AGENTS.md` file (emerging 2026 convention), a `.claude/skills/` folder when applicable, and transparent "how I used AI" notes in each README.

### What each project README must contain

The 2026 standard README, synthesized from top-starred repos and hiring-manager guides, has twelve mandatory components: a one-line hero description plus a demo GIF or video above the fold; a prominent live-demo link; build/deploy/license badges; a problem statement identifying the user and their pain; a bulleted key-features section with screenshots; an architecture diagram rendered inline via Mermaid.js; an explicit tech-stack list with rationale ("why Drizzle over Prisma" — one sentence each); a quickstart runnable in three commands; a `.env.example` shipped in the repo; screenshots or video walkthrough; a roadmap-or-known-limitations section signaling maturity; and measurable metrics when available (e.g., "94% answer accuracy, <2s response time"). AI-era additions that are becoming standard: a one-paragraph "AI-assisted development notes" section transparent about tool use, a prompt library or development log, and the visible `.cursorrules` / `AGENTS.md` files. Frame AI use carefully — write "Built with Cursor + Claude Sonnet as primary pair-programmer; architected and reviewed by me," not "100% AI-generated."

### The GitHub profile signals hiring managers actually weigh

Signal hierarchy, from most to least important: deployed live demos (non-negotiable), README clarity and structure, commit-activity consistency over the past 6 months, TypeScript adoption across projects (table-stakes now, not differentiator), curation of pinned repos to tell a story, meaningful commit messages and PR descriptions, tests present via Vitest/Playwright/RTL, CI/CD badges passing, monorepo structure (pnpm/Turborepo) for larger projects signaling systems thinking, mobile-responsive personal site, star count as weak supporting signal only, and open-source contributions to recognized ecosystem projects (Next.js, shadcn/ui, Drizzle, Vercel AI SDK, official MCP servers, PatrickJS/awesome-cursorrules) as a disproportionately strong signal.

The story your pinned repos should collectively tell: *"I can ship a production SaaS end-to-end; I understand the AI tooling layer deeply enough to extend it; I can handle non-trivial frontend engineering beyond AI wrappers; and I contribute to the ecosystem I build on."* Map each pinned repo to one of those claims.

### On the Meta Frontend Certificate specifically

Include it on your résumé as a single credential line for ATS and non-technical HR reviewers. It carries measurable value in those channels and unlocks the Meta Career Programs Job Board (200+ committed employers). But it is effectively invisible at the AI-native companies you most want — none of the Vercel, Anthropic, Supabase, Anysphere, or Lovable JDs reviewed mention or require certifications, and Scrimba's 2026 roadmap explicitly notes that AI-native employers "prioritize portfolio projects and problem-solving ability over formal credentials." Lead with shipped projects and AI-native tooling experience; the certificate is a garnish, not the main course.

## The three new projects to build, in priority order

From the seven candidate project archetypes identified in research (RAG SaaS, MCP server, agentic browser app, AI dev tool, AI digital twin portfolio, real-time collab app, OSS contribution), these three give you the highest return-on-effort for your profile and the roles you are targeting. Build in this order; each takes 1–3 weeks.

### Project 1: RAG-powered SaaS — "Chat with your [niche]"

**Why build it.** A deployed RAG SaaS with auth, billing, and evaluations is the single clearest demonstration of the full AI-native stack and of "agent leverage" on Augment's framework. Nearly every tier-1 target listing (Stardex, Adaptify, Tradeify, Breezy, Modern Amenities) will weight this above everything else on your portfolio. It proves zero-to-one capability, streaming UI fluency, pgvector knowledge, and production thinking in a single artifact.

**Stack.** Next.js 16 App Router + TypeScript + Tailwind + shadcn/ui + Supabase (auth + pgvector) + Drizzle + Vercel AI SDK on Anthropic Sonnet + Stripe for billing + Resend for email + Vercel deploy. This is literally your existing stack.

**Must-have features.** Document upload with chunking and embedding pipeline, chat interface with streaming responses and inline citations to source chunks, conversation history with persistent storage, usage-based pricing (metered Stripe), a basic admin dashboard showing cost per user, and — the differentiator — a continuous evaluation suite (Braintrust or a custom harness) that runs on every PR with results posted as a GitHub comment showing answer-quality delta. Pick a narrow, non-generic niche: "Chat with every Vercel changelog," "Chat with the Drizzle docs," or "Chat with the last 12 months of shadcn/ui issues." Narrow niches drive organic demo traffic and make the project memorable.

**Timeline.** 2–3 weeks. Launch on Show HN, Product Hunt, and X.

### Project 2: Custom MCP server and client — an agentic tool Claude and Cursor users will actually install

**Why build it.** MCP servers are the current rarest positive signal in 2026 AI-native portfolios. Very few junior candidates have shipped one. A working MCP server demonstrates TypeScript, Node, tool design, OAuth security, protocol literacy, and — most importantly — that you think like the companies building the tooling layer (Anthropic, Vercel, Cursor) rather than just consuming it.

**Stack.** `@modelcontextprotocol/sdk` + TypeScript + Zod + Vercel MCP Adapter + Next.js for the remote hosted server and landing page. Next.js 16 ships a built-in MCP endpoint at `/_next/mcp`, which simplifies the deploy story.

**Must-have features.** Wrap a real, personally-useful API integration — combining two or more of GitHub, Notion, Linear, Supabase, or Stripe. Expose 5–10 typed tools. Implement OAuth 2.0 with proper token handling. Add rate limiting. Publish to npm under a scoped name, submit to the public MCP registry, and record a 90-second setup GIF for both Claude Desktop and Cursor showing the tool in action. README must include an architecture diagram and a security-considerations section. Optionally monetize via MCPize.

**Timeline.** 1–2 weeks.

### Project 3: AI digital twin portfolio site — your portfolio as a live product

**Why build it.** This replaces the traditional "about me / resume / projects" static portfolio with a live RAG chatbot trained on your own case studies, work history, and methodology, styled in your voice. Lovable's 2026 portfolio round-up featured Caleb Ixca's split-screen implementation and it has become the dominant AI-native portfolio pattern. Every recruiter who lands on it will interact with it; the project itself becomes the interview warm-up. It also defends against the Nicky Hancock (AMS, NBC 2026) complaint that "all AI candidates are starting to look the same" — yours objectively will not.

**Stack.** Next.js + Tailwind + shadcn/ui + Framer Motion + Vercel AI SDK + Supabase pgvector + custom domain. 

**Must-have features.** Split-screen UX: case studies, project cards, and resume on the left; live chatbot trained on your writings on the right. The chatbot should answer questions like "What does your code review process look like?" or "Walk me through the hardest bug you fixed," citing specific projects. Include basic prompt-injection defenses (system-prompt hardening, output filtering). Add a "voice mode" bonus using the Vercel AI SDK's voice support. Ship it under yourname.dev and make it the link you send in every application.

**Timeline.** 1 week if you reuse the RAG infrastructure from Project 1.

Beyond these three, reserve bandwidth for **one meaningful open-source PR** per month to Next.js, shadcn/ui, Drizzle, Vercel AI SDK, or the official MCP servers repo. A single merged feature-PR outweighs twenty typo fixes and moves you from "ecosystem user" to "ecosystem contributor" in the eyes of Vercel/Anthropic/Anysphere-tier hiring managers.

## Conclusion: what changes if you execute this plan

The agentic-AI frontend market in April 2026 is structurally favorable to your exact profile, but not uniformly so. The top-of-market companies (Vercel, Anthropic, Anysphere, Supabase) are still gated behind 3–5 years of conventional experience, and the niche vibe-coding boards that explicitly welcome new grads also attract growing competition from career-switchers with similar Meta-cert-plus-60-repos resumes. The marginal move that changes your trajectory is not more repos, more certificates, or more applications — it is **one deployed RAG SaaS, one published MCP server, and one AI-native portfolio site, pinned to a curated GitHub profile, on a custom domain, shared publicly on X and Show HN**, with a résumé rewritten in the AI-native dialect identified above and applications targeted at the 20 listings tabled here.

The counter-intuitive finding across the 90+ listings surveyed is that **hiring managers at AI-native companies explicitly value evidence of *judgment about* AI tool use more than evidence of *volume of* AI tool use**. They are worried about ingesting indistinguishable AI-generated candidates. Your advantage, stated correctly, is not that you have used Cursor and Claude Code for two years — it is that you can articulate which tasks you hand to them, which you override, and why. Every project README, cover letter, and interview answer you write from this point forward should demonstrate that judgment explicitly. That is what converts a 60-project GitHub profile from noise into a hire signal, and it is the single most underused lever available to you right now.