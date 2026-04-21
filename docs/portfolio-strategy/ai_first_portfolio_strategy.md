# AI-First Developer Portfolio Strategy

## Purpose

The purpose of this portfolio cleanup and new-build plan is to reposition the GitHub profile from a collection of many experiments into a focused hiring signal for AI-first developer / product engineer roles.

The goal is not to show “I have many repositories.”

The goal is to show:

> I can ship practical AI-native products, automate tedious workflows, build clean frontend systems, document engineering decisions, and apply security judgment to agentic tools.

This portfolio should make a hiring manager quickly understand:

1. What kind of engineer I am.
2. What problems I build for.
3. What AI tools I use and how I use them responsibly.
4. Which deployed projects prove I can ship.
5. Which repositories demonstrate product thinking, automation, frontend craft, agent workflows, and cybersecurity direction.

The final identity we are building toward:

> **AI-native frontend/product engineer building agentic tools for cybersecurity, learning, and intelligent workflows.**

---

# Hiring Criteria We Are Optimizing For

AI-first companies and agentic engineering roles are usually not looking for random tutorial volume. They are looking for evidence of judgment, shipping ability, and leverage.

## Primary Hiring Signals

### 1. Shipped Product Ability

A strong portfolio should prove that I can take an idea from concept to deployed product.

Evidence:
- Live demo
- Production deploy
- Clean UI
- Real user flow
- Clear problem statement
- Working data layer
- Authentication where relevant
- Basic analytics or logging where relevant

### 2. AI-Native Workflow

The portfolio should prove that I do not merely “use ChatGPT.” It should show that I understand how to build with AI as a development multiplier.

Evidence:
- Cursor / Claude Code / Codex development notes
- Agent workflow documentation
- Clear explanation of what AI helped with and what I personally reviewed
- Prompt or agent rule files where appropriate
- Before / after examples of automation

### 3. Automation / Glue Work

A major hiring signal is the ability to connect systems and reduce repetitive work.

Evidence:
- GitHub Actions
- Queue workers
- PR automation
- Screenshot generation
- Content pipelines
- API integrations
- Background jobs
- CI/CD workflows

### 4. Frontend Product Craft

For frontend/product engineer roles, the portfolio must prove I can create usable interfaces, not just backend demos.

Evidence:
- Next.js / React / TypeScript
- Tailwind / shadcn/ui
- Mobile responsiveness
- Good component structure
- Clean state management
- Accessible design
- Strong README screenshots

### 5. Cybersecurity Awareness

The portfolio should connect my AI/frontend path with my cybersecurity direction.

Evidence:
- Secure auth
- Rate limiting
- Permission scoping
- Audit logs
- Threat modeling
- Prompt-injection defense
- Secure MCP server design
- SOC / analyst workflow projects

### 6. Documentation and Communication

Hiring managers should see that I can explain what I built and why.

Evidence:
- README with architecture diagram
- Case study
- Technical decisions
- Tradeoffs
- Known limitations
- Roadmap
- Setup instructions
- Screenshots / GIFs

---

# Final Portfolio Strategy

We will not polish every repository.

We will curate a small number of high-signal repositories and either:
- polish them into serious case studies, or
- replace them with stronger new builds.

The target portfolio should have **4–6 pinned repositories total**.

Recommended final pinned lineup:

1. **LingoPilot** — automation / agentic workflow proof
2. **365-books** — shipped product and content automation proof
3. **AI Integrator / Portfolio Site** — personal front door
4. **SOC Analyst Agent / Cyber Workbench** — cyber direction and system design proof
5. **New RAG SaaS Flagship** — full-stack AI product proof
6. **New Secure MCP Server** — tooling-layer and security proof

Optional / secondary:
- **Cursor AI TTS Extension** — AI developer-tooling proof
- **Space Robotic AI** — advanced systems proof, useful for robotics / defense / space-adjacent roles but not primary for general AI-first frontend roles

---

# Portfolio Cleanup Projects

## 1. LingoPilot

### What It Is

LingoPilot is an automated localization QA workflow.

Core idea:

> When English copy changes, the system generates a pseudo-localized version, builds the app, captures screenshots of important routes, and opens a PR for visual review.

This is one of the strongest existing projects because it demonstrates the kind of automation loop AI-first teams care about:

> input change → automated transformation → visual verification → pull request artifact

### Why It Matters

LingoPilot proves that I can build automation around real engineering pain.

