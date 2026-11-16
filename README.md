# veliyat.com

Personal site of **Ravi Veliyat** — Tech Lead, full-stack engineer and developer educator.

Built text-first with plain semantic HTML and CSS: zero JavaScript, zero external dependencies, no build step, and system font stack only.

## Preview Locally

```bash
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000). Run from the repository root because internal links and assets are root-relative.

## Project Structure

```
├── index.html            # Home
├── work/
│   └── index.html        # Engineering work & projects
├── teaching/
│   └── index.html        # Developer education & corporate training
├── videos/
│   └── index.html        # Developer tutorial videos catalog
├── about/
│   └── index.html        # Biography & career timeline
├── resume/
│   └── index.html        # Print-optimized CV (targets 2 A4 pages)
├── 404.html              # Custom 404 error page
├── assets/
│   ├── css/
│   │   └── site.css      # The single site stylesheet (light/dark/print/responsive)
│   └── img/
│       ├── favicon.svg   # Favicon
│       ├── social.jpg    # Open Graph social preview (1200 × 630)
│       ├── ravi-pic-big.jpg   # Portrait image
│       └── ravi-pic-big.webp  # Modern WebP portrait asset
├── robots.txt            # Search engine crawler directives
├── sitemap.xml           # XML sitemap for search indexing
└── .gitignore            # Git ignore rules
```

## Design Principles

- **Zero JavaScript**: Pure semantic HTML5 and modern CSS (`:has()`, `clamp()`, CSS Grid, Flexbox).
- **Single Stylesheet**: All rules, themes, animations, and print media queries live in `assets/css/site.css`.
- **System Fonts**: Native font stack (`system-ui`, `-apple-system`, `BlinkMacSystemFont`, `Segoe UI`, `Roboto`) for zero network latency and crisp rendering.
- **Dark & Light Modes**: Automatic palette switching via `prefers-color-scheme` (refined linen light theme and slate dark theme).
- **Responsive Layout**: Fluid typography with `clamp()`; header navigation engineered to fit on a single line at mobile widths (390px); mobile hero arranges portrait and heading side-by-side without dangling space.
- **Print Optimization**: Dedicated `@media print` rules on `/resume/` engineered to fit cleanly onto exactly two A4 pages.
- **Consistent Navigation**: Header navigation (`Home`, `Work`, `Teaching`, `Videos`, `About`, `Resume`) and footer links are structurally consistent across all pages, with `aria-current="page"` set on the active page.

## Site Metadata & Address

`https://veliyat.com` is used in canonical `<link>`, Open Graph, Twitter Cards, and schema.org `ProfilePage` JSON-LD structured data. Each page maintains this block under `SITE-ADDRESS`.

## Status & Open Items

### Completed
- [x] Header navigation updated with `Home` as first link; site name removed per brief v5.
- [x] Portrait image integrated on Home and About (`assets/img/ravi-pic-big.jpg` / `.webp`) with responsive side-by-side mobile layout.
- [x] Work: Optivo Health product tour descriptive button (`https://www.optivohealth.com/product-tour`).
- [x] Work: AI Coding Tutor live app link (`https://ai-coding-tutor-taupe.vercel.app/`) with subtext code icon pointing to GitHub source.
- [x] Work: Verified and linked all GitHub code repositories.
- [x] Resume: Added contact line under `h1`, restored product description subhead, and verified two-page A4 print layout.
- [x] Videos: Meta description and intro updated; group headings hidden pending video catalog.

### Remaining / Waiting on Content
- [ ] Three selected videos for Home: titles and YouTube URLs.
- [ ] Videos page: exact titles, URLs, and group categorisation (AI & Python, React & Redux, JavaScript & Node.js, Angular).
- [ ] Work: update Optivo launch-status copy when Optivo goes live.
- [ ] Resume: replace Google Drive PDF link before launch if a new revision is exported.
- [ ] Review social share card `assets/img/social.jpg` (1200 × 630).
- [ ] Verify Fightrons wording against `fightrons.com` prior to public launch.
