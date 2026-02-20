# Editorial / Magazine Layout Design Reference

Editorial / Magazine Layout is a sophisticated web design aesthetic rooted in centuries of print publication craft, brought into the digital realm with modern CSS capabilities. Pioneered by legendary art directors like Alexey Brodovitch at Harper's Bazaar (1934-1958), the editorial style treats every page as a deliberate composition where asymmetric grids, generous whitespace, commanding typography, and carefully orchestrated visual hierarchy guide the reader's eye with effortless authority. Unlike rigid corporate layouts or maximalist trends, editorial design breathes -- it uses negative space as a structural element, lets oversized serif headlines anchor the visual rhythm, and balances text and imagery with the precision of a gallery curator. In web and UI design, this translates to asymmetric multi-column grids, dramatic type scale contrasts between display headings and body copy, pull quotes that break the column flow, elegant drop caps, full-bleed photography with intentional crops, and an overall sense of restrained luxury that whispers rather than shouts. The aesthetic conveys intelligence, cultural awareness, and quiet confidence.

---

## Visual Characteristics

### Core Design Traits

- **Asymmetric grid layouts** -- columns of unequal width creating dynamic tension and visual interest, breaking from predictable symmetry
- **Dramatic type scale contrast** -- extreme size differences between display headings and body text, often 10:1 or greater ratios
- **Generous whitespace** -- negative space used as a deliberate compositional element, not empty filler; margins and gutters are luxuriously wide
- **Sophisticated serif typography** -- high-contrast serif faces for headlines that evoke literary authority and editorial credibility
- **Drop caps** -- oversized initial letters that mark the beginning of articles, a direct inheritance from print magazine tradition
- **Pull quotes** -- extracted quotations set in large, decorative type that break up body text and create visual entry points
- **Full-bleed photography** -- images that extend edge-to-edge, often with intentional cropping to create cinematic compositions
- **Ruled lines and dividers** -- thin hairline rules that organize content vertically and horizontally, referencing newspaper column dividers
- **Muted, restrained color palettes** -- neutral foundations with selective accent colors; color is used sparingly and with purpose
- **Layered reading hierarchy** -- section labels, kickers, headlines, decks, bylines, body text, and captions each have distinct typographic treatments
- **Text wrapping around images** -- editorial layouts allow text to flow around irregularly placed images, breaking the rigid box model
- **Column-based body text** -- multi-column article text referencing traditional print layouts, with optimal 50-70 character line lengths

### Design Principles

- Treat whitespace as a primary design element, not leftover space -- it creates breathing room and directs attention
- Establish a strict typographic hierarchy with at least 5-6 distinct levels (label, headline, deck, byline, body, caption)
- Use asymmetry purposefully to create visual tension and guide the eye along a deliberate reading path
- Photography should be large, high-quality, and intentionally cropped -- never clip art or generic stock
- Restraint is the governing philosophy: every element must earn its place on the page
- Grid structures should be felt but not rigidly visible -- content should appear to float within an invisible framework
- Color should be used like a spice, not a main ingredient -- one or two accent colors maximum against neutrals
- Body text readability is paramount: proper line height, measure, and spacing are non-negotiable
- Create visual entry points (drop caps, pull quotes, large images) that invite the reader into the content
- The overall impression should be one of curated intelligence and unhurried elegance

---

## Color Palette

### Editorial Neutral Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Ink Black** | `#1A1A1A` | Primary headlines, display text |
| **Deep Charcoal** | `#2C2C2C` | Secondary headings, strong emphasis |
| **Body Text** | `#3D3D3D` | Article body copy, paragraphs |
| **Warm Gray** | `#6B6B6B` | Bylines, captions, metadata |
| **Silver** | `#9A9A9A` | Tertiary text, timestamps, labels |
| **Light Gray** | `#D4D4D4` | Borders, dividers, hairline rules |
| **Pale Stone** | `#E8E4DF` | Subtle backgrounds, blockquote panels |
| **Off-White** | `#F5F3F0` | Primary background, warm paper tone |
| **Pure White** | `#FFFFFF` | Card surfaces, overlay backgrounds |
| **Editorial Red** | `#C41E2A` | Accent color, drop caps, section labels |
| **Deep Navy** | `#1B2A4A` | Alternate accent, links, category markers |
| **Warm Gold** | `#B8860B` | Decorative accents, special features, folio lines |
| **Muted Sage** | `#7A8B6F` | Tertiary accent, tags, soft highlights |
| **Rich Burgundy** | `#6B1D2A` | Pull quote marks, special emphasis |

### CSS Custom Properties

```css
:root {
  /* Text hierarchy */
  --ed-ink: #1a1a1a;
  --ed-charcoal: #2c2c2c;
  --ed-body: #3d3d3d;
  --ed-gray: #6b6b6b;
  --ed-silver: #9a9a9a;

  /* Borders and rules */
  --ed-rule: #d4d4d4;
  --ed-rule-dark: #b0b0b0;

  /* Backgrounds */
  --ed-bg-stone: #e8e4df;
  --ed-bg-paper: #f5f3f0;
  --ed-bg-white: #ffffff;

  /* Accent colors */
  --ed-red: #c41e2a;
  --ed-navy: #1b2a4a;
  --ed-gold: #b8860b;
  --ed-sage: #7a8b6f;
  --ed-burgundy: #6b1d2a;

  /* Functional */
  --ed-link: #1b2a4a;
  --ed-link-hover: #c41e2a;
  --ed-selection-bg: rgba(196, 30, 42, 0.12);
  --ed-selection-text: #1a1a1a;

  /* Spacing scale */
  --ed-space-xs: 4px;
  --ed-space-sm: 8px;
  --ed-space-md: 16px;
  --ed-space-lg: 32px;
  --ed-space-xl: 64px;
  --ed-space-2xl: 96px;
  --ed-space-3xl: 128px;

  /* Content widths */
  --ed-width-narrow: 640px;
  --ed-width-article: 780px;
  --ed-width-wide: 1200px;
  --ed-width-full: 1440px;
}
```

---

## Typography

### Typeface Characteristics

Editorial / Magazine typography is:

- **Serif-dominant for display** -- high-contrast serif typefaces with dramatic thick-thin stroke variation command authority in headlines
- **Clean sans-serif for body** -- highly readable sans-serif or transitional serif for body text, optimized for long-form reading
- **Extreme scale contrast** -- display headings may be 60-120px while body text remains 17-19px, creating powerful visual hierarchy
- **Carefully measured line lengths** -- body text set to 50-70 characters per line (the typographic ideal for readability)
- **Generous line height** -- body text at 1.6-1.8 line-height for comfortable reading; headlines tighter at 1.0-1.15
- **Restrained weight usage** -- typically just 2-3 weights per typeface; bold is used sparingly and with intention
- **Italic for attribution** -- author names, pull quote attributions, and figure captions often set in italic
- **All-caps for labels** -- section identifiers, kickers, and category markers use small uppercase with wide letter-spacing
- **Optical sizing awareness** -- display faces for headlines, text-optimized faces for body, caption-optimized faces for small text

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Playfair Display** | High-contrast serif | Headlines, display text, hero titles |
| **DM Serif Display** | Elegant transitional serif | Headlines, pull quotes, feature titles |
| **Libre Baskerville** | Classic Baskerville revival | Headlines, body text, versatile |
| **Cormorant Garamond** | Refined Garamond interpretation | Display text, pull quotes, elegant headings |
| **Lora** | Contemporary serif | Body text, article copy, readable serif |
| **Source Serif 4** | Adobe's editorial serif | Body text, long-form reading, versatile |
| **Inter** | Highly readable sans-serif | Body text, UI elements, captions |
| **Source Sans 3** | Clean humanist sans | Body text, navigation, metadata |
| **Archivo** | Grotesque sans-serif | Labels, kickers, section markers |
| **Spline Sans** | Modern geometric sans | Navigation, UI text, metadata |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Playfair Display** (700) | **Source Sans 3** (400) | Classic editorial, high contrast elegance |
| **DM Serif Display** (400) | **Inter** (400) | Modern magazine, clean and refined |
| **Cormorant Garamond** (600) | **Source Serif 4** (400) | Literary, all-serif sophistication |
| **Libre Baskerville** (700) | **Inter** (400) | Traditional editorial meets digital clarity |
| **Playfair Display** (900) | **Lora** (400) | Luxury editorial, serif-on-serif warmth |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,400;1,700&family=Source+Sans+3:ital,wght@0,400;0,600;1,400&display=swap');

/* Base typography */
body {
  font-family: 'Source Sans 3', 'Georgia', serif;
  font-weight: 400;
  font-size: 1.0625rem; /* 17px */
  line-height: 1.75;
  color: var(--ed-body);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 700;
  color: var(--ed-ink);
  line-height: 1.1;
  letter-spacing: -0.015em;
}

/* Display headline -- the commanding feature headline */
.ed-display {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 900;
  font-size: clamp(3rem, 6vw, 5.5rem);
  line-height: 1.0;
  letter-spacing: -0.025em;
  color: var(--ed-ink);
}

/* Section kicker / label */
.ed-kicker {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--ed-red);
  margin-bottom: 0.75rem;
  display: block;
}

/* Deck / subtitle */
.ed-deck {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 1.35rem;
  font-weight: 400;
  line-height: 1.5;
  color: var(--ed-gray);
  margin-top: 1rem;
}

/* Byline */
.ed-byline {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.85rem;
  font-weight: 400;
  color: var(--ed-silver);
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.ed-byline strong {
  color: var(--ed-charcoal);
  font-weight: 600;
}

/* Caption */
.ed-caption {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.8rem;
  font-style: italic;
  line-height: 1.5;
  color: var(--ed-gray);
  margin-top: 0.5rem;
}

/* Pull quote */
.ed-pull-quote {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-size: 1.75rem;
  font-style: italic;
  font-weight: 400;
  line-height: 1.35;
  color: var(--ed-charcoal);
}
```

---

## Layout Principles

### Grid and Structure

- **Asymmetric multi-column grids** -- use CSS Grid with unequal column widths (e.g., 2fr 1fr, 3fr 2fr, or 1fr 2fr 1fr) to create the characteristic editorial tension
- **Narrow article measure** -- body text constrained to 640-780px max-width for optimal reading comfort (50-70 characters per line)
- **Wide outer margins** -- generous margins on both sides of the content column, allowing pull quotes and images to break into the margin space
- **Baseline grid alignment** -- all text elements snapping to a consistent vertical rhythm (e.g., increments of 8px or the body line-height)
- **Full-bleed image breaks** -- images that span the full viewport width, punctuating the narrower text column
- **Sidebar and margin content** -- annotations, captions, and secondary information placed in the margins alongside the main text column
- **Modular grid for feature sections** -- multi-column grids for article listings, category pages, and feature spreads
- **Vertical rhythm consistency** -- consistent spacing between sections creates a predictable, comfortable reading pace

### Section Organization

- **Masthead / Navigation**: Minimal, text-based navigation with the publication name in a distinctive serif or custom wordmark; thin rule underneath
- **Hero / Feature**: Large headline with extreme type scale, optional full-bleed image, kicker label, deck text, and byline -- this section breathes with whitespace
- **Article Body**: Single narrow column of body text, punctuated by drop caps, pull quotes, inline images, and subheadings
- **Image Breaks**: Full-width or asymmetrically placed photographs with captions, breaking the text column rhythm
- **Sidebar Modules**: Related articles, author bio, or contextual information placed in a narrower adjacent column
- **Section Dividers**: Thin hairline rules, asterisms (three centered dots/stars), or generous whitespace separating major sections
- **Article Grid / Index**: Multi-column layout for listing articles, using mixed card sizes to create visual hierarchy (one large feature + several smaller items)
- **Footer**: Minimal, restrained footer with thin rule above, muted text, and simple navigation links

### Responsive Approach

- On mobile, collapse asymmetric grids to a single column while maintaining generous side padding (24-32px minimum)
- Scale display headlines aggressively with `clamp()` but maintain the dramatic size contrast between headline and body
- Pull quotes become full-width on mobile instead of breaking into margins
- Full-bleed images remain full-bleed on all breakpoints; they are essential to the editorial rhythm
- Drop caps should remain but may reduce in scale slightly on smaller screens
- Multi-column article grids collapse from 3 or 4 columns to 2 on tablet, then 1 on mobile
- Maintain generous vertical spacing between sections -- do not compress whitespace on mobile
- Navigation collapses to a minimal hamburger or simple text toggle

---

## CSS / Design Techniques

### Editorial Card Component

```css
.ed-card {
  display: flex;
  flex-direction: column;
  background: var(--ed-bg-white);
  border: none;
  position: relative;
}

.ed-card__image {
  width: 100%;
  aspect-ratio: 3 / 2;
  object-fit: cover;
  display: block;
}

.ed-card__content {
  padding: 1.5rem 0;
}

.ed-card__category {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.7rem;
  font-weight: 600;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--ed-red);
  margin-bottom: 0.6rem;
  display: block;
}

.ed-card__title {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-size: 1.5rem;
  font-weight: 700;
  line-height: 1.2;
  color: var(--ed-ink);
  margin-bottom: 0.75rem;
  letter-spacing: -0.01em;
}

.ed-card__title a {
  color: inherit;
  text-decoration: none;
  transition: color 0.2s ease;
}

.ed-card__title a:hover {
  color: var(--ed-red);
}

.ed-card__excerpt {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.95rem;
  line-height: 1.6;
  color: var(--ed-gray);
  margin-bottom: 1rem;
}

.ed-card__meta {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.75rem;
  color: var(--ed-silver);
  text-transform: uppercase;
  letter-spacing: 0.06em;
}

/* Feature card -- larger variant */
.ed-card--feature .ed-card__title {
  font-size: 2.25rem;
  letter-spacing: -0.02em;
}