Localization QA is tedious. Teams often need to check whether translated or expanded text breaks layouts. LingoPilot turns that into an automated workflow.

This demonstrates:
- product thinking
- frontend awareness
- CI/CD automation
- GitHub workflow design
- quality assurance automation
- practical engineering leverage

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Automation | English change triggers pseudo-localization and screenshot generation |
| Frontend QA | Checks important UI routes in pseudo-locale |
| GitHub workflow thinking | Opens PR artifacts for review |
| Product sense | Solves a real tedious workflow |
| AI-first fit | Shows ability to automate repetitive engineering work |
| DevOps | GitHub Actions / build / screenshot pipeline |

### Current Strengths

- Clear workflow concept
- Strong problem framing
- Practical automation loop
- Good match for AI-first roles
- Can become a strong case study quickly

### What It Needs

#### Must Fix

- Confirm and restore the GitHub Action workflow file.
- Add working demo screenshots.
- Add one short demo GIF.
- Add architecture diagram.
- Update README headline from prototype language to outcome language.
- Make the repo public only after checking secrets and environment files.

#### README Upgrade

The README should lead with:

> **LingoPilot automates localization QA by generating pseudo-localized builds, capturing screenshots, and opening visual review PRs whenever English copy changes.**

Sections to add:
- Problem
- Solution
- Architecture
- Workflow
- Demo
- Tech stack
- What I built
- What AI assisted with
- Security / limitations
- Roadmap

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | Medium now, high after demo polish |
| AI-native workflow | Medium; can be high if AI/dev notes are added |
| Automation / glue work | Very high |
| Frontend product craft | Medium; depends on dashboard polish |
| Cybersecurity awareness | Low, unless auth/security notes are added |
| Documentation | Medium now, high after case study |

### Portfolio Role

**Lead automation project.**

This should be one of the first repositories a recruiter sees.

---

## 2. 365-books

### What It Is

365-books is a daily book insights web application. It presents one book, one insight, and one practice in under five minutes.

It includes:
- Next.js app
- MDX content system
- archive
- audio player
- podcast integration
- YouTube integration
- email newsletter system
- Vercel deployment
- analytics / performance tools

### Why It Matters

This is one of the strongest existing projects because it is a real product, not just a coding exercise.

It shows that I can build and maintain a content platform with a real audience direction.

It also connects to my long-term personal development / learning brand.

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Product shipping | Live web app and content platform |
| Frontend engineering | Next.js, responsive UI, navigation, MDX |
| Content operations | Episode creation and content guide |
| Integration | Podcast, YouTube, email newsletter |
| System thinking | Documentation and app status docs |
| Brand building | Clear user-facing product identity |

### Current Strengths

- Real product concept
- Good README
- Deployed on Vercel
- Strong personal brand alignment
- Content + technology combination
- Can become an AI automation case study

### Main Gap

The README currently reads like a product/content app, not like an AI-native automation project.

The AI pipeline needs to be surfaced clearly.

### What It Needs

#### README Additions

Add a section called:

## How This Product Uses AI Automation

Explain the workflow:

1. Book or topic selected.
2. AI-assisted research / summarization.
3. Episode structure generated.
4. Script / post / metadata produced.
5. Content published through MDX.
6. Newsletter or distribution workflow prepared.

#### Case Study Needed

Create:

`docs/case-study-ai-content-pipeline.md`

It should explain:
- the manual process before automation
- the AI-assisted process now
- inputs and outputs
- tools used
- time saved
- how quality is reviewed
- what is not fully automated

#### Suggested Metrics

Even if estimated honestly:
- “Reduced first-draft episode creation from X hours to Y minutes.”
- “Supports repeatable content production pipeline.”
- “Designed for daily publishing cadence.”

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | High |
| AI-native workflow | Medium now, high after README/case study |
| Automation / glue work | Medium now, high if content pipeline is documented |
| Frontend product craft | High |
| Cybersecurity awareness | Low |
| Documentation | Medium/high |

### Portfolio Role

**Shipped real product.**

This repo proves I can build something people can actually use.

---

## 3. AI Integrator / Personal Portfolio Front Door

### What It Is

AI Integrator is the current personal clarity / portfolio direction.

It explains:
- who I am
- what I do
- who I help
- how I think
- how people can contact me

It is already built with a modern stack and includes deployment and CI notes.

### Why It Matters

This becomes the main public identity hub.

A recruiter should not have to inspect 60 repositories to understand me. This site should explain the story immediately.

