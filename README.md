# GILITOGES — Courier & Delivery Services (Website)

Static website for GILITOGES (Gift Lifumbo Towing and General Services) — a courier concierge service operating in Lusaka, Zambia. This repository contains a lightweight, responsive single-page HTML site for booking pickups and deliveries via WhatsApp or email.

## Files

- `Index.html` — Main site HTML (entry point).
- `gilitoges-website.html` — Alternate/backup copy of the site HTML.
- Images are embedded as data URIs inside the HTML files.

## Features

- Responsive single-page layout with CSS-only styling.
- Booking form that opens a pre-filled WhatsApp message or email with the request details.
- Floating WhatsApp quick-chat button for immediate contact.
- Coverage list and service descriptions for customers in Lusaka.

## Run locally

Since this is a static site, you can open `Index.html` directly in your browser. For a better local experience (so links and relative resources work like a server), run a simple static server:

Using Python 3:

```
# serve current directory at http://localhost:8000
python3 -m http.server 8000
```

Then open http://localhost:8000/Index.html in your browser.

Or with Node (install `serve` first):

```
npm install -g serve
serve -s .
```

## Deploy

A quick option is GitHub Pages — push the repo to GitHub and enable Pages from the repository settings, serving from the `main` (or `gh-pages`) branch. You can also host on any static host (Netlify, Vercel, Surge, etc.).

## Configuration

The WhatsApp number and owner email are defined in the embedded script at the bottom of the HTML files:

- `WHATSAPP_NUMBER` — international phone number without `+` or spaces (e.g. `260776801806`).
- `OWNER_EMAIL` — email address used in the mailto link.

Edit these values directly in the HTML files if you need to change contact details.

## Accessibility & Improvements (suggestions)

- Add form-server integration to store booking requests (e.g., a serverless function, email service, or Google Forms) instead of relying only on client mail/WhatsApp.
- Move inline styles to a separate CSS file for maintainability.
- Extract images from data URIs into an `/assets/` folder to reduce HTML size and ease editing.
- Add basic unit tests or HTML validation and CI (GitHub Actions) for automated deploys.

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-change`
3. Commit your changes: `git commit -m "Add feature"`
4. Push to your branch and open a pull request

## License

This repository does not include a license file. If you want to make the project open-source, consider adding an open license (for example, MIT). Example `LICENSE` contents (MIT) can be added on request.

## Contact

Owner / contact listed in the site: Gift Lifumbo — lifumbogift92@gmail.com · +260 776 801 806

---

If you want, I can also:
- Add a small GitHub Actions workflow to deploy the site to GitHub Pages automatically.
- Split CSS and JS into separate files and update HTML.
- Add a LICENSE file (MIT) and create it for you.

Tell me which of these you'd like me to do next and I'll make the changes.