# Chubby's Burgers — Design System Brief
**Version 1.0 | Prepared for: Claude Design**

---

## 1. Project Context

**Business:** Chubby's Burgers (Chubby's Smash Burger)
**Location:** Inside Uwajimaya Food Court, 600 S Weller St, Seattle, WA — Chinatown-International District
**Owner:** Nation & Nicole
**Type:** Fast-casual smash burger counter

**What this document is:** A design system brief to guide the creation of a mobile-first, SEO-optimized website for Chubby's Burgers. Use this as the single source of truth for all visual and structural decisions.

---

## 2. Brand Personality

### Vision Reference
The owner's reference site is **Bottega Veneta (bottegaveneta.com)**. Key qualities to extract from that reference:
- Extreme whitespace — content breathes, nothing competes
- Full-bleed photography — images carry the entire emotional weight
- Restrained typography — one or two fonts, used sparingly
- No clutter — no banners, no popups, no aggressive CTAs
- Confidence through silence — the less the page says, the more premium it feels

### The Core Tension to Resolve
The logo is loud, retro, and fun. The vision site is quiet and restrained. The design system's job is to hold both. The logo is the personality. The website is the clean white plate it's served on. **Do not let the site compete with the logo. Let the logo be the loudest thing on the page.**

### Brand Adjectives
Confident · Clean · Playful · Unpretentious · Focused · Satisfying

### Physical Space Reference
The actual Chubby's counter features:
- White square subway tile
- Polished steel hood vents
- Navy digital menu boards (white text on navy background)
- Zero decorative elements — purely functional

This space is the design language. The website should feel like a digital extension of standing in front of that counter.

---

## 3. Color System

### Primary Palette

| Token | Hex | Usage |
|---|---|---|
| `--navy` | `#131267` | Primary brand color. Logo, headlines, buttons, nav, footer background |
| `--white` | `#FFFFFF` | Primary background. Dominant. Most of the page should be this. |

### Extended Palette (Derived)

| Token | Hex | Usage |
|---|---|---|
| `--off-white` | `#F5F5F3` | Alternate section backgrounds. Subtle section breaks. Never stark. |
| `--navy-soft` | `#1A1980` | Hover states on navy elements |
| `--navy-10` | `#E8E8F5` | Borders, dividers, very light tints |
| `--text-primary` | `#131267` | Body copy — use navy, not black |
| `--text-muted` | `#6B6B99` | Secondary labels, captions, metadata |

### Color Rules
- **No warm tones in the UI.** Warmth comes exclusively from food photography.
- **No gradients.** Flat color only.
- **Navy on white or white on navy.** These are the only two combinations.
- The off-white (`#F5F5F3`) should be used sparingly — only for alternating section breaks to add rhythm without adding color.
- Never use black (`#000000`). Navy IS the dark color.

---

## 4. Typography

### Font Pairing

| Role | Font | Weight | Source |
|---|---|---|---|
| **Display / Wordmark** | `Bebas Neue` or `Playfair Display` | 400–700 | Google Fonts |
| **Body / UI** | `DM Sans` | 300, 400, 500 | Google Fonts |

> **Note to designer:** If going bolder/more editorial, use `Bebas Neue` for display. If going more refined/luxurious (closer to the Bottega reference), use `Playfair Display`. Recommend testing both and aligning with Nation before finalizing.

### Type Scale

| Token | Size | Weight | Usage |
|---|---|---|---|
| `--text-hero` | 56–72px (mobile: 36–48px) | 700 | Hero headline only |
| `--text-section` | 32–40px (mobile: 24–28px) | 600 | Section headings |
| `--text-item` | 20–24px (mobile: 18px) | 500 | Menu item names |
| `--text-body` | 16px | 400 | Descriptions, paragraphs |
| `--text-small` | 13–14px | 400 | Captions, labels, metadata |
| `--text-nav` | 13–14px | 500, uppercase, tracked | Navigation links |

### Typography Rules
- Navigation links: ALL CAPS, letter-spacing: 0.1–0.15em
- Headlines: sentence case or all caps only — never title case for section headings
- Menu item prices: same size as item name, navy, no dollar sign styling needed
- Never center-align body text blocks longer than 2 lines
- Line height for body: 1.6. Line height for headlines: 1.1–1.2.

---

## 5. Spacing & Layout

### Grid
- **Mobile:** Single column, 20px horizontal padding
- **Tablet:** Single or 2-column, 32px horizontal padding
- **Desktop:** Max-width 1200px, centered, 48–64px horizontal padding

### Spacing Scale (8pt base)

| Token | Value | Usage |
|---|---|---|
| `--space-xs` | 4px | Inline gaps, tight pairs |
| `--space-sm` | 8px | Between label and value |
| `--space-md` | 16px | Between related elements |
| `--space-lg` | 32px | Between components |
| `--space-xl` | 64px | Between sections |
| `--space-2xl` | 128px | Major section breaks, hero padding |

### Layout Rules
- **Mobile-first.** Design and build for 390px width first.
- Hero section: full viewport height on mobile (`100svh`)
- Sections should have generous top/bottom padding — minimum `--space-xl` (64px), ideally `--space-2xl` (128px) on desktop
- Menu items: single column on mobile, 2-column max on desktop
- No sidebars. No multi-column layouts on mobile. Ever.

---

## 6. Logo Usage

### The Logo
Retro cartoon mascot — an anthropomorphized smash burger character wearing a snapback, throwing a peace sign, winking. Wordmark "CHUBBY'S" in chunky bubbly lettering arched above. Single color: `#131267` navy.

