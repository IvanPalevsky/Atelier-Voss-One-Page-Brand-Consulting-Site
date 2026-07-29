# Atelier Voss — One-Page Brand & Consulting Site

A single-page marketing site for an independent brand-and-interiors consultancy, built to do one job well: turn a visitor into a booked enquiry, without a multi-page navigation maze getting in the way.

---

## Overview

Atelier Voss is a concept site for a small, high-touch consulting practice — the kind of business where credibility and restraint matter more than a large feature set. The brief behind it: one continuous scroll, editorial typography, and a clear narrative arc from "who this is for" to "get in touch," with no distracting navigation or unnecessary pages.

Every section is built to earn its place in the scroll: eyebrow → headline → proof (client list) → substance (about, services) → social proof (testimonial) → single call to action. Nothing is included that doesn't move a visitor toward booking a call.

## Features

**Structure & narrative**
- Single continuous page with anchored nav links (`Work`, `Approach`, `Contact`) for quick jumps without leaving the flow
- Infinite-scrolling client-name marquee as lightweight, tasteful social proof
- Three-part services breakdown (Identity / Interiors / Advisory), laid out as a numbered list — used because the offering is genuinely a short, ordered set, not decoration for its own sake
- Dedicated testimonial block with a large pull-quote treatment
- Single, unambiguous closing call to action

**Motion & polish**
- Scroll-triggered reveal animations (fade + rise) built with `IntersectionObserver` — content animates in once, on first view, with no jank or re-triggering on scroll-back
- Infinite CSS-only marquee for the client list, no JavaScript animation loop required
- Fully responsive layout, including a services grid that reflows cleanly on mobile

**Design system**
- Typeface pairing: Newsreader (italic serif, used for headlines and the brand mark) + Inter (UI/body) + JetBrains Mono (eyebrows/labels)
- Warm, paper-toned palette (`#F4F2ED`) with a single oxblood accent (`#6E2A34`) — chosen to read as considered and editorial rather than corporate
- Generous whitespace and a restrained type scale, in line with the "quiet, considered" positioning the copy itself argues for

## Tech Stack

| Layer | Choice |
|---|---|
| Markup/Styling | Semantic HTML5, CSS3 (custom properties, CSS Grid, Flexbox, `@keyframes`) |
| Interactivity | Vanilla JavaScript — a single `IntersectionObserver` for scroll reveals |
| Fonts | Google Fonts (Newsreader, Inter, JetBrains Mono) |
| Build tooling | None required — static file |

## Project Structure

```
visitka-atelier-voss.html   → single-file build: markup, styles, and script
```

Copy, client names, and services are plain text in the markup, making this trivial to re-skin for a different consultant, studio, or personal brand without touching the layout or animation logic.

## Running Locally

No install step needed:

```bash
git clone https://github.com/IvanPalevsky/Atelier-Voss-One-Page-Brand-Consulting-Site.git
cd Atelier-Voss-One-Page-Brand-Consulting-Site
open visitka-atelier-voss.html   # or just double-click the file
```

For live-reload during development:

```bash
npx serve .
```

## Deploying

Static file, deploys anywhere with zero configuration:

- **Vercel / Netlify:** drag-and-drop, or connect the repo directly
- **GitHub Pages:** enable Pages on this repo, pointing to the root

## What This Demonstrates

- A conversion-oriented one-page structure, not just a visually nice scroll
- Restrained, editorial design choices tied to the brand's actual positioning, rather than a generic "landing page" template
- Lightweight, dependency-free motion — the scroll-reveal system adds under 15 lines of JavaScript

---

Built as a portfolio piece by [Ivan Palevsky](https://github.com/IvanPalevsky). Available for landing page, brand site, and full-stack web development work.
