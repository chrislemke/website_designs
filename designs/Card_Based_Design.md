# Card-Based Design Reference

Card-Based Design is a modular UI pattern that organizes content into discrete, self-contained rectangular units -- cards -- each representing a single idea, product, article, or action. Rooted in the physical metaphor of index cards, playing cards, and sticky notes, the pattern gained massive digital traction through Microsoft's Metro "live tiles" (2010), Google Now's information cards (2012), and Google's Material Design system (2014). Pinterest's masonry-grid layout became the definitive visual expression of card-based browsing at scale. The aesthetic prizes containment, scannability, and modularity: every card is a digestible chunk of content with clear boundaries, consistent internal structure, and the flexibility to be rearranged, filtered, or reflowed across any viewport. In modern web and UI design, Card-Based Design translates to clean surfaces with subtle elevation, generous white space, rounded corners, image-forward compositions, and responsive grid systems that adapt gracefully from multi-column masonry layouts on desktop to single-column stacks on mobile.

---

## Visual Characteristics

### Core Design Traits

- **Contained content units** -- each card is a bounded rectangle grouping a single piece of related content (image, title, description, action)
- **Subtle elevation and shadow** -- cards float slightly above the background canvas via soft box-shadows, creating a layered paper-like depth
- **Rounded corners** -- gently rounded rectangles (8-16px radius) soften the visual feel and distinguish cards from rigid table cells
- **Generous white space** -- ample padding within cards and generous gaps between them create breathing room and reduce cognitive load
- **Image-forward layouts** -- cards frequently lead with a thumbnail, hero image, or icon, making the grid visually rich and scannable
- **Consistent internal hierarchy** -- each card follows a predictable structure: media, title, supporting text, actions
- **Masonry and grid arrangements** -- cards are laid out in Pinterest-style masonry grids, uniform grids, or carousel rows
- **Clean flat surfaces** -- backgrounds are typically white, off-white, or light gray; card surfaces are white or very slightly tinted
- **Micro-interactions on hover** -- cards lift, shadows deepen, images scale, or overlays appear when the user hovers, signaling interactivity
- **Typographic clarity** -- short, scannable text with strong hierarchy: bold title, muted description, colored action link
- **Border and divider subtlety** -- separations achieved through shadow and spacing rather than heavy borders
- **Responsive fluidity** -- cards reflow naturally from multi-column grids to single-column stacks without breaking visual coherence

### Design Principles

- Every card should represent one complete thought, item, or action -- never split a single concept across cards
- Use the common-region Gestalt principle: grouping content within a bounded container makes it perceived as a unit
- Maintain consistent card anatomy across a collection: if one card has image-title-description-button, all should follow that pattern
- Elevation (shadow depth) communicates hierarchy -- resting cards have light shadow; focused or active cards have deeper shadow
- Cards should be scannable in under three seconds -- prioritize glanceable content over dense text
- White space is structural, not decorative -- it separates content groups and guides the eye
- The grid should feel organic, not rigid -- masonry layouts embrace variable heights for visual interest
- Cards are inherently responsive: their modular nature makes them the ideal building block for fluid layouts
- Interactivity should be discoverable through hover states, cursor changes, and subtle motion
- Accessibility matters: ensure sufficient color contrast, focus indicators, and semantic markup for screen readers

---

## Color Palette

