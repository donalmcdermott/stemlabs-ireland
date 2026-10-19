# STEM Labs Ireland website

Static single-page site, ready for GitHub Pages. No build step, no JavaScript,
no dependencies beyond two Google Fonts.

## Files

- `index.html` — the whole site
- `styles.css` — all styling

## Deploy to GitHub Pages

1. Create a new public repo (e.g. `stemlabs-ireland` or `stemlabs.ie`).
2. Push these two files to the repo's root on the `main` branch.
3. Repo Settings > Pages > Source: "Deploy from a branch", Branch: `main`, folder `/ (root)`.
4. The site will be live at `https://<user>.github.io/<repo>/` within a minute or two.

## When the domain is bought

1. In the repo, add a file named `CNAME` containing just the domain (e.g. `stemlabs.ie`).
2. At your DNS provider, point the domain at GitHub Pages:
   - Apex (`stemlabs.ie`): A records to `185.199.108.153`, `185.199.109.153`,
     `185.199.110.153`, `185.199.111.153`
   - Or `www`: CNAME to `<user>.github.io`
3. Tick "Enforce HTTPS" in the Pages settings once DNS resolves.

## Things to change before going live

- `hello@stemlabs.ie` is used for contact and the grants "Register interest"
  button. Swap it for the real address when the domain is set up
  (search-and-replace across `index.html`).
- The founder quote is a draft written for Donal. Tweak or replace it with his
  own words.
- Breakpoint is deliberately vague (no Luma link, no event details) per request.
