# Work log (agentic-job-readiness + related repos)

## 2026-04-29 — LingoPilot E2E / pseudo screenshots housecleaning

- **lingopilot-engine (worker):** Removed temporary debug instrumentation (`agent-debug-log`, NDJSON ingest, `[LP-DEBUG]` console). Kept **path-based screenshot URLs** when `WORKER_INTERNAL_RUNNER=1` (`effectiveScreenshotLocaleMode`) so Next Pages i18n resolves `zz-pseudo` (query `?locale=` does not).
- **next-i18next-sample:** Added `lowerCaseLng: true` in `next-i18next.config.cjs` so i18next accepts `zz-pseudo` resources (avoids `zz-PSEUDO` vs `zz-pseudo` supportedLngs mismatch and English-only screenshots). `.gitignore` for `screenshots-debug*/`.
- **agentic-job-readiness:** Tracked `.claude/settings.json` and `docs/ai-layer/ai-layer-suggestion.md` (prior commit).
- **lingopilot-dashboard:** `CLAUDE.md` formatting / command reference refresh (same-day housecleaning commit).
