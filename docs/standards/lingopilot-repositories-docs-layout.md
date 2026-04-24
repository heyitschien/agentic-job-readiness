# LingoPilot multi-repo — documentation layout standard

**Purpose:** When you open `docs/` in **lingopilot-dashboard** or **lingopilot-engine**, you see a **small, intentional** set of folders (not ad-hoc `phase-*` trees at the top level).

**Relationship:** This complements [`industry-standard-repository-framework.md`](./industry-standard-repository-framework.md). That file defines the **universal** README, CI, and hiring checklist. This file defines the **LingoPilot-specific** *folder contract* for each repo’s `docs/`.

## Principles

1. **One obvious entry:** `docs/README.md` lists *maintained* material first; archive second.
2. **Diátaxis-style separation** (simplified):
   - **Tutorials / procedures** → `docs/runbooks/`
   - **System explanation** → `docs/architecture/`
   - **Security / trust** → `docs/security/`
   - **How to build and integrate (repo-specific)** → `docs/development/` (dashboard) or `services/*/README.md` (engine)
3. **Archive is not the product** — `docs/archive/legacy-2025/` holds old phase-1/2/3 and planning drafts. Nothing new goes there; nothing in archive is the live spec unless copied forward.

## Current layout (as of 2026-04-24)

### lingopilot-dashboard

| Path | Role |
| --- | --- |
| `docs/README.md` | Index. |
| `docs/STRUCTURE.md` | Layout contract + pointer back to *this* standard in `agentic-job-readiness`. |
| `docs/architecture/` | Mermaid + context for the UI in the full stack. |
| `docs/runbooks/` | e.g. Supabase restore. |
| `docs/security/` | Remediation tracker, etc. |
| `docs/development/` | e.g. `backend-integration/`, `backup-policy.md`. |
| `docs/archive/legacy-2025/` | Former `phase-1-mvp`, `phase-2-mvp-v2`, `lp-v2-build-road-map`, `dash-board-designs`, playbooks. |

### lingopilot-engine

| Path | Role |
| --- | --- |
| `docs/README.md` | Index. |
| `docs/STRUCTURE.md` | Layout contract. |
| `docs/architecture/` | Bot + worker + queue + DB context. |
| `docs/runbooks/` | e.g. Railway E2E. |
| `docs/security/` | Posture and remediation. |
| `docs/archive/legacy-2025/` | Former `phase-1-mvp`, `phase-2-mvp-v2`, `phase-3-future-labs` (ex-`phase-3-next-level-langchain-aiskd`). |
| `services/bot/README.md`, `services/worker/README.md` | Service-level truth. |

## Definition of done (docs)

- [ ] `docs/README.md` and `docs/STRUCTURE.md` exist in each Lingo repo.
- [ ] No *new* material added under `docs/archive/` except optional moves from the maintained tree.
- [ ] Recruiters and teammates can start at root `README.md` and land on `docs/README.md` in ≤2 clicks.

*Last updated: 2026-04-24*
