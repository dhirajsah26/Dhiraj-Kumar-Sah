# dhiraj-sah.com.np

Personal site of Dhiraj Kumar Sah. Plain static HTML and one stylesheet — no build step, no framework. Deployed with GitHub Pages at `www.dhiraj-sah.com.np` (see `CNAME`).

## Structure

```
index.html            home
about/ work/ projects/ contact/   one index.html each
writing/              essay index + one folder per essay
css/site.css          all styles (design tokens at the top)
assets/               favicon, OG image, photo, CV
sitemap.xml robots.txt llms.txt feed.xml
404.html
```

## Editing

- Each page is a complete HTML file. Header and footer are repeated in every file; if you change the nav, change it everywhere (search for `site-nav`).
- To add an essay: copy an existing folder under `writing/`, edit the title, date, description, body and the JSON-LD block in `<head>`; then add it to `writing/index.html`, `index.html` (Writing list), `sitemap.xml`, `feed.xml` and `llms.txt`.
- Swap in real files at `assets/dhiraj-kumar-sah.jpg` (square, at least 600×600) and `assets/dhiraj-kumar-sah-cv.pdf`.
- Fonts load from Google Fonts (STIX Two Text, IBM Plex Sans/Mono). To self-host, drop the files in `assets/fonts/` and replace the `<link>` in each page.

## After deploying

1. Submit `https://www.dhiraj-sah.com.np/sitemap.xml` in Google Search Console and Bing Webmaster Tools.
2. Check the home page with Google's Rich Results Test (Person + WebSite schema) and a social-card preview tool (OG image).
3. Enable "Enforce HTTPS" in the repo's Pages settings if it isn't already.