The portfolio site should communicate:

> I am an AI-native frontend/product engineer who builds practical automation tools and is moving toward cybersecurity workflows.

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Personal positioning | Clear professional narrative |
| Frontend craft | Landing page, design system, responsive UX |
| Communication | Explains value clearly |
| Deployment | Vercel deploy and production checklist |
| CI discipline | GitHub Actions install/lint/build |
| Product taste | Polished public-facing site |

### Current Strengths

- Already aligned with “Practical AI for Real Life”
- Clean positioning direction
- Has production checklist
- Has CI notes
- Can become the home for project case studies

### What It Needs

#### Naming Cleanup

Fix typo:

- Current: `ai-intergrator`
- Better: `ai-integrator`
- Or replace with final custom domain repo name:
  - `chien.dev`
  - `portfolio`
  - `chien-ai-portfolio`

#### Content Upgrade

Add sections:
- Hero: “AI-native frontend/product engineer building agentic tools for cybersecurity and learning workflows.”
- Featured projects
- Case studies
- AI workflow notes
- GitHub / LinkedIn / resume links
- Contact / schedule link

#### Later Upgrade

After the RAG project is built, upgrade this into the **AI Digital Twin Portfolio**.

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | Medium |
| AI-native workflow | Medium now, high after chatbot upgrade |
| Automation / glue work | Low/medium |
| Frontend product craft | High |
| Cybersecurity awareness | Medium if positioning is updated |
| Documentation | Medium/high |

### Portfolio Role

**The front door.**

This should be the link used in applications.

---

## 4. SOC Analyst Agent / Cyber Analyst Workbench

### What It Is

SOC Analyst Agent / Cyber Analyst Workbench is a local-first cyber intelligence workbench concept.

It is designed to sit on top of existing detection systems such as Wazuh and turn raw alerts into structured investigations and cases with AI assistance.

### Why It Matters

This project connects the portfolio to the cybersecurity path.

It shows that my AI/frontend skills are not generic. They are being directed toward security operations, analyst workflows, case management, and human-in-the-loop investigation.

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Cybersecurity direction | SOC workflow, cases, detection systems |
| Systems thinking | Architecture docs and domain model |
| Product strategy | V1 scope, non-goals, roadmap |
| Documentation rigor | Canonical docs, ADRs, schemas |
| AI judgment | Human-in-the-loop AI assistance |
| Security awareness | Security/auth documentation |

### Current Strengths

- Strong mission
- Strong architecture thinking
- Strong documentation structure
- Very aligned with cybersecurity career direction

### Main Gap

It is currently documentation-heavy and code-light.

The README says the application source is not present yet. That means it cannot be treated as a shipped product until a working V1 exists.

### What It Needs

#### Minimum V1 to Become Portfolio-Ready

Build a small working version:

- Alert ingestion mock API
- Event table
- Case creation
- Timeline view
- MITRE ATT&CK mapping field
- AI-generated triage summary
- Human approve/edit workflow
- Audit log
- Basic auth
- Seed data
- Demo mode

#### README Upgrade

Add a clear status label:

> Phase 0: Architecture and product design complete.  
> Phase 1: Event ingestion and case dashboard in progress.

#### Demo Needed

Create a recorded walkthrough:

1. Alert enters system.
2. Analyst opens event.
3. AI suggests triage summary.
4. Analyst edits/approves.
5. Case timeline updates.
6. Audit log records action.

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | Low now, high after V1 |
| AI-native workflow | Medium |
| Automation / glue work | Medium |
| Frontend product craft | Medium after dashboard |
| Cybersecurity awareness | Very high |
| Documentation | High |

### Portfolio Role

**Cyber direction proof.**

This should not be the lead repo until V1 code exists, but it is important for the long-term career narrative.

---

## 5. Cursor AI TTS Extension

### What It Is

A Cursor / VS Code extension that adds text-to-speech capabilities to AI assistant responses.

It allows users to listen to AI responses, control voice, adjust rate and pitch, skip code blocks, and use keyboard shortcuts.

### Why It Matters

This is a rare repo type compared to normal web apps.

It shows I can build developer tooling inside an existing editor environment.

It also supports my personal learning style and accessibility-oriented workflow.

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Developer tooling | Cursor / VS Code extension |
| AI workflow support | Reads AI assistant responses |
| UX thinking | Voice, rate, pitch, settings |
| Practical automation | Auto-read responses |
| Accessibility | Audio support for learning/coding |
| Product utility | Solves a real workflow need |

