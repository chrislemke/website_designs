# Split Screen Design Reference

Split Screen is a bold, high-impact layout aesthetic built on the principle of dividing the viewport into two (or more) equally weighted vertical panels, each carrying distinct but complementary content. Rooted in editorial print design -- where facing pages have long been used for dramatic juxtaposition -- the technique migrated to web design in the mid-2010s and has grown steadily as a favored pattern for landing pages, portfolio sites, and brand storytelling. The aesthetic thrives on visual tension: light against dark, image against text, warm against cool, photography against illustration. Unlike traditional single-column layouts that guide the eye in one direction, Split Screen presents a deliberate duality that invites comparison, highlights contrast, and gives users an immediate choice. In web and UI design, Split Screen translates to bold 50/50 flexbox or grid divisions, high-contrast color blocking, dramatic typography anchored to one panel, strong vertical center lines (sometimes replaced by diagonal or angled dividers), and hover-driven interactions that let one panel expand or reveal content at the expense of the other.

---

## Visual Characteristics

### Core Design Traits

- **50/50 vertical divisions** -- the viewport is split into two equal (or near-equal) panels running the full height of the section, creating a strong vertical axis
- **High-contrast color blocking** -- adjacent panels use opposing tones (black and white, dark navy and bright coral, deep charcoal and crisp ivory) to maximize visual separation
- **Image-versus-text pairing** -- one panel typically carries a large photograph or illustration while the opposite holds typographic content and calls to action
- **Strong center dividing line** -- the boundary between panels is architecturally emphasized, sometimes as a visible rule, a thin gap, a diagonal slash, or a contrasting stripe
- **Dramatic hover interactions** -- panels expand, contract, or shift on mouse hover, creating an interactive tug-of-war between the two halves
- **Full-viewport hero sections** -- split panels span the entire screen height (100vh), creating an immersive, edge-to-edge first impression
- **Bold, oversized typography** -- headlines are large and assertive, often placed on the solid-colored panel for maximum legibility against a flat background
- **Diagonal and angled dividers** -- instead of a straight vertical cut, many split layouts use CSS clip-path or skewed transforms to create angular, dynamic separations
- **Asymmetric content balance** -- while the spatial division is equal, the visual weight is intentionally unequal (heavy image vs. minimal text) to create directional pull
- **Minimal ornamentation** -- the split itself is the design statement; extraneous decorative elements are stripped away to maintain focus on the duality
- **Scroll-triggered reveals** -- as users scroll, new split sections appear with alternating panel orientations (image-left then image-right)
- **Parallax depth between panels** -- left and right panels scroll at slightly different rates, adding a sense of layered depth

### Design Principles

- Embrace duality -- the split layout is fundamentally about two things in conversation with each other
- Contrast is the engine of the aesthetic: every design choice should amplify the difference between the two halves
- Give each panel a clear purpose -- one informs, the other entices; one shows, the other tells
- The center division is sacred -- it is the spine of the composition and should be treated as a deliberate design element
- Maintain balance even in asymmetry -- visual weight should feel considered, not accidental
- Use full-bleed imagery and edge-to-edge color fills to eliminate any sense of floating panels
- Typography on solid backgrounds should be bold and generously sized; let the negative space do the work
- Interactions should reinforce the split metaphor -- hover effects that expand one panel at the cost of the other emphasize the duality
- On mobile, the split becomes a vertical stack -- design each panel to work independently when collapsed
- Color contrast ratios between panels should be dramatic enough to read as two distinct zones, not a subtle gradient

---

## Color Palette

### Contrast Block Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Panel Dark** | `#1A1A2E` | Dark panel background, deep navy-charcoal foundation |
| **Panel Light** | `#F5F0EB` | Light panel background, warm ivory canvas |
| **Pure Black** | `#0D0D0D` | Maximum contrast text on light panels, deepest dark |
| **Pure White** | `#FFFFFF` | Text on dark panels, maximum brightness |
| **Accent Coral** | `#FF6B6B` | Primary accent, CTAs, active states, hover highlights |
| **Accent Electric** | `#4ECDC4` | Secondary accent, links, interactive elements on dark panels |
| **Deep Teal** | `#1B998B` | Tertiary accent, icons, secondary buttons |
| **Warm Amber** | `#F7B731` | Warning states, highlights, attention-drawing accents |
| **Soft Graphite** | `#2D3436` | Dark panel alternate, card backgrounds, overlays |
| **Mist Gray** | `#DFE6E9` | Light panel borders, subtle dividers, secondary backgrounds |
| **Slate Text** | `#636E72` | Secondary text on light panels, captions, metadata |
| **Lavender Mist** | `#A29BFE` | Decorative accent, hover states, gradient endpoints |
| **Crimson Bold** | `#E74C3C` | Bold emphasis, split divider accent, strong CTAs |
| **Midnight Blue** | `#0C2461` | Alternative dark panel, premium/corporate variant |

### CSS Custom Properties

