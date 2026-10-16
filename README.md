# Fii website

Static pages for the stores: landing page, privacy policy, terms, support and account deletion
(each in Turkish and English). Built by `tools/make_site.py`; edit the texts there and run
`python3 tools/make_site.py` from the repo root.

## Publish free on GitHub Pages (about 5 minutes, no domain needed)

1. Sign in to github.com as `OguzhanKaracorlu`. The address becomes
   `https://oguzhankaracorlu.github.io/fii/` (GitHub writes the user name in lower case;
   the app already uses this address, see `app/src/lib/brand.ts`).
2. New repository → name `fii` → Public → Create.
3. "uploading an existing file" → drag in everything from this folder (the .html files,
   style.css, icon.png, favicon.png) → Commit changes.
4. Settings → Pages → Source: "Deploy from a branch", Branch: `main`, folder `/ (root)` → Save.
5. After a minute the site is live. Store forms:
   - Privacy policy URL: `https://oguzhankaracorlu.github.io/fii/privacy.html`
   - Account deletion URL (Google Play): `https://oguzhankaracorlu.github.io/fii/delete-account.html`
   - Support URL (App Store): `https://oguzhankaracorlu.github.io/fii/support.html`
   - Marketing URL (optional): `https://oguzhankaracorlu.github.io/fii/`

To update a page later: run the script, then upload the changed files to the same repository.
A custom domain can be added later in Settings → Pages without changing anything else.