/* Horizontal card variant */
.ed-card--horizontal {
  flex-direction: row;
  gap: 1.5rem;
}

.ed-card--horizontal .ed-card__image {
  width: 40%;
  flex-shrink: 0;
  aspect-ratio: 4 / 3;
}

/* Article grid layout */
.ed-article-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 2rem;
}

.ed-article-grid .ed-card--feature {
  grid-column: 1 / -1;
}

@media (max-width: 768px) {
  .ed-article-grid {
    grid-template-columns: 1fr;
  }
  .ed-card--horizontal {
    flex-direction: column;
  }
  .ed-card--horizontal .ed-card__image {
    width: 100%;
  }
}
```

### Editorial Button

```css
.ed-button {
  display: inline-block;
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--ed-ink);
  background: transparent;
  border: 1.5px solid var(--ed-ink);
  padding: 12px 32px;
  text-decoration: none;
  cursor: pointer;
  transition: background 0.25s ease, color 0.25s ease;
}

.ed-button:hover {
  background: var(--ed-ink);
  color: var(--ed-bg-white);
}

/* Filled variant */
.ed-button--filled {
  background: var(--ed-ink);
  color: var(--ed-bg-white);
  border-color: var(--ed-ink);
}

.ed-button--filled:hover {
  background: var(--ed-charcoal);
  border-color: var(--ed-charcoal);
}

/* Red accent variant */
.ed-button--accent {
  color: var(--ed-red);
  border-color: var(--ed-red);
}

.ed-button--accent:hover {
  background: var(--ed-red);
  color: var(--ed-bg-white);
}

/* Text-only link button */
.ed-button--text {
  border: none;
  padding: 0;
  font-size: 0.8rem;
  letter-spacing: 0.1em;
  color: var(--ed-ink);
  position: relative;
}

.ed-button--text::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 100%;
  height: 1px;
  background: var(--ed-ink);
  transform: scaleX(0);
  transform-origin: right;
  transition: transform 0.3s ease;
}

.ed-button--text:hover::after {
  transform: scaleX(1);
  transform-origin: left;
}
```

### Navigation Bar

```css
.ed-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: var(--ed-width-wide);
  margin: 0 auto;
  padding: 1.5rem 2.5rem;
  border-bottom: 1px solid var(--ed-rule);
}

.ed-nav__masthead {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-size: 1.75rem;
  font-weight: 700;
  color: var(--ed-ink);
  text-decoration: none;
  letter-spacing: -0.02em;
}

.ed-nav__links {
  display: flex;
  gap: 2rem;
  list-style: none;
  margin: 0;
  padding: 0;
}

.ed-nav__links a {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  color: var(--ed-gray);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  transition: color 0.2s ease;
  position: relative;
}

.ed-nav__links a:hover {
  color: var(--ed-ink);
}

.ed-nav__links a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  width: 100%;
  height: 1px;
  background: var(--ed-ink);
  transform: scaleX(0);
  transform-origin: center;
  transition: transform 0.25s ease;
}

.ed-nav__links a:hover::after {
  transform: scaleX(1);
}

/* Section sub-navigation */
.ed-subnav {
  display: flex;
  justify-content: center;
  gap: 2.5rem;
  padding: 1rem 2.5rem;
  border-bottom: 1px solid var(--ed-rule);
  list-style: none;
  margin: 0;
}

.ed-subnav a {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--ed-silver);
  text-decoration: none;
  transition: color 0.2s ease;
}

.ed-subnav a:hover,
.ed-subnav a.active {
  color: var(--ed-ink);
}

@media (max-width: 768px) {
  .ed-nav { padding: 1rem 1.5rem; }
  .ed-nav__links { gap: 1.25rem; }
  .ed-subnav { gap: 1.25rem; overflow-x: auto; }
}
```

### Hero Section

```css
.ed-hero {
  max-width: var(--ed-width-wide);
  margin: 0 auto;
  padding: var(--ed-space-3xl) 2.5rem;
  text-align: center;
}

.ed-hero__kicker {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--ed-red);
  margin-bottom: 1.5rem;
  display: block;
}

.ed-hero__headline {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 900;
  font-size: clamp(2.75rem, 6vw, 5rem);
  line-height: 1.05;
  letter-spacing: -0.025em;
  color: var(--ed-ink);
  max-width: 900px;
  margin: 0 auto 1.5rem;
}

.ed-hero__deck {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 1.25rem;
  line-height: 1.6;
  color: var(--ed-gray);
  max-width: 600px;
  margin: 0 auto 1.5rem;
}

.ed-hero__byline {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.8rem;
  color: var(--ed-silver);
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.ed-hero__byline strong {
  color: var(--ed-charcoal);
  font-weight: 600;
}

/* Hero with full-bleed image */
.ed-hero--image {
  position: relative;
  max-width: 100%;
  padding: 0;
}

.ed-hero--image img {
  width: 100%;
  height: 70vh;
  object-fit: cover;
  display: block;
}

.ed-hero--image .ed-hero__content {
  max-width: var(--ed-width-article);
  margin: 0 auto;
  padding: var(--ed-space-xl) 2.5rem;
  text-align: center;
}

/* Split hero -- image + text side by side */
.ed-hero--split {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0;
  max-width: 100%;
  padding: 0;
  text-align: left;
}

.ed-hero--split img {
  width: 100%;
  height: 85vh;
  object-fit: cover;
}

.ed-hero--split .ed-hero__content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: var(--ed-space-xl) var(--ed-space-xl);
  max-width: 540px;
}

@media (max-width: 768px) {
  .ed-hero { padding: var(--ed-space-xl) 1.5rem; }
  .ed-hero--split { grid-template-columns: 1fr; }
  .ed-hero--split img { height: 50vh; }
  .ed-hero--split .ed-hero__content {
    padding: var(--ed-space-lg) 1.5rem;
    max-width: 100%;
  }
}
```

### Drop Cap

```css
/* Standard editorial drop cap */
.ed-dropcap::first-letter {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 700;
  font-size: 4.5em;
  float: left;
  line-height: 0.8;
  margin-right: 0.08em;
  margin-top: 0.05em;
  color: var(--ed-ink);
}

/* Red accent drop cap */
.ed-dropcap--accent::first-letter {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 900;
  font-size: 5em;
  float: left;
  line-height: 0.75;
  margin-right: 0.1em;
  margin-top: 0.05em;
  color: var(--ed-red);
}

/* Drop cap with background block */
.ed-dropcap--block::first-letter {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 700;
  font-size: 3.5em;
  float: left;
  line-height: 1;
  margin-right: 0.15em;
  padding: 0.05em 0.15em;
  background: var(--ed-ink);
  color: var(--ed-bg-white);
}
```

### Pull Quote

```css
/* Standard pull quote */
.ed-pull-quote {
  margin: var(--ed-space-xl) 0;
  padding: var(--ed-space-lg) 0;
  border-top: 2px solid var(--ed-ink);
  border-bottom: 1px solid var(--ed-rule);
}

