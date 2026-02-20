# Indie Sleaze - Design Reference

## Overview

Indie Sleaze is the visual language of the hedonistic, blog-documented party scene that thrived from roughly 2005 to 2014 in neighborhoods like Williamsburg, Brooklyn and Shoreditch, London. Defined by harsh flash photography, film grain, neon accents, and a deliberate messiness that blurred the line between high fashion and thrift-store abandon, the aesthetic drew its visual DNA from The Cobrasnake's candid nightlife documentation, American Apparel's provocative ad campaigns, MySpace profile customization, DIY zine culture, and the electro-clash music scene of bands like The Strokes, Yeah Yeah Yeahs, and LCD Soundsystem. On the web it translates into gritty textures, blown-out photography, chaotic collage layouts, bold hand-drawn type, neon-on-black color palettes, and an intentional rawness that rejects the polished perfection of corporate design in favor of authentic, sweaty, nocturnal energy.

---

## Visual Characteristics

### Core Design Traits

- **Flash-photography grain**: Surfaces and backgrounds simulate the washed-out, high-contrast look of compact digital cameras and disposable film -- harsh direct flash, red-eye artifacts, visible noise, and overexposed highlights that flatten depth into a gritty, documentary texture
- **Neon-on-dark contrast**: Hot pink, electric yellow, and acid green elements burn against deep black or charcoal backgrounds, mimicking neon bar signs, glow sticks, and club lighting that defined late-night Williamsburg and Lower East Side venues
- **Collage and overlap**: Layered imagery, rotated photo stacks, torn-edge cutouts, and overlapping text blocks evoke DIY zine paste-ups, Tumblr mood boards, and the chaotic MySpace profile pages of the era
- **Hand-drawn and blocky lettering**: Typography leans toward imperfect, marker-style display fonts and chunky block letters reminiscent of party flyers photocopied at Kinko's and wheat-pasted on construction walls
- **Messy glamour texture**: Smudged edges, halftone dots, VHS scan lines, and film-scratch overlays add a layer of analog decay that signals authenticity and rejects the clinical sharpness of modern digital design
- **Provocative editorial imagery**: Photo treatments reference American Apparel's raw, sexually charged advertising style -- unretouched skin, harsh lighting, casual poses, and a voyeuristic intimacy
- **Sticker and badge elements**: Small decorative elements like peeling stickers, safety pins, X marks (for straight-edge or club entry stamps), and hand-scrawled annotations float across layouts as if applied to a laptop lid or bathroom mirror

### Design Principles

- **Authenticity over polish**: Imperfection is the point; designs should look like they were made at 2 AM after a show, not in a corporate boardroom
- **Nocturnal energy**: The palette, lighting, and mood should evoke nighttime -- clubs, after-parties, dimly lit bars, flash-lit sidewalks
- **Democratic chaos**: Hierarchy is loose and overlapping; the eye should wander across the page the way it wanders across a crowded party
- **DIY resourcefulness**: Layouts should feel handmade and resourceful, as if assembled from whatever materials were available -- photocopies, Sharpie markers, disposable cameras, sticker sheets
- **Nostalgia as texture**: Reference early social media (MySpace, Tumblr, Flickr), flip phones, and mid-2000s web culture as visual shorthand for the era
- **Hedonistic maximalism**: More is more -- layer textures, stack photos, mix fonts, and let the visual noise communicate the sensory overload of the scene

---

## Color Palette

The Indie Sleaze palette is built around the contrast between dark nightclub environments and the neon, flash-lit highlights that punctuate them. Blacks and deep grays form the foundation, while hot pinks, electric yellows, and acid greens provide the charged energy of the scene.

| Color Name | Hex | Role / Usage |
|---|---|---|
| Blackout | `#0A0A0A` | Primary background, deep shadows, base surface |
| Charcoal Venue | `#1C1C1C` | Secondary background, card surfaces, dark UI panels |
| Smoke Machine | `#2E2E2E` | Tertiary background, subtle elevation, borders |
| Flash White | `#F5F0EB` | Overexposed highlights, flash-lit text, hero display type |
| Hot Neon Pink | `#FF2D87` | Primary accent, CTAs, links, highlighted text, neon glow |
| Electric Yellow | `#FFE714` | Secondary accent, warning badges, sticker elements, hover states |
| Acid Green | `#39FF14` | Tertiary accent, online indicators, success states, glow effects |
| Bruise Purple | `#8B2FC9` | Visited links, secondary highlights, ultraviolet club lighting |
| Cheap Beer Gold | `#C9A84C` | Metallic accents, premium badges, sequin shimmer effects |
| Red Eye | `#CC1100` | Error states, flash red-eye artifacts, danger, raw urgency |
| Cigarette Ash | `#8A8A8A` | Muted text, metadata, disabled states, secondary body copy |
| Polaroid Cream | `#F0E6D3` | Alt light background, photo borders, nostalgic warmth |
| Dive Bar Blue | `#1A3A5C` | Dark accent, denim references, moody undertone panels |
| Silver Lame | `#C0C0C0` | Metallic UI elements, reflective surfaces, disco shimmer |

### CSS Custom Properties

```css
:root {
  /* Dark foundations */
  --sleaze-black: #0a0a0a;
  --sleaze-charcoal: #1c1c1c;
  --sleaze-smoke: #2e2e2e;

  /* Light / flash tones */
  --sleaze-flash: #f5f0eb;
  --sleaze-cream: #f0e6d3;

  /* Neon accents */
  --sleaze-pink: #ff2d87;
  --sleaze-yellow: #ffe714;
  --sleaze-green: #39ff14;
  --sleaze-purple: #8b2fc9;

  /* Supporting tones */
  --sleaze-gold: #c9a84c;
  --sleaze-red: #cc1100;
  --sleaze-ash: #8a8a8a;
  --sleaze-blue: #1a3a5c;
  --sleaze-silver: #c0c0c0;

  /* Functional tokens */
  --sleaze-bg: var(--sleaze-black);
  --sleaze-surface: var(--sleaze-charcoal);
  --sleaze-text: var(--sleaze-flash);
  --sleaze-text-muted: var(--sleaze-ash);
  --sleaze-accent: var(--sleaze-pink);
  --sleaze-accent-alt: var(--sleaze-yellow);
  --sleaze-link: var(--sleaze-pink);
  --sleaze-link-hover: var(--sleaze-yellow);
  --sleaze-border: var(--sleaze-smoke);

  /* Effects */
  --sleaze-glow-pink: 0 0 20px rgba(255, 45, 135, 0.6);
  --sleaze-glow-yellow: 0 0 20px rgba(255, 231, 20, 0.5);
  --sleaze-glow-green: 0 0 20px rgba(57, 255, 20, 0.5);
  --sleaze-grain: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.08'/%3E%3C/svg%3E");
}
```