```css
:root {
  /* Panel backgrounds */
  --split-panel-dark: #1a1a2e;
  --split-panel-light: #f5f0eb;
  --split-black: #0d0d0d;
  --split-white: #ffffff;

  /* Accents */
  --split-coral: #ff6b6b;
  --split-electric: #4ecdc4;
  --split-teal: #1b998b;
  --split-amber: #f7b731;

  /* Neutrals */
  --split-graphite: #2d3436;
  --split-mist: #dfe6e9;
  --split-slate: #636e72;

  /* Decorative */
  --split-lavender: #a29bfe;
  --split-crimson: #e74c3c;
  --split-midnight: #0c2461;

  /* Functional */
  --split-divider: #ff6b6b;
  --split-divider-width: 4px;
  --split-transition-speed: 0.5s;
  --split-panel-gap: 0px;

  /* Gradients */
  --split-gradient-dark: linear-gradient(135deg, #1a1a2e 0%, #0c2461 100%);
  --split-gradient-warm: linear-gradient(135deg, #ff6b6b 0%, #f7b731 100%);
  --split-gradient-cool: linear-gradient(135deg, #4ecdc4 0%, #a29bfe 100%);

  /* Shadows */
  --split-shadow-left: 4px 0 20px rgba(0, 0, 0, 0.15);
  --split-shadow-right: -4px 0 20px rgba(0, 0, 0, 0.15);
  --split-shadow-card: 0 8px 30px rgba(0, 0, 0, 0.12);
}
```

---

## Typography

### Typeface Characteristics

Split Screen typography is:

- **Bold and high-contrast** -- headlines must command attention on one panel while competing with a strong image on the other
- **Sans-serif dominant** -- clean geometric or grotesque sans-serifs reinforce the modern, architectural feel of the split layout
- **Oversized display text** -- hero headlines are dramatically large (often 4-8rem), using the generous space of a dedicated text panel
- **Uppercase for impact** -- section headers and navigation use all-caps with wide letter-spacing for structural authority
- **Weight-contrasted pairings** -- heavy 700-900 weight headings paired with light 300-400 body text amplify the contrast theme
- **Color-inverted across panels** -- white text on the dark panel, dark text on the light panel, maintaining legibility in both contexts
- **Minimal line lengths** -- with each panel being only 50% of the viewport, text columns are naturally narrow, demanding careful typographic sizing

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Inter** | Clean geometric sans | Body text, versatile across both panels |
| **Space Grotesk** | Geometric, contemporary | Headlines, modern split layouts |
| **Bebas Neue** | Condensed display | Large hero headlines, dramatic impact |
| **Poppins** | Geometric, friendly | Subheadings, body text, balanced weight range |
| **Sora** | Geometric, modern | Headlines, navigation, tech-forward layouts |
| **DM Sans** | Clean, geometric | Body text, readable at small sizes |
| **Playfair Display** | High-contrast serif | Editorial headlines, luxury split layouts |
| **Archivo Black** | Ultra-bold grotesque | Maximum impact headlines, bold statements |
| **Outfit** | Modern geometric sans | Body text, labels, clean readability |
| **Clash Display** | Variable geometric | Striking display text, branding headers |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Bebas Neue** (400) | **Inter** (400) | Bold editorial, magazine-style drama |
| **Space Grotesk** (700) | **DM Sans** (400) | Modern tech, clean and architectural |
| **Archivo Black** (400) | **Outfit** (400) | Maximum impact, strong and direct |
| **Playfair Display** (700) | **Poppins** (300) | Editorial luxury, refined contrast |
| **Sora** (700) | **Inter** (400) | Contemporary minimal, balanced weight |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@300;400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Bebas Neue', sans-serif;
  font-weight: 400;
  letter-spacing: 0.04em;
  line-height: 1.05;
}

/* Display / Hero text -- oversized for text panels */
.split-display {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(3.5rem, 8vw, 7rem);
  letter-spacing: 0.03em;
  line-height: 0.95;
  text-transform: uppercase;
}

/* Display text on dark panel */
.split-display--light {
  color: var(--split-white);
}

/* Display text on light panel */
.split-display--dark {
  color: var(--split-black);
}

/* Accent-colored display */
.split-display--accent {
  color: var(--split-coral);
}

/* Body text */
body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
}

/* Body text on dark panels */
.text-on-dark {
  color: rgba(255, 255, 255, 0.85);
}

/* Body text on light panels */
.text-on-light {
  color: var(--split-graphite);
}