.ed-pull-quote blockquote {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-size: 1.85rem;
  font-style: italic;
  font-weight: 400;
  line-height: 1.35;
  color: var(--ed-charcoal);
  margin: 0 0 1rem;
}

.ed-pull-quote cite {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.8rem;
  font-style: normal;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--ed-silver);
}

/* Margin pull quote -- breaks out of the text column */
.ed-pull-quote--margin {
  float: right;
  width: 280px;
  margin: 0 -120px var(--ed-space-lg) var(--ed-space-lg);
  padding: var(--ed-space-lg) 0 var(--ed-space-lg) var(--ed-space-lg);
  border-top: none;
  border-bottom: none;
  border-left: 2px solid var(--ed-red);
}

.ed-pull-quote--margin blockquote {
  font-size: 1.35rem;
}

/* Large centered pull quote with decorative marks */
.ed-pull-quote--large {
  text-align: center;
  margin: var(--ed-space-2xl) auto;
  max-width: 700px;
  border-top: none;
  border-bottom: none;
  position: relative;
  padding: var(--ed-space-xl) 0;
}

.ed-pull-quote--large::before {
  content: '\201C'; /* left double quotation mark */
  font-family: 'Playfair Display', 'Georgia', serif;
  font-size: 6rem;
  color: var(--ed-red);
  position: absolute;
  top: -0.2em;
  left: 50%;
  transform: translateX(-50%);
  line-height: 1;
  opacity: 0.3;
}

.ed-pull-quote--large blockquote {
  font-size: 2.25rem;
  line-height: 1.3;
}

@media (max-width: 768px) {
  .ed-pull-quote--margin {
    float: none;
    width: 100%;
    margin: var(--ed-space-lg) 0;
    padding: var(--ed-space-lg) 0;
    border-left: 2px solid var(--ed-red);
    padding-left: var(--ed-space-lg);
  }
  .ed-pull-quote--large blockquote {
    font-size: 1.5rem;
  }
}
```

### Asymmetric Grid Layout

```css
/* 7-column editorial grid -- the classic magazine grid */
.ed-grid-7 {
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  gap: 1.5rem;
  max-width: var(--ed-width-full);
  margin: 0 auto;
  padding: 0 2.5rem;
}

/* Asymmetric 2-column: wide content + narrow sidebar */
.ed-layout-article {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: var(--ed-space-xl);
  max-width: var(--ed-width-wide);
  margin: 0 auto;
  padding: var(--ed-space-xl) 2.5rem;
}

/* Asymmetric 2-column: narrow sidebar + wide content */
.ed-layout-article--reversed {
  grid-template-columns: 1fr 2fr;
}

/* Asymmetric 3-column feature layout */
.ed-layout-feature {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  gap: var(--ed-space-lg);
  max-width: var(--ed-width-wide);
  margin: 0 auto;
  padding: var(--ed-space-xl) 2.5rem;
  align-items: start;
}

/* The center column holds the main article */
.ed-layout-feature__main {
  grid-column: 2;
}

/* Left and right columns for margin notes, captions, pull quotes */
.ed-layout-feature__aside {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.85rem;
  color: var(--ed-gray);
  padding-top: 0.25rem;
}

/* Mixed-size article grid for index / section pages */
.ed-grid-mixed {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: auto;
  gap: 2rem;
  max-width: var(--ed-width-wide);
  margin: 0 auto;
  padding: var(--ed-space-xl) 2.5rem;
}

/* Feature story spans 2 columns and 2 rows */
.ed-grid-mixed__feature {
  grid-column: span 2;
  grid-row: span 2;
}

/* Standard story occupies 1 cell */
.ed-grid-mixed__standard {
  grid-column: span 1;
}

/* Wide story spans 2 columns */
.ed-grid-mixed__wide {
  grid-column: span 2;
}

@media (max-width: 1024px) {
  .ed-layout-article { grid-template-columns: 1fr; }
  .ed-layout-article--reversed { grid-template-columns: 1fr; }
  .ed-layout-feature { grid-template-columns: 1fr; }
  .ed-layout-feature__main { grid-column: 1; }
  .ed-grid-mixed { grid-template-columns: repeat(2, 1fr); }
  .ed-grid-mixed__feature { grid-column: span 2; grid-row: span 1; }
}

@media (max-width: 768px) {
  .ed-grid-mixed { grid-template-columns: 1fr; }
  .ed-grid-mixed__feature { grid-column: span 1; }
  .ed-grid-mixed__wide { grid-column: span 1; }
}
```

### Editorial Image Treatments

```css
/* Full-bleed image -- breaks out of article column */
.ed-image-full {
  width: 100vw;
  margin-left: calc(-50vw + 50%);
  margin-top: var(--ed-space-xl);
  margin-bottom: var(--ed-space-xl);
}

.ed-image-full img {
  width: 100%;
  height: auto;
  display: block;
}

.ed-image-full figcaption {
  max-width: var(--ed-width-article);
  margin: 0.75rem auto 0;
  padding: 0 2.5rem;
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.8rem;
  font-style: italic;
  color: var(--ed-gray);
}

/* Offset image -- asymmetric placement breaking the text column */
.ed-image-offset {
  float: right;
  width: 55%;
  margin: 0 calc(-10% - 2.5rem) var(--ed-space-lg) var(--ed-space-lg);
  position: relative;
}

.ed-image-offset img {
  width: 100%;
  height: auto;
  display: block;
}

.ed-image-offset figcaption {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.8rem;
  font-style: italic;
  color: var(--ed-gray);
  margin-top: 0.5rem;
}

/* Image with border frame */
.ed-image-framed {
  padding: var(--ed-space-sm);
  border: 1px solid var(--ed-rule);
  display: inline-block;
}

.ed-image-framed img {
  display: block;
  width: 100%;
  height: auto;
}

/* Image duo -- two images side by side with unequal sizes */
.ed-image-duo {
  display: grid;
  grid-template-columns: 3fr 2fr;
  gap: var(--ed-space-md);
  margin: var(--ed-space-xl) 0;
}

.ed-image-duo img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* Inset image with text wrap */
.ed-image-inset {
  float: left;
  width: 45%;
  margin: 0.25rem var(--ed-space-lg) var(--ed-space-md) 0;
}

.ed-image-inset img {
  width: 100%;
  height: auto;
  display: block;
}

@media (max-width: 768px) {
  .ed-image-offset {
    float: none;
    width: 100%;
    margin: var(--ed-space-lg) 0;
  }
  .ed-image-duo { grid-template-columns: 1fr; }
  .ed-image-inset {
    float: none;
    width: 100%;
    margin: var(--ed-space-lg) 0;
  }
}
```

### Section Dividers and Rules

```css
/* Thin hairline rule */
.ed-rule {
  border: none;
  height: 1px;
  background: var(--ed-rule);
  margin: var(--ed-space-xl) 0;
}

