# deadserious.ai

One-page static website for the Dead Serious LLC business, hosted on GitHub Pages at https://deadserious.ai/.

## Stack & layout
- Plain static HTML/CSS, no build step, no dependencies. All CSS and JS are inline in `index.html`.
- `index.html` — the whole site: header, hero, "What we do" (3 cards), "How we work", contact, footer.
- `favicon.ico` (16/32/48/64) and `apple-touch-icon.png` (180) — red "DS" on a dark rounded square, generated with Pillow (no source logo exists yet).
- `CNAME` — custom domain `deadserious.ai`. Don't delete or the domain breaks.
- `.nojekyll` — serve files as-is.
- `README.md` — local preview and DNS/Pages setup.

## Hosting
- Repo: `git@github.com:dmitryvmr/deadserious.git`, branch `main`.
- GitHub Pages deploys from `main` / root. Pushing to `main` deploys automatically (check with `gh api repos/dmitryvmr/deadserious/pages/builds/latest`).
- Preview locally: `python3 -m http.server 8000`.

## Content decisions
- Do NOT mention "Dead Serious LLC" / "LLC" anywhere on the site. The brand name "Dead Serious" (logo, titles) and "deadserious.ai" are fine. Footer reads "© <year> deadserious.ai".
- Contact email is `support@deadserious.ai` (mailbox/forwarding must be set up separately). Don't use `hello@`.
- Marketing copy (AI strategy / custom build / advisory, "How we work") is placeholder guesswork from the `.ai` domain. The user hasn't described what the business actually does — confirm before treating it as final.

## Design
- Dark theme with red accent (`--accent`), auto light mode via `prefers-color-scheme`. System font stack. Mobile-friendly; respects reduced motion.
- Colors are CSS variables in `:root` at the top of `index.html`.

## Conventions
- Commit messages end with the Co-Authored-By / Claude-Session attribution lines.
- Push to `main` only when the user asks (they've asked each time so far).