### Clean Surface Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Canvas Gray** | `#F5F5F7` | Page background, the surface cards sit upon |
| **Card White** | `#FFFFFF` | Primary card surface, clean and bright |
| **Warm Canvas** | `#FAF9F6` | Alternative warm page background |
| **Soft Gray** | `#E8E8ED` | Card borders, dividers, inactive states |
| **Medium Gray** | `#C7C7CC` | Placeholder text, disabled elements |
| **Text Primary** | `#1D1D1F` | Headlines, primary card titles |
| **Text Secondary** | `#6E6E73` | Descriptions, supporting text, metadata |
| **Text Tertiary** | `#9A9AA0` | Captions, timestamps, subtle labels |
| **Action Blue** | `#0071E3` | Primary CTAs, links, interactive accents |
| **Action Hover** | `#0062CC` | Hovered links and buttons, darker active state |
| **Success Green** | `#34C759` | Positive indicators, success badges |
| **Warning Amber** | `#FF9500` | Alerts, attention-required badges |
| **Error Red** | `#FF3B30` | Errors, destructive actions, urgent badges |
| **Card Shadow** | `rgba(0,0,0,0.08)` | Default card elevation shadow |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --card-bg-canvas: #f5f5f7;
  --card-bg-canvas-warm: #faf9f6;
  --card-bg-surface: #ffffff;

  /* Borders & Dividers */
  --card-border-light: #e8e8ed;
  --card-border-medium: #c7c7cc;

  /* Text */
  --card-text-primary: #1d1d1f;
  --card-text-secondary: #6e6e73;
  --card-text-tertiary: #9a9aa0;

  /* Actions */
  --card-action-blue: #0071e3;
  --card-action-hover: #0062cc;

  /* Status */
  --card-success: #34c759;
  --card-warning: #ff9500;
  --card-error: #ff3b30;

  /* Elevation Shadows */
  --card-shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.06), 0 1px 2px rgba(0, 0, 0, 0.04);
  --card-shadow-md: 0 4px 12px rgba(0, 0, 0, 0.08), 0 2px 4px rgba(0, 0, 0, 0.04);
  --card-shadow-lg: 0 12px 32px rgba(0, 0, 0, 0.12), 0 4px 8px rgba(0, 0, 0, 0.06);
  --card-shadow-xl: 0 20px 48px rgba(0, 0, 0, 0.16), 0 8px 16px rgba(0, 0, 0, 0.08);

  /* Border Radius */
  --card-radius-sm: 8px;
  --card-radius-md: 12px;
  --card-radius-lg: 16px;
  --card-radius-xl: 20px;

  /* Spacing */
  --card-gap: 24px;
  --card-padding: 24px;
  --card-padding-compact: 16px;

  /* Transitions */
  --card-transition: 0.25s cubic-bezier(0.4, 0, 0.2, 1);
}
```

---

## Typography

### Typeface Characteristics

Card-Based Design typography is:

- **Clean and legible** -- sans-serif typefaces that prioritize readability at small sizes within constrained card widths
- **Hierarchically structured** -- strong contrast between bold card titles, lighter description text, and small metadata
- **Compact and efficient** -- text must communicate within limited vertical space; every line earns its place
- **Neutral and versatile** -- typefaces that work across categories (news, e-commerce, social, dashboard) without imposing a strong personality
- **Scannable** -- short titles (1-2 lines), truncated descriptions (2-3 lines), and prominent action text guide the eye quickly
- **System-friendly** -- often uses system font stacks or widely available Google Fonts for performance and consistency

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Inter** | Modern geometric sans | Card titles, body text, all-purpose |
| **Roboto** | Material Design standard | Cards in Material-inspired layouts |
| **DM Sans** | Geometric, friendly | Card titles, clean modern layouts |
| **Plus Jakarta Sans** | Rounded geometric | Warm, approachable card designs |
| **Source Sans 3** | Humanist sans | Body text, descriptions, metadata |
| **Nunito** | Rounded, soft | Friendly card UIs, consumer apps |
| **Manrope** | Modern, geometric | Tech dashboards, SaaS card layouts |
| **Lato** | Stable, warm | Body text, subtle and professional |
| **Work Sans** | Slightly condensed | Navigation, labels, compact cards |
| **Space Grotesk** | Geometric, contemporary | Feature cards, modern portfolios |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **DM Sans** (700) | **Inter** (400) | Clean, modern, tech-friendly |
| **Plus Jakarta Sans** (700) | **Source Sans 3** (400) | Warm, approachable, editorial |
| **Manrope** (800) | **Inter** (400) | Bold headers, clean reading |
| **Space Grotesk** (600) | **Lato** (400) | Geometric contrast, professional |
| **Nunito** (700) | **Work Sans** (400) | Rounded warmth, efficient body text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Inter:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  color: var(--card-text-primary);
  line-height: 1.25;
  letter-spacing: -0.01em;
}

/* Card title */
.card-title {
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  font-size: 1.125rem;
  color: var(--card-text-primary);
  line-height: 1.35;
  margin-bottom: 8px;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

/* Card description */
.card-description {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 0.9rem;
  color: var(--card-text-secondary);
  line-height: 1.6;
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

/* Body text */
body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.65;
  color: var(--card-text-primary);
}

/* Metadata / Labels */
.card-meta {
  font-family: 'Inter', sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  letter-spacing: 0.02em;
  text-transform: uppercase;
  color: var(--card-text-tertiary);
}

/* Card action link */
.card-action {
  font-family: 'DM Sans', sans-serif;
  font-size: 0.875rem;
  font-weight: 600;
  color: var(--card-action-blue);
  text-decoration: none;
  transition: color var(--card-transition);
}

.card-action:hover {
  color: var(--card-action-hover);
}
```

---

## Layout Principles

### Grid and Structure

- **Responsive multi-column grids** -- cards arrange in 3-4 columns on desktop, 2 columns on tablet, 1 column on mobile
- **CSS Grid with auto-fit** -- `grid-template-columns: repeat(auto-fit, minmax(300px, 1fr))` is the workhorse for card layouts
- **Masonry layouts** -- for variable-height content, masonry grids (via CSS `masonry-rows` or column-based CSS) fill vertical gaps naturally
- **Consistent gap spacing** -- 20-32px gutters between cards maintain rhythm without feeling crowded
- **Maximum container width** -- content constrained to 1200-1440px with centered alignment and horizontal padding
- **Card aspect ratios** -- image regions often follow 16:9, 4:3, or 1:1 ratios for visual consistency across the grid
- **Equal-height rows** -- in uniform grids, cards stretch to match the tallest card in each row for clean alignment
- **Nested grids** -- dashboard layouts may nest card grids within larger card panels for information hierarchy

### Section Organization

- **Navigation**: Clean, minimal top bar with logo and links; often white or transparent with subtle bottom border
- **Hero**: Can be a large featured card or a hero banner with a grid of cards immediately below
- **Content Grid**: The primary section; a responsive grid of content cards that is the visual centerpiece
- **Filters and Controls**: Horizontal filter bar or sidebar with category chips and sort controls above the card grid
- **Featured Row**: A horizontally scrolling carousel of highlighted or promoted cards
- **Detail Expansion**: Clicking a card opens a modal, side panel, or navigates to a detail page
- **CTA Section**: A single wide card or banner encouraging a primary action
- **Footer**: Minimal footer with links organized in a clean multi-column layout

