# northboundsignal-site

Public marketing site for Northbound Signal &mdash; a 14-day placement-leak audit for founder-led specialty staffing firms.

Deployed via GitHub Pages from the `main` branch at <https://northboundsignal.com/>.

## Local preview

Plain static HTML / CSS &mdash; no build step. To preview locally:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Layout

- `index.html` &mdash; landing page
- `styles.css` &mdash; single stylesheet
- `404.html` &mdash; custom not-found page
- `assets/` &mdash; images
- `CNAME` &mdash; custom domain (`northboundsignal.com`)
- `.nojekyll` &mdash; disables GitHub Pages Jekyll processing
- `robots.txt`, `sitemap.xml`, `favicon.svg`, `apple-touch-icon.png` &mdash; standard ancillary files

## Image generation

Hero, OG, and apple-touch-icon images are generated via OpenAI&rsquo;s GPT Image 2. Prompts and review checklist live in the private agents repo.