### Current Strengths

- Clear purpose
- Practical features
- Directly related to Cursor / AI coding workflows
- Different from typical frontend portfolio projects

### What It Needs

- Demo GIF
- VSIX release link
- Updated screenshots
- Install instructions verified
- Known limitations cleaned up
- Security/privacy note explaining what text is processed and where
- Optional: publish to marketplace if feasible

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | Medium |
| AI-native workflow | High |
| Automation / glue work | Medium |
| Frontend product craft | Low/medium |
| Cybersecurity awareness | Medium if privacy/security note is added |
| Documentation | Medium |

### Portfolio Role

**AI developer-tooling proof.**

This can be pinned if polished, especially for AI-first companies that value internal tooling.

---

## 6. Space Robotic AI

### What It Is

An AI / robotics / space systems lab that combines:

- ROS 2
- Webots simulation
- Foxglove Studio
- rosbridge
- dual WebSocket telemetry
- Docker / Colima
- Next.js mission dashboard
- rover telemetry topics

### Why It Matters

This project shows advanced systems thinking and cross-domain ambition.

It is impressive technically, but it must be framed carefully so it does not distract from the AI-first frontend/cyber hiring goal.

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Systems thinking | ROS, Docker, telemetry, simulation |
| Realtime data | WebSocket telemetry streams |
| Dashboard engineering | Next.js mission control UI |
| Robotics curiosity | Webots rover simulation |
| Operations | Runbooks and setup scripts |
| Architecture | System diagrams and phased roadmap |

### Main Risk

It can look unfocused for a frontend AI job unless framed as:

> Real-time mission dashboard and telemetry orchestration system.

Do not lead with the entire “AI + robotics + space” vision for general AI-first frontend roles.

### What It Needs

- One concrete demo loop
- Shorter README for recruiter view
- GIF of dashboard receiving telemetry
- Clear explanation of what the frontend displays
- Clear separation between current shipped system and future research vision
- Optional case study: “Building a real-time telemetry dashboard on Apple Silicon”

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | Medium |
| AI-native workflow | Low/medium currently |
| Automation / glue work | Medium |
| Frontend product craft | Medium |
| Cybersecurity awareness | Low |
| Documentation | High |

### Portfolio Role

**Optional advanced systems proof.**

Useful for robotics, defense, aerospace, or systems-heavy roles. Not a main pin for normal AI-first frontend roles unless polished.

---

# New Build Projects

These are the new projects that complete the portfolio and move it from “good existing repos” to “AI-first hiring portfolio.”

---

## New Build 1: Niche RAG SaaS Flagship

### Working Title

**SOC Playbook Copilot**

Alternative names:
- Security+ Study Copilot
- Cyber Analyst Playbook Chat
- Incident Response Copilot
- AI Job Fit Copilot

Recommended choice:

> **SOC Playbook Copilot**

### What It Is

A full-stack AI SaaS application where users can upload or browse security playbooks, analyst notes, incident response guides, and detection references, then ask questions with cited answers.

Example questions:
- “What should a Tier 1 analyst do first for this alert?”
- “What MITRE technique does this behavior map to?”
- “What evidence should I collect next?”
- “Summarize this alert for escalation.”
- “Which playbook applies to suspicious PowerShell activity?”

### Why It Matters

This becomes the strongest proof that I can build a serious AI-native product.

It combines:
- frontend engineering
- RAG
- vector database
- streaming AI
- citations
- auth
- storage
- evaluation
- cybersecurity workflow knowledge

### Demonstration Purpose

This project proves:

> I can build full-stack AI products that solve real workflow problems, not just toy chatbots.

### Core Features

#### V1 Must-Haves

- Next.js App Router
- TypeScript
- Tailwind
- shadcn/ui
- Supabase auth
- Supabase pgvector or equivalent vector database
- Document upload
- Chunking and embedding pipeline
- Streaming chat UI
- Inline citations
- Conversation history
- Saved playbooks
- Basic dashboard
- Seed SOC playbook examples
- Evaluation set with expected answers
- Deployment on Vercel

#### V2 Features