### Responsive Approach

- Cards are the ideal responsive primitive: they stack, reflow, and resize naturally at every breakpoint
- Use `auto-fit` with `minmax()` to let the browser determine column count based on available space
- On mobile, cards become full-width single-column stacks with reduced padding
- Horizontal card carousels become vertically stacked lists on smaller viewports
- Image aspect ratios may shift (e.g., landscape on desktop to square on mobile) to save vertical space
- Touch targets on card action buttons should be at least 44px on mobile
- Reduce shadow intensity on mobile for cleaner rendering and performance

---

## CSS / Design Techniques

### Standard Card Component

```css
.card {
  background: var(--card-bg-surface);
  border-radius: var(--card-radius-md);
  box-shadow: var(--card-shadow-md);
  overflow: hidden;
  display: flex;
  flex-direction: column;
  transition:
    transform var(--card-transition),
    box-shadow var(--card-transition);
  cursor: pointer;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: var(--card-shadow-lg);
}

.card__image {
  width: 100%;
  aspect-ratio: 16 / 9;
  object-fit: cover;
  display: block;
}

.card__body {
  padding: var(--card-padding);
  flex: 1;
  display: flex;
  flex-direction: column;
}

.card__category {
  font-size: 0.7rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  color: var(--card-action-blue);
  margin-bottom: 8px;
}

.card__title {
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  font-size: 1.125rem;
  color: var(--card-text-primary);
  line-height: 1.35;
  margin-bottom: 8px;
}

.card__text {
  font-family: 'Inter', sans-serif;
  font-size: 0.9rem;
  color: var(--card-text-secondary);
  line-height: 1.6;
  flex: 1;
}

.card__footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 16px;
  margin-top: 16px;
  border-top: 1px solid var(--card-border-light);
}

/* Card Grid */
.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: var(--card-gap);
}
```

### Button Component

```css
.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  font-family: 'DM Sans', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  padding: 12px 24px;
  border-radius: var(--card-radius-sm);
  border: none;
  cursor: pointer;
  text-decoration: none;
  transition:
    background var(--card-transition),
    box-shadow var(--card-transition),
    transform var(--card-transition);
}

/* Primary */
.btn--primary {
  background: var(--card-action-blue);
  color: #ffffff;
}

.btn--primary:hover {
  background: var(--card-action-hover);
  box-shadow: 0 4px 12px rgba(0, 113, 227, 0.3);
  transform: translateY(-1px);
}

/* Secondary / Outlined */
.btn--secondary {
  background: transparent;
  color: var(--card-action-blue);
  border: 1.5px solid var(--card-border-light);
}

.btn--secondary:hover {
  background: var(--card-bg-canvas);
  border-color: var(--card-action-blue);
}

/* Ghost / Text Button */
.btn--ghost {
  background: transparent;
  color: var(--card-action-blue);
  padding: 8px 12px;
}

.btn--ghost:hover {
  background: rgba(0, 113, 227, 0.06);
}
```

### Navigation Bar

```css
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 16px 32px;
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(255, 255, 255, 0.85);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--card-border-light);
}

.navbar__logo {
  font-family: 'DM Sans', sans-serif;
  font-size: 1.25rem;
  font-weight: 700;
  color: var(--card-text-primary);
  text-decoration: none;
  letter-spacing: -0.02em;
}

.navbar__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.navbar__links a {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--card-text-secondary);
  text-decoration: none;
  transition: color var(--card-transition);
  position: relative;
}

.navbar__links a:hover {
  color: var(--card-text-primary);
}

.navbar__links a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--card-action-blue);
  transition: width var(--card-transition);
}

.navbar__links a:hover::after {
  width: 100%;
}
```

### Hero Section with Featured Card

```css
.hero {
  padding: 80px 32px;
  max-width: 1200px;
  margin: 0 auto;
}

.hero__featured {
  display: grid;
  grid-template-columns: 1.2fr 1fr;
  gap: 32px;
  align-items: center;
  background: var(--card-bg-surface);
  border-radius: var(--card-radius-lg);
  box-shadow: var(--card-shadow-lg);
  overflow: hidden;
}

.hero__image {
  width: 100%;
  height: 100%;
  min-height: 400px;
  object-fit: cover;
  display: block;
}

.hero__content {
  padding: 48px 48px 48px 16px;
}

.hero__label {
  font-family: 'Inter', sans-serif;
  font-size: 0.7rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--card-action-blue);
  margin-bottom: 16px;
}

.hero__title {
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  font-size: clamp(1.75rem, 3vw, 2.5rem);
  color: var(--card-text-primary);
  line-height: 1.2;
  letter-spacing: -0.02em;
  margin-bottom: 16px;
}

.hero__description {
  font-family: 'Inter', sans-serif;
  font-size: 1.05rem;
  color: var(--card-text-secondary);
  line-height: 1.65;
  margin-bottom: 32px;
}

@media (max-width: 768px) {
  .hero__featured {
    grid-template-columns: 1fr;
  }
  .hero__image { min-height: 240px; }
  .hero__content { padding: 32px; }
}
```