---

## Typography

### Typeface Characteristics

Indie Sleaze typography oscillates between two poles: the blocky, hand-drawn display lettering found on DIY party flyers and zine covers, and the condensed sans-serifs that dominated MySpace band pages and American Apparel advertisements. Body text tends toward simple, slightly rough sans-serifs that read as casual and un-designed. Display text is loud, irregular, and often set in all-caps with tight or negative letter-spacing. The overall effect should feel like someone designed a flyer with a Sharpie and a photocopier, then scanned it and dropped it onto a Tumblr page.

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|---|---|---|
| Bebas Neue | Condensed all-caps display sans | Headlines, hero text, poster-style display |
| Permanent Marker | Hand-drawn marker script | Accent text, callouts, zine-style annotations |
| Oswald | Condensed gothic sans-serif | Subheadings, navigation, compact UI labels |
| Barlow Condensed | Narrow humanist sans-serif | Body text, descriptions, readable compact copy |
| Special Elite | Typewriter slab | Blog-style body text, editorial captions, alt body |
| Rock Salt | Rough handwriting | Decorative annotations, sticker text, scrawled notes |
| Anton | Ultra-condensed display sans | Large-scale titles, event names, splash headings |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---|---|---|
| Bebas Neue | Barlow Condensed | Classic party flyer meets readable blog layout |
| Permanent Marker + Anton | Barlow Condensed | Hand-scrawled zine energy with clean body readability |
| Oswald (700) | Special Elite | Condensed editorial authority paired with raw typewriter intimacy |
| Anton | Barlow Condensed (300) | Massive poster impact with lightweight, breathable body text |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Anton&family=Barlow+Condensed:wght@300;400;600&family=Bebas+Neue&family=Permanent+Marker&family=Special+Elite&display=swap');

/* === Base Typography === */
body {
  font-family: 'Barlow Condensed', 'Arial Narrow', Helvetica, sans-serif;
  font-weight: 400;
  font-size: 17px;
  line-height: 1.6;
  color: var(--sleaze-text);
  background-color: var(--sleaze-bg);
  letter-spacing: 0.01em;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Bebas Neue', 'Anton', 'Impact', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  line-height: 0.95;
  margin: 0 0 0.5em 0;
  color: var(--sleaze-flash);
}

h1 {
  font-size: clamp(3.5rem, 10vw, 9rem);
  letter-spacing: -0.02em;
}

h2 {
  font-size: clamp(2rem, 6vw, 5rem);
}

h3 {
  font-size: clamp(1.5rem, 3.5vw, 2.5rem);
}

a {
  color: var(--sleaze-link);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: color 0.15s ease, border-color 0.15s ease, text-shadow 0.15s ease;
}

a:hover {
  color: var(--sleaze-link-hover);
  border-bottom-color: var(--sleaze-link-hover);
  text-shadow: var(--sleaze-glow-yellow);
}

.annotation {
  font-family: 'Permanent Marker', cursive;
  color: var(--sleaze-pink);
  transform: rotate(-2deg);
  display: inline-block;
}

.typewriter {
  font-family: 'Special Elite', 'Courier New', monospace;
  letter-spacing: 0.03em;
}

blockquote {
  font-family: 'Permanent Marker', cursive;
  font-size: 1.4rem;
  color: var(--sleaze-yellow);
  border-left: 3px solid var(--sleaze-pink);
  padding-left: 1rem;
  transform: rotate(-1deg);
}
```

---

## Layout Principles

### Grid and Structure

- **Asymmetric collage grids**: Avoid perfectly balanced columns; use CSS Grid with varying track sizes to create off-kilter, magazine-style layouts where content blocks overlap and compete for attention
- **Intentional overflow and bleed**: Allow images and decorative elements to break out of their containers and bleed to viewport edges, mimicking the way zine content runs off the page
- **Stacked photo clusters**: Group images in overlapping stacks with slight rotations (2-5 degrees), as if tossed onto a table or pinned haphazardly to a wall
- **Generous negative space in unexpected places**: While the overall layout is chaotic, pockets of empty black space create dramatic breathing room that mimics dark club corners between bursts of neon
- **Z-index layering**: Use deliberate stacking orders to create depth -- text over images, stickers over text, grain textures over everything

### Section Organization

- **Hero splash**: Full-viewport opening with oversized type, a grainy background image or video still, and a neon-accented CTA
- **Photo grid / gallery**: Masonry or collage-style grid of flash-lit photography with torn-edge or Polaroid-style framing
- **Editorial content blocks**: Text sections with pull quotes in hand-drawn fonts, offset images, and margin annotations
- **Event / lineup section**: Band-poster-style listing with dates, names, and venue information in condensed all-caps type
- **Social proof strip**: Scrolling or static row of logos, press mentions, or Tumblr-style reblog counts
- **Footer as afterparty**: Dense, dark footer with small text, hidden easter eggs, and a sense of the night winding down

### Responsive Approach

- **Mobile-first nocturnal**: The dark background and high-contrast neon accents naturally suit OLED mobile screens; start with single-column stacked layouts
- **Collage unfolds at wider breakpoints**: Photo overlaps and rotations activate only above tablet widths where there is room for the chaos to breathe
- **Touch-friendly hit targets**: Despite the chaotic visual style, interactive elements maintain comfortable tap sizes (minimum 44px) to stay usable on phones at parties
- **Font scaling preserves impact**: Use `clamp()` for display type so massive headlines scale down gracefully without losing their poster-wall presence
- **Grain and texture effects degrade gracefully**: Film grain overlays use CSS pseudo-elements that layer non-destructively and can be simplified on lower-powered devices via `prefers-reduced-motion`

---

## CSS / Design Techniques

### Flash Photo Card

A content card that evokes the look of a flash-lit Polaroid or point-and-shoot snapshot, with slight rotation, a gritty border treatment, and neon hover glow.

```css
.sleaze-card {
  background-color: var(--sleaze-charcoal);
  border: 1px solid var(--sleaze-smoke);
  padding: 0;
  overflow: hidden;
  transform: rotate(-1.5deg);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  position: relative;
}

