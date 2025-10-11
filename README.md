# Stamatis Petridis — Cloudflare Resume

This repository contains the source for the single-page resume of Stamatis Petridis. The site is a static HTML document hosted on Cloudflare Pages and optimized for quick loading, easy printing, and remote-friendly sharing.

## Repository Layout
- `index.html` — Main resume content and inline styles.
- `cvphoto.jpg` — Profile photo referenced in the header.
- `_headers`, `_redirects` — Optional Cloudflare Pages metadata for HTTP headers and redirects.

## Local Preview
No build step is required. Serve the root directory with any static file server to preview the page locally.

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080` in your browser. Use the “Print / Save as PDF” button in the header to generate a print-friendly version.

## Updating Content
1. Edit `index.html` to adjust text, sections, or styling. The document uses semantic HTML and a minimal inline stylesheet.
2. Replace `cvphoto.jpg` with a new portrait if needed. Keep the filename identical to avoid breaking the `<img>` tag.
3. Verify that contact links, canonical URL, and Open Graph metadata remain up to date.

## Deployment
The site is designed for Cloudflare Pages:

1. Connect the repository to Cloudflare Pages and select the root directory as the build output.
2. Choose the “Direct Upload” option or configure Pages to serve the repository as-is (no build command necessary).
3. Publish. The resume will be available at the configured Pages domain (currently `stamatispetridisresume.pages.dev`).

For manual deployments you can use Wrangler:

```bash
wrangler pages deploy .
```

## Maintenance Checklist
- ✅ Update experience, certifications, and projects quarterly or whenever major milestones occur.
- ✅ Confirm the timestamp script still renders correctly in browsers you support.
- ✅ Test the print view after significant layout changes to ensure the PDF exports cleanly.

## Support
For questions or collaboration, reach out via the contact details listed in the resume header.
