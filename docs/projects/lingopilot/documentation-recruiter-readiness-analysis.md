# LingoPilot — documentation structure & recruiter readiness analysis

**Date:** April 24, 2026  
**Scope:** `lingopilot-dashboard` · `lingopilot-engine` · standards in this repo  
**Authoring note:** This analysis is the single place to answer: *Do our docs meet industry expectations? What’s in the archive that still matters? What should we add for recruiters?*

---

## 1. How we judge “industry standard”

We use two documents in `agentic-job-readiness/docs/standards/`:

| Document | What it enforces |
| --- | --- |
| [`industry-standard-repository-framework.md`](../../standards/industry-standard-repository-framework.md) | **Universal** portfolio signals: identity (description, topics), README hero + 12-section pattern, `.env.example`, Mermaid, AI-dev notes, `.cursorrules`, `AGENTS.md`, CI badge, test strategy, hygiene, **type-specific** add-ons. |
| [`lingopilot-repositories-docs-layout.md`](../../standards/lingopilot-repositories-docs-layout.md) | **Lingo-specific** `docs/` *shape*: `README` + `STRUCTURE`, `architecture/`, `runbooks/`, `security/`, `development/` (dashboard), `archive/legacy-2025/`, service READMEs (engine). |

**Project context** (what the product is, E2E proof, tone) is captured in [`job-readiness-analysis.md`](./job-readiness-analysis.md).

Together: the **framework** = recruiter *first impression* (README, CI, public demo, GIF); the **Lingo layout** = *navigable* `docs/` for humans and future you; **job-readiness** = story + manual checklist (public repos, GIF, topics).

---

## 2. Current `docs/` structures (April 24, 2026)

### 2.1 Dashboard — `lingopilot-dashboard/docs/`

| Top-level | Purpose | Industry role |
| --- | --- | --- |
| `README.md` | Landing for all `docs/` | Diátaxis “entry” |
| `STRUCTURE.md` | Folder contract + link to standards | Reduces confusion |
| `architecture/` | `system-context.md` (Mermaid, framing) | **Explanation** |
| `runbooks/` | e.g. Supabase restore | **How-to / procedures** |
| `security/` | Remediation tracker | **Trust & ops** |
| `development/` | `backend-integration/`, `backup-policy.md` | **Build & integration** |
| `archive/legacy-2025/` | Old phase, road map, design, playbooks (large tree) | **History only** |

*Local-only:* `docs/database-backup/` may exist on disk (gitignored) for dump files; policy lives under `development/`.

### 2.2 Engine — `lingopilot-engine/docs/`

| Top-level | Purpose | Industry role |
| --- | --- | --- |
| `README.md` | `docs/` index | Entry |
| `STRUCTURE.md` | Layout contract | Contract |
| `architecture/` | `system-context.md` (bot, worker, queue) | Explanation |
| `runbooks/` | `railway-e2e.md` (canonical ops story) | Procedures |
| `security/` | Posture + remediation narrative + root `SECURITY-REVIEW-2026-04-22.md` | Trust |
| `archive/legacy-2025/` | phase-1, phase-2, `phase-3-future-labs` | History |
| *Outside `docs/`* | `services/bot/README.md`, `services/worker/README.md` | **Service API / behavior** |

---

## 3. Do we meet the *industry-standard framework* (both repos)?

**Summary: largely yes for Tier 2–3 *documentation* signals; a few *portfolio* items remain manual (GIF, public repos, topics).**

### 3.1 Universal core (from framework) — typical status

| Area | Dashboard | Engine | Recruiter note |
| --- | --- | --- | --- |
| README: value prop, demo link, Mermaid, problem, stack + rationale, quickstart, AI notes, limitations, roadmap, test strategy | Covered in main READMEs (per prior sprint + job-readiness) | Same | Strong |
| `.env.example` / secrets hygiene | Yes + remediation doc | Yes on services + security docs | Good |
| `AGENTS.md`, `.cursorrules` | Yes | Yes | 2026 signal |
| CI badge (green) | `ci.yml` in README | Railway deploy context in README | Good |
| Demo GIF in README | **Not done** (placeholder / manual) | **Not done** | High-impact *visual proof* |
| GitHub description + topics (profile) | **Manual** (private repo caveat) | **Manual** | Discoverability |
| `LICENSE` | MIT (per job-readiness) | MIT | Good |