- Stripe billing
- Admin dashboard
- Cost-per-user tracking
- Role-based workspaces
- MITRE ATT&CK mapping helper
- Exportable incident summary
- GitHub PR comment eval report
- Prompt injection testing

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Full-stack AI | Auth, DB, vector search, AI SDK |
| RAG | Chunking, embeddings, retrieval, citations |
| Product engineering | Real user workflow and dashboard |
| Cybersecurity direction | SOC playbooks and analyst workflows |
| AI judgment | Citations, limitations, evaluation |
| Production thinking | Deployment, env vars, auth, logging |

### README Requirements

- Demo GIF above the fold
- Live demo link
- Architecture diagram
- Problem statement
- Target user
- Tech stack rationale
- Quickstart
- `.env.example`
- Data model
- RAG pipeline explanation
- Evaluation approach
- Security notes
- AI-assisted development notes
- Known limitations
- Roadmap

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | Very high |
| AI-native workflow | Very high |
| Automation / glue work | Medium/high |
| Frontend product craft | High |
| Cybersecurity awareness | Very high |
| Documentation | High if done properly |

### Portfolio Role

**Flagship AI SaaS.**

This should be one of the strongest pinned repositories.

---

## New Build 2: AI Digital Twin Portfolio

### Working Title

**Chien AI Portfolio Twin**

Alternative names:
- Ask Chien
- Chien.dev AI Twin
- Portfolio Copilot
- AI-Native Portfolio

### What It Is

A personal portfolio site with a chatbot trained on my own professional materials:

- resume
- project READMEs
- case studies
- career story
- technical decisions
- AI workflow notes
- cybersecurity learning path
- project documentation

Recruiters can ask questions like:
- “What are Chien’s best AI projects?”
- “How does he use Cursor and Claude Code?”
- “Which project best shows automation?”
- “What is his cybersecurity direction?”
- “Walk me through LingoPilot.”
- “What makes him different from a normal junior frontend developer?”

### Why It Matters

This turns the portfolio itself into a product demo.

Instead of a static page, the recruiter interacts with a working AI interface that demonstrates RAG, citations, personalization, and product taste.

### Demonstration Purpose

This project proves:

> I can build a personalized AI product and use it to communicate my own engineering story.

### Core Features

#### V1 Must-Haves

- Next.js
- TypeScript
- Tailwind
- shadcn/ui
- Framer Motion
- Vercel AI SDK
- Supabase pgvector
- Split-screen UI
- Project cards on left
- Chat interface on right
- Answers with citations to project docs
- Resume download
- Contact / schedule link
- Prompt-injection defense basics
- Deployed custom domain

#### V2 Features

- Voice mode
- Project recommendation flow
- Recruiter mode
- Role-fit analysis
- “Generate interview questions based on my projects”
- Admin content ingestion panel

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Portfolio positioning | Clear story and identity |
| Frontend craft | Split-screen UX and polished UI |
| RAG | Trained on personal/project docs |
| Product taste | Recruiter-friendly interaction |
| AI safety | Prompt-injection defense and source grounding |
| Communication | Explains technical experience clearly |

### README Requirements

- Live demo link
- Screenshot / GIF
- Architecture diagram
- Data sources used
- RAG pipeline explanation
- Safety and prompt-injection notes
- Deployment instructions
- AI-assisted development notes
- Known limitations

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | High |
| AI-native workflow | Very high |
| Automation / glue work | Medium |
| Frontend product craft | Very high |
| Cybersecurity awareness | Medium/high if safety notes included |
| Documentation | High |

### Portfolio Role

**Main public front door.**

This is the link used in job applications.

---

## New Build 3: Secure MCP Server

### Working Title

**Secure Portfolio MCP Server**

Alternative names:
- GitHub Portfolio Auditor MCP
- SOC Helper MCP
- AI Engineer Workflow MCP
- Secure Dev Workflow MCP

Recommended direction:

> **GitHub Portfolio Auditor MCP**

### What It Is

A Model Context Protocol server that exposes useful tools to AI assistants like Claude Desktop, Cursor, or other MCP-compatible clients.

The MCP server should wrap real APIs and provide typed tools for practical developer workflows.

Example tools:
- `analyze_repository_readme`
- `score_portfolio_repo`
- `check_project_hiring_signals`
- `generate_cleanup_tasks`
- `summarize_recent_commits`
- `find_missing_ci_files`
- `review_security_notes`
- `create_case_study_outline`

### Why It Matters

MCP servers are rare in junior portfolios.

A secure MCP project shows that I can build at the tooling layer, not just consume AI tools.

It also connects directly to the current AI agent ecosystem.

### Demonstration Purpose

