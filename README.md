# 無為 · Wu Wei

Personal site for 無為 / Wu Wei (`bianwuwei`) — useful software grounded in real problems.

Live: https://bianwuwei.github.io/portfolio/

## Structure

- Hero with bilingual toggle (中文 | EN)
- Works — quiet space for future case studies
- About — AI vision practice → personal tools
- Contact — email + WeChat

## Develop

Node.js >= 22.12 (or Bun).

```bash
bun install
bun --bun run dev
```

Preview: http://localhost:4321/portfolio/

## Build & publish (GitHub Pages via docs/)

```bash
bun --bun run build
rm -rf docs && cp -a dist docs && touch docs/.nojekyll
```

Astro config: `base: /portfolio/`.