.sleaze-card::after {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--sleaze-grain);
  pointer-events: none;
  opacity: 0.15;
  mix-blend-mode: overlay;
}

.sleaze-card:hover {
  transform: rotate(0deg) scale(1.03);
  box-shadow: var(--sleaze-glow-pink);
}

.sleaze-card img {
  width: 100%;
  display: block;
  filter: contrast(1.15) brightness(1.05) saturate(0.9);
}

.sleaze-card .caption {
  padding: 1rem 1.2rem;
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 0.9rem;
  color: var(--sleaze-ash);
}

.sleaze-card .caption strong {
  display: block;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.3rem;
  color: var(--sleaze-flash);
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-bottom: 0.25rem;
}
```

### Neon Glow Button

A CTA button that pulses with neon energy, referencing the glowing signage of dive bars and club entrances.

```css
.sleaze-btn {
  display: inline-block;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.1rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  padding: 0.8rem 2rem;
  color: var(--sleaze-pink);
  background: transparent;
  border: 2px solid var(--sleaze-pink);
  cursor: pointer;
  text-decoration: none;
  position: relative;
  transition: all 0.2s ease;
}

.sleaze-btn:hover {
  color: var(--sleaze-black);
  background-color: var(--sleaze-pink);
  box-shadow: var(--sleaze-glow-pink);
  text-shadow: none;
}

.sleaze-btn--yellow {
  color: var(--sleaze-yellow);
  border-color: var(--sleaze-yellow);
}

.sleaze-btn--yellow:hover {
  color: var(--sleaze-black);
  background-color: var(--sleaze-yellow);
  box-shadow: var(--sleaze-glow-yellow);
}

.sleaze-btn--solid {
  color: var(--sleaze-black);
  background-color: var(--sleaze-pink);
  border-color: var(--sleaze-pink);
}

.sleaze-btn--solid:hover {
  background-color: var(--sleaze-flash);
  border-color: var(--sleaze-flash);
  box-shadow: 0 0 30px rgba(255, 45, 135, 0.4);
}
```

### Dive Bar Navigation

A navigation bar that feels like the neon-lit menu board of a Lower East Side bar, with glowing hover states and condensed all-caps type.

```css
.sleaze-nav {
  background-color: var(--sleaze-black);
  border-bottom: 1px solid var(--sleaze-smoke);
  padding: 0 1.5rem;
  position: sticky;
  top: 0;
  z-index: 100;
}

.sleaze-nav ul {
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 0;
  margin: 0;
  padding: 0;
}

.sleaze-nav .logo {
  font-family: 'Permanent Marker', cursive;
  font-size: 1.3rem;
  color: var(--sleaze-pink);
  text-decoration: none;
  margin-right: auto;
  padding: 0.8rem 0;
  text-shadow: var(--sleaze-glow-pink);
}

.sleaze-nav a {
  display: block;
  padding: 0.9rem 1rem;
  color: var(--sleaze-ash);
  text-decoration: none;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 0.95rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  border-bottom: 2px solid transparent;
  transition: color 0.15s ease, border-color 0.15s ease;
}

.sleaze-nav a:hover {
  color: var(--sleaze-pink);
  border-bottom-color: var(--sleaze-pink);
  text-shadow: var(--sleaze-glow-pink);
}

.sleaze-nav a.active {
  color: var(--sleaze-flash);
  border-bottom-color: var(--sleaze-pink);
}
```

### Hero Section with Grain Overlay

A full-viewport hero that layers grainy texture over a dark background with oversized display type and neon accents.

```css
.sleaze-hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 4rem 2.5rem;
  background-color: var(--sleaze-black);
  position: relative;
  overflow: hidden;
}

.sleaze-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--sleaze-grain);
  opacity: 0.12;
  pointer-events: none;
  z-index: 1;
}

.sleaze-hero::after {
  content: '';
  position: absolute;
  top: -50%;
  right: -20%;
  width: 600px;
  height: 600px;
  background: radial-gradient(circle, rgba(255, 45, 135, 0.15) 0%, transparent 70%);
  pointer-events: none;
  z-index: 0;
}

.sleaze-hero > * {
  position: relative;
  z-index: 2;
}

.sleaze-hero h1 {
  font-size: clamp(4rem, 12vw, 12rem);
  line-height: 0.88;
  color: var(--sleaze-flash);
  margin: 0;
}

.sleaze-hero h1 span {
  color: var(--sleaze-pink);
  text-shadow: var(--sleaze-glow-pink);
}

.sleaze-hero p {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: clamp(1.05rem, 2vw, 1.4rem);
  font-weight: 300;
  color: var(--sleaze-ash);
  max-width: 50ch;
  margin-top: 1.5rem;
  line-height: 1.6;
}

.sleaze-hero .btn-row {
  margin-top: 2rem;
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}
```

### Zine Pull Quote

A styled blockquote that looks like a scrawled annotation torn from a DIY zine, with rotation and hand-drawn font treatment.

```css
.sleaze-pullquote {
  font-family: 'Permanent Marker', cursive;
  font-size: clamp(1.5rem, 3.5vw, 2.5rem);
  color: var(--sleaze-yellow);
  line-height: 1.3;
  padding: 2rem 2.5rem;
  margin: 3rem 0;
  background-color: var(--sleaze-charcoal);
  border-left: 4px solid var(--sleaze-pink);
  position: relative;
  transform: rotate(-1deg);
}

.sleaze-pullquote::before {
  content: '\201C';
  font-size: 5rem;
  color: var(--sleaze-pink);
  position: absolute;
  top: -0.2em;
  left: 0.3rem;
  opacity: 0.5;
  line-height: 1;
}

.sleaze-pullquote cite {
  display: block;
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 0.85rem;
  font-style: normal;
  color: var(--sleaze-ash);
  margin-top: 1rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}