### Usage Rules
- **On white backgrounds:** Navy logo as-is
- **On navy backgrounds:** White version of the logo (color swap only)
- **Minimum size:** 48px height on mobile, 64px on desktop
- **Clear space:** Equal to the height of the "C" in CHUBBY'S on all sides
- **Never:** Stretch, recolor, add drop shadows, place on busy backgrounds, or outline with a stroke
- **Logo in nav:** Use at reduced size (40–48px height). Can use wordmark-only lockup if mascot becomes too small to read.
- The mascot character can be used independently as an icon/favicon/stamp element — it's strong enough to stand alone.

---

## 7. Imagery & Photography Art Direction

### Role of Photography
Photography is the ONLY source of warmth in this design system. The UI provides the clean white plate. The food photography provides everything else — color, appetite appeal, energy.

### Shot Types Needed
1. **Hero shot** — one anchor image. Full-bleed. The burger, smashed, golden crust, melted cheese pull, dramatic close-up. Shoot on white or dark surface, not in the store.
2. **Menu item shots** — each menu item photographed overhead or at 45°, clean background, consistent framing. Square or 4:5 ratio.
3. **In-store atmosphere** — the white tile counter, the menu board, the hands making the burger. Candid, not staged.
4. **Detail shots** — cheese drip, sesame seeds, crispy edges. Macro. These become background accents.

### Photography Style
- **Lighting:** Natural or soft studio light. No harsh flash. No filters.
- **Background:** White, black, or the white tile counter. Never busy backgrounds.
- **Color temperature:** Warm (food looks better warm). The golden-brown of a properly smashed patty is the brand's warmth.
- **No stock photos.** All imagery should be of the actual Chubby's product.

---

## 8. Component Patterns

### Navigation
- Fixed to top on scroll
- Logo left, links right
- Mobile: hamburger menu or bottom navigation bar
- Background: white with a 1px `--navy-10` bottom border on scroll. Transparent over hero.
- Links: ALL CAPS, `--text-nav` scale, navy color

### Hero Section
- Full-bleed food photography background OR white background with hero image
- One headline (max 6 words)
- One sub-label (location + type: "Smash Burgers · CID Seattle")
- One CTA: "See the Menu" — navy button, white text, no border-radius or pill shape. Sharp corners OR very subtle radius (4px max). Flat, no shadows.
- No autoplay video. No sliders.

### Menu Cards
- Item name — `--text-item` scale, navy, bold
- Price — same line as name, right-aligned or directly after
- Short description — 1 line max, `--text-small`, `--text-muted`
- Optional: item photo above, square, full-width of card
- No borders on cards — use spacing alone to separate items
- Divider: 1px `--navy-10` line between items

### Buttons
- **Primary:** Navy background, white text, flat (no gradient, no shadow), 12–16px padding vertical, 24–32px horizontal
- **Secondary:** Navy text, navy 1px border, white background
- **No pill shapes.** Sharp corners (0px radius) or very subtle (4px). This matches the tile aesthetic.
- Hover: opacity 0.85 or `--navy-soft`

### Footer
- Navy background, white text
- Three columns on desktop, stacked on mobile: Hours · Location · Order Links
- Logo (white version) centered or left-aligned
- Minimal — address, hours, Uber Eats / DoorDash links, Instagram link

---

## 9. SEO Foundations

### Page Structure Requirements
Every page must include:
- `<title>` tag: "Chubby's Burgers — Smash Burgers in Seattle's Chinatown-International District"
- `<meta name="description">`: 150–160 characters describing the food, location, and price point
- `<h1>`: One per page only. Should contain primary keyword.
- Proper heading hierarchy: H1 → H2 → H3 (never skip levels)
- `alt` text on every image — be descriptive ("crispy smash burger with melted american cheese on a sesame bun")

### Structured Data (JSON-LD)
Implement `Restaurant` schema on the homepage:
```json
{
  "@context": "https://schema.org",
  "@type": "Restaurant",
  "name": "Chubby's Burgers",
  "servesCuisine": "American, Burgers",
  "priceRange": "$",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "600 S Weller St",
    "addressLocality": "Seattle",
    "addressRegion": "WA",
    "postalCode": "98104"
  },
  "telephone": "",
  "url": "",
  "openingHours": []
}
```

### Target Keywords
- "smash burger Seattle"
- "smash burger Chinatown Seattle"
- "burgers near Uwajimaya"
- "CID Seattle food"
- "best smash burger Seattle"

### Performance Rules (Core Web Vitals)
- Images: WebP format, compressed, lazy-loaded below the fold
- No render-blocking scripts
- Fonts: preload the two primary fonts
- No heavy animations on mobile
- Target: LCP under 2.5s on mobile

---

## 10. Voice & Copy Guidelines

### Tone
Short. Confident. No fluff. Never precious about itself.

### Examples

| ❌ Don't | ✅ Do |
|---|---|
| "Experience the ultimate smash burger journey" | "Smashed. Crispy. Done right." |
| "We take pride in crafting each burger with care" | "House-made sauce. Crispy edges. Simple menu." |
| "Welcome to Chubby's Burgers, your destination for..." | "Smash Burgers. CID Seattle." |

### Copy Rules
- Hero headline: 4–6 words maximum
- Menu descriptions: 1 line or none at all
- CTAs: verb-first ("See Menu", "Get Directions", "Order Now")
- No exclamation points in UI copy

---

## 11. What This Site Is NOT

To keep scope focused, the website does NOT need to:
- Process orders (Uber Eats and DoorDash handle this)
- Have a reservation system
- Have a blog
- Have multiple pages beyond: Home + Menu (single page is fine)
- Use video
- Have animations beyond subtle fade-ins on scroll

**The entire site can and should be a single, well-crafted page.** Everything a customer needs: menu, prices, location, hours, order links. That's it.

---

*End of Design System Brief — Chubby's Burgers v1.0*
