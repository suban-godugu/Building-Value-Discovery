# Building Value Discovery

Static web app (no build step, no backend). Files:

- index.html  page markup
- styles.css  all styling
- app.js      all logic and embedded data (OEH strategy matrix, sample bills/manual)

## Run locally
    python3 -m http.server 8080   # then open http://localhost:8080

## Deploy
Upload the folder as-is to any static host (Netlify, Vercel, GitHub Pages,
Cloudflare Pages, S3 + CloudFront, Azure Static Web Apps, nginx/Apache).
Publish directory = the folder root; no build command.

Needs internet access for CDN libraries (pdf.js 3.11.174, SheetJS 0.18.5,
html2canvas 1.4.1, jsPDF 2.5.1) and Google Fonts. For offline/intranet use,
download those and point the <script>/<link> tags in index.html to local copies.