```

### Event Lineup Poster

A section styled like a gig poster or club night lineup, with hierarchical band-name sizing and neon date highlights.

```css
.sleaze-lineup {
  background-color: var(--sleaze-black);
  padding: 3rem 2rem;
  text-align: center;
  border: 1px solid var(--sleaze-smoke);
  position: relative;
}

.sleaze-lineup::after {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--sleaze-grain);
  opacity: 0.1;
  pointer-events: none;
}

.sleaze-lineup .date {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1rem;
  color: var(--sleaze-yellow);
  text-transform: uppercase;
  letter-spacing: 0.3em;
  margin-bottom: 0.5rem;
  text-shadow: var(--sleaze-glow-yellow);
}

.sleaze-lineup .headliner {
  font-family: 'Anton', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  color: var(--sleaze-flash);
  text-transform: uppercase;
  line-height: 0.95;
  margin-bottom: 0.5rem;
}

.sleaze-lineup .support {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(1.2rem, 3vw, 2rem);
  color: var(--sleaze-pink);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-bottom: 0.3rem;
}

.sleaze-lineup .opener {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 1rem;
  color: var(--sleaze-ash);
  text-transform: uppercase;
  letter-spacing: 0.15em;
}

.sleaze-lineup .venue {
  font-family: 'Special Elite', monospace;
  font-size: 0.85rem;
  color: var(--sleaze-gold);
  margin-top: 1.5rem;
  letter-spacing: 0.1em;
}
```

### Film Grain Overlay Utility

A reusable CSS technique for applying film grain texture to any element, evoking the analog photography of the era.

```css
.grain-overlay {
  position: relative;
}

.grain-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--sleaze-grain);
  opacity: 0.12;
  pointer-events: none;
  mix-blend-mode: overlay;
  z-index: 10;
}

/* Animated grain variant for hero sections */
@keyframes grain-shift {
  0%, 100% { transform: translate(0, 0); }
  10% { transform: translate(-2%, -3%); }
  30% { transform: translate(3%, 2%); }
  50% { transform: translate(-1%, 3%); }
  70% { transform: translate(2%, -2%); }
  90% { transform: translate(-3%, 1%); }
}

.grain-animated::after {
  content: '';
  position: absolute;
  inset: -50%;
  background: var(--sleaze-grain);
  opacity: 0.1;
  pointer-events: none;
  mix-blend-mode: overlay;
  z-index: 10;
  animation: grain-shift 0.5s steps(4) infinite;
}

/* Flash / overexposure effect on images */
.flash-effect {
  filter: contrast(1.2) brightness(1.1) saturate(0.85);
  position: relative;
}

.flash-effect::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.15) 0%,
    transparent 50%,
    rgba(0, 0, 0, 0.1) 100%
  );
  pointer-events: none;
}
```

### Sticker Badge

Small decorative badges that mimic peeling stickers, club entry stamps, and laptop decals scattered across layouts.

```css
.sleaze-sticker {
  display: inline-block;
  font-family: 'Permanent Marker', cursive;
  font-size: 0.8rem;
  padding: 0.4rem 0.8rem;
  background-color: var(--sleaze-yellow);
  color: var(--sleaze-black);
  transform: rotate(3deg);
  border-radius: 2px;
  box-shadow: 2px 2px 0 rgba(0, 0, 0, 0.3);
  position: relative;
  white-space: nowrap;
}

.sleaze-sticker--pink {
  background-color: var(--sleaze-pink);
  color: var(--sleaze-flash);
  transform: rotate(-2deg);
}

