# Byte-256.github.io

Personal portfolio of Sanjay K — a modern, minimal, dark developer landing page built with Tailwind CSS.

## Tech

- Single-page HTML (`index.html`)
- Tailwind CSS v4 (compiled via the Tailwind CLI)
- Vanilla JS (`assets/js/main.js`)
- GitHub Pages — no runtime build, serves precompiled static files

## Development

```sh
npm install
npm run build   # compile Tailwind once  → assets/css/main.css
npm run watch   # recompile on change
```

## Structure

```
index.html            # landing page
src/styles.css        # Tailwind source (theme tokens + component classes)
assets/css/main.css   # compiled output (committed for GitHub Pages)
assets/js/main.js     # mobile nav, scroll reveal, footer year
images/me.jpeg        # portrait
resume.pdf            # resume (add your file here)
```

## Adding content

- Theme tokens (colors, fonts) live in `src/styles.css` under `@theme`.
- Reusable component classes (`card`, `chip`, `btn-primary`, `nav-link`, …) live in `@layer components`.
- Rebuild after editing: `npm run build`.

## Deploy

Push to `main`. GitHub Pages serves the repo root. `resume.pdf` and `images/me.jpeg` are referenced directly.