This project proves:

> I understand agent tooling, typed tool design, secure API integration, and permission-aware automation.

### Core Features

#### V1 Must-Haves

- TypeScript
- Official MCP TypeScript SDK
- Zod schemas
- 5–10 typed tools
- GitHub API integration
- OAuth or secure token handling
- Rate limiting
- Logging / audit trail
- Clear install instructions
- Demo with Claude Desktop and/or Cursor
- Published package or installable repo

#### V2 Features

- Supabase storage
- Stripe or usage limit
- Web dashboard
- User permissions
- Multi-provider integrations
- Notion / Linear / GitHub combination
- Public MCP registry submission

### Security Requirements

This project must explicitly include security design.

Required security notes:
- token storage model
- least-privilege permissions
- rate limiting
- audit logging
- tool allowlist
- prompt-injection considerations
- safe output boundaries
- what the tool will not do
- environment variable handling
- local vs remote deployment tradeoff

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Agent tooling | MCP server exposed to AI clients |
| TypeScript backend | Typed tools and schemas |
| Security judgment | Auth, rate limits, audit logs |
| API integration | GitHub / Notion / Supabase / Linear |
| AI-first ecosystem fluency | Builds for Cursor / Claude workflows |
| Product thinking | Solves a real workflow problem |

### README Requirements

- One-line value proposition
- Install instructions
- Tool list and schemas
- Demo GIF
- Architecture diagram
- Security model
- Rate limit policy
- Example prompts
- AI-assisted development notes
- Known limitations
- Roadmap

### Hiring Criteria Match

| Hiring Criteria | Match |
|---|---|
| Shipped product ability | Medium/high |
| AI-native workflow | Very high |
| Automation / glue work | Very high |
| Frontend product craft | Low unless dashboard added |
| Cybersecurity awareness | Very high |
| Documentation | High if security model is clear |

### Portfolio Role

**Rare tooling-layer signal.**

This makes the portfolio stand out from normal frontend candidates.

---

## New Build 4: Meaningful Open Source Contribution

### What It Is

A monthly contribution to a real ecosystem project.

Target ecosystems:
- Next.js
- shadcn/ui
- Drizzle
- Vercel AI SDK
- MCP servers
- Supabase examples
- AI SDK examples
- security tooling docs

### Why It Matters

Open-source contribution shows I am not just building private projects. I am participating in the ecosystem.

A single meaningful PR can be more valuable than many small tutorial repos.

### Demonstration Purpose

This proves:

> I can read an unfamiliar codebase, follow contribution standards, communicate clearly, and improve real developer tools.

### Best Contribution Types

Good:
- docs improvement with real examples
- bug fix
- example app
- starter template
- test improvement
- accessibility fix
- missing edge case
- MCP server example
- AI SDK integration example

Weak:
- typo-only PRs
- formatting-only PRs
- random README changes
- low-context drive-by changes

### What It Demonstrates

| Skill | Demonstration |
|---|---|
| Ecosystem participation | PR to real project |
| Communication | Issue discussion / PR description |
| Code quality | Passing CI and review |
| Learning velocity | Ability to work in new codebases |
| Professionalism | Follows maintainer expectations |

### Portfolio Role

**Ecosystem credibility.**

This supports the rest of the portfolio.

---

# Final Execution Order

## Phase 1: Portfolio Cleanup

### Week 1: GitHub Curation and LingoPilot

Goals:
- Choose final pinned repos.
- Unpin weak or tiny projects.
- Polish LingoPilot into a case study.
- Fix missing automation files.
- Add screenshots / demo.
- Update README.

Outcome:

> LingoPilot becomes the lead proof of automation and AI-first workflow thinking.

---

### Week 2: 365-books and Portfolio Front Door

Goals:
- Add AI automation section to 365-books README.
- Add 365-books case study.
- Clean up AI Integrator / portfolio site.
- Clarify public positioning.
- Add featured project cards.

Outcome:

> Public identity becomes clear and recruiter-friendly.

---

### Week 3: SOC Analyst Agent and Cursor Extension

Goals:
- Clarify SOC Analyst Agent status.
- Define V1 build scope.
- Add roadmap and demo plan.
- Polish Cursor AI TTS Extension README.
- Add privacy/security note.

Outcome:

> Portfolio clearly shows cyber direction and AI developer-tooling experience.

---

## Phase 2: New Builds

### Weeks 4–5: Build RAG SaaS Flagship

