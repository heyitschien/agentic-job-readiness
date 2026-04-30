# Product feature: locale visual QA (pseudo + optional real locales)

**Status:** Captured (product framing). **Last updated:** 2026-04-29.

## Problem

Teams need confidence that localized UIs do not regress—layout, truncation, wrong-language strings, and missing keys—without relying on every reviewer running the app locally in every locale.

## Positioning

| Capability | Primary question |
|------------|------------------|
| **Pseudo (`zz-pseudo`)** from source | Do strings **stress layout** (length, wrapping, placeholders) deterministically? |
| **Real locale screenshots** (e.g. `fr`) | Does **actual translated copy** render correctly on key surfaces at a pinned commit? |

Pseudo is **not** a substitute for human translation QA; it is **layout and i18n wiring** stress from one generated locale.

## Local development vs automated capture

- **Local UI** is sufficient when a single developer switches locale, touches known screens, and self-verifies. Fast loop; no bot required.
- **Automated PR screenshots** add value when reviewers will not run the branch, when coverage must be **systematic** across routes/viewports, when **evidence on the PR** is required, or when build/runtime should match a **fixed recipe** (SHA, flags, headless).

Product copy: position the bot as **optional discipline for teams and PRs**, not a replacement for the developer’s local preview.

## Natural progression (roadmap hints)

1. Keep **one pseudo** from source (industry-typical); avoid “pseudo per natural language” unless a niche need appears.
2. Optional **second pass**: screenshot **real locales** present in the repo (`fr`, `de`, …) for content and layout with real strings—not pseudo variants.
3. **Configuration** over time: which locales, which paths/screens, org/project defaults.

## Engineering anchors (related work)

- Worker uses **path-based locale URLs** for internal runner so Next Pages i18n resolves `zz-pseudo` (query-only locale is insufficient for some stacks).
- Sample apps must align i18next **locale normalization** with `supportedLngs` (e.g. `lowerCaseLng` + `zz-pseudo`).

## Open questions (for later grooming)

- Dashboard UX for “pseudo only” vs “pseudo + selected real locales.”
- Cost/latency tradeoffs for multi-locale matrix per run.
