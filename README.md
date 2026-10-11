# INLAND LUXURY — multi-page interior design website

## Run locally

This is a static HTML/CSS/JavaScript website. No build step or package installation is required. From this directory run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`. Keep the folder structure intact. Every page is a standalone HTML file, so direct routes and refreshes work on static hosting.

## Pages and routing

`routes.json` is the route inventory. There are **49 HTML routes** including the homepage, core pages, services, room inspiration, calculators, three illustrative project detail pages, material collections, and legal pages. `sitemap.xml` and `robots.txt` are included.

## Functionality

- Sticky header with a precisely centered wordmark, desktop mega-menus and mobile navigation.
- Search across page titles, categories and descriptions.
- Static homepage hero with a single headline, description, background image and consultation calls to action.
- Room/material horizontal scrolling, service tabs, FAQ accordions and project filtering.
- Full-home, kitchen and wardrobe estimators with live ranges and WhatsApp handoff.
- Consultation form validation and prefilled WhatsApp handoff. It does **not** falsely claim server-side submission.
- SEO titles, descriptions, canonical URLs, sitemap and robots file.

## Important production notes

1. Images use remote Unsplash image URLs and require internet access. Replace them with licensed, approved, locally hosted assets before launch and verify image rights.
2. The homepage hero uses a static remote image. Confirm image rights and replace it with an approved, locally hosted asset before launch if needed.
3. Portfolio pages are explicitly illustrative concepts, not verified completed projects.
4. The supplied source files did not contain review text for Sudhanshu Singh, Mohit Avana or Samash Tarvez. The review section is intentionally marked pending verification rather than fabricating quotes. Insert the exact approved wording before publication.
5. Estimator rates are illustrative, configurable assumptions in `scripts/site.js`. They are not Inland Luxury pricing. Replace them with owner-approved data before promoting the tool.
6. The form opens WhatsApp at +91 96543 80951 with a prefilled message. It does not send data to a server or CRM. Confirm the number is WhatsApp-enabled.
7. Founder and CEO is listed as Gurmmit Singh only where owner-approved content is added; no founder biography or portrait is fabricated.
8. The contact address and Instagram URL are based on the supplied business details. Verify address and contact details before launch.
9. Deploy the entire folder to static hosting. Since every route is a physical HTML file, no SPA rewrite rules are needed.

## QA status

- Automated structure check: every route in `routes.json` maps to a generated HTML file.
- Local code checks: HTML page count, shared stylesheet/script references, key interaction hooks and relative internal links are checked by the build script.
- Not claimed as tested: live image loading, cross-browser visual QA, mobile device QA, browser console inspection or WhatsApp delivery. Those require running the site in a browser and validating the live environment.
