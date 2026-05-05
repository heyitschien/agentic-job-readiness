# LingoPilot — recruiter-ready execution plan

**Stamped:** 2026-05-04  
**Purpose:** Single checklist to align engineering proof, docs, and portfolio surface. **Visual proof (GIF)** and **GitHub visibility** are owner tasks on a separate branch/workstream when convenient.

**Related:** [job-readiness-analysis.md](./job-readiness-analysis.md) · [product-feature-locale-visual-qa.md](./product-feature-locale-visual-qa.md) · [unofficial-recruiter-portfolio-validation-2026-05-04.md](../../analysis/unofficial-recruiter-portfolio-validation-2026-05-04.md)

---

## A. Story lock (what to say)

LingoPilot is an **autonomous localization QA workflow**: when English UI copy changes in a connected repo, a **GitHub App** enqueues work, a **worker** generates deterministic **pseudo** strings (`zz-pseudo`) for layout stress, captures **Puppeteer** screenshots, and opens a **PR** with evidence—plus run status in a **Next.js dashboard**. Pseudo is **layout / i18n wiring** stress, not machine translation.

For product framing (pseudo vs optional real locales later), see [product-feature-locale-visual-qa.md](./product-feature-locale-visual-qa.md).

---

## B. Automation proof (engineering checklist)

Use this to confirm the pipeline story matches reality after deploys or config changes.

- [ ] Push to monitored English locale files on the demo repo (e.g. `public/locales/en/*.json`).
- [ ] Bot receives `push` webhook and enqueues a job (**Upstash Redis**).
- [ ] Worker dequeues, clones at **exact commit SHA**, generates / refreshes **`zz-pseudo`** namespaces.
- [ ] Target app starts (**`next dev`** by default in worker), screenshots run for configured routes.
- [ ] Worker opens or updates a **GitHub PR** with screenshot artifacts / links.
- [ ] **Supabase** run record ends in a terminal success (or documented failure) state.
- [ ] **Dashboard** shows the run, PR link, and status.

**Canonical procedure:** [`lingopilot-engine/docs/runbooks/railway-e2e.md`](https://github.com/heyitschien/lingopilot-engine/blob/main/docs/runbooks/railway-e2e.md) (clone of record in workspace: `lingopilot-engine/docs/runbooks/railway-e2e.md`).

**Live E2E:** Walk-through / Antigravity validation is the ground truth; local `typecheck`/`lint` does not replace a real push.

---

## C. Pseudo screenshots (technical note)

- **Path-based locale URLs** are required for **Next.js Pages `i18n`** when using the internal runner: query-only `?locale=` is not enough for some stacks. The worker uses `effectiveScreenshotLocaleMode` → **`path`** when `WORKER_INTERNAL_RUNNER=1` (see `lingopilot-engine/services/worker/src/jobs/localization.ts`).
- Demo apps should align **i18next locale normalization** with `supportedLngs` (e.g. `lowerCaseLng` and `zz-pseudo` in the reference `next-i18next-sample`).

After a run, open the PR screenshots and confirm UI shows **pseudo** (stretched / bracketed copy), not plain English only.

---

## D. Repo hygiene before public

- [ ] No secrets in **working tree**; **git history** safe for public per each repo’s security remediation (`lingopilot-engine/docs/security/`, `lingopilot-dashboard/docs/security/`).
- [ ] **CI green** on default branch (dashboard: lint + `tsc`; engine: typecheck per service as configured).
- [ ] READMEs **cross-link** dashboard ↔ engine and list live demo (`lingopilot.app`).

---

## E. Owner track (portfolio surface)

| Task | Owner | Done |
| --- | --- | --- |
| Record demo GIF or short screen capture | Owner | [ ] |
| Embed GIF in **dashboard** + **engine** READMEs | Owner | [ ] |
| Make **both** repos public (after D) | Owner | [ ] |
| Pin entry repo + set **GitHub topics** (e.g. `nextjs`, `typescript`, `supabase`, `upstash`, `github-app`, `probot`, `localization`, `automation`) | Owner | [ ] |

---

## F. Workspace portfolio (agentic-job-readiness)

Broader “full GitHub profile” readiness (curation, 3-minute story, flagship focus) lives in the planning repo README and [unofficial-recruiter-portfolio-validation-2026-05-04.md](../../analysis/unofficial-recruiter-portfolio-validation-2026-05-04.md).

---

## Local verification stamp (typecheck / lint)

**Last local verification run:** **2026-05-04** (recruiter-ready prep pass)

| Repo / scope | Command | Result |
| --- | --- | --- |
| `lingopilot-dashboard` | `npx tsc --noEmit` | Pass |
| `lingopilot-dashboard` | `npm run lint` | Pass (warnings only: hooks deps, `no-img-element`) |
| `lingopilot-engine/services/worker` | `npm run typecheck` | Pass |
| `lingopilot-engine/services/bot` | `npm run typecheck` | Pass |

Dashboard fixes on branch `docs/recruiter-ready-prep`: removed invalid `GETRender`/`POSTRender` exports from `app/api/runs/route.ts`, added `components/ui/separator.tsx`, extended `EmptyState` with optional `action`, added ESLint config + devDependencies, fixed `api-keys-card` unescaped entities.
