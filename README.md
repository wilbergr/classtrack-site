# classtrack-site

Marketing website for **ClassTrack**, a homework & test tracker mobile app. Live at [classtrack.gwilber.com](https://classtrack.gwilber.com).

Plain static site — no build step, no dependencies. `index.html`, `privacy.html`, and `support.html` at the repo root, with styles in `css/` and brand art in `assets/`. Cloudflare Pages serves it directly with zero configuration.

To preview locally:

```sh
python3 -m http.server 8000
```

then open <http://localhost:8000>.
