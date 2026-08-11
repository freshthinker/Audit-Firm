# Aakash & Associates — Audit Firm Website

A modern, fully responsive corporate website for **Aakash & Associates**, an audit, tax, risk and transaction advisory firm — built in the bold yellow-and-charcoal visual language of Big 4 firms like EY.

## Pages

| Page | Description |
|---|---|
| `index.html` | Home — hero, services overview, stats, industries, insights, testimonials, CTA |
| `about.html` | Firm history, values, timeline and leadership team |
| `services.html` | Audit & Assurance, Tax Advisory, Risk & Consulting, Transaction Advisory, process, engagement models |
| `industries.html` | Sector expertise across 8 industries |
| `insights.html` | Articles, reports and newsletter signup |
| `careers.html` | Why join, perks, open roles |
| `contact.html` | Contact form, office locations, FAQ |
| `404.html` | Custom not-found page |

## Tech

Plain **HTML5 / CSS3 / vanilla JavaScript** — no build step, no framework, no dependencies. Fonts load from Google Fonts (Poppins + Inter); all icons are inline SVG.

```
├── index.html
├── about.html
├── services.html
├── industries.html
├── insights.html
├── careers.html
├── contact.html
├── 404.html
├── css/style.css      # design system + all page styles
├── js/main.js          # nav, scroll reveal, counters, FAQ, forms
├── assets/favicon.svg
└── .github/workflows/pages.yml
```

## Running locally

No build tools required — just open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying to GitHub Pages

A workflow at `.github/workflows/pages.yml` deploys the site automatically on every push to `main`. To enable it:

1. Push this repository to GitHub.
2. Go to **Settings → Pages** and set **Source** to **GitHub Actions**.
3. Push to `main` (or run the workflow manually from the **Actions** tab) — your site will be live at `https://<your-username>.github.io/<repo-name>/`.

## Customizing

- **Brand name & copy**: search-and-replace "Aakash & Associates" and edit copy directly in each HTML file.
- **Colors**: all brand colors are CSS variables at the top of `css/style.css` (`--yellow`, `--black`, `--charcoal`, etc.) — change them once and the whole site updates.
- **Images**: hero and section images are hotlinked from Unsplash for demo purposes — replace the `url('...')` references with your own photography before going live.
- **Contact form**: the form in `contact.html` is a front-end demo (no backend). Wire it up to a form service (Formspree, Netlify Forms, etc.) or your own backend before production use.
