# Trackit

Browser food/day logging workspace with structured entry, JSON editing, local storage, and file import/export. Current daily records live in browser `localStorage.foodLog`; planned mixed-note capture features should not be assumed delivered.

Serve this directory with a static server (Python 3 example):

```text
python -m http.server 5500 --bind 127.0.0.1
```

Open `http://127.0.0.1:5500/`; stop with Ctrl+C. Existing app has no configured build/package installation. Keep the same origin for local storage and export important logs before migration. External fonts require network availability.

The main runtime is `index.html`; local styles are under `css/` and `theme.css`. Personal `_private/`, history, and rebuilt log material are not general-purpose test fixtures. Their consumer/retention status is deferred to an explicitly scoped data task; do not upload or remove them as part of a source cleanup.

No automated app/build/lint suite is configured. Syntax checks cover inline JS only; manually verify edit/delete/undo/reorder, JSON/manual synchronization, date switching, and valid/invalid imports with synthetic data when changing behavior. Existing personal data must remain untouched.

See [AGENTS.md](AGENTS.md) for engineering/privacy boundaries. Optional local docs at `../_docs/README.md` may be absent in a clone. No hosting configuration is supplied; review source versus private/support delivery inputs explicitly rather than relying on Git ignore alone.
