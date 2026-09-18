# GroMo Festive Partner Page

A single-file, static landing page for GroMo's festive credit-card partner campaign.

## Live site

Published via GitHub Pages — see the repository's **Settings → Pages** for the URL.

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | The entire landing page — markup, CSS and JS inline, images embedded as base64 data URIs. No build step, no dependencies. |
| `.nojekyll` | Tells GitHub Pages to serve files as-is instead of running Jekyll. |

## Running locally

Open `index.html` directly in a browser, or serve it:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## Editing

Everything lives in `index.html`:

- **Fonts** — DM Sans + Poppins, loaded from Google Fonts.
- **Styles** — one `<style>` block near the top, with `@media` blocks for tablet (`980px`) and phone (`620px`).
- **Content** — sections in order: hero, why credit cards, bank picks, how it works, top picks, season bonus, self-sale, comparison, FAQ, footer.
- **Behaviour** — one `<script>` at the bottom handling CTA links and the FAQ accordion.

Images are inlined as data URIs, which is why the file is large. Commit changes and push to `main`; GitHub Pages redeploys automatically.
