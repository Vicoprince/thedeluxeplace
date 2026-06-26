# The Deluxe Place — Website Demo
### Designed & Built by Improsoft Technologies

---

## Overview

This is a fully custom, multi-page website demo built for **The Deluxe Place** — the personal luxury menswear brand of **Shodipe Adebola**, Lagos' most trusted premium fashion connoisseur.

The site was designed from scratch — no templates, no themes — to reflect the identity, philosophy and aesthetic of the brand. Every design decision, from the antique gold accent to the vertical rule signature element, was made with one goal: to give The Deluxe Place a digital presence that matches the premium standard of the brand itself.

---

## Pages

| Page | Route | Purpose |
|------|-------|---------|
| Home | `#home` | First impression — hero, collections preview, brand story, stats, Instagram grid, CTA |
| About | `#about` | Shodipe's story, philosophy, and the three principles he never compromises on |
| Collections | `#collections` | Filterable catalogue — Native Luxury, Bespoke Suiting, Deluxe Edit, Accessories |
| Lookbook | `#lookbook` | Full-bleed editorial gallery with click-to-expand lightbox |
| Order | `#order` | Structured enquiry form with category, occasion and budget selectors |
| Contact | `#contact` | All contact channels — WhatsApp, Instagram, Email — presented as premium touchpoints |

---

## Design System

### Colour Palette

| Token | Hex | Usage |
|-------|-----|-------|
| Near Black | `#0A0A0A` | Hero backgrounds, nav, dark sections |
| Soft Black | `#1A1A1A` | Cards, footer, secondary dark surfaces |
| Antique Gold | `#C9A84C` | Primary accent — labels, rules, hover states, CTAs |
| Gold Light | `#E2C97E` | Gold hover and gradient partner |
| Pure White | `#FFFFFF` | Content section backgrounds |
| Off White | `#F5F0E8` | Subtle section backgrounds, form areas |
| Cream | `#FAF7F2` | Card backgrounds, warm neutrals |
| Mid Grey | `#6B6B6B` | Body text, secondary copy |
| Light Grey | `#E8E8E8` | Borders, dividers |

### Typography

| Role | Font | Weight | Usage |
|------|------|--------|-------|
| Display / Headlines | Cormorant Garamond | 300, 400, 600, 700 | Hero titles, section headers, card names |
| Body / UI | DM Sans | 300, 400, 500 | Body copy, nav, buttons, forms, labels |
| Labels / Tags | Bebas Neue | 400 | Section eyebrows, category badges, marquee |

### Signature Design Element
A **vertical gold rule** (`1px, rgba gold, 40% opacity`) anchors every dark hero section on the left — positioned at `22mm` from the left edge. It animates in via a `scaleY` keyframe on page load and acts as the visual spine that ties every dark page together, like the binding of a luxury fashion magazine.

---

## Features

### Navigation
- **Adaptive nav theme** — automatically switches between dark mode (black pages) and light mode (white pages) based on the active page
- **Scroll compression** — nav padding reduces on scroll for a cleaner browsing experience
- **Active state tracking** — current page is highlighted in all nav instances (desktop, mobile, footer)
- **Solid mobile menu** — full `#0A0A0A` background overlay, no transparency, no bleed-through. Body scroll is locked while open
- **Animated hamburger** — transforms into `✕` on open via CSS transforms

### Interactivity
- **Antigravity particle system** — 60 gold/white particles that actively repel from the mouse cursor, built on HTML5 Canvas with per-frame physics
- **Scroll-reveal animations** — elements fade and slide up into view as they enter the viewport, using `IntersectionObserver`
- **Page transition animation** — every page switch triggers a `fadeIn + translateY` animation for smooth navigation
- **Lightbox** — full-screen image viewer on Lookbook and Gallery pages, closeable via click-outside, close button, or `Escape` key
- **Collection filter** — client-side category filtering on the Collections page with animated active state on filter buttons
- **Marquee strip** — auto-scrolling brand keyword ticker, duplicated for seamless looping
- **Form feedback** — submit buttons animate through a loading state and success confirmation

