# M.M. Knitwear Ltd. — Corporate Website

Official corporate website for [M.M. Knitwear Ltd.](https://www.mmknitwear.com), a 100% export-oriented knitwear manufacturer in Bangladesh, in operation since September 2001. The site is a static multi-page site hosted on GitHub Pages.

## Company at a Glance

- **Established:** September 2001
- **Capacity:** 200,000 garments per day
- **Floor space:** 15,23,000 sqft
- **Workforce:** 10,982 employees
- **Annual turnover:** $140M (2026)
- **Owned facilities:** Knitting, dyeing, AOP, printing, embroidery, cutting, laundry, sampling & CAD, and garmenting — with an in-house ETP (280 m³/hr)

## Pages

| Page | Purpose |
| --- | --- |
| `index.html` | Home — hero, capacity counters, accreditation grid |
| `about-us.html` | Company profile, facilities at a glance, business growth, building description, team |
| `projects.html` | Production divisions: knitting, dyeing, garments, AOP, printing, embroidery, sample & CAD, cutting, laundry |
| `out-projects.html` | Subcontracting / outsourcing capabilities |
| `portfolio.html` | Showcase of products with Mens / Womens / Kids filter and lightbox gallery |
| `compliance.html` | Compliance & sustainability, GHG reduction roadmap, CSR |
| `newspaper.html` | Press & news |
| `contact.html` | Head office (Uttara, Dhaka) and factory (Gazipur) contact details |

## Tech Stack

- Plain HTML5 / CSS3 / JavaScript (jQuery), based on the GoodLayers "Kleanity" theme
- No build step — files deploy as-is
- Google Fonts, Font Awesome icons, Isotope filtering, iLightbox galleries
- Google Analytics (`G-70FWYE26S8`)
- Hosted on **GitHub Pages** (branch `main`, repo root)

## Repository Structure

```
├── *.html            # One page per route (index, about-us, projects, ...)
├── css/              # Theme and page-builder stylesheets
├── js/               # jQuery, theme scripts, Isotope, page-builder
├── fonts/            # Icon and display fonts
├── images/           # Logos, gallery photos, social/OG images
├── upload/           # Facility photos, product photos, downloadable PDF
├── quform/           # Contact form backend
├── sitemap.xml       # Search-engine sitemap
├── robots.txt
├── CNAME             # www.mmknitwear.com
└── _assets-2026/     # Working copy of the 2026 company profile source (git-ignored)
```

## Deployment

The site is deployed with GitHub Pages. Pushing to `main` triggers a rebuild:

```bash
git add .
git commit -m "Update content"
git push origin main
```

Changes go live at https://www.mmknitwear.com once the Pages build finishes (usually under a minute).

## Local Preview

Serve the repo root and open the output in a browser:

```bash
python -m http.server 8080
# open http://127.0.0.1:8080/index.html
```

> **Note:** some theme scripts reference an external demo WordPress AJAX URL; it does not affect static page rendering.

## Maintenance Notes

- Keep meta descriptions at or under 130 characters; one `<h1>` per page.
- New photos: upload full-resolution originals to `upload/` and reference them with plain relative paths (e.g. `upload/product-1.jpg`).
- The downloadable company profile (`upload/Company-Profile-Of-MM-Knitwear-Ltd.pdf`) is the current 22-page 2026 edition.

---

© 2026 M.M. Knitwear Ltd. All rights reserved.
