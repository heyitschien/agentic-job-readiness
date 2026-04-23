# Industry-Standard Repository Framework

**For:** AI-First Frontend / Full-Stack Engineer  
**Date:** April 2026  
**Sources:** Three-Agent Synthesis (Apr 20, 2026) · Claude Code Job Market Report (90+ JDs) · JetBrains AI Pulse April 2026 · Augment Code hiring framework · Kula 2026 recruiting data

> **This document is the permanent reference standard.** Apply it to every repository before sharing with recruiters, pinning to your GitHub profile, or including in any application.

---

## Is There One Standard, or Is Every Project Different?

Both. There is a **Universal Core** of 21 requirements that never change regardless of project type, stack, size, or domain. Missing any of them creates doubt with hiring managers. On top of that, each project type has **additive extensions** — you stack them on top of the core, never replace it.

| Profile | Adds to Core |
|---|---|
| Frontend-Only | UI/UX signals: accessibility, responsive screenshots, Lighthouse, state management rationale |
| Backend/API-Only | Systems signals: OpenAPI docs, DB schema, auth model, deployment instructions |
| Full-Stack | Both of the above + system topology diagram + multi-repo relationship doc + shared contracts |
| AI / Agentic | Model transparency, prompt notes, human-in-the-loop docs, failure modes, eval strategy |

A full-stack AI project carries the heaviest documentation burden by design. **Context shapes depth, not presence** — a weekend prototype and a 6-month production service both need a live demo URL and a problem statement; the depth differs.

---

## Universal Core — Every Repository, Every Type

These 21 requirements apply to every single repository. A recruiter auditing repos carefully will check every item.

### Identity

| Required Item | What Recruiters Read Into It |
|---|---|
| Repo name: lowercase, no typos, no underscores | First impression — broken names signal carelessness before they open the repo |
| GitHub description field completed (1–2 sentences) | Shows in the profile grid; many recruiters only ever see this field |
| Topics/tags set (e.g. `nextjs`, `typescript`, `ai-agent`) | GitHub search discoverability + visual taxonomy on your profile |

### README — Hero (Above the Fold)

| Required Item | What Recruiters Read Into It |
|---|---|
| One-line value proposition at the very top | 10-second read test — most hiring managers will not scroll past the fold |
| Live demo URL above the fold | No demo = not portfolio-ready; recruiters skip repos with no proof of shipping |
| Demo GIF or screenshot inline in README | Visual proof of a real, working product — separates builders from clone-followers |

### README — Core Sections

| Required Item | What Recruiters Read Into It |
|---|---|
| Problem statement: who the user is and their specific pain | Signals product thinking and empathy — not just code execution |
| Tech stack list with one-sentence rationale per choice | Signals architectural judgment — "why Drizzle over Prisma" is a hiring-manager magnet |
| Architecture diagram (Mermaid.js inline or linked image) | Rare at junior level; immediately signals systems thinking and documentation culture |
| Quickstart runnable in 3 commands max | Proves it is real, reproducible, and that you respect the reader's time |
| `.env.example` shipped in repo with every variable described | Security best practice + lowers contributor friction + signals professionalism |
| Known limitations section | Signals maturity and honest self-assessment — juniors who hide flaws raise red flags |
| Roadmap section | Shows long-term product vision and that you think beyond the current commit |
| Tests or documented test strategy | Absence is a yellow flag; presence (even lightweight) signals engineering discipline |

### README — AI-Native Signals (2026 Standard)

| Required Item | What Recruiters Read Into It |
|---|---|
| AI-assisted development notes (which tools, how used) | 2026 transparency standard — "Built with Cursor + Claude as pair programmer; architected and reviewed by me" |

### Repo Files

| Required Item | What Recruiters Read Into It |
|---|---|
| `.cursorrules` file committed to repo | 2026 AI-native convention — signals active Cursor workflow and project-specific AI context |
| `AGENTS.md` file committed to repo | Emerging 2026 standard — signals multi-agent awareness and collaboration maturity |

### Hygiene

