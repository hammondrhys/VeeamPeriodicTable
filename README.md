# VeeamPeriodicTable

The Veeam Ecosystem Periodic Table is a single-page web application built with HTML5, CSS3, and vanilla JavaScript. It presents the Veeam platform as a periodic-table-style interface with live search, category highlighting, and hover-driven product descriptions.

## Stack

- Static HTML
- Embedded CSS
- Embedded JavaScript
- No build step
- No runtime dependencies

## Project Structure

- `index.html` - the full application, including styles, data, and interaction logic
- `README.md` - project and deployment notes
- `LICENSE` - repository license

## Local Preview

Because the app is a static page, you can preview it by opening `index.html` directly in a browser.

## Cloudflare Pages Deployment

This repository is ready for Cloudflare Pages as a static site.

Use these settings when creating the Pages project:

- Framework preset: `None`
- Build command: leave blank
- Build output directory: `/`
- Root directory: leave blank unless you later move the app into a subfolder

Cloudflare Pages will serve `index.html` from the repository root.

## Git Workflow

To publish changes:

```bash
git add .
git commit -m "Describe your change"
git push origin main
```

## Notes

- The UI is optimized as a standalone static page for simple hosting.
- The data model for the periodic table is embedded directly in `index.html` for portability and easy testing.
