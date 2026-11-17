# Infin Group Website

Official company website for **Infin Group**, a Gauteng-based provider of integrated **security**, **cleaning** and **construction** services.

> Reliable, professional and efficient security, cleaning and construction services across Gauteng.

---

## About the company

Infin Group is an emerging service provider serving offices and commercial premises, residential clients, shared facilities, events and building projects. Offering all three services under one roof gives clients a single, dependable point of contact instead of several suppliers to manage.

| | |
|---|---|
| **Mission** | Deliver dependable security and cleaning services that protect people and property and promote a clean, safe and welcoming environment. |
| **Vision** | To be recognised as the leading provider of integrated security and cleaning solutions, setting the benchmark for quality, innovation and customer satisfaction. |

### Services

- **Security:** 24/7 patrols, access control systems, surveillance monitoring, event security management, risk assessment and consulting
- **Cleaning:** office and commercial, residential, deep cleaning, shared spaces and facilities, post-construction
- **Construction:** building and renovations, maintenance and repairs, painting and finishing, paving and boundary work, project management

## About this repository

A fast, dependency-free static site built with plain HTML and CSS. No build step, no framework, no package manager.

**Features**

- Single-page layout: About, Services, Team, Why Us, Contact
- Responsive, mobile-first design
- Automatic light and dark mode (follows the visitor's system setting) with matching logo variants
- Sticky navigation with smooth scrolling
- SEO and social sharing meta tags
- Auto-deploys to GitHub Pages on every push to `main`

## Project structure

```
infin-group-website/
├── index.html                  # Page content
├── css/
│   └── styles.css              # All styling, with colour tokens in :root
├── assets/
│   └── images/
│       ├── logo-on-light.png   # Logo for light backgrounds
│       └── logo-on-dark.png    # Logo for dark backgrounds
├── .github/
│   └── workflows/
│       └── pages.yml           # GitHub Pages deployment
├── .gitignore
├── LICENSE
└── README.md
```

## Run locally

No installation needed. Either open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

### GitHub Pages (included)

1. Push this repository to GitHub.
2. Go to **Settings → Pages** and set **Source** to **GitHub Actions**.
3. Push to `main`. The workflow in `.github/workflows/pages.yml` publishes the site.

### Custom domain (infingroup.net.za)

1. In **Settings → Pages → Custom domain**, enter your domain.
2. At your DNS provider, add the records GitHub lists (A records for the apex domain, or a CNAME for `www`).
3. Tick **Enforce HTTPS** once the certificate is issued.

## Editing content

| To change | Edit |
|---|---|
| Company text, services, team, contact details | `index.html` |
| Colours, fonts, spacing | `css/styles.css` (variables at the top, in `:root`) |
| Logos | Replace the files in `assets/images/` (keep the same names, transparent PNG) |

## Content still to complete

These placeholders from the original company profile are still in `index.html`:

- [ ] Team names for **Operations Manager**, **Team Supervisor** and **Control Room**
- [ ] Social media handles (Contact section currently reads "[handle to confirm]")
- [ ] Confirm which email addresses should be public (personal addresses for the CEO and Admin Manager are currently listed)
- [ ] Add registration details if desired (company registration number, PSIRA registration for the security division, CIDB grading for construction, B-BBEE certificate)
- [ ] Add a physical address or service-area map, if applicable

## Suggested next steps

- Add a contact form (for example Formspree or Netlify Forms, since the site is static)
- Add a favicon and a social sharing image (`og:image`)
- Add project photos or a "Clients & Projects" section
- Add a short privacy notice if you start collecting enquiries

## Contributing

This is a private company project. Create a branch, make your change, and open a pull request for review before merging to `main`.

## License

Copyright © Infin Group. All rights reserved. See [LICENSE](LICENSE).

## Contact

- Email: info@infingroup.net.za
- Phone: 067 606 7754