### Masonry Grid Layout

```css
/* CSS Columns Masonry (widely supported) */
.masonry {
  column-count: 3;
  column-gap: var(--card-gap);
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 32px;
}

.masonry .card {
  break-inside: avoid;
  margin-bottom: var(--card-gap);
  display: inline-block;
  width: 100%;
}

@media (max-width: 1024px) {
  .masonry { column-count: 2; }
}

@media (max-width: 640px) {
  .masonry { column-count: 1; }
}

/* CSS Grid Masonry (experimental, progressive enhancement) */
@supports (grid-template-rows: masonry) {
  .masonry-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    grid-template-rows: masonry;
    gap: var(--card-gap);
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 32px;
  }

  .masonry-grid .card {
    break-inside: auto;
    margin-bottom: 0;
    display: flex;
  }
}
```

### Card Hover Effects

```css
/* Lift and deepen shadow */
.card--lift {
  transition:
    transform var(--card-transition),
    box-shadow var(--card-transition);
}

.card--lift:hover {
  transform: translateY(-6px);
  box-shadow: var(--card-shadow-xl);
}

/* Image zoom on hover */
.card--zoom .card__image-wrap {
  overflow: hidden;
  border-radius: var(--card-radius-md) var(--card-radius-md) 0 0;
}

.card--zoom .card__image {
  transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}

.card--zoom:hover .card__image {
  transform: scale(1.06);
}

/* Border highlight on hover */
.card--border {
  border: 2px solid transparent;
  transition:
    border-color var(--card-transition),
    box-shadow var(--card-transition);
}

.card--border:hover {
  border-color: var(--card-action-blue);
  box-shadow: 0 0 0 4px rgba(0, 113, 227, 0.08);
}

/* Overlay reveal on hover */
.card--overlay {
  position: relative;
}

.card--overlay .card__overlay {
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0;
  transition: opacity var(--card-transition);
  border-radius: var(--card-radius-md);
}

.card--overlay:hover .card__overlay {
  opacity: 1;
}

/* Focus visible state for accessibility */
.card:focus-visible {
  outline: 3px solid var(--card-action-blue);
  outline-offset: 2px;
  box-shadow: var(--card-shadow-lg);
}
```

### Horizontal Card Carousel

```css
.carousel {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 32px;
}

.carousel__header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 24px;
}

.carousel__title {
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  font-size: 1.5rem;
  color: var(--card-text-primary);
}

.carousel__controls {
  display: flex;
  gap: 8px;
}

.carousel__btn {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  border: 1.5px solid var(--card-border-light);
  background: var(--card-bg-surface);
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.1rem;
  color: var(--card-text-secondary);
  transition:
    background var(--card-transition),
    border-color var(--card-transition);
}

.carousel__btn:hover {
  background: var(--card-bg-canvas);
  border-color: var(--card-action-blue);
  color: var(--card-action-blue);
}

.carousel__track {
  display: flex;
  gap: var(--card-gap);
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  scroll-behavior: smooth;
  -ms-overflow-style: none;
  scrollbar-width: none;
  padding-bottom: 8px;
}

.carousel__track::-webkit-scrollbar {
  display: none;
}

.carousel__track .card {
  flex: 0 0 300px;
  scroll-snap-align: start;
}

@media (max-width: 640px) {
  .carousel__track .card {
    flex: 0 0 85vw;
  }
}
```

### Filter / Chip Bar

```css
.filter-bar {
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
  margin-bottom: 32px;
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding: 0 32px 32px;
}

.chip {
  font-family: 'Inter', sans-serif;
  font-size: 0.825rem;
  font-weight: 500;
  padding: 8px 18px;
  border-radius: 100px;
  border: 1.5px solid var(--card-border-light);
  background: var(--card-bg-surface);
  color: var(--card-text-secondary);
  cursor: pointer;
  transition:
    background var(--card-transition),
    border-color var(--card-transition),
    color var(--card-transition);
  white-space: nowrap;
}

.chip:hover {
  border-color: var(--card-action-blue);
  color: var(--card-action-blue);
}

.chip--active {
  background: var(--card-action-blue);
  border-color: var(--card-action-blue);
  color: #ffffff;
}

.chip--active:hover {
  background: var(--card-action-hover);
  border-color: var(--card-action-hover);
  color: #ffffff;
}
```

---

## Design Do's and Don'ts

### Do

- Keep each card focused on a single content item or action -- one card, one idea
- Use consistent internal structure across all cards in a grid (image, title, text, action in the same order)
- Apply subtle box-shadows for elevation rather than heavy borders or outlines
- Use generous and consistent spacing: padding inside cards (16-32px) and gaps between cards (20-32px)
- Lead with imagery when content is visual (products, articles, portfolios)
- Truncate long text with line-clamp to keep cards compact and uniform in height
- Provide clear hover and focus states to signal interactivity
- Use rounded corners consistently across all cards (8-16px radius)
- Maintain a clean, neutral background so cards pop through elevation contrast
- Make cards responsive using `auto-fit` / `minmax()` grid patterns or masonry columns
- Ensure accessibility: semantic HTML, proper heading levels, focus-visible outlines, ARIA labels on interactive cards
- Use category labels, badges, or colored accents to help users filter and identify card types at a glance

### Don't