/* Eyebrow / Label */
.split-label {
  font-family: 'Inter', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--split-coral);
}
```

---

## Layout Principles

### Grid and Structure

- **50/50 flexbox or grid divisions** -- the fundamental unit is two panels splitting the viewport evenly using `display: flex` with `flex: 1` or `grid-template-columns: 1fr 1fr`
- **Full-viewport height sections** -- each split section spans `min-height: 100vh` for maximum immersive impact
- **Edge-to-edge panels** -- no outer margins or padding on the split container; panels extend to screen edges
- **Zero gap or thin divider** -- panels sit flush against each other, separated by either nothing, a thin colored line, or a diagonal clip-path
- **Content padding within panels** -- generous inner padding (48-80px) creates breathing room inside each panel while maintaining the edge-to-edge outer container
- **Alternating panel order** -- successive sections alternate which side carries the image and which carries text (image-left/text-right, then text-left/image-right)
- **Sticky scroll patterns** -- one panel can remain fixed while the other scrolls, creating a parallax-like effect within the split
- **Nested splits** -- within a text panel, further subdivision can occur (e.g., a stat grid or mini card layout)

### Section Organization

- **Navigation**: Transparent overlay spanning both panels, or integrated into the top of one panel; minimal and unobtrusive
- **Hero**: Full-viewport split -- large image or video on one side, bold headline + tagline + CTA on the other
- **About / Story**: Image panel showing team/product, text panel with narrative content
- **Features**: Alternating split rows, each featuring a different product shot or illustration opposite descriptive text
- **Comparison**: Two equal panels presenting contrasting options (e.g., two products, before/after, two services)
- **CTA section**: Bold color-blocked split with strong headline on one side and form or button on the other
- **Footer**: Can maintain the split theme or collapse to a single unified bar

### Responsive Approach

- At tablet breakpoints (~1024px), maintain the split but reduce inner padding
- At mobile breakpoints (~768px), stack panels vertically -- image above text
- Maintain full-width color blocking on stacked mobile panels to preserve the contrast aesthetic
- Scale display typography aggressively with `clamp()` to prevent overflow in narrow panels
- Hover-expand interactions should be disabled on touch devices; use tap or scroll-triggered reveals instead
- Diagonal dividers can simplify to straight horizontal lines on mobile for clarity
- Ensure each panel has sufficient standalone visual interest when viewed independently in the stacked layout

---

## CSS / Design Techniques

### Split Screen Card Component

```css
.split-card {
  display: flex;
  background: var(--split-white);
  border-radius: 0;
  overflow: hidden;
  box-shadow: var(--split-shadow-card);
}

.split-card__image {
  flex: 1;
  min-height: 300px;
  background-size: cover;
  background-position: center;
}

.split-card__content {
  flex: 1;
  padding: 48px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  background: var(--split-panel-dark);
  color: var(--split-white);
}

.split-card__content h3 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 2rem;
  letter-spacing: 0.03em;
  margin-bottom: 16px;
}

.split-card__content p {
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  line-height: 1.7;
  color: rgba(255, 255, 255, 0.75);
  margin-bottom: 24px;
}

/* Alternating card layout */
.split-card:nth-child(even) {
  flex-direction: row-reverse;
}

/* Card grid for multiple split cards */
.split-card-stack {
  display: flex;
  flex-direction: column;
  gap: 0;
}

@media (max-width: 768px) {
  .split-card,
  .split-card:nth-child(even) {
    flex-direction: column;
  }

  .split-card__image {
    min-height: 220px;
  }

  .split-card__content {
    padding: 32px 24px;
  }
}
```

### Split Screen Button

```css
.split-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 16px 40px;
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  text-decoration: none;
  border: 2px solid currentColor;
  background: transparent;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: color var(--split-transition-speed), background var(--split-transition-speed);
}

/* Button on dark panels */
.split-btn--on-dark {
  color: var(--split-white);
  border-color: var(--split-white);
}

.split-btn--on-dark:hover {
  color: var(--split-panel-dark);
  background: var(--split-white);
}

/* Button on light panels */
.split-btn--on-light {
  color: var(--split-black);
  border-color: var(--split-black);
}

.split-btn--on-light:hover {
  color: var(--split-white);
  background: var(--split-black);
}

/* Accent filled button */
.split-btn--accent {
  color: var(--split-white);
  background: var(--split-coral);
  border-color: var(--split-coral);
}

.split-btn--accent:hover {
  background: #e85555;
  border-color: #e85555;
}

/* Sliding fill animation */
.split-btn--slide {
  z-index: 1;
}

.split-btn--slide::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 0%;
  height: 100%;
  background: var(--split-coral);
  transition: width var(--split-transition-speed) ease;
  z-index: -1;
}

.split-btn--slide:hover::before {
  width: 100%;
}

.split-btn--slide:hover {
  color: var(--split-white);
  border-color: var(--split-coral);
}
```

### Navigation Bar

```css
.split-nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 24px 48px;
  z-index: 100;
  mix-blend-mode: difference;
}

.split-nav__logo {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.6rem;
  color: var(--split-white);
  text-decoration: none;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.split-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.split-nav__links a {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--split-white);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  position: relative;
  transition: opacity 0.3s;
}

.split-nav__links a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--split-coral);
  transition: width 0.3s ease;
}

.split-nav__links a:hover::after {
  width: 100%;
}

.split-nav__links a:hover {
  opacity: 0.9;
}

/* Using mix-blend-mode: difference ensures the nav text inverts
   color against both light and dark panels automatically */
```

### Hero Section -- Full Viewport Split

```css
.split-hero {
  display: flex;
  min-height: 100vh;
  width: 100%;
}

.split-hero__panel {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 60px;
  position: relative;
  overflow: hidden;
  transition: flex var(--split-transition-speed) ease;
}

/* Dark text panel */
.split-hero__panel--dark {
  background: var(--split-panel-dark);
  color: var(--split-white);
}

/* Image panel */
.split-hero__panel--image {
  background-size: cover;
  background-position: center;
  padding: 0;
}

/* Optional: image overlay for text readability */
.split-hero__panel--image::after {
  content: '';
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0.15);
}

