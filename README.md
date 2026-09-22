# Saxton Group

A single-page consulting and executive coaching website. The page uses plain HTML and CSS and has no runtime dependencies or build step.

## Local development

Run `python3 -m http.server 4173 --directory dist` from this repository and visit `http://localhost:4173`.

## Contributing

Edit `dist/index.html` and `dist/styles.css`. Keep the page accessible and responsive, and verify internal links, contact links, and images before publishing. Keep authored files under `dist/` tracked. The firm name appears in the HTML title, metadata, header, and footer.

The legacy site supplied Bruce Saxton's biography, the firm's founding year, client scope, and portrait. Bruce’s Ernst & Young Entrepreneur Of The Year award was confirmed by the site owner. Contact details and contact links are temporarily omitted while new ones are established. Do not introduce unverified coach credentials, client names, or testimonials.

Incoming biographies and photographs may be placed in `incoming/`, which is excluded from Git. Only reviewed public profile copy and selected portrait assets belong in `dist/`. Kristen Chin’s bio and portrait were supplied by the site owner. Additional team members use the reusable `consultant-profile` layout.

## Hosting

The source repository is [Saxton-Group/saxton-group-site](https://github.com/Saxton-Group/saxton-group-site). The production branch is `main`.

### GitHub Pages review

The `Publish review site to GitHub Pages` workflow publishes only the static files in `dist/`. Run it manually from the repository's Actions tab on `main`. GitHub Pages uses **GitHub Actions** as its source. Publication is manual so pushing a change does not automatically update the review site.

The repository and [GitHub Pages review site](https://saxton-group.github.io/saxton-group-site/) are public, as authorized by the owner. Anyone can view them, including people outside the organization.

The repository history was cleaned of retired contact details before publication. Do not merge old history from the legacy Sites repository or private archive; transfer any needed changes as reviewed file edits to avoid restoring removed contact data.

Asset references are relative so the page works both at a domain root and under a GitHub Pages project path.

### Future production hosting

The planned production workflow is GitHub → Cloudflare Pages. Connect this repository, select `main`, use no framework preset, and publish the `dist` directory. The site requires no build step. The Cloudflare connection and final domain are not configured yet.

The existing private Sites publication remains a review copy. Its project identity is stored in `.openai/hosting.json`; that file is not needed by Cloudflare. The `origin` Git remote points to GitHub and the `sites` remote preserves the review site's source repository.

This is an independent repository and does not require the containing workspace.