- Overload cards with too much information -- if you need a paragraph, it belongs on a detail page, not a card
- Mix wildly different card sizes, structures, or styles in the same grid -- consistency is key
- Use harsh, thick borders instead of shadows for card definition -- it creates a dated, boxy look
- Neglect white space by cramming cards edge-to-edge with no breathing room
- Apply excessive animation or complex hover effects that distract from content scanning
- Use dark backgrounds as the default canvas -- card-based design relies on light surfaces for its clean, airy feel
- Forget mobile users: ensure cards work as single-column stacks with proper touch targets (44px minimum)
- Make every card look clickable if some are not interactive -- unclear affordances confuse users
- Use masonry layouts when uniform alignment is important (e.g., data dashboards, comparison grids)
- Rely solely on color to communicate meaning -- always pair color indicators with text or icons for accessibility

---

## Related Aesthetics

| Aesthetic | Relationship to Card-Based Design |
|-----------|----------------------------------|
| **Material Design** | Google's design system formalized the card as a primary UI component; Material Design is card-based design codified with specific elevation, motion, and color rules |
| **Metro Design** | Microsoft's "live tiles" were an early card-like pattern; Metro uses flat, borderless tiles while card-based design adds elevation and rounded corners |
| **Flat Design** | Cards evolved from flat design by reintroducing subtle depth (shadows, layering) while retaining clean, minimal surfaces |
| **Minimalism** | Shares the emphasis on white space, typography hierarchy, and content focus; card-based design adds the modular container structure |
| **Brutalist Web Design** | The anti-card aesthetic: rejects containment, shadows, and polished surfaces in favor of raw, undecorated layouts |
| **Neumorphism** | Takes the card elevation concept further with soft inner/outer shadows that make cards appear extruded from the background |
| **Glassmorphism** | Applies frosted-glass transparency to card surfaces; a stylistic variant of card-based design with blur and translucency |
| **Dashboard UI** | Heavily relies on card-based layouts for data widgets, metric panels, and chart containers |
| **Pinterest / Masonry** | The visual archetype of card-based design at scale; variable-height cards in a waterfall grid |

---

