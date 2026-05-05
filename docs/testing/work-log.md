# Work log (agentic-job-readiness + related repos)

## 2026-04-29 — LingoPilot E2E / pseudo screenshots housecleaning

- **lingopilot-engine (worker):** Removed temporary debug instrumentation (`agent-debug-log`, NDJSON ingest, `[LP-DEBUG]` console). Kept **path-based screenshot URLs** when `WORKER_INTERNAL_RUNNER=1` (`effectiveScreenshotLocaleMode`) so Next Pages i18n resolves `zz-pseudo` (query `?locale=` does not).
- **next-i18next-sample:** Added `lowerCaseLng: true` in `next-i18next.config.cjs` so i18next accepts `zz-pseudo` resources (avoids `zz-PSEUDO` vs `zz-pseudo` supportedLngs mismatch and English-only screenshots). `.gitignore` for `screenshots-debug*/`.
- **agentic-job-readiness:** Tracked `.claude/settings.json` and `docs/ai-layer/ai-layer-suggestion.md` (prior commit).
- **lingopilot-dashboard:** `CLAUDE.md` formatting / command reference refresh (same-day housecleaning commit).

## 2026-04-29 (end of day) — Product capture + housekeeping stamp

- **Product:** Logged locale visual QA as a tracked feature: local dev vs PR screenshot bot, pseudo vs real locales, and roadmap hints → `docs/projects/lingopilot/product-feature-locale-visual-qa.md`.
- **Housekeeping:** Work log and product doc committed and pushed from `agentic-job-readiness`; related repos already received earlier same-day commits (engine worker cleanup, dashboard `CLAUDE.md`, sample `lowerCaseLng` / `.gitignore`).

## 2026-05-04 — Unofficial recruiter/portfolio validation log

- **Analysis doc:** Captured assistant synthesis of recruiter readiness (full portfolio vs LingoPilot flagship), sources consulted, rationale, current snapshot, and next steps → `docs/analysis/unofficial-recruiter-portfolio-validation-2026-05-04.md`.
- **Note:** Informal only; does not replace formal standards or live audits; explicit “what we did not run” listed in that file.

## 2026-05-04 (later) — Analysis doc readability pass

- **Same file:** Reformatted with emoji section headers, 🟢🟡🔴🔵 legend, GitHub `> [!NOTE|TIP|IMPORTANT|WARNING|CAUTION]` callouts for color/tint in compatible viewers, and medal-priority next steps (🥇🥈🥉).

## 2026-05-04 — Recruiter-ready prep (docs + verification branches)

- **Branch:** `docs/recruiter-ready-prep` on each touched repo (not `main`).
- **agentic-job-readiness:** Refreshed [`job-readiness-analysis.md`](../projects/lingopilot/job-readiness-analysis.md) (Tier 3 truth, completed vs remaining tables); supersession banner on [`lingopilot-recruiter-readiness-report.md`](../standards/lingopilot-recruiter-readiness-report.md); new [`recruiter-ready-execution-plan.md`](../projects/lingopilot/recruiter-ready-execution-plan.md); README link under Purpose; work-log updated.
- **lingopilot-dashboard** (`docs/recruiter-ready-prep`): `tsc` + `lint` green — removed non-route `GETRender`/`POSTRender` from `app/api/runs/route.ts`, added `separator` UI, `EmptyState` `action` prop, `.eslintrc.json` + `eslint` / `eslint-config-next@15.2.8`, fixed `api-keys-card` ESLint errors.
- **lingopilot-engine** (`docs/recruiter-ready-prep`): README Known Limitations — bot installation stubs called out; worker + bot `npm run typecheck` pass.
- **Owner still:** demo GIF, public repos, profile pin/topics (see execution plan).

## 2026-05-04 — Session close / milestone lock

- **Locked record:** [`docs/projects/lingopilot/MILESTONE-LOCK-recruiter-prep-2026-05-04.md`](../projects/lingopilot/MILESTONE-LOCK-recruiter-prep-2026-05-04.md) — frozen git anchors (`docs/recruiter-ready-prep` → `9f108f5` / `43c0222` / `518c0c1`), **recruiter readiness snapshot** (engineering + docs strong; GitHub surface pending GIF/public/pin; full profile still moderate), canonical doc map, handoff checklist.
- **Execution plan** header updated to point at the milestone lock and **next session: Antigravity walk-through** (live E2E proof).
- **Shop closed for this wave:** merge PRs when ready; no further work assumed until Antigravity session.