*Exact line-by-line README ordering vs the 12-block table is best verified when preparing to go public; the intent is met.*

### 3.2 Type-specific: full-stack + “agentic / workflow”

| Extension (framework) | Status |
| --- | --- |
| System topology (multi-repo) | Mermaid in both READMEs + `docs/architecture/system-context.md`; **no single committed `CROSS-REPO.md` in a repo** (optional add below). |
| Shared contracts (API / types) | Described in README + integration notes; **no published OpenAPI** for dashboard API (acceptable for many portfolios if README lists routes—already there on dashboard). |
| AI / agentic transparency | “Localization QA workflow” framing in job-readiness; not “LLM product”—aligned. **No separate “failure modes” / eval** doc; optional if you want Tier-4 depth. |

**Verdict:** For **recruiter scanning**, you are in **Tier 2–3 documentation** *content-wise*; the remaining **blockers to “fully polished”** are mostly **non-doc**: public repos, **demo GIF**, GitHub description/topics, pin to profile (listed in `job-readiness-analysis.md`).

---

## 4. Do we meet the *Lingo* `docs/` layout standard?

| Requirement (`lingopilot-repositories-docs-layout.md`) | Met? |
| --- | --- |
| `docs/README.md` + `docs/STRUCTURE.md` in each Lingo repo | Yes (both) |
| Small maintained tree; phase junk not at top level | Yes — moved to `docs/archive/legacy-2025/` |
| `architecture/`, `runbooks/`, `security/` | Yes (both) |
| `development/` (dashboard) with integration | Yes |
| “≤2 clicks from root README to `docs/README`” | Yes (link in main README) |

**Verdict: yes** — the **folder contract** in that standard is implemented.

---

## 5. What other docs do we need to be *recruiter ready* (beyond the framework minimum)?

These are the **highest-leverage** additions that recruiters and senior engineers *notice* and that your archive does **not** fully replace (because it is long, duplicative, or historical).

| Priority | Doc / artifact | Repo | Why |
| --- | --- | --- | --- |
| P0 (non-doc) | **Demo GIF or short video** in both READMEs | Both | Framework explicit; only proof the system is real. |
| P0 (non-doc) | **Public repos** + **GitHub description + topics** | Both | Identity row in framework. |
| P1 | **One-page `docs/architecture/multi-repo.md`** (or `CROSS-REPO.md`) in *either* repo or in `agentic-job-readiness` | Either / portfolio | Fulfills “multi-repo relationship” extension cleanly without reading archive. |
| P1 | **Dashboard: `CONTRIBUTING.md` at root** (optional) | Dashboard | Framework “recommended”; you have `CONTRIBUTING` only in archive snapshots today. |
| P2 | **OpenAPI or static “API.md”** for dashboard API routes (table → optional request/response) | Dashboard | Strengthens “backend/API” extension for the Next.js API layer. |
| P2 | **DB overview** (Mermaid ERD or link to `supabase/migration` SQL) | Engine (or one shared doc) | Strengthens backend extension; RLS / tables summarized in one screen. |
| P2 | **Accessibility / perf note** (short: WCAG target, Lighthouse once, stack choices) | Dashboard | Frontend extension row in framework. |
| P3 | **Changelog** or **release tag discipline** | Both | Nice for “shipping culture”; not required for first hire pass. |

---

## 6. From the *archive* — what is “canonical” to preserve or extract?

The archive is **not** the live spec, but a few *categories* there contain material worth **one-time distillation** into the maintained set (or leaving as “see archive path” in `docs/README`).

### 6.1 Dashboard `archive/legacy-2025/`