## Quick-Start: Minimal Card-Based Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Card-Based Design</title>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --card-bg-canvas: #f5f5f7;
      --card-bg-surface: #ffffff;
      --card-border-light: #e8e8ed;
      --card-text-primary: #1d1d1f;
      --card-text-secondary: #6e6e73;
      --card-text-tertiary: #9a9aa0;
      --card-action-blue: #0071e3;
      --card-action-hover: #0062cc;
      --card-shadow-sm: 0 1px 3px rgba(0,0,0,0.06), 0 1px 2px rgba(0,0,0,0.04);
      --card-shadow-md: 0 4px 12px rgba(0,0,0,0.08), 0 2px 4px rgba(0,0,0,0.04);
      --card-shadow-lg: 0 12px 32px rgba(0,0,0,0.12), 0 4px 8px rgba(0,0,0,0.06);
      --card-radius-sm: 8px;
      --card-radius-md: 12px;
      --card-radius-lg: 16px;
      --card-gap: 24px;
      --card-padding: 24px;
      --card-transition: 0.25s cubic-bezier(0.4, 0, 0.2, 1);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--card-bg-canvas);
      color: var(--card-text-primary);
      font-family: 'Inter', sans-serif;
      font-size: 1rem;
      line-height: 1.65;
    }

    h1, h2, h3 {
      font-family: 'DM Sans', sans-serif;
      font-weight: 700;
      line-height: 1.25;
      letter-spacing: -0.01em;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 16px 32px;
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(245, 245, 247, 0.85);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
    }

    nav a.logo {
      font-family: 'DM Sans', sans-serif;
      font-size: 1.25rem;
      font-weight: 700;
      color: var(--card-text-primary);
      text-decoration: none;
      letter-spacing: -0.02em;
    }

    nav ul {
      display: flex;
      gap: 32px;
      list-style: none;
    }

    nav ul a {
      font-family: 'Inter', sans-serif;
      font-weight: 500;
      font-size: 0.9rem;
      color: var(--card-text-secondary);
      text-decoration: none;
      transition: color var(--card-transition);
    }

    nav ul a:hover {
      color: var(--card-text-primary);
    }

    /* Hero */
    .hero {
      max-width: 1200px;
      margin: 0 auto;
      padding: 60px 32px 48px;
    }

    .hero-card {
      display: grid;
      grid-template-columns: 1.2fr 1fr;
      background: var(--card-bg-surface);
      border-radius: var(--card-radius-lg);
      box-shadow: var(--card-shadow-lg);
      overflow: hidden;
    }

    .hero-image {
      min-height: 380px;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      color: rgba(255,255,255,0.3);
      font-size: 4rem;
    }

    .hero-body {
      padding: 48px;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .hero-label {
      font-size: 0.7rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--card-action-blue);
      margin-bottom: 16px;
    }

    .hero-body h1 {
      font-size: clamp(1.75rem, 3vw, 2.5rem);
      color: var(--card-text-primary);
      margin-bottom: 16px;
      letter-spacing: -0.02em;
    }

    .hero-body p {
      font-size: 1rem;
      color: var(--card-text-secondary);
      margin-bottom: 32px;
      line-height: 1.65;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-family: 'DM Sans', sans-serif;
      font-weight: 600;
      font-size: 0.9rem;
      padding: 12px 28px;
      border-radius: var(--card-radius-sm);
      border: none;
      cursor: pointer;
      text-decoration: none;
      transition: background var(--card-transition), box-shadow var(--card-transition), transform var(--card-transition);
    }

    .btn--primary {
      background: var(--card-action-blue);
      color: #ffffff;
    }

    .btn--primary:hover {
      background: var(--card-action-hover);
      box-shadow: 0 4px 12px rgba(0,113,227,0.3);
      transform: translateY(-1px);
    }

    .btn--secondary {
      background: transparent;
      color: var(--card-action-blue);
      border: 1.5px solid var(--card-border-light);
      margin-left: 12px;
    }

    .btn--secondary:hover {
      border-color: var(--card-action-blue);
      background: rgba(0,113,227,0.04);
    }

    /* Filter Chips */
    .filters {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 32px 32px;
    }

    .chip {
      font-family: 'Inter', sans-serif;
      font-size: 0.825rem;
      font-weight: 500;
      padding: 8px 18px;
      border-radius: 100px;
      border: 1.5px solid var(--card-border-light);
      background: var(--card-bg-surface);
      color: var(--card-text-secondary);
      cursor: pointer;
      transition: background var(--card-transition), border-color var(--card-transition), color var(--card-transition);
    }

    .chip:hover {
      border-color: var(--card-action-blue);
      color: var(--card-action-blue);
    }

    .chip--active {
      background: var(--card-action-blue);
      border-color: var(--card-action-blue);
      color: #ffffff;
    }

    /* Section headings */
    .section-header {
      max-width: 1200px;
      margin: 0 auto;
      padding: 48px 32px 24px;
    }

    .section-header h2 {
      font-size: 1.5rem;
      color: var(--card-text-primary);
    }

    .section-header p {
      font-size: 0.95rem;
      color: var(--card-text-secondary);
      margin-top: 6px;
    }

    /* Card Grid */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: var(--card-gap);
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 32px 48px;
    }

    .card {
      background: var(--card-bg-surface);
      border-radius: var(--card-radius-md);
      box-shadow: var(--card-shadow-md);
      overflow: hidden;
      display: flex;
      flex-direction: column;
      transition: transform var(--card-transition), box-shadow var(--card-transition);
      cursor: pointer;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow: var(--card-shadow-lg);
    }

    .card-img {
      width: 100%;
      aspect-ratio: 16 / 9;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      color: rgba(255,255,255,0.4);
    }

    .card-body {
      padding: var(--card-padding);
      flex: 1;
      display: flex;
      flex-direction: column;
    }

    .card-cat {
      font-size: 0.7rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      color: var(--card-action-blue);
      margin-bottom: 8px;
    }

    .card-body h3 {
      font-size: 1.1rem;
      margin-bottom: 8px;
      line-height: 1.35;
    }

    .card-body p {
      font-size: 0.9rem;
      color: var(--card-text-secondary);
      line-height: 1.6;
      flex: 1;
      display: -webkit-box;
      -webkit-line-clamp: 3;
      -webkit-box-orient: vertical;
      overflow: hidden;
    }

    .card-footer {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding-top: 16px;
      margin-top: 16px;
      border-top: 1px solid var(--card-border-light);
      font-size: 0.8rem;
      color: var(--card-text-tertiary);
    }

    .card-footer a {
      font-family: 'DM Sans', sans-serif;
      font-weight: 600;
      font-size: 0.825rem;
      color: var(--card-action-blue);
      text-decoration: none;
    }

    .card-footer a:hover {
      color: var(--card-action-hover);
    }

    /* Masonry Section */
    .masonry {
      column-count: 3;
      column-gap: var(--card-gap);
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 32px 48px;
    }

    .masonry .card {
      break-inside: avoid;
      margin-bottom: var(--card-gap);
      display: inline-block;
      width: 100%;
    }

    .masonry .card-img {
      aspect-ratio: auto;
      min-height: 120px;
    }

    /* Carousel */
    .carousel-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 48px 32px 24px;
    }

    .carousel-header h2 {
      font-size: 1.5rem;
      color: var(--card-text-primary);
    }

    .carousel-controls {
      display: flex;
      gap: 8px;
    }

    .carousel-btn {
      width: 38px;
      height: 38px;
      border-radius: 50%;
      border: 1.5px solid var(--card-border-light);
      background: var(--card-bg-surface);
      cursor: pointer;
      font-size: 1rem;
      color: var(--card-text-secondary);
      display: flex;
      align-items: center;
      justify-content: center;
      transition: border-color var(--card-transition), color var(--card-transition);
    }

    .carousel-btn:hover {
      border-color: var(--card-action-blue);
      color: var(--card-action-blue);
    }

    .carousel-track {
      display: flex;
      gap: var(--card-gap);
      overflow-x: auto;
      scroll-snap-type: x mandatory;
      scroll-behavior: smooth;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 32px 48px;
      -ms-overflow-style: none;
      scrollbar-width: none;
    }

    .carousel-track::-webkit-scrollbar { display: none; }

    .carousel-track .card {
      flex: 0 0 280px;
      scroll-snap-align: start;
    }

    /* CTA Banner */
    .cta-banner {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 32px 48px;
    }

    .cta-card {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      border-radius: var(--card-radius-lg);
      padding: 64px;
      text-align: center;
      color: #ffffff;
    }

    .cta-card h2 {
      font-size: clamp(1.5rem, 3vw, 2.25rem);
      color: #ffffff;
      margin-bottom: 12px;
    }

    .cta-card p {
      font-size: 1.05rem;
      color: rgba(255,255,255,0.8);
      margin-bottom: 32px;
      max-width: 520px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn--white {
      background: #ffffff;
      color: #764ba2;
      font-family: 'DM Sans', sans-serif;
      font-weight: 600;
      font-size: 0.9rem;
      padding: 14px 32px;
      border-radius: var(--card-radius-sm);
      border: none;
      cursor: pointer;
      text-decoration: none;
      transition: box-shadow var(--card-transition), transform var(--card-transition);
    }

    .btn--white:hover {
      box-shadow: 0 6px 20px rgba(0,0,0,0.2);
      transform: translateY(-2px);
    }

    /* Footer */
    footer {
      background: var(--card-bg-surface);
      border-top: 1px solid var(--card-border-light);
    }

    .footer-inner {
      max-width: 1200px;
      margin: 0 auto;
      padding: 40px 32px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .footer-brand {
      font-family: 'DM Sans', sans-serif;
      font-weight: 700;
      font-size: 1.1rem;
      color: var(--card-text-primary);
    }

    .footer-links {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    .footer-links a {
      font-size: 0.85rem;
      color: var(--card-text-secondary);
      text-decoration: none;
    }

    .footer-links a:hover {
      color: var(--card-text-primary);
    }

    .footer-copy {
      font-size: 0.8rem;
      color: var(--card-text-tertiary);
      text-align: center;
      padding: 0 32px 24px;
      max-width: 1200px;
      margin: 0 auto;
    }

    /* Responsive */
    @media (max-width: 768px) {
      nav { padding: 14px 20px; }
      nav ul { gap: 20px; }
      .hero { padding: 40px 20px 32px; }
      .hero-card { grid-template-columns: 1fr; }
      .hero-image { min-height: 200px; }
      .hero-body { padding: 32px; }
      .card-grid { padding: 0 20px 32px; }
      .masonry { column-count: 1; padding: 0 20px 32px; }
      .carousel-track .card { flex: 0 0 85vw; }
      .cta-card { padding: 40px 24px; }
      .filters { padding: 0 20px 24px; }
      .section-header { padding: 32px 20px 16px; }
      .carousel-header { padding: 32px 20px 16px; }
      .carousel-track { padding: 0 20px 32px; }
      .cta-banner { padding: 0 20px 32px; }
      .footer-inner { flex-direction: column; gap: 16px; text-align: center; padding: 32px 20px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Cardfolio</a>
    <ul>
      <li><a href="#">Explore</a></li>
      <li><a href="#">Collections</a></li>
      <li><a href="#">Trending</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="hero-card">
      <div class="hero-image">&#9670;</div>
      <div class="hero-body">
        <span class="hero-label">Featured Collection</span>
        <h1>Discover Curated Content</h1>
        <p>Browse through beautifully organized cards. Every piece of content has its own space, making discovery effortless and delightful.</p>
        <div>
          <a href="#" class="btn btn--primary">Get Started</a>
          <a href="#" class="btn btn--secondary">Learn More</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Filters -->
  <div class="filters">
    <button class="chip chip--active">All</button>
    <button class="chip">Design</button>
    <button class="chip">Development</button>
    <button class="chip">Photography</button>
    <button class="chip">Illustration</button>
    <button class="chip">Typography</button>
  </div>

  <!-- Uniform Card Grid -->
  <section class="card-grid">
    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);">&#9733;</div>
      <div class="card-body">
        <span class="card-cat">Design</span>
        <h3>Principles of Visual Hierarchy</h3>
        <p>Learn how size, color, and spacing guide the viewer's eye through a composition to create clear communication.</p>
        <div class="card-footer">
          <span>5 min read</span>
          <a href="#">Read More &rarr;</a>
        </div>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);">&#9830;</div>
      <div class="card-body">
        <span class="card-cat">Development</span>
        <h3>Building Responsive Grid Systems</h3>
        <p>A practical guide to CSS Grid and Flexbox patterns that adapt beautifully across every device and screen size.</p>
        <div class="card-footer">
          <span>8 min read</span>
          <a href="#">Read More &rarr;</a>
        </div>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);">&#9827;</div>
      <div class="card-body">
        <span class="card-cat">Photography</span>
        <h3>Composition and the Rule of Thirds</h3>
        <p>Discover how professional photographers use compositional grids to create balanced and compelling images.</p>
        <div class="card-footer">
          <span>4 min read</span>
          <a href="#">Read More &rarr;</a>
        </div>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #fa709a 0%, #fee140 100%);">&#9824;</div>
      <div class="card-body">
        <span class="card-cat">Illustration</span>
        <h3>Color Theory for Digital Artists</h3>
        <p>Understanding warm and cool color relationships, contrast ratios, and accessible palettes for screen-based work.</p>
        <div class="card-footer">
          <span>6 min read</span>
          <a href="#">Read More &rarr;</a>
        </div>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #a18cd1 0%, #fbc2eb 100%);">&#10022;</div>
      <div class="card-body">
        <span class="card-cat">Typography</span>
        <h3>The Art of Font Pairing</h3>
        <p>How to combine typefaces for contrast and harmony, from classic serif-sans pairings to modern geometric combinations.</p>
        <div class="card-footer">
          <span>7 min read</span>
          <a href="#">Read More &rarr;</a>
        </div>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);">&#9672;</div>
      <div class="card-body">
        <span class="card-cat">Design</span>
        <h3>White Space as a Design Element</h3>
        <p>Why the empty areas of your layout are just as important as the content they surround and how to use them with purpose.</p>
        <div class="card-footer">
          <span>3 min read</span>
          <a href="#">Read More &rarr;</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Masonry Section -->
  <div class="section-header">
    <h2>Masonry Collection</h2>
    <p>Variable-height cards in a Pinterest-style waterfall layout.</p>
  </div>

  <section class="masonry">
    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); min-height: 200px;">&#9670;</div>
      <div class="card-body">
        <span class="card-cat">Design</span>
        <h3>Layout Fundamentals</h3>
        <p>Exploring the building blocks of page structure.</p>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); min-height: 280px;">&#9733;</div>
      <div class="card-body">
        <span class="card-cat">Photography</span>
        <h3>Golden Hour Techniques</h3>
        <p>Capture the warm, soft light that makes outdoor photographs feel magical. Tips on timing, exposure, and composition during the golden hour window.</p>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%); min-height: 160px;">&#9830;</div>
      <div class="card-body">
        <span class="card-cat">Development</span>
        <h3>CSS Grid Tricks</h3>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%); min-height: 240px;">&#9827;</div>
      <div class="card-body">
        <span class="card-cat">Illustration</span>
        <h3>Geometric Abstraction</h3>
        <p>Using simple shapes to create complex visual narratives that communicate ideas without words.</p>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #fa709a 0%, #fee140 100%); min-height: 180px;">&#9824;</div>
      <div class="card-body">
        <span class="card-cat">Typography</span>
        <h3>Variable Fonts in Action</h3>
        <p>How a single font file can replace dozens of weights and styles.</p>
      </div>
    </div>

    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #a18cd1 0%, #fbc2eb 100%); min-height: 300px;">&#10022;</div>
      <div class="card-body">
        <span class="card-cat">Design</span>
        <h3>Designing for Accessibility</h3>
        <p>Inclusive design practices that ensure your interfaces are usable by everyone, regardless of ability or assistive technology. Color contrast, keyboard navigation, and semantic markup all play critical roles.</p>
      </div>
    </div>
  </section>

  <!-- Carousel -->
  <div class="carousel-header">
    <h2>Trending Now</h2>
    <div class="carousel-controls">
      <button class="carousel-btn">&larr;</button>
      <button class="carousel-btn">&rarr;</button>
    </div>
  </div>

  <div class="carousel-track">
    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%); aspect-ratio: 4/3;">&#9672;</div>
      <div class="card-body">
        <span class="card-cat">Trending</span>
        <h3>Micro-interactions Guide</h3>
        <p>Small animations that make big differences in user experience.</p>
      </div>
    </div>
    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #d4fc79 0%, #96e6a1 100%); aspect-ratio: 4/3;">&#9670;</div>
      <div class="card-body">
        <span class="card-cat">Trending</span>
        <h3>Design Tokens Explained</h3>
        <p>The building blocks of scalable design systems.</p>
      </div>
    </div>
    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #84fab0 0%, #8fd3f4 100%); aspect-ratio: 4/3;">&#9733;</div>
      <div class="card-body">
        <span class="card-cat">Trending</span>
        <h3>AI in UI Design</h3>
        <p>How artificial intelligence is transforming interface design workflows.</p>
      </div>
    </div>
    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #cfd9df 0%, #e2ebf0 100%); aspect-ratio: 4/3;">&#9830;</div>
      <div class="card-body">
        <span class="card-cat">Trending</span>
        <h3>Minimalism in 2026</h3>
        <p>The evolution of less-is-more in modern web design.</p>
      </div>
    </div>
    <div class="card">
      <div class="card-img" style="background: linear-gradient(135deg, #fccb90 0%, #d57eeb 100%); aspect-ratio: 4/3;">&#9827;</div>
      <div class="card-body">
        <span class="card-cat">Trending</span>
        <h3>Container Queries Deep Dive</h3>
        <p>Responsive components that adapt to their parent, not the viewport.</p>
      </div>
    </div>
  </div>

  <!-- CTA -->
  <div class="cta-banner">
    <div class="cta-card">
      <h2>Start Building with Cards</h2>
      <p>Modular, responsive, and endlessly adaptable. Card-based design is the foundation of modern interfaces.</p>
      <a href="#" class="btn--white">Create Your Collection</a>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <div class="footer-inner">
      <span class="footer-brand">Cardfolio</span>
      <ul class="footer-links">
        <li><a href="#">Terms</a></li>
        <li><a href="#">Privacy</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">GitHub</a></li>
      </ul>
    </div>
    <p class="footer-copy">Designed with modular thinking. Every card tells a story.</p>
  </footer>
</body>
</html>
```
