# Project agent memory

Marketing site for the ClassTrack mobile app (app repo: `classtrack` in the same projects tree). Deployed via Cloudflare Pages to `classtrack.gwilber.com`.

- **Plain static site, no build step — deliberately.** `index.html` at the repo root plus `css/` and `assets/`; Cloudflare Pages serves it with zero config. Do not add a framework, bundler, or npm dependency.
- **Theme = the app's Ember palette.** CSS custom properties at the top of `css/style.css` mirror `emberLight`/`emberDark` in the app repo's `src/theme/palettes.ts`; keep them in sync if the app palette changes. `--accent-strong` is site-only: a darker Ember shade because `#D9480F` falls short of WCAG AA for small text on light surfaces.
- **`assets/*.png` are copies of the app's generated branding** (from the app repo's `assets/`, produced by its `npm run branding`). Never hand-edit them; re-copy from the app repo after branding regenerates.
- **Copy rulebook applies to site copy too**: warm and encouraging, no shame/pressure language, nothing framed as lost or failed. See "Copy rulebook" in the app repo's `CLAUDE.md`.
- **No fabricated content**: no fake app screenshots until real ones exist; store buttons stay "Coming soon" badges (not links) until the App Store / Google Play listings are live.
- Contact email `hello@gwilber.com` is an unconfirmed placeholder — marked with `<!-- TODO: confirm contact email -->` in `privacy.html` and `support.html`.

## Maintaining this file

Keep this file for knowledge useful to almost every future agent session in this project.
Do not repeat what the codebase already shows; point to the authoritative file or command instead.
Prefer rewriting or pruning existing entries over appending new ones.
When updating this file, preserve this bar for all agents and keep entries concise.
