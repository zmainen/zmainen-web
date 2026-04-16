# Site Template

`page.html` is the canonical style template for zmainen.org. Copy it to start any new page.

## Placeholders

Replace these HTML comments with actual content:

| Placeholder | Where | What |
|:--|:--|:--|
| `<!-- TITLE -->` | `<title>` tag | Page title (appears before " — Zach Mainen") |
| `<!-- DESCRIPTION -->` | `<meta>` tag | One-line summary for search engines / link previews |
| `<!-- NAV -->` | Inside back-link `<a>` | Back-link text (e.g. "Zach Mainen" or "Selected Writing") |
| `<!-- HEADING -->` | `<h1>` | Page heading |
| `<!-- SUBTITLE -->` | `.subtitle` | One-line teaser below heading (remove element if unused) |
| `<!-- META -->` | `.meta` | Date or byline (remove element if unused) |
| `<!-- CONTENT -->` | After `</header>` | Page body — wrap in `<article>` for essays, `<section>` for structured pages |

## Identity

| Property | Value |
|:--|:--|
| Headings | Instrument Serif 400, negative letter-spacing |
| Body | Inter 300, 17px, line-height 1.8 |
| Accent | `#2a5a5a` (teal) / `#6aaeae` dark mode |
| Background | `#FAFAF8` warm off-white / `#131313` dark |
| Content width | 720px centered |
| Theme toggle | Fixed circle, top-right, moon/sun glyph, persists via localStorage (`zm-theme`) |

## Typography quick reference

| Role | Family | Usage |
|:--|:--|:--|
| Headings | Instrument Serif | `h1`, `h2`, `h3`, `.card-title`, `.highlight` |
| Body text | Inter 300 | `p`, `.card-desc`, `.subtitle`, `.endnote` |
| Meta / labels | Inter 400 | `.meta`, `nav` |

## Available components

- **`.wrap`** — centered container (720px)
- **`.card`** / **`.cards`** — bordered cards with subtle shadow, hover accent
- **`.highlight`** — italic Instrument Serif pull-quote in accent color
- **`.callout`** — left-bordered highlight block
- **`.divider`** — thin horizontal rule
- **`.endnote`** — smaller muted text for notes
- **`.edit-link`** — ghost-opacity link to GitHub edit URL
- **`section`** — bottom-bordered content section

## Rules

- All CSS is inline in `<style>`. No external stylesheets, no frameworks.
- Only external dependency: Google Fonts (Instrument Serif + Inter, preconnected).
- Light by default, dark via `[data-theme="dark"]`. Colors via CSS custom properties in `:root`.
- Responsive breakpoint at 540px.
- Essays use external `writing/style.css` (same palette, body weight 300, article structure). This template inlines equivalent styles for standalone pages.