| Required Item | What Recruiters Read Into It |
|---|---|
| No secrets in any tracked file or git history | Active credential exposure is an automatic, immediate disqualifier — no exceptions |
| Commit activity within the last 30 days | Signals an engaged, active developer — not an abandoned side project |
| CI/CD badge (green) displayed in README | Shows automation mindset and that the build is healthy right now |
| Meaningful commit messages (not "fix" or "update") | Auditable professional workflow — many hiring managers read the commit log |

---

## Type-Specific Extensions

### Frontend-Only

Add these on top of the Universal Core:

- Component breakdown or Storybook link (shows component architecture)
- Accessibility notes — WCAG level targeted and how it was tested
- Mobile-responsive screenshots across breakpoints (mobile, tablet, desktop)
- Lighthouse / Core Web Vitals score or explicit performance target
- State management choice and rationale (Zustand vs Redux vs Context)
- Design system or component library decisions (shadcn/ui, Radix, etc.)
- Vercel preview URL automatically generated per PR

### Backend / API-Only

Add these on top of the Universal Core:

- API reference: OpenAPI / Swagger UI link or equivalent interactive docs
- Database schema diagram (ERD or Mermaid entity diagram)
- Authentication + authorization model documented (JWT, OAuth, sessions)
- Rate limiting, error handling, and retry strategy explicitly noted
- Queue / job processing architecture documented (workers, queues, retries)
- Deployment instructions: Docker Compose, Railway, Render, or equivalent
- Every environment variable explained in `.env.example` with example values

### Full-Stack

Add everything in Frontend-Only + Backend-Only above, plus:

- Clear labeling: which repo/folder is frontend vs backend vs shared
- System architecture diagram showing full data flow end-to-end
- Multi-repo relationship diagram (how frontend and backend communicate)
- Deployment topology: Vercel (frontend) + Railway/Render (backend) — explicit
- Integration points: how frontend calls backend (REST, WebSocket, queue)
- Shared contracts: API types, Zod schemas, or OpenAPI spec linking both repos

### AI / Agentic

Add these on top of the Universal Core (in addition to any type extensions above):

- Model documentation: which model, version, provider, and why it was chosen
- Prompt engineering notes or committed prompt library (shows craft)
- Human-in-the-loop explanation: when AI acts vs when human approves
- Failure modes, fallbacks, and guardrails explicitly documented
- Evaluation / test strategy for AI output quality (eval harness or manual process)
- Latency and cost per operation (if applicable to the product)
- Precise framing: "autonomous localization QA workflow" not "AI translation" — accuracy matters

---

## Repository Maturity Tiers

| Tier | Label | What It Means | What Gets You There |
|---|---|---|---|
| **Tier 1** | Passing | Recruiter does not immediately skip | Live demo URL + README exists + no secrets + clean repo name |
| **Tier 2** | Credible | Recruiter bookmarks for follow-up | All 12 README sections + demo GIF above fold + working quickstart + green CI badge |
| **Tier 3** | Industry Standard | Recruiter proactively reaches out | Tier 2 + architecture diagram + AI notes + `.cursorrules` + `AGENTS.md` + tests + full-stack topology |
| **Tier 4** | Exceptional | Gets shared, earns stars, opens doors | Tier 3 + build-in-public blog post + measurable metrics + ecosystem contributions + Show HN / Product Hunt launch |

---

## Canonical File Architecture

### Root-Level Required Files

| File | Purpose | Status |
|---|---|---|
| `README.md` | Primary docs — all 12 sections present | Required |
| `.env.example` | All vars described, no real values | Required |
| `.cursorrules` | AI coding conventions for this repo | 2026 Standard |
| `AGENTS.md` | Multi-agent instructions and context | 2026 Standard |
| `.gitignore` | Excludes `.env`, `node_modules`, build output | Required |
| `LICENSE` | MIT, Apache 2.0, or similar open license | Recommended |
| `CONTRIBUTING.md` | Contribution guide (open-source signal) | Recommended |
| `.github/workflows/` | CI pipeline: lint + type-check minimum | Recommended |

### README Section Order

Sections must appear in this order. Each position is intentional.