.sleaze-sticker--stamp {
  font-family: 'Bebas Neue', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  border: 2px solid var(--sleaze-pink);
  border-radius: 50%;
  width: 60px;
  height: 60px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: transparent;
  color: var(--sleaze-pink);
  transform: rotate(-15deg);
  padding: 0;
  font-size: 0.7rem;
}
```

---

## Design Do's and Don'ts

### Do

- **Embrace grain and noise**: Layer film grain, halftone dots, or subtle SVG noise textures over backgrounds and images to maintain the analog, lo-fi authenticity of the era
- **Use neon sparingly for maximum impact**: Reserve hot pink, electric yellow, and acid green for key interactive elements and focal points; let the dark background do the heavy lifting
- **Mix typefaces with intention**: Combine a clean condensed sans for structure with a hand-drawn marker font for personality; the tension between order and chaos is central to the aesthetic
- **Rotate and offset elements slightly**: Apply small CSS transforms (1-4 degrees) to cards, images, and pull quotes to break the grid and create the scattered, pinned-to-a-wall feeling
- **Reference the era's visual artifacts**: Include nods to flash photography, MySpace-era UI elements, disposable camera frames, Polaroid borders, and zine-style cutouts as decorative touches
- **Create depth with glow effects**: Use `box-shadow` and `text-shadow` with neon colors at low spread values to simulate the luminous haze of neon signs and club lighting
- **Design for darkness first**: Start with a near-black background and build upward; the darkness is not just a color choice but the foundational mood of the entire aesthetic
- **Include interactive surprise moments**: Hidden hover states, unexpected cursor changes, and subtle animations reward exploration the way discovering a new band at a random warehouse show did

### Don't

- **Don't use clean, corporate layouts**: Perfectly aligned grids, generous whitespace, and minimalist Swiss-style design are the antithesis of Indie Sleaze's chaotic energy
- **Don't over-saturate the neon**: If everything glows, nothing glows; using neon for every element creates visual fatigue and loses the contrast that makes the accents feel electric
- **Don't use stock photography**: Polished, well-lit, smiling-people stock photos destroy the gritty authenticity immediately; use grainy, candid, flash-lit imagery or no photography at all
- **Don't forget the grain**: A dark background with neon accents but no texture reads as generic dark-mode UI, not Indie Sleaze; the analog texture layer is what separates this from modern dark themes
- **Don't use rounded, friendly UI elements**: Large border-radius values, soft gradients, and bubbly shapes belong to other aesthetics; keep edges sharp or deliberately rough
- **Don't make it too legible**: While actual content should remain readable, the overall visual impression should feel slightly raw and challenging -- if it looks comfortable, it is not sleazy enough
- **Don't use pastel colors**: Soft, muted pastels belong to Tumblr Soft Grunge or Cottagecore; Indie Sleaze demands harsh, vibrating neon against deep black
- **Don't neglect performance for effect**: Film grain animations and glow effects should use GPU-accelerated properties (transform, opacity) to avoid janky scrolling on mobile devices

---

## Related Aesthetics

| Aesthetic | Relationship |
|---|---|
| [Y2K Futurism](Y2K_Futurism.md) | Chronological predecessor; shares the neon palette and nightlife energy but Y2K leans cleaner, more chrome and cyber, while Indie Sleaze is grittier and more analog |
| [DIY Punk](DIY_Punk.md) | Spiritual ancestor; shares the anti-corporate, handmade, zine-culture ethos but Punk is more political and monochrome where Indie Sleaze is hedonistic and neon-soaked |
| [Vaporwave](Vaporwave.md) | Fellow nostalgia-driven aesthetic; both mine recent cultural history for visual material, but Vaporwave is ironic and pastel while Indie Sleaze is earnest and harsh |
| [Grunge Revival](Grunge_Revival.md) | Shares the gritty texture and anti-polish philosophy; Grunge leans toward flannel earth tones and 90s melancholy while Indie Sleaze is neon-lit and hedonistic |
| [McBling](McBling.md) | Direct cultural opponent from the same era; McBling is polished, logo-driven maximalism while Indie Sleaze is raw, thrift-store maximalism -- the two defined the mid-2000s tension |
| [Tumblr Aesthetic](Tumblr_Aesthetic.md) | Platform overlap; Indie Sleaze content lived on Tumblr but the broader Tumblr aesthetic tends softer and more curated while Indie Sleaze is deliberately messy |
| [Lo-Fi / Analog](Lo_Fi_Analog.md) | Shares the celebration of analog imperfection, film grain, and cassette-tape warmth; Lo-Fi is quieter and more contemplative where Indie Sleaze is loud and nocturnal |
| [Wabi-Sabi](Wabi_Sabi.md) | Both find beauty in imperfection, but Wabi-Sabi is serene, natural, and meditative while Indie Sleaze is urban, nocturnal, and chaotic |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NITE CRAWL - Indie Sleaze Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Anton&family=Barlow+Condensed:wght@300;400;600&family=Bebas+Neue&family=Permanent+Marker&family=Special+Elite&display=swap" rel="stylesheet">
  <style>
    /* --- Custom Properties --- */
    :root {
      --sleaze-black: #0a0a0a;
      --sleaze-charcoal: #1c1c1c;
      --sleaze-smoke: #2e2e2e;
      --sleaze-flash: #f5f0eb;
      --sleaze-cream: #f0e6d3;
      --sleaze-pink: #ff2d87;
      --sleaze-yellow: #ffe714;
      --sleaze-green: #39ff14;
      --sleaze-purple: #8b2fc9;
      --sleaze-gold: #c9a84c;
      --sleaze-red: #cc1100;
      --sleaze-ash: #8a8a8a;
      --sleaze-blue: #1a3a5c;
      --sleaze-silver: #c0c0c0;
      --glow-pink: 0 0 20px rgba(255, 45, 135, 0.6);
      --glow-yellow: 0 0 20px rgba(255, 231, 20, 0.5);
      --glow-green: 0 0 20px rgba(57, 255, 20, 0.5);
    }

    /* --- Reset --- */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    /* --- Base --- */
    body {
      font-family: 'Barlow Condensed', 'Arial Narrow', Helvetica, sans-serif;
      font-weight: 400;
      font-size: 17px;
      line-height: 1.6;
      color: var(--sleaze-flash);
      background-color: var(--sleaze-black);
    }

    /* --- Film Grain Overlay --- */
    body::after {
      content: '';
      position: fixed;
      inset: 0;
      background: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.07'/%3E%3C/svg%3E");
      pointer-events: none;
      z-index: 9999;
      mix-blend-mode: overlay;
      opacity: 0.5;
    }

    /* --- Typography --- */
    h1, h2, h3, h4 {
      font-family: 'Bebas Neue', 'Anton', 'Impact', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      line-height: 0.95;
    }

    a { color: var(--sleaze-pink); text-decoration: none; transition: all 0.15s ease; }
    a:hover { color: var(--sleaze-yellow); text-shadow: var(--glow-yellow); }

    /* --- Navigation --- */
    .nav {
      background-color: var(--sleaze-black);
      border-bottom: 1px solid var(--sleaze-smoke);
      padding: 0 2rem;
      position: sticky;
      top: 0;
      z-index: 1000;
      display: flex;
      align-items: center;
    }

    .nav-logo {
      font-family: 'Permanent Marker', cursive;
      font-size: 1.4rem;
      color: var(--sleaze-pink);
      text-shadow: var(--glow-pink);
      margin-right: auto;
      padding: 0.7rem 0;
    }

    .nav ul { list-style: none; display: flex; gap: 0; }

    .nav a {
      display: block;
      padding: 0.9rem 1rem;
      color: var(--sleaze-ash);
      font-family: 'Bebas Neue', sans-serif;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      border-bottom: 2px solid transparent;
    }

    .nav a:hover {
      color: var(--sleaze-pink);
      border-bottom-color: var(--sleaze-pink);
      text-shadow: var(--glow-pink);
    }

    /* --- Hero --- */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 4rem 2.5rem;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: -30%;
      right: -15%;
      width: 700px;
      height: 700px;
      background: radial-gradient(circle, rgba(255, 45, 135, 0.12) 0%, transparent 65%);
      pointer-events: none;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: -20%;
      left: -10%;
      width: 500px;
      height: 500px;
      background: radial-gradient(circle, rgba(255, 231, 20, 0.06) 0%, transparent 65%);
      pointer-events: none;
    }

    .hero > * { position: relative; z-index: 2; }

    .hero h1 {
      font-family: 'Anton', sans-serif;
      font-size: clamp(4rem, 13vw, 14rem);
      line-height: 0.88;
      color: var(--sleaze-flash);
      margin: 0;
    }

    .hero h1 .neon { color: var(--sleaze-pink); text-shadow: var(--glow-pink); }
    .hero h1 .neon-y { color: var(--sleaze-yellow); text-shadow: var(--glow-yellow); }

    .hero .subtitle {
      font-family: 'Permanent Marker', cursive;
      font-size: clamp(1rem, 2.5vw, 1.6rem);
      color: var(--sleaze-yellow);
      margin-top: 1rem;
      transform: rotate(-2deg);
      display: inline-block;
    }

    .hero .desc {
      font-size: clamp(1rem, 1.8vw, 1.25rem);
      font-weight: 300;
      color: var(--sleaze-ash);
      max-width: 50ch;
      margin-top: 1.5rem;
    }

    .btn-row { display: flex; flex-wrap: wrap; gap: 1rem; margin-top: 2rem; }

    /* --- Buttons --- */
    .btn {
      display: inline-block;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.05rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      padding: 0.75rem 2rem;
      border: 2px solid var(--sleaze-pink);
      color: var(--sleaze-pink);
      background: transparent;
      cursor: pointer;
      text-decoration: none;
      transition: all 0.2s ease;
    }

    .btn:hover {
      background: var(--sleaze-pink);
      color: var(--sleaze-black);
      box-shadow: var(--glow-pink);
      text-shadow: none;
    }

    .btn--solid {
      background: var(--sleaze-pink);
      color: var(--sleaze-black);
    }

    .btn--solid:hover {
      background: var(--sleaze-flash);
      border-color: var(--sleaze-flash);
      box-shadow: 0 0 30px rgba(255, 45, 135, 0.3);
    }

    .btn--yellow { border-color: var(--sleaze-yellow); color: var(--sleaze-yellow); }
    .btn--yellow:hover { background: var(--sleaze-yellow); color: var(--sleaze-black); box-shadow: var(--glow-yellow); }

    /* --- Section --- */
    .section {
      padding: 5rem 2.5rem;
      position: relative;
    }

    .section h2 {
      font-size: clamp(2.5rem, 6vw, 5rem);
      margin-bottom: 1rem;
    }

    .section h2 .accent { color: var(--sleaze-pink); }
    .section .lead { color: var(--sleaze-ash); max-width: 60ch; margin-bottom: 2.5rem; font-weight: 300; }

    /* --- Photo Grid --- */
    .photo-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 1.5rem;
      margin-top: 2rem;
    }

    .photo-card {
      background: var(--sleaze-charcoal);
      border: 1px solid var(--sleaze-smoke);
      overflow: hidden;
      position: relative;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    .photo-card:nth-child(odd) { transform: rotate(-1.5deg); }
    .photo-card:nth-child(even) { transform: rotate(1deg); }
    .photo-card:hover { transform: rotate(0deg) scale(1.02); box-shadow: var(--glow-pink); z-index: 2; }

    .photo-card .img-placeholder {
      width: 100%;
      aspect-ratio: 4 / 3;
      background: linear-gradient(135deg, var(--sleaze-smoke) 0%, var(--sleaze-charcoal) 50%, var(--sleaze-smoke) 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Permanent Marker', cursive;
      font-size: 2rem;
      color: var(--sleaze-smoke);
      overflow: hidden;
      position: relative;
    }

    .photo-card .img-placeholder::after {
      content: '';
      position: absolute;
      inset: 0;
      background: linear-gradient(135deg, rgba(255, 255, 255, 0.08) 0%, transparent 50%, rgba(0, 0, 0, 0.1) 100%);
    }

    .photo-card .card-body {
      padding: 1rem 1.2rem;
    }

    .photo-card .card-title {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.2rem;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      color: var(--sleaze-flash);
    }

    .photo-card .card-meta {
      font-size: 0.8rem;
      color: var(--sleaze-ash);
      margin-top: 0.25rem;
    }

    .photo-card .tag {
      display: inline-block;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 0.7rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      border: 1px solid var(--sleaze-pink);
      color: var(--sleaze-pink);
      padding: 0.15rem 0.5rem;
      margin-top: 0.5rem;
      margin-right: 0.3rem;
    }

    /* --- Pull Quote --- */
    .pullquote {
      font-family: 'Permanent Marker', cursive;
      font-size: clamp(1.5rem, 3.5vw, 2.5rem);
      color: var(--sleaze-yellow);
      line-height: 1.35;
      padding: 3rem;
      margin: 0;
      border-left: 4px solid var(--sleaze-pink);
      background: var(--sleaze-charcoal);
      transform: rotate(-1deg);
      position: relative;
    }

    .pullquote::before {
      content: '\201C';
      font-size: 5rem;
      color: var(--sleaze-pink);
      position: absolute;
      top: 0;
      left: 0.5rem;
      line-height: 1;
      opacity: 0.4;
    }

    .pullquote cite {
      display: block;
      font-family: 'Barlow Condensed', sans-serif;
      font-style: normal;
      font-size: 0.85rem;
      color: var(--sleaze-ash);
      margin-top: 1rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    /* --- Lineup / Events --- */
    .lineup {
      text-align: center;
      padding: 4rem 2rem;
      background: var(--sleaze-charcoal);
      border: 1px solid var(--sleaze-smoke);
      margin-top: 2.5rem;
      position: relative;
    }

    .lineup .date {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1rem;
      color: var(--sleaze-yellow);
      letter-spacing: 0.3em;
      text-transform: uppercase;
      text-shadow: var(--glow-yellow);
    }

    .lineup .headliner {
      font-family: 'Anton', sans-serif;
      font-size: clamp(3rem, 9vw, 7rem);
      color: var(--sleaze-flash);
      text-transform: uppercase;
      line-height: 0.95;
      margin: 0.5rem 0;
    }

    .lineup .support {
      font-family: 'Bebas Neue', sans-serif;
      font-size: clamp(1.3rem, 3.5vw, 2.2rem);
      color: var(--sleaze-pink);
      text-transform: uppercase;
      letter-spacing: 0.06em;
    }

    .lineup .openers {
      font-size: 0.95rem;
      color: var(--sleaze-ash);
      text-transform: uppercase;
      letter-spacing: 0.12em;
      margin-top: 0.5rem;
    }

    .lineup .venue {
      font-family: 'Special Elite', monospace;
      font-size: 0.85rem;
      color: var(--sleaze-gold);
      margin-top: 1.5rem;
      letter-spacing: 0.08em;
    }

    .lineup-divider {
      width: 60px;
      height: 2px;
      background: var(--sleaze-pink);
      margin: 2.5rem auto;
      box-shadow: var(--glow-pink);
    }

    /* --- Stickers --- */
    .sticker {
      display: inline-block;
      font-family: 'Permanent Marker', cursive;
      font-size: 0.8rem;
      padding: 0.35rem 0.7rem;
      background: var(--sleaze-yellow);
      color: var(--sleaze-black);
      transform: rotate(3deg);
      box-shadow: 2px 2px 0 rgba(0, 0, 0, 0.3);
      white-space: nowrap;
    }

    .sticker--pink { background: var(--sleaze-pink); color: var(--sleaze-flash); transform: rotate(-2deg); }
    .sticker--green { background: var(--sleaze-green); color: var(--sleaze-black); transform: rotate(4deg); }

    /* --- Newsletter --- */
    .newsletter {
      padding: 4rem 2.5rem;
      text-align: center;
      border-top: 1px solid var(--sleaze-smoke);
    }

    .newsletter h2 {
      font-family: 'Permanent Marker', cursive;
      font-size: clamp(1.8rem, 4vw, 3rem);
      color: var(--sleaze-pink);
      text-shadow: var(--glow-pink);
      transform: rotate(-1.5deg);
      margin-bottom: 0.5rem;
    }

    .newsletter p {
      color: var(--sleaze-ash);
      margin-bottom: 1.5rem;
      font-weight: 300;
    }

    .newsletter-form {
      display: flex;
      gap: 0;
      max-width: 450px;
      margin: 0 auto;
    }

    .newsletter-form input {
      flex: 1;
      font-family: 'Barlow Condensed', sans-serif;
      font-size: 1rem;
      padding: 0.75rem 1rem;
      background: var(--sleaze-charcoal);
      border: 2px solid var(--sleaze-smoke);
      border-right: none;
      color: var(--sleaze-flash);
      outline: none;
    }

    .newsletter-form input::placeholder { color: var(--sleaze-ash); }
    .newsletter-form input:focus { border-color: var(--sleaze-pink); }

    .newsletter-form button {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      padding: 0.75rem 1.5rem;
      background: var(--sleaze-pink);
      color: var(--sleaze-black);
      border: 2px solid var(--sleaze-pink);
      cursor: pointer;
      transition: all 0.2s ease;
    }

    .newsletter-form button:hover {
      background: var(--sleaze-flash);
      border-color: var(--sleaze-flash);
    }

    /* --- Footer --- */
    .footer {
      padding: 3rem 2.5rem;
      border-top: 1px solid var(--sleaze-smoke);
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 2rem;
    }

    .footer h4 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 0.9rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--sleaze-flash);
      margin-bottom: 0.75rem;
    }

    .footer ul { list-style: none; }
    .footer li { padding: 0.2rem 0; }
    .footer a { color: var(--sleaze-ash); font-size: 0.9rem; }
    .footer a:hover { color: var(--sleaze-pink); }

    .footer-bottom {
      padding: 1.5rem 2.5rem;
      border-top: 1px solid var(--sleaze-smoke);
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 1rem;
    }

    .footer-bottom p {
      font-size: 0.8rem;
      color: var(--sleaze-ash);
    }

    .footer-bottom .logo-text {
      font-family: 'Permanent Marker', cursive;
      color: var(--sleaze-pink);
      text-shadow: var(--glow-pink);
      font-size: 1.1rem;
    }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      .nav { padding: 0 1.2rem; }
      .nav-logo { font-size: 1.2rem; }
      .nav a { padding: 0.7rem 0.6rem; font-size: 0.8rem; letter-spacing: 0.08em; }
      .hero { padding: 3rem 1.5rem; min-height: 85vh; }
      .section { padding: 3.5rem 1.5rem; }
      .pullquote { padding: 2rem 1.5rem; font-size: 1.3rem; }
      .lineup { padding: 3rem 1.5rem; }
      .photo-card:nth-child(odd),
      .photo-card:nth-child(even) { transform: none; }
      .photo-card:hover { transform: scale(1.01); }
      .newsletter { padding: 3rem 1.5rem; }
      .newsletter-form { flex-direction: column; gap: 0; }
      .newsletter-form input { border-right: 2px solid var(--sleaze-smoke); border-bottom: none; }
      .footer { padding: 2rem 1.5rem; }
      .footer-bottom { padding: 1.5rem; }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="nav">
    <span class="nav-logo">NITE CRAWL</span>
    <ul>
      <li><a href="#photos">Photos</a></li>
      <li><a href="#events">Events</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#subscribe">Subscribe</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <section class="hero" id="top">
    <h1>
      LAST<br>
      <span class="neon">NITE</span><br>
      <span class="neon-y">WAS</span><br>
      WILD
    </h1>
    <span class="subtitle">Brooklyn, NY &mdash; Since 2007</span>
    <p class="desc">
      Documenting the flash-lit chaos of the underground.
      Basement shows, rooftop parties, dive bar dance floors,
      and everything in between. No filters. No apologies.
    </p>
    <div class="btn-row">
      <a href="#photos" class="btn btn--solid">View Gallery</a>
      <a href="#events" class="btn btn--yellow">Upcoming Shows</a>
    </div>
  </section>

  <!-- PHOTO GALLERY -->
  <section class="section" id="photos">
    <h2>THE <span class="accent">ROLL</span></h2>
    <p class="lead">
      36 exposures. One disposable camera. No second takes.
      Every frame from last weekend's crawl through Bushwick.
    </p>
    <div class="photo-grid">
      <div class="photo-card">
        <div class="img-placeholder">01</div>
        <div class="card-body">
          <div class="card-title">Glasslands Gallery</div>
          <div class="card-meta">Kent Ave, Williamsburg &mdash; 11:47 PM</div>
          <span class="tag">Flash</span>
          <span class="tag">Crowd</span>
        </div>
      </div>
      <div class="photo-card">
        <div class="img-placeholder">02</div>
        <div class="card-body">
          <div class="card-title">Bathroom Line Confessional</div>
          <div class="card-meta">Death By Audio &mdash; 12:30 AM</div>
          <span class="tag">Candid</span>
          <span class="tag">Portrait</span>
        </div>
      </div>
      <div class="photo-card">
        <div class="img-placeholder">03</div>
        <div class="card-body">
          <div class="card-title">DJ Booth Smoke Machine</div>
          <div class="card-meta">285 Kent &mdash; 1:15 AM</div>
          <span class="tag">Electro</span>
          <span class="tag">Haze</span>
        </div>
      </div>
      <div class="photo-card">
        <div class="img-placeholder">04</div>
        <div class="card-body">
          <div class="card-title">Sidewalk Cigarette Break</div>
          <div class="card-meta">Grand St, Williamsburg &mdash; 2:03 AM</div>
          <span class="tag">Street</span>
        </div>
      </div>
      <div class="photo-card">
        <div class="img-placeholder">05</div>
        <div class="card-body">
          <div class="card-title">Sequin Jacket Mosh Pit</div>
          <div class="card-meta">Market Hotel, Bushwick &mdash; 1:45 AM</div>
          <span class="tag">Messy</span>
          <span class="tag">Live</span>
        </div>
      </div>
      <div class="photo-card">
        <div class="img-placeholder">06</div>
        <div class="card-body">
          <div class="card-title">Rooftop Dawn Survivors</div>
          <div class="card-meta">Somewhere in Bushwick &mdash; 5:20 AM</div>
          <span class="tag">Golden Hour</span>
        </div>
      </div>
    </div>
  </section>

  <!-- PULL QUOTE -->
  <section class="section" style="padding-top: 2rem; padding-bottom: 2rem;">
    <blockquote class="pullquote">
      The best photos happen when nobody is posing and the flash is the only light source.
      <cite>Shot on a Canon PowerShot, 2009</cite>
    </blockquote>
  </section>

  <!-- EVENTS / LINEUP -->
  <section class="section" id="events">
    <h2>COMING <span class="accent">UP</span></h2>
    <p class="lead">
      Our picks for the shows worth losing sleep over this month.
      Get there early. Leave when they kick you out.
    </p>

    <div class="lineup">
      <div class="date">Friday &mdash; Feb 21, 2026</div>
      <div class="headliner">Crystal Castles</div>
      <div class="support">Health &bull; Salem</div>
      <div class="openers">DJ sets by Frankie Chan + Mishka</div>
      <div class="venue">Market Hotel &mdash; 1140 Myrtle Ave, Brooklyn &mdash; Doors 9PM &mdash; $12</div>
    </div>

    <div class="lineup-divider"></div>

    <div class="lineup">
      <div class="date">Saturday &mdash; Feb 22, 2026</div>
      <div class="headliner">CSS</div>
      <div class="support">Matt & Kim &bull; Sleigh Bells</div>
      <div class="openers">Hosted by Misshapes</div>
      <div class="venue">Glasslands Gallery &mdash; 289 Kent Ave, Brooklyn &mdash; Doors 10PM &mdash; $15</div>
    </div>

    <div class="lineup-divider"></div>

    <div class="lineup">
      <div class="date">Thursday &mdash; Feb 27, 2026</div>
      <div class="headliner">MGMT</div>
      <div class="support">Yeasayer &bull; Neon Indian</div>
      <div class="openers">Afterparty TBA</div>
      <div class="venue">Music Hall of Williamsburg &mdash; 66 N 6th St, Brooklyn &mdash; Doors 8PM &mdash; $18</div>
    </div>
  </section>

  <!-- ABOUT -->
  <section class="section" id="about" style="border-top: 1px solid var(--sleaze-smoke);">
    <h2>ABOUT <span class="accent">US</span></h2>
    <p class="lead">
      NITE CRAWL started in 2007 as a Blogspot page run out of a Williamsburg
      apartment. One camera, one flash, and an open invitation to document
      whatever happened between midnight and sunrise.
    </p>
    <p style="color: var(--sleaze-ash); max-width: 60ch; margin-bottom: 1.5rem; font-weight: 300;">
      What started as a personal photo diary became the go-to nightlife
      chronicle for a scene that existed between MySpace and Instagram,
      between The Strokes and Vampire Weekend, between cheap PBR and
      overpriced cocktails. We archived the basement shows, the warehouse
      parties, the sidewalk aftermaths, and the cab rides home at dawn.
    </p>
    <div style="display: flex; gap: 0.75rem; flex-wrap: wrap;">
      <span class="sticker">EST. 2007</span>
      <span class="sticker--pink sticker">NO FLASH NO ENTRY</span>
      <span class="sticker--green sticker">ALWAYS OPEN</span>
    </div>
  </section>

  <!-- NEWSLETTER -->
  <section class="newsletter" id="subscribe">
    <h2>Get on the List</h2>
    <p>Weekly dispatches from the underground. Delivered Thursdays at midnight.</p>
    <form class="newsletter-form" onsubmit="return false;">
      <input type="email" placeholder="your@email.com" aria-label="Email address">
      <button type="submit">Subscribe</button>
    </form>
  </section>

  <!-- FOOTER -->
  <footer class="footer">
    <div>
      <h4>Navigate</h4>
      <ul>
        <li><a href="#photos">Photo Roll</a></li>
        <li><a href="#events">Upcoming Shows</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#subscribe">Newsletter</a></li>
      </ul>
    </div>
    <div>
      <h4>Archive</h4>
      <ul>
        <li><a href="#">2009 &mdash; The Early Days</a></li>
        <li><a href="#">2010 &mdash; Peak Sleaze</a></li>
        <li><a href="#">2011 &mdash; Last Call</a></li>
        <li><a href="#">2012 &mdash; The Hangover</a></li>
      </ul>
    </div>
    <div>
      <h4>Connect</h4>
      <ul>
        <li><a href="#">Tumblr</a></li>
        <li><a href="#">Flickr</a></li>
        <li><a href="#">Last.fm</a></li>
        <li><a href="#">RSS Feed</a></li>
      </ul>
    </div>
    <div>
      <h4>Legal</h4>
      <ul>
        <li><a href="#">Privacy Policy</a></li>
        <li><a href="#">Photo Credits</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </div>
  </footer>

  <div class="footer-bottom">
    <span class="logo-text">NITE CRAWL</span>
    <p>No rights reserved. Steal this website. &copy; 2007&ndash;forever.</p>
  </div>

</body>
</html>
```
