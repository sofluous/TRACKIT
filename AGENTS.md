# Trackit Development

Read [README](README.md) for setup and data boundaries.

- Preserve browser `localStorage.foodLog`, date-keyed records, JSON/manual editing consistency, import/export, and undo/reorder behavior. Keep existing data intact until schema/migration validation is explicit.
- Main application logic is inline in `index.html`; `css/` and `theme.css` are local style resources. Do not infer that history/rebuilt log files are runtime requirements or disposable output without scoped review.
- No package/build/lint or automated regression suite is configured. Parse changed inline JS and manually verify affected data workflows with synthetic browser storage, never the user's live log.
- Private/rebuild/history material requires an explicitly scoped task; do not read `_private/` during cleanup. Do not publish or stage personal data automatically.
- Follow applicable parent instructions when available. Optional local context is `../_docs/README.md`; normal app serving must not require it. Preserve unrelated edits and report unavailable validation.
