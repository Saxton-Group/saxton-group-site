# Saxton Group

A single-page consulting and executive coaching website. The page uses plain HTML and CSS and has no runtime dependencies or build step.

## Local development

Run `python3 -m http.server 4173 --directory dist` from this repository and visit `http://localhost:4173`.

## Contributing

Edit `dist/index.html` and `dist/styles.css`. Keep the page accessible and responsive, and verify internal links, contact links, and images before publishing. Keep authored files under `dist/` tracked. The firm name appears in the HTML title, metadata, header, and footer.

The legacy site supplied Bruce Saxton's biography, the firm's founding year, client scope, and portrait. Contact details and contact links are temporarily omitted while new ones are established. Do not introduce unverified coach credentials, client names, or testimonials.

## Hosting

Sites hosts the static files in `dist/`. The project identity is stored in `.openai/hosting.json`. This is an independent repository and does not require the containing workspace.