### Performance & Structure
- Single HTML file — zero dependencies, no build tools required
- All fonts loaded via Google Fonts with `rel="preconnect"` for speed
- Images sourced from Unsplash CDN with width parameters for optimised loading
- `IntersectionObserver` used for all scroll animations — no scroll event listeners
- CSS custom properties (`var()`) used throughout for maintainable theming

---

## File Structure

```
thedeluxeplace.html        # Main website file (self-contained)
deluxeplace-proposal.pdf   # Client proposal document
deluxeplace-pitch-content.md  # Pitch messages, Loom script, follow-up sequence
README.md                  # This file
```

---

## Customisation Guide

When handing off to the client or preparing for live deployment, the following placeholders should be updated:

### Content to Replace

| Item | Current Value | Replace With |
|------|--------------|--------------|
| WhatsApp number | `+234 807 878 0897` | Shodipe's actual WhatsApp number |
| Email address | `hello@thedeluxeplace.com` | Actual business email |
| Instagram link | `https://www.instagram.com/thedeluxeplace/` | Already correct ✓ |
| Google Maps link | Not currently linked | Add actual business location if needed |
| Stats — Years | `5+` | Adjust to actual years in business |
| Proposal pricing | `₦200,000` | Adjust per agreed contract price |

### Images
All images are currently sourced from **Unsplash** as placeholders. For the live site, replace with:
- Actual product photography from The Deluxe Place catalogue
- Shodipe's personal brand photography / portraits
- Real lookbook images from Instagram archive

To replace an image, find the `<img>` tag and update the `src` attribute:
```html
<!-- Replace this -->
<img src="https://images.unsplash.com/photo-XXXXXX?w=700&q=80" alt="...">

<!-- With this -->
<img src="path/to/your/actual/image.jpg" alt="Descriptive alt text">
```

### Colours
All colours are defined as CSS custom properties at the top of the `<style>` block:
```css
:root {
  --gold: #C9A84C;      /* Change accent colour here */
  --black: #0A0A0A;     /* Change dark background here */
  /* etc. */
}
```

---

## Deployment

This is a single HTML file. To deploy:

1. **Quick demo** — open `thedeluxeplace.html` directly in any browser
2. **Hosted demo** — upload to any static host (Netlify, Vercel, GitHub Pages)
   ```bash
   # Netlify drag-and-drop
   # Just drag the HTML file to netlify.com/drop

   # Vercel CLI
   vercel deploy thedeluxeplace.html
   ```
3. **WordPress** — for delivery via WordPress/Elementor, the design system and layout in this file serve as the approved design reference for the Elementor build

---

## Browser Support

| Browser | Support |
|---------|---------|
| Chrome 90+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Mobile Chrome | ✅ Full |
| Mobile Safari | ✅ Full |

---

## Pitch Package Contents

This demo is part of a complete pitch package prepared by Improsoft Technologies:

- `thedeluxeplace.html` — Live demo website
- `deluxeplace-proposal.pdf` — 6-page branded proposal document
- `deluxeplace-pitch-content.md` — Cold pitch messages, Loom video script, 3-step follow-up sequence

---

## About Improsoft Technologies

Improsoft Technologies is a web design and technology agency specialising in custom digital experiences for businesses and personal brands across Nigeria and beyond.

We build websites that don't just look good — they work. Every project starts with research, is grounded in brand strategy, and is delivered with the kind of attention to detail that turns browsers into buyers.

**Website:** [www.improsofttech.com](https://www.improsofttech.com)
**Instagram:** [@improsofttech](https://www.instagram.com/improsofttech)
**Email:** hello@improsoft.com

---

*© 2025 Improsoft Technologies. This demo was created as a speculative pitch for The Deluxe Place and remains the intellectual property of Improsoft Technologies until a project agreement is signed.*