.split-hero__content {
  max-width: 480px;
  position: relative;
  z-index: 2;
}

.split-hero__content .split-label {
  margin-bottom: 16px;
}

.split-hero__content h1 {
  font-size: clamp(3rem, 5vw, 5.5rem);
  margin-bottom: 24px;
  line-height: 0.95;
}

.split-hero__content p {
  font-size: 1.05rem;
  line-height: 1.7;
  margin-bottom: 32px;
  opacity: 0.8;
}

@media (max-width: 768px) {
  .split-hero {
    flex-direction: column;
  }

  .split-hero__panel {
    min-height: 50vh;
    padding: 60px 32px;
  }

  .split-hero__panel--image {
    min-height: 40vh;
  }
}
```

### Hover-Expand Panels

One of the signature interactions of Split Screen design: panels that grow and shrink on hover, creating a tug-of-war effect.

```css
.split-expand {
  display: flex;
  min-height: 100vh;
  width: 100%;
  overflow: hidden;
}

.split-expand__panel {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
  transition: flex 0.6s cubic-bezier(0.25, 0.8, 0.25, 1);
  cursor: pointer;
}

/* On hover, the hovered panel grows while its sibling shrinks */
.split-expand:hover .split-expand__panel {
  flex: 0.7;
}

.split-expand:hover .split-expand__panel:hover {
  flex: 1.3;
}

/* Panel overlay for darkening/lightening on state change */
.split-expand__panel::before {
  content: '';
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0);
  transition: background 0.6s ease;
  z-index: 1;
}

.split-expand:hover .split-expand__panel::before {
  background: rgba(0, 0, 0, 0.3);
}

.split-expand:hover .split-expand__panel:hover::before {
  background: rgba(0, 0, 0, 0);
}

/* Content fades in on the active panel */
.split-expand__content {
  position: relative;
  z-index: 2;
  text-align: center;
  color: var(--split-white);
  opacity: 0.7;
  transform: scale(0.95);
  transition: opacity 0.5s, transform 0.5s;
}

.split-expand__panel:hover .split-expand__content {
  opacity: 1;
  transform: scale(1);
}

.split-expand__content h2 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(2rem, 4vw, 4rem);
  margin-bottom: 16px;
}

.split-expand__content p {
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  max-width: 320px;
  margin: 0 auto;
  opacity: 0;
  transform: translateY(10px);
  transition: opacity 0.5s 0.1s, transform 0.5s 0.1s;
}

.split-expand__panel:hover .split-expand__content p {
  opacity: 0.85;
  transform: translateY(0);
}

@media (max-width: 768px) {
  .split-expand {
    flex-direction: column;
  }

  .split-expand:hover .split-expand__panel,
  .split-expand:hover .split-expand__panel:hover {
    flex: 1;
  }

  .split-expand__content {
    opacity: 1;
    transform: scale(1);
  }

  .split-expand__content p {
    opacity: 0.85;
    transform: translateY(0);
  }
}
```

### Diagonal Split Divider

Instead of a straight vertical cut, this technique uses CSS `clip-path` to create an angled boundary between panels, adding dynamic energy to the split.

```css
.split-diagonal {
  display: flex;
  min-height: 100vh;
  width: 100%;
  position: relative;
  overflow: hidden;
}

.split-diagonal__left {
  flex: 0 0 55%;
  background: var(--split-panel-dark);
  clip-path: polygon(0 0, 100% 0, 85% 100%, 0 100%);
  display: flex;
  align-items: center;
  padding: 80px;
  padding-right: 120px;
  z-index: 2;
}

.split-diagonal__right {
  flex: 0 0 55%;
  margin-left: -10%;
  background: var(--split-panel-light);
  display: flex;
  align-items: center;
  justify-content: flex-end;
  padding: 80px;
  padding-left: 120px;
}

/* Angled accent stripe between panels */
.split-diagonal::after {
  content: '';
  position: absolute;
  top: 0;
  bottom: 0;
  left: 48%;
  width: var(--split-divider-width);
  background: var(--split-coral);
  transform: skewX(-8deg);
  z-index: 3;
}

/* Alternate direction for variety */
.split-diagonal--reverse .split-diagonal__left {
  clip-path: polygon(15% 0, 100% 0, 100% 100%, 0 100%);
  order: 2;
  padding-left: 120px;
  padding-right: 80px;
}

.split-diagonal--reverse .split-diagonal__right {
  order: 1;
  margin-left: 0;
  margin-right: -10%;
  justify-content: flex-start;
  padding-right: 120px;
  padding-left: 80px;
}

.split-diagonal--reverse::after {
  left: auto;
  right: 48%;
  transform: skewX(8deg);
}

@media (max-width: 768px) {
  .split-diagonal {
    flex-direction: column;
  }

  .split-diagonal__left,
  .split-diagonal__right {
    flex: none;
    width: 100%;
    min-height: 50vh;
    margin: 0;
    padding: 48px 32px;
    clip-path: none;
  }

  .split-diagonal::after {
    display: none;
  }
}
```

### Scroll-Reveal Split Sections

Split sections that reveal content with a staggered animation as they enter the viewport, emphasizing the left-right duality.

```css
.split-reveal {
  display: flex;
  min-height: 80vh;
  width: 100%;
  overflow: hidden;
}