| Order | Section | Why This Position |
|---|---|---|
| 1 | Hero: one-line value prop + badges | 10-second test — this is all many will read |
| 2 | Live demo URL + GIF or screenshot | Proof of work above the fold |
| 3 | Problem statement (user + pain) | Context before features |
| 4 | Key features with screenshots | Sells the project to the skimmer |
| 5 | Architecture diagram | Separates engineer from tutorial-follower |
| 6 | Tech stack + rationale | Signals judgment, not copy-paste |
| 7 | Quickstart (3 commands) | Respects the reader's time |
| 8 | `.env.example` reference | Security + completeness signal |
| 9 | AI-assisted development notes | 2026 transparency standard |
| 10 | Known limitations | Maturity and self-awareness |
| 11 | Roadmap | Product thinking beyond shipping |
| 12 | Tests / test strategy | Engineering rigor signal |

---

## Definition of Done

A repository is not portfolio-ready until every item in this checklist is complete.

### Security (Non-Negotiable First)

- [ ] No secrets in any tracked file
- [ ] No secrets anywhere in git history (verified with `git log -p | grep -i secret` or BFG scan)
- [ ] `.env.example` committed with all variables described but no real values
- [ ] `.gitignore` explicitly excludes `.env`, `.env.local`, and any credential files

### Identity and Discoverability

- [ ] Repo name is lowercase, no typos, no underscores
- [ ] GitHub description field completed (1–2 sentences)
- [ ] Topics / tags set on GitHub

### README

- [ ] One-line value proposition at the top
- [ ] Live demo URL above the fold
- [ ] Demo GIF or screenshot inline
- [ ] Problem statement (user + pain)
- [ ] Key features section with screenshots
- [ ] Architecture diagram (Mermaid.js or image)
- [ ] Tech stack with one-sentence rationale per choice
- [ ] Quickstart runnable in 3 commands
- [ ] `.env.example` referenced and explained
- [ ] AI-assisted development notes
- [ ] Known limitations section
- [ ] Roadmap section
- [ ] Test strategy documented

### Repo Files

- [ ] `.cursorrules` committed
- [ ] `AGENTS.md` committed
- [ ] `LICENSE` present
- [ ] `.github/workflows/` CI pipeline present

### Hygiene

- [ ] Commit activity within the last 30 days
- [ ] Meaningful commit messages throughout
- [ ] CI/CD badge (green) in README
- [ ] No placeholder or template text remaining

### Type-Specific (add as applicable)

- [ ] **Frontend:** Lighthouse score documented, mobile screenshots, accessibility notes
- [ ] **Backend:** OpenAPI docs live, DB schema diagram, deployment instructions complete
- [ ] **Full-Stack:** System topology diagram, multi-repo relationship doc, shared contracts
- [ ] **AI/Agentic:** Model choice documented, prompt notes, human-in-the-loop explained, failure modes listed

---

## AI-Assisted Development Notes Template

Copy this into every README. Customize the tools and your role description.

```markdown
## How This Was Built

Developed using Cursor as the primary IDE with Claude Sonnet as a pair programmer for code generation, architecture review, and refactoring suggestions. All architectural decisions, code review, and final implementation were made and verified by me. AI tooling was used to accelerate development velocity, not replace engineering judgment.

**Tools used:** Cursor, Claude Code, [add others]  
**My role:** Architect, reviewer, product decision-maker, and shipping engineer
```

---

## The Framing Rule for Agentic Projects

Precision in language matters with technical recruiters. Use the most accurate description of what the system actually does:

| What It Does | Correct Framing | Incorrect Framing |
|---|---|---|
| Runs deterministic text transformation rules | "Automated localization QA workflow" | "AI-powered translation" |
| Calls an LLM API and uses the response | "LLM-assisted content generation" | "AI writes the content" |
| Uses a vector search to retrieve relevant docs | "RAG-based retrieval system" | "AI knows your documents" |
| Routes tasks between agents based on rules | "Agentic workflow orchestration" | "Autonomous AI agent" |
| Shows AI suggestions, human approves | "Human-in-the-loop AI workflow" | "Fully automated AI" |

---

*Last updated: April 2026 — review and update quarterly or when significant new hiring signal emerges.*