| Area | What’s valuable | Canonical action |
| --- | --- | --- |
| `phase-1-mvp/lingopilot-phase0/docs/` | `ARCHITECTURE.md`, `OPERATIONS.md`, `SECURITY.md`, `ROADMAP.md` | **Keep in archive**; *live* story is root README + `docs/architecture/system-context.md` + `runbooks/` + `security/`. If anything contradicts the shipped app, **edit the maintained file**, not the archive. |
| `development` was `backend-integration/` (now out of archive) | Integration source-of-truth, Supabase guides | **Already** the maintained integration home. |
| `lp-v2-build-road-map/`, `phase-2-mvp-v2/build-road-map/` | North-star and planning | **History / product thinking** only; do not merge into “truth” without rewrite. |
| `dash-board-designs/` | HTML/JSX prototypes | **Design archaeology**; not needed for recruiters unless you add a “Design” section with one screenshot in README. |

### 6.2 Engine `archive/legacy-2025/`

| Area | What’s valuable | Canonical action |
| --- | --- | --- |
| `phase-1-mvp/ARCHITECTURE.md`, `OPERATIONS.md` | Monorepo-era narrative | **Archive**; **live** = README + `system-context.md` + `runbooks/railway-e2e.md` + `services/*` |
| `phase-2-mvp-v2/implementation-plans-worker/` | `engine-v2-single-source-of-truth.md`, milestones | **Engineering roadmap / depth**; link from `docs/README` *optional* (“deep dive in archive: …”) |
| `phase-3-future-labs/` | Speculative stack | **Clearly non-canonical**; keep archived only. |

**Rule of thumb:** If a recruiter only reads **root README + `docs/README` + one runbook + `system-context`**, they should understand the system. Everything else is **supporting** or **historical**.

---

## 7. Gaps: what we have *not* done yet (can we create it?)

| Item | Create it? | Effort |
| --- | --- | --- |
| `docs/architecture/multi-repo.md` (or portfolio doc) with diagram + “dashboard ↔ engine ↔ Supabase ↔ Redis ↔ GitHub” | **Yes — recommended** | ~1–2 hours |
| Root `CONTRIBUTING.md` (dashboard) | **Yes, optional** | ~30 min |
| `API.md` or OpenAPI for dashboard | **Yes, if** you want maximum backend credit | Half day (small surface) |
| ERD / `DATABASE.md` | **Yes, optional** | 1–2 hours |
| Extract 1–2 pages from `archive/.../OPERATIONS.md` into `docs/runbooks/operations-snapshot.md` | **Only if** you want ops text without opening archive | ~1–2 h reading + write |

**We should not** duplicate the entire archive into `docs/`; we **should** add **1–2 canonical “distilled”** files where the framework’s type-specific rows are still thin.

---

## 8. Conclusion: recruiter readiness vs documentation

- **Standards compliance:** The **Lingo `docs/` layout** standard is **met**. The **industry framework** is **largely met** for written docs and repo hygiene; the **largest remaining gaps** are the **universal** items that are *not* markdown files: **demo GIF, public profile, description/topics, pinning the repo.**
- **Documentation quality for hiring:** You have a **credible, navigable** `docs/` story **plus** a **clean archive**—this matches what strong candidates do. Adding **`multi-repo` / cross-repo** and optionally **API** + **DB** summaries would check the remaining **full-stack** extension boxes *without* reopening the phase folders.

---

## 9. Suggested next actions (ordered)

1. Record and embed **demo GIF**; make repos **public**; set **description + topics** (see `job-readiness-analysis.md` checklist).  
2. Add **`multi-repo` / `CROSS-REPO` doc** (one place, link from both READMEs).  
3. (Optional) **API.md** + **DATABASE.md** (short).  
4. (Optional) Root **CONTRIBUTING.md** (dashboard).  
5. When anything in archive becomes **wrong** relative to production, **update maintained docs first**, then leave archive as historical record or delete obsolete subtrees in a follow-up (with a tag first).

---

*Related files: [`job-readiness-analysis.md`](./job-readiness-analysis.md) · [`../../standards/industry-standard-repository-framework.md`](../../standards/industry-standard-repository-framework.md) · [`../../standards/lingopilot-repositories-docs-layout.md`](../../standards/lingopilot-repositories-docs-layout.md)*
