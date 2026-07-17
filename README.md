# jordoncissna.github.io

User-page redirect for Milo. Any request to the bare domain
`https://jordoncissna.github.io/` (including stale Supabase confirmation
links whose redirect target was frozen before the Site URL was fixed) is
forwarded to the app at `/mileage-tracker/`, preserving the URL hash so the
`#access_token=...` from auth links completes the sign-in.

- `index.html` — redirect for the root path
- `404.html`   — same redirect for any unmatched path under the domain

No build step. GitHub Pages serves this automatically from `main`.
