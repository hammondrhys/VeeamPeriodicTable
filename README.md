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

## Cloudflare Deployment

This repository is configured for Wrangler static asset deployment.

The included `wrangler.toml` tells Cloudflare to deploy the repository root as a static site, so a build step is not required.

If your Cloudflare project is currently running this deploy command, keep it as:

```bash
npx wrangler deploy
```

If you deploy from the command line locally, run the same command from the repository root.

Important notes:

- `index.html` is served from the repository root.
- Unknown routes fall back to `index.html`, which is useful for single-page app style routing.
- Because the assets directory is set to `.`, any additional files you place in the repository root can also be published unless you move the site into a dedicated output folder later.

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