Build:
- SOC Playbook Copilot

Outcome:

> Full-stack AI product with cyber workflow relevance.

---

### Week 6: Build AI Digital Twin Portfolio

Build:
- Chien AI Portfolio Twin

Outcome:

> Portfolio becomes interactive product demo and application link.

---

### Weeks 7–8: Build Secure MCP Server

Build:
- GitHub Portfolio Auditor MCP or Secure Dev Workflow MCP

Outcome:

> Rare agent-tooling and security signal.

---

### Ongoing: Open Source PRs

Goal:
- One meaningful PR per month.

Outcome:

> Evidence of ecosystem participation and professional engineering habits.

---

# Final Pinned Repository Map

| Slot | Repository | Purpose |
|---|---|---|
| 1 | AI Digital Twin Portfolio | Main public identity and recruiter front door |
| 2 | SOC Playbook Copilot | Full-stack RAG AI SaaS flagship |
| 3 | LingoPilot | Automation / localization QA workflow |
| 4 | Secure MCP Server | Agent tooling + security judgment |
| 5 | 365-books | Shipped real product / content automation |
| 6 | SOC Analyst Agent or Cursor AI TTS Extension | Cyber direction or AI developer-tooling proof |

---

# What Each Repo Should Prove Together

The portfolio should tell a complete story:

## LingoPilot

> I can automate tedious engineering workflows.

## 365-books

> I can ship and maintain a real product.

## AI Portfolio Twin

> I can present myself clearly and build personalized AI experiences.

## SOC Playbook Copilot

> I can build full-stack AI products with RAG, citations, and security-domain relevance.

## Secure MCP Server

> I can build agent tooling with security judgment.

## SOC Analyst Agent

> I understand cybersecurity workflows and can design systems for analysts.

## Cursor AI TTS Extension

> I can build tools that improve AI-assisted development workflows.

---

# Resume / Interview Positioning

## Main Positioning Statement

> I am an AI-native frontend/product engineer who builds practical agentic tools for cybersecurity, learning, and developer workflows. I use Cursor, Claude Code, and modern TypeScript systems to ship quickly, but I focus on human judgment, clean interfaces, security boundaries, and measurable workflow improvement.

## Short Version

> AI-native frontend engineer building agentic tools for cybersecurity and workflow automation.

## Project-Based Interview Pitch

### LingoPilot Pitch

> LingoPilot automates localization QA. When English copy changes, it generates pseudo-localized text, builds the app, captures screenshots of key routes, and opens a PR for visual review. It shows how I think about AI-first engineering: remove tedious manual work, create reviewable artifacts, and keep humans in the loop.

### 365-books Pitch

> 365-books is a daily book insights platform with MDX content, podcast and YouTube integrations, email newsletter infrastructure, and a repeatable content pipeline. It shows that I can ship a real product, not just demos.

### SOC Playbook Copilot Pitch

> SOC Playbook Copilot is a RAG-based AI assistant for security workflows. It helps analysts query playbooks, map alerts to next actions, and generate cited triage summaries. It connects my frontend skills with my cybersecurity direction.

### Secure MCP Server Pitch

> The secure MCP server demonstrates that I can build tools for AI agents, not just use them. It exposes typed tools, integrates with APIs, and includes auth, rate limiting, audit logging, and permission boundaries.

---

# Definition of Done for Any Pinned Repo

A repository is not portfolio-ready until it has:

- Clear one-line value proposition
- Live demo or demo video
- README with screenshots
- Architecture diagram
- Tech stack and rationale
- Local setup instructions
- `.env.example`
- Tests or explanation of test strategy
- CI/build status if applicable
- Deployment instructions
- AI-assisted development notes
- Known limitations
- Roadmap
- Security/privacy notes where relevant
- Recent commit activity
- Clean repo name
- No secrets
- No confusing template text
- No claims that cannot be demonstrated

---

# Success Criteria

This portfolio plan succeeds when a hiring manager can look at the profile for 60 seconds and understand:

1. This candidate ships real things.
2. This candidate understands modern frontend engineering.
3. This candidate uses AI tools with judgment.
4. This candidate can automate workflows.
5. This candidate has cybersecurity direction.
6. This candidate documents clearly.
7. This candidate is not just another “vibe coder.”

The intended reaction:

> “This person is early-career, but unusually AI-native, practical, and systems-minded. They can probably help us ship internal tools, automation workflows, frontend products, and agentic systems faster.”
