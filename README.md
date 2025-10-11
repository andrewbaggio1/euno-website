# euno-website

Static site for GitHub Pages.

## Edit Locally

- Open `index.html` in a browser (double-click) to preview.
- Edit `index.html` and assets in `assets/`.

## Publish with GitHub Pages

1. Commit and push changes to `main`.
2. In GitHub → Repository `Settings` → `Pages`:
   - Build and deployment: `Deploy from a branch`
   - Branch: `main` (root)
3. Wait ~1–3 minutes. Your site will be live at your repo’s Pages URL or your custom domain.

## Custom Domain (`CNAME`)

`CNAME` contains:

```
euno.ai
```

In `Settings` → `Pages` → `Custom domain`, enter `euno.ai` and enable HTTPS. GitHub will auto-provision a TLS cert once DNS is correct.

### DNS

- If `euno.ai` is an apex/root domain, add A (and optionally AAAA) records pointing to GitHub Pages. See the latest IPs here: `https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site`.
- If using `www.euno.ai`, create a CNAME record pointing to `<username>.github.io` (or the repo domain GitHub shows).

Keep the `CNAME` file in the repo root so Pages keeps your domain attached.

## No Jekyll

`.nojekyll` ensures static files are served as-is (no Jekyll processing).
