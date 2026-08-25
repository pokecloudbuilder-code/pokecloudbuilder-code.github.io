# AGENTS.md

Read `/Users/kidayuichi/Documents/repos/CODEX_CONTEXT.md` before working in this repository.

サイトのデザインやかのうさを変更する前に、`docs/KANOUSA_BRAND.md` と `/Users/kidayuichi/Documents/repos/KanoUsaRoulett/design/kanousa-character.json` を必ず読む。

## Repository

- Path: `/Users/kidayuichi/Documents/repos/pokecloudbuilder-code.github.io`
- GitHub: `https://github.com/pokecloudbuilder-code/pokecloudbuilder-code.github.io`
- Public site: `https://www.pokecloudbuilder.com/`
- Hosting: GitHub Pages.
- Purpose: Static business/product page for pokecloudbuilder.

## Files

- `index.html`: Main business/product page.
- `contact.html`: Contact form and business information.
- `privacy-policy.html`: Privacy policy.
- `CNAME`: Custom domain for GitHub Pages.

## Services

- Contact form: Formspree endpoint `https://formspree.io/f/mredjzkz`.
- Business site hosting: GitHub Pages.
- Domain: `pokecloudbuilder.com`.
- Domain/DNS provider context: お名前.com is used for domain/DNS/mail according to project notes.

## Current Content Rules

- Public product cards on `index.html` must be ordered by release recency, newest public release first. Planned products stay after public products.
- Contact form app options should include every public product plus planned products that users might ask about.
- かのうさぎの日常スタンプ is public:
  - URL: `https://line.me/S/sticker/36098630`
  - Show it as the newest public product until a newer product is released.
- 立体視メーカー is public:
  - URL: `https://rittai.pokecloudbuilder.com/`
  - Zenn article: `https://zenn.dev/pokecloudlab/articles/stereoscopic-vision-maker-cloudflare-pages`
  - Product-specific article links should stay inside or near its product card.
- Jam Blocks is public:
  - URL: `https://jam.pokecloudbuilder.com/`
  - Zenn article: `https://zenn.dev/pokecloudlab/articles/jam-blocks-alpha`
  - Product-specific article links should stay inside or near its product card.
- 年齢・学年・和暦チェッカー is public:
  - URL: `https://nenrei.pokecloudbuilder.com/`
  - Zenn article: `https://zenn.dev/pokecloudlab/articles/age-grade-era-checker-cloudflare-pages`
  - Product-specific article links should stay inside or near its product card.
- かのうさルーレット is public:
  - URL: `https://kanousa.pokecloudbuilder.com/`
  - Zenn article: `https://zenn.dev/pokecloudlab/articles/kanousa-cloudflare-pages`
  - Product-specific article links should stay inside or near its product card.
- Scientific Calculator is not public yet:
  - Describe it as `公開予定`, `公開準備中`, or similar.
  - Do not imply it is already available on Google Play until released.
- General articles such as Google Play preparation should go in a development log or articles section.

## Workflow

1. Run `git pull --ff-only` before editing when the user asks for current/live updates.
2. Check `git status --short`.
3. Edit only relevant static files.
4. Avoid committing `.DS_Store`.
5. Verify locally when practical, for example with a temporary static server.
6. Commit with a concise message.
7. Push `main` to publish through GitHub Pages.
8. Check `https://www.pokecloudbuilder.com/` after propagation.

## Notes

- This is a simple static HTML site with inline CSS.
- Keep the page accurate and modest: public products first, planned products clearly marked, and articles placed where they provide context.