.split-reveal__panel {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 60px;
}

/* Initial hidden state -- panels slide in from opposite sides */
.split-reveal__panel--left {
  transform: translateX(-60px);
  opacity: 0;
  transition: transform 0.8s cubic-bezier(0.25, 0.8, 0.25, 1),
              opacity 0.8s ease;
}

.split-reveal__panel--right {
  transform: translateX(60px);
  opacity: 0;
  transition: transform 0.8s cubic-bezier(0.25, 0.8, 0.25, 1) 0.15s,
              opacity 0.8s ease 0.15s;
}

/* Visible state -- triggered by Intersection Observer adding .is-visible */
.split-reveal.is-visible .split-reveal__panel--left,
.split-reveal.is-visible .split-reveal__panel--right {
  transform: translateX(0);
  opacity: 1;
}

/* Accent vertical line in the center */
.split-reveal::after {
  content: '';
  position: absolute;
  top: 10%;
  bottom: 10%;
  left: 50%;
  width: 2px;
  background: var(--split-coral);
  transform: translateX(-50%) scaleY(0);
  transition: transform 0.6s ease 0.4s;
}

.split-reveal.is-visible::after {
  transform: translateX(-50%) scaleY(1);
}

/* JavaScript: Intersection Observer to trigger .is-visible */
/*
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('is-visible');
      }
    });
  }, { threshold: 0.2 });

  document.querySelectorAll('.split-reveal').forEach(el => observer.observe(el));
*/
```

### Sticky Panel Scroll

A technique where one panel remains fixed in place while the other scrolls through multiple content blocks, creating a guided storytelling effect.

```css
.split-sticky {
  display: flex;
  min-height: 100vh;
  width: 100%;
}

/* Fixed panel -- stays in view */
.split-sticky__fixed {
  flex: 0 0 50%;
  position: sticky;
  top: 0;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: var(--split-panel-dark);
  overflow: hidden;
}

.split-sticky__fixed img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Scrolling panel -- multiple content blocks */
.split-sticky__scroll {
  flex: 0 0 50%;
  background: var(--split-panel-light);
}

.split-sticky__block {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 60px;
  border-bottom: 1px solid var(--split-mist);
}

.split-sticky__block:last-child {
  border-bottom: none;
}

.split-sticky__block-content {
  max-width: 420px;
}

.split-sticky__block-content h2 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 2.5rem;
  color: var(--split-black);
  margin-bottom: 20px;
}

.split-sticky__block-content p {
  font-family: 'Inter', sans-serif;
  color: var(--split-slate);
  line-height: 1.7;
  margin-bottom: 16px;
}

