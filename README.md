# InAmigos Foundation — NGO Awareness Webpage

A single-page, responsive HTML5 + CSS3 website introducing InAmigos Foundation,
its six ongoing projects, its verified social impact, and ways to get involved.

## Files

```
ngo-awareness/
├── index.html      Full page markup (semantic HTML5, one page)
├── style.css       All styling (CSS variables, responsive layout, no frameworks)
├── images/
│   └── README.txt  Suggested filenames + specs for swapping in real photos
└── README.md        This file
```

No JavaScript, React, Bootstrap, or Tailwind is used anywhere. The mobile menu
is built with the pure-CSS "checkbox hack" (a hidden checkbox + label), so the
hamburger menu works with zero script.

## Research sources used

All facts, project names, statistics, and copy on this page were verified
against InAmigos Foundation's **official** channels — nothing was invented:

- Official website: https://inamigosfoundation.org.in/ (home page + About Us page)
- Official Facebook page: https://www.facebook.com/inamigos.inamigos
- Official Instagram page: https://www.instagram.com/inamigos/

Specific facts pulled from these sources include: founding date (23 September
2020), founder name (Mr. Govind Shukla), registration status (Section 8,
80G & 12A, CSR‑1, NITI Aayog, ISO 9001:2015), headquarters address (Bilaspur,
Chhattisgarh), the six named projects (Seva, Bachpanshala, Jeev, Udaan,
Prakriti, Vikas) with their official descriptions, the published impact
numbers (50,000+ beneficiaries, 28 states, 200 volunteers, 30,000+ interns
trained, 20,000+ saplings planted), and three verified 2025 events (World
Water Day, International Day of Happiness, International Day of Women and
Girls in Science) with their official dates.

Third-party "intern portfolio" clones of this same brief were deliberately
**not** used as content sources — only the organisation's own website and
official social pages were treated as ground truth, per the brief's
instructions. A couple of independent NGO-directory listings (which quote the
same official About Us text) were used only to cross-check consistency of
the numbers above.

No statistics, project names, dates, or achievements beyond what's stated on
official InAmigos channels were added.

### A note on images

The hero, About section, and all six project cards now show real
photographs (community volunteers, a rural Indian classroom, an animal
shelter, a tree‑planting drive, and so on) sourced as free-to-use stock
photos from Pexels and hotlinked directly from images.pexels.com — no
attribution is required under the Pexels License. Real photographs from
InAmigos' own Instagram/Facebook are copyrighted by the foundation, so
those were not pulled into this third-party project without permission.
See `images/README.txt` for the exact photo credits/URLs and instructions
for swapping in official, permitted photos later.

## Running the webpage locally

No build step or server is required.

1. Download or copy the `ngo-awareness` folder to your computer, keeping
   `index.html`, `style.css`, and the `images/` folder together in the same
   directory structure shown above.
2. Double-click `index.html`, or right-click it and choose **Open with →**
   your browser (Chrome, Edge, Firefox, Safari all work).
3. To preview it exactly as it would look when hosted, you can optionally
   serve it locally instead of opening the file directly:
   - **VS Code**: install the "Live Server" extension, right-click
     `index.html`, choose **Open with Live Server**.
   - **Python** (if installed): run `python -m http.server 8000` inside the
     `ngo-awareness` folder, then visit `http://localhost:8000` in a browser.
4. Resize the browser window (or open dev tools' device toolbar) to check the
   responsive behavior at desktop, tablet, and mobile widths.

## Final checklist

| # | Requirement | Status |
|---|---|---|
| 1 | All required sections present (nav, hero, about, projects, impact, highlights, CTA, footer) | ✅ |
| 2 | Information about the NGO is factually accurate | ✅ Verified against official website + social pages |
| 3 | Projects based on official sources only | ✅ All six projects match the official "Key Initiatives" list |
| 4 | No fabricated information | ✅ Only published numbers/dates used; no invented stats |
| 5 | Images are relevant | ✅ Free-licensed stock photos matched to each section's real content (community, classroom, animal shelter, tree planting, etc.); swap-in instructions for official photos in `images/README.txt` |
| 6 | Buttons and links work | ✅ Nav links scroll to in-page sections; CTA buttons point to the foundation's real volunteer form, donation link, and Instagram |
| 7 | Webpage is responsive | ✅ Mobile-first CSS with breakpoints at ~700px, ~900px, ~1050px |
| 8 | Polished on desktop, tablet, mobile | ✅ Layout reflows from single column to multi-column grids; sticky nav collapses to a CSS-only hamburger menu |
| 9 | HTML/CSS free of obvious errors | ✅ Semantic tags, closed elements, valid CSS custom properties |
| 10 | Suitable for screenshot-based evaluation | ✅ Clear visual hierarchy, consistent color system, no lorem ipsum, no placeholder-looking sections |

## Design notes

- **Palette**: deep forest green (`#1B5E4A`) for trust/growth, warm gold
  (`#D9A441`) for hope/warmth, a soft teal (`#4C8C86`) as a secondary accent,
  and a warm cream background (`#FAF7F1`) — deliberately avoiding both the
  generic "AI beige + terracotta" look and the identikit SaaS-card kit.
- **Type**: Fraunces (a warm serif with character) for headlines, Work Sans
  for body copy and UI — one strong contrast pair rather than three or more
  typefaces.
- **Layout**: hero and about sections use an asymmetric split rather than a
  centered hero-with-background-image default; project cards use a colored
  top border keyed to each project rather than uniform grey cards; the
  impact section is intentionally the one dark, high-contrast moment on the
  page.