/* Heavy rule -- used above section headings */
.ed-rule--heavy {
  height: 3px;
  background: var(--ed-ink);
}

/* Double rule */
.ed-rule--double {
  height: 0;
  border: none;
  border-top: 3px solid var(--ed-ink);
  border-bottom: 1px solid var(--ed-ink);
  padding-top: 3px;
  margin: var(--ed-space-xl) 0;
}

/* Asterism (three-dot section break) */
.ed-asterism {
  text-align: center;
  margin: var(--ed-space-xl) 0;
  font-size: 1.25rem;
  letter-spacing: 0.5em;
  color: var(--ed-silver);
}

.ed-asterism::before {
  content: '***';
}

/* Section heading with top rule */
.ed-section-heading {
  border-top: 2px solid var(--ed-ink);
  padding-top: var(--ed-space-md);
  margin-bottom: var(--ed-space-lg);
}

.ed-section-heading__title {
  font-family: 'Source Sans 3', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--ed-ink);
}
```

---

## Design Do's and Don'ts

### Do

- Use generous whitespace as a primary compositional tool -- let the page breathe
- Establish a rigorous typographic hierarchy with at least 5 levels (kicker, headline, deck, byline, body, caption)
- Choose high-contrast serif typefaces for display headlines to convey editorial authority
- Employ asymmetric grids that create visual tension and guide the eye
- Use drop caps to mark article beginnings and create visual entry points
- Set body text at proper measure (50-70 characters per line) with generous line height (1.6-1.8)
- Include pull quotes to break up long text and create secondary entry points
- Use thin hairline rules to organize and separate content sections
- Keep the color palette restrained: neutral foundation with 1-2 accent colors maximum
- Make images large, high-quality, and intentionally cropped -- editorial photography should feel curated
- Use all-caps with wide letter-spacing for category labels, kickers, and navigation elements
- Maintain consistent vertical rhythm throughout the page

### Don't

- Clutter the layout with too many elements -- editorial design values restraint over density
- Use more than 2-3 typefaces on a single page -- one serif display, one sans body, and optionally one accent face
- Apply bright, saturated colors as backgrounds -- reserve vivid color for small accents (red drop caps, labels)
- Center everything -- editorial layouts derive their sophistication from asymmetry, not bilateral symmetry
- Use generic stock photography -- the editorial aesthetic demands intentional, high-quality imagery
- Set body text wider than 80 characters per line -- readability degrades sharply beyond proper measure
- Add decorative borders, shadows, or rounded corners liberally -- keep surfaces clean and flat
- Ignore the vertical rhythm -- inconsistent spacing between elements destroys the sense of order
- Use all-caps or letter-spacing for body text -- these treatments are reserved for labels and navigation
- Place text over busy images without proper contrast handling -- use overlays or place text adjacent
- Make everything the same size -- the power of editorial design comes from dramatic scale contrast
- Neglect mobile typography -- headings should still be noticeably larger than body text, even on small screens

---

## Related Aesthetics

| Aesthetic | Relationship to Editorial / Magazine Layout |
|-----------|-------------------------------------------|
| **Swiss / International Typographic Style** | Shares the grid-based structure and typographic focus; Swiss is more rigid and geometric, Editorial is more fluid and asymmetric |
| **Minimalism** | Both use whitespace and restraint; Minimalism is reductive, Editorial maintains content richness within a refined structure |
| **Brutalism (Web)** | Both can use strong typography; Brutalism deliberately breaks conventions, Editorial follows refined print traditions |
| **New York Times / Newspaper Layout** | Direct ancestor -- multi-column grids, strict hierarchy, rules; newspaper layout is denser and more information-packed |
| **Art Deco** | Shares appreciation for elegant typography and ruled lines; Art Deco is more ornamental and geometric |
| **Material Design** | Both use systematic spacing and hierarchy; Material is component-driven UI, Editorial is content-driven publication |
| **Wabi-Sabi** | Both value whitespace and restraint; Wabi-Sabi embraces imperfection, Editorial values precision and polish |
| **Corporate Clean** | Both use professional typography and muted colors; Corporate is utilitarian, Editorial is expressive and artful |
| **Bauhaus** | Shares functional typography principles; Bauhaus is more experimental with color and geometry |

---

## Quick-Start: Minimal Editorial Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Chronicle -- Editorial Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,400;1,700&family=Source+Sans+3:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
  <style>
    :root {
      --ed-ink: #1a1a1a;
      --ed-charcoal: #2c2c2c;
      --ed-body: #3d3d3d;
      --ed-gray: #6b6b6b;
      --ed-silver: #9a9a9a;
      --ed-rule: #d4d4d4;
      --ed-bg-stone: #e8e4df;
      --ed-bg-paper: #f5f3f0;
      --ed-bg-white: #ffffff;
      --ed-red: #c41e2a;
      --ed-navy: #1b2a4a;
      --ed-gold: #b8860b;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--ed-bg-paper);
      color: var(--ed-body);
      font-family: 'Source Sans 3', 'Georgia', serif;
      font-size: 1.0625rem;
      line-height: 1.75;
      -webkit-font-smoothing: antialiased;
    }

    h1, h2, h3, h4 {
      font-family: 'Playfair Display', 'Georgia', serif;
      color: var(--ed-ink);
      line-height: 1.1;
      letter-spacing: -0.015em;
    }

    ::selection {
      background: rgba(196, 30, 42, 0.12);
      color: var(--ed-ink);
    }

    a { color: var(--ed-navy); text-decoration: none; transition: color 0.2s; }
    a:hover { color: var(--ed-red); }

    img { display: block; max-width: 100%; height: auto; }

    /* ---- Navigation ---- */
    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 1.5rem 2.5rem;
    }

    .nav__masthead {
      font-family: 'Playfair Display', 'Georgia', serif;
      font-size: 2rem;
      font-weight: 700;
      color: var(--ed-ink);
      text-decoration: none;
      letter-spacing: -0.03em;
    }

    .nav__links {
      display: flex;
      gap: 2rem;
      list-style: none;
    }

    .nav__links a {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.75rem;
      font-weight: 600;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--ed-gray);
    }

    .nav__links a:hover { color: var(--ed-ink); }

    .nav-rule {
      border: none;
      height: 1px;
      background: var(--ed-rule);
      max-width: 1200px;
      margin: 0 auto;
    }

    /* ---- Hero ---- */
    .hero {
      max-width: 1200px;
      margin: 0 auto;
      padding: 5rem 2.5rem 3rem;
      text-align: center;
    }

    .hero__kicker {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.72rem;
      font-weight: 600;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--ed-red);
      margin-bottom: 1.5rem;
      display: block;
    }

    .hero__headline {
      font-family: 'Playfair Display', 'Georgia', serif;
      font-weight: 900;
      font-size: clamp(2.75rem, 6vw, 4.75rem);
      line-height: 1.05;
      letter-spacing: -0.03em;
      color: var(--ed-ink);
      max-width: 860px;
      margin: 0 auto 1.5rem;
    }

    .hero__deck {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 1.2rem;
      line-height: 1.6;
      color: var(--ed-gray);
      max-width: 580px;
      margin: 0 auto 1.25rem;
    }

    .hero__byline {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.78rem;
      color: var(--ed-silver);
      text-transform: uppercase;
      letter-spacing: 0.07em;
    }

    .hero__byline strong { color: var(--ed-charcoal); font-weight: 600; }

    /* ---- Hero Image ---- */
    .hero-image {
      width: 100%;
      max-width: 1200px;
      margin: 0 auto 2rem;
      padding: 0 2.5rem;
    }

    .hero-image img {
      width: 100%;
      height: 420px;
      object-fit: cover;
      background: var(--ed-rule);
    }

    .hero-image figcaption {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.78rem;
      font-style: italic;
      color: var(--ed-gray);
      margin-top: 0.5rem;
      text-align: right;
    }

    /* ---- Article Layout ---- */
    .article-layout {
      display: grid;
      grid-template-columns: 1fr minmax(0, 680px) 260px;
      gap: 3rem;
      max-width: 1200px;
      margin: 0 auto;
      padding: 2rem 2.5rem 4rem;
    }

    .article-layout__spacer { /* empty left column for asymmetry */ }

    .article-body p {
      margin-bottom: 1.5rem;
    }

    .article-body h2 {
      font-size: 1.75rem;
      font-weight: 700;
      margin-top: 3rem;
      margin-bottom: 1.25rem;
      letter-spacing: -0.01em;
    }

    /* Drop cap */
    .dropcap::first-letter {
      font-family: 'Playfair Display', 'Georgia', serif;
      font-weight: 900;
      font-size: 4.2em;
      float: left;
      line-height: 0.78;
      margin-right: 0.08em;
      margin-top: 0.06em;
      color: var(--ed-red);
    }

    /* Pull quote */
    .pull-quote {
      margin: 2.5rem 0;
      padding: 2rem 0;
      border-top: 2px solid var(--ed-ink);
      border-bottom: 1px solid var(--ed-rule);
    }

    .pull-quote blockquote {
      font-family: 'Playfair Display', 'Georgia', serif;
      font-size: 1.65rem;
      font-style: italic;
      font-weight: 400;
      line-height: 1.35;
      color: var(--ed-charcoal);
      margin: 0 0 0.75rem;
    }

    .pull-quote cite {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.75rem;
      font-style: normal;
      font-weight: 600;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--ed-silver);
    }

    /* Inline image */
    .article-image {
      margin: 2.5rem 0;
    }

    .article-image img {
      width: 100%;
      height: 320px;
      object-fit: cover;
      background: var(--ed-rule);
    }

    .article-image figcaption {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.78rem;
      font-style: italic;
      color: var(--ed-gray);
      margin-top: 0.5rem;
    }

    /* ---- Sidebar ---- */
    .sidebar {
      padding-top: 0.25rem;
    }

    .sidebar-section {
      margin-bottom: 2.5rem;
    }

    .sidebar-section__heading {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--ed-ink);
      border-bottom: 2px solid var(--ed-ink);
      padding-bottom: 0.5rem;
      margin-bottom: 1rem;
    }

    .sidebar-item {
      margin-bottom: 1.25rem;
      padding-bottom: 1.25rem;
      border-bottom: 1px solid var(--ed-rule);
    }

    .sidebar-item:last-child { border-bottom: none; }

    .sidebar-item__title {
      font-family: 'Playfair Display', 'Georgia', serif;
      font-size: 1rem;
      font-weight: 700;
      line-height: 1.3;
      color: var(--ed-ink);
      margin-bottom: 0.25rem;
    }

    .sidebar-item__meta {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.72rem;
      color: var(--ed-silver);
      text-transform: uppercase;
      letter-spacing: 0.06em;
    }

    /* ---- Divider ---- */
    .section-rule {
      border: none;
      height: 1px;
      background: var(--ed-rule);
      max-width: 1200px;
      margin: 0 auto;
    }

    .section-rule--heavy {
      height: 3px;
      background: var(--ed-ink);
    }

    /* ---- Featured Stories Grid ---- */
    .featured {
      max-width: 1200px;
      margin: 0 auto;
      padding: 3rem 2.5rem 4rem;
    }

    .featured__heading {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.72rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--ed-ink);
      border-top: 2px solid var(--ed-ink);
      padding-top: 0.75rem;
      margin-bottom: 2rem;
    }

    .featured-grid {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 2rem;
    }

    .story-card { }

    .story-card__image {
      width: 100%;
      height: 220px;
      object-fit: cover;
      margin-bottom: 1rem;
      background: var(--ed-rule);
    }

    .story-card__category {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.68rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--ed-red);
      margin-bottom: 0.5rem;
      display: block;
    }

    .story-card__title {
      font-family: 'Playfair Display', 'Georgia', serif;
      font-size: 1.35rem;
      font-weight: 700;
      line-height: 1.2;
      color: var(--ed-ink);
      margin-bottom: 0.6rem;
      letter-spacing: -0.01em;
    }

    .story-card__title a { color: inherit; }
    .story-card__title a:hover { color: var(--ed-red); }

    .story-card__excerpt {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.92rem;
      line-height: 1.55;
      color: var(--ed-gray);
      margin-bottom: 0.75rem;
    }

    .story-card__meta {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.72rem;
      color: var(--ed-silver);
      text-transform: uppercase;
      letter-spacing: 0.06em;
    }

    /* ---- CTA / Subscribe ---- */
    .subscribe {
      max-width: 1200px;
      margin: 0 auto;
      padding: 4rem 2.5rem;
      text-align: center;
    }

    .subscribe__inner {
      max-width: 520px;
      margin: 0 auto;
    }

    .subscribe h2 {
      font-family: 'Playfair Display', 'Georgia', serif;
      font-size: 2rem;
      font-weight: 700;
      margin-bottom: 0.75rem;
      letter-spacing: -0.02em;
    }

    .subscribe p {
      font-size: 1rem;
      color: var(--ed-gray);
      margin-bottom: 1.5rem;
    }

    .subscribe-form {
      display: flex;
      gap: 0;
      max-width: 420px;
      margin: 0 auto;
    }

    .subscribe-form input {
      flex: 1;
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.9rem;
      padding: 12px 16px;
      border: 1.5px solid var(--ed-rule);
      border-right: none;
      background: var(--ed-bg-white);
      color: var(--ed-body);
      outline: none;
    }

    .subscribe-form input::placeholder { color: var(--ed-silver); }

    .subscribe-form input:focus {
      border-color: var(--ed-ink);
    }

    .subscribe-form button {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.72rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      background: var(--ed-ink);
      color: var(--ed-bg-white);
      border: 1.5px solid var(--ed-ink);
      padding: 12px 24px;
      cursor: pointer;
      transition: background 0.25s, color 0.25s;
    }

    .subscribe-form button:hover {
      background: var(--ed-bg-white);
      color: var(--ed-ink);
    }

    /* ---- Footer ---- */
    footer {
      max-width: 1200px;
      margin: 0 auto;
      padding: 2rem 2.5rem;
      border-top: 1px solid var(--ed-rule);
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    footer p {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.75rem;
      color: var(--ed-silver);
      letter-spacing: 0.04em;
    }

    footer nav {
      display: flex;
      gap: 1.5rem;
    }

    footer nav a {
      font-family: 'Source Sans 3', sans-serif;
      font-size: 0.72rem;
      color: var(--ed-silver);
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    footer nav a:hover { color: var(--ed-ink); }

    /* ---- Responsive ---- */
    @media (max-width: 1024px) {
      .article-layout {
        grid-template-columns: 1fr;
        padding: 2rem 1.5rem 3rem;
      }
      .article-layout__spacer { display: none; }
      .sidebar { border-top: 1px solid var(--ed-rule); padding-top: 2rem; }
      .featured-grid { grid-template-columns: 1fr 1fr; }
    }

    @media (max-width: 768px) {
      .nav { padding: 1.25rem 1.5rem; }
      .nav__masthead { font-size: 1.5rem; }
      .nav__links { gap: 1rem; }
      .nav__links a { font-size: 0.68rem; }
      .hero { padding: 3rem 1.5rem 2rem; }
      .hero-image { padding: 0 1.5rem; }
      .hero-image img { height: 280px; }
      .article-layout { padding: 1.5rem 1.5rem 3rem; gap: 2rem; }
      .article-image img { height: 240px; }
      .featured { padding: 2rem 1.5rem 3rem; }
      .featured-grid { grid-template-columns: 1fr; }
      .subscribe { padding: 3rem 1.5rem; }
      .subscribe-form { flex-direction: column; }
      .subscribe-form input { border-right: 1.5px solid var(--ed-rule); }
      footer { flex-direction: column; gap: 1rem; text-align: center; padding: 2rem 1.5rem; }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav class="nav">
    <a href="#" class="nav__masthead">The Chronicle</a>
    <ul class="nav__links">
      <li><a href="#">Culture</a></li>
      <li><a href="#">Design</a></li>
      <li><a href="#">Technology</a></li>
      <li><a href="#">Opinion</a></li>
      <li><a href="#">Archive</a></li>
    </ul>
  </nav>
  <hr class="nav-rule">

  <!-- Hero -->
  <header class="hero">
    <span class="hero__kicker">Longform Feature</span>
    <h1 class="hero__headline">The Quiet Revolution of Thoughtful Design</h1>
    <p class="hero__deck">How a return to editorial principles is reshaping the way we read, think, and engage with digital content in an age of noise.</p>
    <p class="hero__byline">By <strong>Eleanor Voss</strong> &mdash; February 18, 2026 &mdash; 12 min read</p>
  </header>

  <!-- Hero Image -->
  <figure class="hero-image">
    <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='1200' height='420' viewBox='0 0 1200 420'%3E%3Crect fill='%23e8e4df' width='1200' height='420'/%3E%3Crect fill='%23d4d4d4' x='80' y='60' width='400' height='300' rx='2'/%3E%3Crect fill='%23c41e2a' x='80' y='60' width='400' height='4'/%3E%3Cline x1='540' y1='80' x2='1120' y2='80' stroke='%23d4d4d4' stroke-width='1'/%3E%3Crect fill='%23d4d4d4' x='540' y1='100' width='580' height='12' y='100' rx='1'/%3E%3Crect fill='%23d4d4d4' x='540' width='480' height='12' y='124' rx='1'/%3E%3Crect fill='%23d4d4d4' x='540' width='520' height='12' y='148' rx='1'/%3E%3Crect fill='%23d4d4d4' x='540' width='400' height='12' y='172' rx='1'/%3E%3Crect fill='%23d4d4d4' x='540' width='560' height='12' y='208' rx='1'/%3E%3Crect fill='%23d4d4d4' x='540' width='500' height='12' y='232' rx='1'/%3E%3Crect fill='%23d4d4d4' x='540' width='440' height='12' y='256' rx='1'/%3E%3Crect fill='%231a1a1a' x='540' width='300' height='24' y='300' rx='1'/%3E%3Crect fill='%239a9a9a' x='540' width='200' height='10' y='336' rx='1'/%3E%3C/svg%3E" alt="Abstract editorial layout composition">
    <figcaption>An editorial spread demonstrating asymmetric column arrangement</figcaption>
  </figure>

  <hr class="section-rule">

  <!-- Article Layout: asymmetric grid with sidebar -->
  <div class="article-layout">
    <div class="article-layout__spacer"></div>

    <!-- Main article column -->
    <article class="article-body">
      <p class="dropcap">There is a particular quality to a well-designed magazine page that transcends mere information delivery. It is the feeling of space orchestrated with intention, of typography that commands the eye with quiet authority, of images placed not to fill gaps but to punctuate a rhythm. This is the language of editorial design, and it is making a striking return to the digital world after years of template-driven uniformity.</p>

      <p>The resurgence is not accidental. As the web matured through phases of skeuomorphism, flat design, and component-driven systems, something essential was lost: the art of the page. Websites became grids of identical cards. Content was poured into containers like water into ice cube trays, each piece indistinguishable from the next. The editorial tradition offers an alternative vocabulary, one where hierarchy is earned through scale, where whitespace is a structural member rather than leftover margin, and where every spread tells a story before a single word is read.</p>

      <h2>The Grid as Invisible Architecture</h2>

      <p>At the foundation of every great editorial layout is a grid, but not the rigid, equal-column grids that dominate contemporary web frameworks. The editorial grid is asymmetric by nature. Alexey Brodovitch, the legendary art director who transformed Harper's Bazaar from 1934 to 1958, treated the double-page spread as a single canvas. His grids were felt, not seen. Content floated within invisible structures that guided the eye along deliberate paths.</p>

      <!-- Pull Quote -->
      <div class="pull-quote">
        <blockquote>The page is a field upon which the designer composes a symphony of text, image, and space. The silence between the notes matters as much as the notes themselves.</blockquote>
        <cite>Alexey Brodovitch</cite>
      </div>

      <p>In CSS terms, this translates to grid systems with unequal column widths. A typical editorial article might use a three-column grid defined as <code>1fr 2fr 1fr</code>, where the center column holds the main text and the flanking columns serve as space for margin notes, pull quotes, or simply intentional emptiness. The key insight is that unused columns are not wasted space. They are the design.</p>

      <!-- Inline Image -->
      <figure class="article-image">
        <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='680' height='320' viewBox='0 0 680 320'%3E%3Crect fill='%23e8e4df' width='680' height='320'/%3E%3Ctext x='340' y='160' text-anchor='middle' font-family='Georgia' font-size='18' fill='%239a9a9a'%3EPhotograph%3C/text%3E%3Ctext x='340' y='185' text-anchor='middle' font-family='sans-serif' font-size='12' fill='%23b0b0b0'%3E680 %C3%97 320%3C/text%3E%3C/svg%3E" alt="Typographic detail study">
        <figcaption>Detail from a contemporary editorial spread showing the interplay of scale and whitespace</figcaption>
      </figure>

      <h2>Typography as Voice</h2>

      <p>If the grid is the skeleton of editorial design, typography is its voice. The editorial tradition demands a rigorously defined hierarchy. A typical article page might employ six or more distinct typographic levels: the section label (small, uppercase, widely spaced), the headline (large, serif, commanding), the deck or standfirst (medium, lighter weight, summarizing), the byline (small, structured), the body text (optimally sized and measured), and captions (small, often italic).</p>

      <p>Each level serves a specific purpose in the reading architecture. The section label orients the reader within the publication. The headline arrests attention. The deck provides enough context to decide whether to continue. The byline establishes authority. The body delivers the substance. The captions annotate the visual elements. Remove any one level and the architecture weakens. Add unnecessary levels and the hierarchy collapses into noise.</p>

      <p>The choice of typeface matters enormously. High-contrast serif faces like Playfair Display, with their dramatic thick-thin stroke variation, carry the authority of centuries of print tradition. They signal that this content has been considered, edited, and presented with care. For body text, the priority shifts to readability. A well-designed sans-serif or a transitional serif with even color and generous x-height ensures that long-form reading remains comfortable across the full measure of the text column.</p>

      <h2>The Art of the Entry Point</h2>

      <p>One of the most valuable concepts from print editorial design is the entry point: a visual element that invites the reader into the content. The drop cap is the most recognizable example. An oversized initial letter, often in a contrasting color or weight, marks the beginning of the narrative and creates a moment of visual drama on the page. Pull quotes serve a similar function mid-article, lifting a compelling sentence out of the body text and presenting it at display scale, breaking the columnar rhythm and offering a new invitation to engage.</p>

      <p>These elements are not decorative afterthoughts. They are strategic tools for managing reader attention in an environment where attention is the scarcest resource. A well-placed pull quote can catch a scanning eye and draw it into the surrounding paragraphs. A drop cap can signal the transition from preparatory material (headline, deck, byline) to the substance of the article itself.</p>
    </article>

    <!-- Sidebar -->
    <aside class="sidebar">
      <div class="sidebar-section">
        <h3 class="sidebar-section__heading">Related Stories</h3>
        <div class="sidebar-item">
          <h4 class="sidebar-item__title"><a href="#">The Return of the Serif</a></h4>
          <p class="sidebar-item__meta">Culture &mdash; Feb 12, 2026</p>
        </div>
        <div class="sidebar-item">
          <h4 class="sidebar-item__title"><a href="#">Grid Systems and the Digital Canvas</a></h4>
          <p class="sidebar-item__meta">Design &mdash; Feb 8, 2026</p>
        </div>
        <div class="sidebar-item">
          <h4 class="sidebar-item__title"><a href="#">Why Whitespace Matters More Than Ever</a></h4>
          <p class="sidebar-item__meta">Opinion &mdash; Jan 29, 2026</p>
        </div>
        <div class="sidebar-item">
          <h4 class="sidebar-item__title"><a href="#">Brodovitch and the Modern Web</a></h4>
          <p class="sidebar-item__meta">Design &mdash; Jan 15, 2026</p>
        </div>
      </div>

      <div class="sidebar-section">
        <h3 class="sidebar-section__heading">About the Author</h3>
        <p style="font-size: 0.88rem; color: var(--ed-gray); line-height: 1.6;">Eleanor Voss writes about design, culture, and the intersection of technology and craft. She is a contributing editor at The Chronicle.</p>
      </div>
    </aside>
  </div>

  <hr class="section-rule section-rule--heavy" style="max-width: 1200px; margin: 0 auto;">

  <!-- Featured Stories Grid -->
  <section class="featured">
    <h2 class="featured__heading">More from The Chronicle</h2>
    <div class="featured-grid">
      <article class="story-card">
        <img class="story-card__image" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='220' viewBox='0 0 400 220'%3E%3Crect fill='%23e8e4df' width='400' height='220'/%3E%3Ctext x='200' y='115' text-anchor='middle' font-family='Georgia' font-size='14' fill='%239a9a9a'%3EPhotograph%3C/text%3E%3C/svg%3E" alt="Story image">
        <span class="story-card__category">Culture</span>
        <h3 class="story-card__title"><a href="#">The Spaces Between: Architecture and Negative Space</a></h3>
        <p class="story-card__excerpt">How contemporary architects are rediscovering the power of emptiness in an age of maximalist construction.</p>
        <p class="story-card__meta">By <strong>M. Ishikawa</strong> &mdash; Feb 14, 2026</p>
      </article>

      <article class="story-card">
        <img class="story-card__image" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='220' viewBox='0 0 400 220'%3E%3Crect fill='%23e8e4df' width='400' height='220'/%3E%3Ctext x='200' y='115' text-anchor='middle' font-family='Georgia' font-size='14' fill='%239a9a9a'%3EPhotograph%3C/text%3E%3C/svg%3E" alt="Story image">
        <span class="story-card__category">Technology</span>
        <h3 class="story-card__title"><a href="#">Variable Fonts and the Future of Digital Typography</a></h3>
        <p class="story-card__excerpt">A single font file that contains an entire design space. The implications for editorial design are profound.</p>
        <p class="story-card__meta">By <strong>R. Chen</strong> &mdash; Feb 10, 2026</p>
      </article>

      <article class="story-card">
        <img class="story-card__image" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='220' viewBox='0 0 400 220'%3E%3Crect fill='%23e8e4df' width='400' height='220'/%3E%3Ctext x='200' y='115' text-anchor='middle' font-family='Georgia' font-size='14' fill='%239a9a9a'%3EPhotograph%3C/text%3E%3C/svg%3E" alt="Story image">
        <span class="story-card__category">Opinion</span>
        <h3 class="story-card__title"><a href="#">Against the Feed: A Case for Slower Reading</a></h3>
        <p class="story-card__excerpt">The infinite scroll trained us to consume. Editorial design might teach us to absorb once more.</p>
        <p class="story-card__meta">By <strong>J. Andersson</strong> &mdash; Feb 6, 2026</p>
      </article>
    </div>
  </section>

  <hr class="section-rule">

  <!-- Subscribe -->
  <section class="subscribe">
    <div class="subscribe__inner">
      <h2>Stay Considered</h2>
      <p>A weekly letter on design, typography, and the craft of thoughtful communication. No noise.</p>
      <form class="subscribe-form" onsubmit="return false;">
        <input type="email" placeholder="Your email address" aria-label="Email address">
        <button type="submit">Subscribe</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2026 The Chronicle. All rights reserved.</p>
    <nav>
      <a href="#">Privacy</a>
      <a href="#">Terms</a>
      <a href="#">Contact</a>
      <a href="#">RSS</a>
    </nav>
  </footer>

</body>
</html>
```