@media (max-width: 768px) {
  .split-sticky {
    flex-direction: column;
  }

  .split-sticky__fixed {
    position: relative;
    flex: none;
    width: 100%;
    height: 50vh;
  }

  .split-sticky__scroll {
    flex: none;
    width: 100%;
  }

  .split-sticky__block {
    min-height: auto;
    padding: 48px 32px;
  }
}
```

---

## Design Do's and Don'ts

### Do

- Use high-contrast pairings between panels -- dark against light, image against solid color, warm against cool
- Maintain a strict 50/50 (or intentionally asymmetric like 60/40) division as the structural backbone
- Give each panel a singular clear purpose: one for visual, one for textual content
- Use full-viewport-height split sections for maximum immersive impact in hero areas
- Leverage hover-expand interactions to create dynamic, engaging panel behavior
- Alternate panel orientation across sections (image-left then image-right) to create visual rhythm
- Apply `mix-blend-mode: difference` on navigation overlaying both panels for automatic color adaptation
- Design each panel to work as a standalone unit when stacked on mobile
- Use bold, oversized typography on the text panel -- the dedicated space demands it
- Treat the center divider as a design element: a colored stripe, diagonal slash, or animated reveal line

### Don't

- Use similar colors on adjacent panels -- the whole aesthetic depends on contrast between the two halves
- Place dense text on image panels -- that undermines the clarity of the split layout
- Forget mobile breakpoints -- a split layout that does not stack gracefully on small screens fails its users
- Add too many decorative elements -- the split itself is the design statement; keep ornamentation minimal
- Mix more than three typefaces -- the dual-panel structure already provides visual complexity
- Create panels with unequal height that break the horizontal alignment of the split
- Use thin, low-contrast dividers that make the split look accidental rather than intentional
- Apply hover-expand effects on touch devices where hover states do not exist
- Neglect the vertical rhythm of alternating sections -- inconsistent panel ordering feels chaotic
- Overload both panels with equal amounts of content -- asymmetric content weight drives the eye

---

## Related Aesthetics

| Aesthetic | Relationship to Split Screen |
|-----------|------------------------------|
| **Editorial / Magazine** | Shares the print-inspired layout tradition; Editorial uses multi-column grids while Split Screen focuses on binary division |
| **Brutalist** | Both use bold, high-contrast visual statements; Brutalist is raw and deliberately unpolished, Split Screen is precise and balanced |
| **Swiss / International** | Both prize structural clarity and grid discipline; Swiss Design uses modular grids, Split Screen simplifies to a single binary axis |
| **Minimalist** | Split Screen often employs Minimalist principles (negative space, limited palette) within its dual-panel structure |
| **Material Design** | Material uses cards and layered surfaces; Split Screen flattens the hierarchy into two co-equal planes |
| **Parallax** | Both create depth through scroll behavior; Parallax layers elements vertically, Split Screen layers them horizontally |
| **Asymmetric Layout** | Split Screen is a specific case of asymmetric design where the spatial division is equal but the content weight is unbalanced |
| **Color Block** | Shares the bold solid-fill approach; Color Block uses multiple color zones, Split Screen constrains to two primary zones |
| **Metro / Flat Design** | Both favor clean edges and solid colors; Metro tiles can be seen as micro-splits within a grid |

---

## Quick-Start: Minimal Split Screen Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Split Screen Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --split-panel-dark: #1a1a2e;
      --split-panel-light: #f5f0eb;
      --split-black: #0d0d0d;
      --split-white: #ffffff;
      --split-coral: #ff6b6b;
      --split-electric: #4ecdc4;
      --split-graphite: #2d3436;
      --split-mist: #dfe6e9;
      --split-slate: #636e72;
      --split-transition: 0.5s;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Inter', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
      color: var(--split-graphite);
      background: var(--split-panel-light);
    }

    h1, h2, h3 {
      font-family: 'Bebas Neue', sans-serif;
      font-weight: 400;
      letter-spacing: 0.04em;
      line-height: 1.05;
    }

    /* ---- Navigation ---- */
    nav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 24px 48px;
      z-index: 100;
      mix-blend-mode: difference;
    }

    nav a.logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.6rem;
      color: var(--split-white);
      text-decoration: none;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      font-family: 'Inter', sans-serif;
      font-weight: 500;
      font-size: 0.85rem;
      color: var(--split-white);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      position: relative;
      transition: opacity 0.3s;
    }

    nav ul a::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 2px;
      background: var(--split-coral);
      transition: width 0.3s ease;
    }

    nav ul a:hover::after {
      width: 100%;
    }

    /* ---- Split Hero ---- */
    .hero {
      display: flex;
      min-height: 100vh;
      width: 100%;
    }

    .hero__panel {
      flex: 1;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 80px 60px;
      position: relative;
      overflow: hidden;
      transition: flex var(--split-transition) ease;
    }

    .hero__panel--dark {
      background: var(--split-panel-dark);
    }

    .hero__panel--image {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      position: relative;
    }

    /* Decorative geometric shapes on image panel */
    .hero__panel--image::before {
      content: '';
      position: absolute;
      top: 15%;
      left: 15%;
      width: 200px;
      height: 200px;
      border: 3px solid rgba(255, 255, 255, 0.2);
      border-radius: 50%;
      animation: float 6s ease-in-out infinite;
    }

    .hero__panel--image::after {
      content: '';
      position: absolute;
      bottom: 20%;
      right: 20%;
      width: 120px;
      height: 120px;
      border: 3px solid rgba(255, 255, 255, 0.15);
      transform: rotate(45deg);
      animation: float 8s ease-in-out infinite reverse;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-20px) rotate(5deg); }
    }

    .hero__content {
      max-width: 440px;
      position: relative;
      z-index: 2;
    }

    .hero__label {
      font-family: 'Inter', sans-serif;
      font-size: 0.75rem;
      font-weight: 600;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--split-coral);
      margin-bottom: 20px;
    }

    .hero__content h1 {
      font-size: clamp(3rem, 5vw, 5rem);
      color: var(--split-white);
      margin-bottom: 24px;
      line-height: 0.95;
    }

    .hero__content p {
      font-size: 1.05rem;
      line-height: 1.7;
      color: rgba(255, 255, 255, 0.7);
      margin-bottom: 36px;
    }

    .btn {
      display: inline-block;
      padding: 16px 40px;
      font-family: 'Inter', sans-serif;
      font-weight: 600;
      font-size: 0.85rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      text-decoration: none;
      border: 2px solid var(--split-white);
      color: var(--split-white);
      background: transparent;
      cursor: pointer;
      position: relative;
      overflow: hidden;
      transition: color var(--split-transition), background var(--split-transition);
    }

    .btn:hover {
      color: var(--split-panel-dark);
      background: var(--split-white);
    }

    .btn--accent {
      border-color: var(--split-coral);
      color: var(--split-white);
      background: var(--split-coral);
    }

    .btn--accent:hover {
      background: #e85555;
      border-color: #e85555;
    }

    .btn--dark {
      border-color: var(--split-black);
      color: var(--split-black);
    }

    .btn--dark:hover {
      background: var(--split-black);
      color: var(--split-white);
    }

    /* ---- Hover-Expand Section ---- */
    .expand-section {
      display: flex;
      min-height: 70vh;
      width: 100%;
      overflow: hidden;
    }

    .expand-panel {
      flex: 1;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
      cursor: pointer;
      transition: flex 0.6s cubic-bezier(0.25, 0.8, 0.25, 1);
    }

    .expand-panel--a {
      background: var(--split-coral);
    }

    .expand-panel--b {
      background: var(--split-electric);
    }

    .expand-section:hover .expand-panel {
      flex: 0.7;
    }

    .expand-section:hover .expand-panel:hover {
      flex: 1.3;
    }

    .expand-panel::before {
      content: '';
      position: absolute;
      inset: 0;
      background: rgba(0, 0, 0, 0);
      transition: background 0.6s ease;
      z-index: 1;
    }

    .expand-section:hover .expand-panel::before {
      background: rgba(0, 0, 0, 0.2);
    }

    .expand-section:hover .expand-panel:hover::before {
      background: rgba(0, 0, 0, 0);
    }

    .expand-panel__content {
      position: relative;
      z-index: 2;
      text-align: center;
      color: var(--split-white);
      padding: 40px;
    }

    .expand-panel__content h2 {
      font-size: clamp(2rem, 4vw, 3.5rem);
      margin-bottom: 12px;
    }

    .expand-panel__content p {
      font-size: 0.95rem;
      max-width: 300px;
      margin: 0 auto;
      opacity: 0;
      transform: translateY(10px);
      transition: opacity 0.5s 0.1s, transform 0.5s 0.1s;
    }

    .expand-panel:hover .expand-panel__content p {
      opacity: 0.9;
      transform: translateY(0);
    }

    /* ---- Alternating Feature Splits ---- */
    .feature-split {
      display: flex;
      min-height: 80vh;
      width: 100%;
    }

    .feature-split:nth-child(even) {
      flex-direction: row-reverse;
    }

    .feature-split__image {
      flex: 1;
      min-height: 400px;
      background-size: cover;
      background-position: center;
    }

    .feature-split__image--gradient-1 {
      background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
    }

    .feature-split__image--gradient-2 {
      background: linear-gradient(135deg, #2d3436 0%, #636e72 100%);
    }

    .feature-split__image--gradient-3 {
      background: linear-gradient(135deg, #0c2461 0%, #1e3799 100%);
    }

    .feature-split__text {
      flex: 1;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 80px 60px;
    }

    .feature-split__text--light {
      background: var(--split-panel-light);
    }

    .feature-split__text--white {
      background: var(--split-white);
    }

    .feature-split__content {
      max-width: 420px;
    }

    .feature-split__content .split-label {
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--split-coral);
      margin-bottom: 16px;
    }

    .feature-split__content h2 {
      font-size: clamp(2rem, 3vw, 3rem);
      color: var(--split-black);
      margin-bottom: 20px;
    }

    .feature-split__content p {
      color: var(--split-slate);
      margin-bottom: 28px;
      line-height: 1.8;
    }

    /* Decorative geometric elements inside gradient panels */
    .feature-split__image {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .geo-shape {
      width: 120px;
      height: 120px;
      border: 2px solid rgba(255, 255, 255, 0.15);
      position: absolute;
    }

    .geo-shape--circle {
      border-radius: 50%;
      top: 25%;
      left: 30%;
    }

    .geo-shape--square {
      transform: rotate(45deg);
      bottom: 25%;
      right: 25%;
      width: 80px;
      height: 80px;
    }

    .geo-shape--line {
      border: none;
      border-top: 2px solid rgba(255, 255, 255, 0.1);
      width: 60%;
      height: 0;
      top: 50%;
      left: 20%;
    }

    /* ---- Diagonal Split CTA ---- */
    .diagonal-cta {
      display: flex;
      min-height: 50vh;
      width: 100%;
      position: relative;
      overflow: hidden;
    }

    .diagonal-cta__left {
      flex: 0 0 55%;
      background: var(--split-panel-dark);
      clip-path: polygon(0 0, 100% 0, 88% 100%, 0 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 60px 80px;
      z-index: 2;
    }

    .diagonal-cta__right {
      flex: 0 0 55%;
      margin-left: -10%;
      background: var(--split-coral);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 60px 80px;
    }

    .diagonal-cta__left h2 {
      font-size: clamp(2rem, 4vw, 3.5rem);
      color: var(--split-white);
      max-width: 400px;
    }

    .diagonal-cta__right p {
      font-size: 1.1rem;
      color: var(--split-white);
      max-width: 360px;
      margin-bottom: 28px;
    }

    /* ---- Divider ---- */
    .split-divider {
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 0;
      height: 4px;
      background: linear-gradient(90deg,
        var(--split-panel-dark) 0%,
        var(--split-panel-dark) 50%,
        var(--split-coral) 50%,
        var(--split-coral) 100%
      );
    }

    /* ---- Footer ---- */
    footer {
      display: flex;
      min-height: 200px;
    }

    .footer__left {
      flex: 1;
      background: var(--split-panel-dark);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 40px;
    }

    .footer__right {
      flex: 1;
      background: var(--split-black);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 40px;
    }

    .footer__left p,
    .footer__right p {
      font-size: 0.85rem;
      color: rgba(255, 255, 255, 0.5);
    }

    .footer__left a.footer-logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.4rem;
      color: var(--split-white);
      text-decoration: none;
      letter-spacing: 0.08em;
    }

    .footer__right ul {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    .footer__right ul a {
      font-size: 0.8rem;
      color: rgba(255, 255, 255, 0.5);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      transition: color 0.3s;
    }

    .footer__right ul a:hover {
      color: var(--split-coral);
    }

    /* ---- Responsive ---- */
    @media (max-width: 768px) {
      nav {
        padding: 20px 24px;
      }

      nav ul {
        gap: 16px;
      }

      .hero {
        flex-direction: column;
      }

      .hero__panel {
        min-height: 50vh;
        padding: 60px 32px;
      }

      .expand-section {
        flex-direction: column;
        min-height: auto;
      }

      .expand-panel {
        min-height: 40vh;
      }

      .expand-section:hover .expand-panel,
      .expand-section:hover .expand-panel:hover {
        flex: 1;
      }

      .expand-panel__content p {
        opacity: 0.9;
        transform: translateY(0);
      }

      .feature-split,
      .feature-split:nth-child(even) {
        flex-direction: column;
      }

      .feature-split__image {
        min-height: 250px;
      }

      .feature-split__text {
        padding: 48px 32px;
      }

      .diagonal-cta {
        flex-direction: column;
      }

      .diagonal-cta__left,
      .diagonal-cta__right {
        flex: none;
        width: 100%;
        clip-path: none;
        margin: 0;
        padding: 48px 32px;
      }

      footer {
        flex-direction: column;
      }

      .footer__left,
      .footer__right {
        padding: 32px 24px;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <a href="#" class="logo">Divide</a>
    <ul>
      <li><a href="#">Work</a></li>
      <li><a href="#">Studio</a></li>
      <li><a href="#">Journal</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero Split -->
  <section class="hero">
    <div class="hero__panel hero__panel--dark">
      <div class="hero__content">
        <div class="hero__label">Design Studio</div>
        <h1>Two Sides.<br>One Vision.</h1>
        <p>We believe the best ideas emerge from tension -- the space between opposing forces where creativity thrives.</p>
        <a href="#" class="btn">Explore Work</a>
      </div>
    </div>
    <div class="hero__panel hero__panel--image">
    </div>
  </section>

  <!-- Split Divider -->
  <div class="split-divider"></div>

  <!-- Hover-Expand Panels -->
  <section class="expand-section">
    <div class="expand-panel expand-panel--a">
      <div class="expand-panel__content">
        <h2>Create</h2>
        <p>From concept to execution, we craft digital experiences that resonate and endure.</p>
      </div>
    </div>
    <div class="expand-panel expand-panel--b">
      <div class="expand-panel__content">
        <h2>Discover</h2>
        <p>Research-driven strategy that uncovers insights and transforms them into opportunity.</p>
      </div>
    </div>
  </section>

  <!-- Feature Splits -->
  <section>
    <div class="feature-split">
      <div class="feature-split__image feature-split__image--gradient-1">
        <div class="geo-shape geo-shape--circle"></div>
        <div class="geo-shape geo-shape--square"></div>
      </div>
      <div class="feature-split__text feature-split__text--light">
        <div class="feature-split__content">
          <div class="split-label">Strategy</div>
          <h2>Bold Thinking, Clear Direction</h2>
          <p>Every project begins with understanding. We map the landscape, identify tensions, and chart a path that balances ambition with precision.</p>
          <a href="#" class="btn btn--dark">Learn More</a>
        </div>
      </div>
    </div>

    <div class="feature-split">
      <div class="feature-split__image feature-split__image--gradient-2">
        <div class="geo-shape geo-shape--circle"></div>
        <div class="geo-shape geo-shape--line"></div>
      </div>
      <div class="feature-split__text feature-split__text--white">
        <div class="feature-split__content">
          <div class="split-label">Craft</div>
          <h2>Precision in Every Pixel</h2>
          <p>Design is in the details. We obsess over typography, spacing, and interaction to create interfaces that feel inevitable -- as if they could not have been made any other way.</p>
          <a href="#" class="btn btn--dark">Our Process</a>
        </div>
      </div>
    </div>

    <div class="feature-split">
      <div class="feature-split__image feature-split__image--gradient-3">
        <div class="geo-shape geo-shape--square"></div>
        <div class="geo-shape geo-shape--line"></div>
      </div>
      <div class="feature-split__text feature-split__text--light">
        <div class="feature-split__content">
          <div class="split-label">Impact</div>
          <h2>Results That Speak</h2>
          <p>Beautiful design means nothing without performance. We measure, iterate, and refine until the numbers match the ambition.</p>
          <a href="#" class="btn btn--dark">Case Studies</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Diagonal Split CTA -->
  <section class="diagonal-cta">
    <div class="diagonal-cta__left">
      <h2>Ready to See Both Sides?</h2>
    </div>
    <div class="diagonal-cta__right">
      <div>
        <p>Let us show you what happens when contrast meets collaboration. Start a conversation today.</p>
        <a href="#" class="btn">Get in Touch</a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="footer__left">
      <a href="#" class="footer-logo">Divide</a>
    </div>
    <div class="footer__right">
      <ul>
        <li><a href="#">Work</a></li>
        <li><a href="#">Studio</a></li>
        <li><a href="#">Journal</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </div>
  </footer>

</body>
</html>
```
