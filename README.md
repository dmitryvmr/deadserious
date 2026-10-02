# deadserious.ai

One-page website for Dead Serious LLC. Plain static HTML/CSS — no build step.

## Local preview

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Hosting (GitHub Pages)

1. Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main` / `(root)`.
2. The `CNAME` file sets the custom domain to `deadserious.ai`.
3. At your DNS provider, add:

   | Type  | Host  | Value                  |
   |-------|-------|------------------------|
   | A     | `@`   | `185.199.108.153`      |
   | A     | `@`   | `185.199.109.153`      |
   | A     | `@`   | `185.199.110.153`      |
   | A     | `@`   | `185.199.111.153`      |
   | CNAME | `www` | `<github-username>.github.io` |

4. Once DNS propagates, tick **Enforce HTTPS** in the Pages settings.
