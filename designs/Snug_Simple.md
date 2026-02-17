# Snug Simple -- Design Reference

Snug Simple is a cozy, human-centered web design aesthetic that prioritizes warmth, approachability, and intentional simplicity. It is the anti-corporate antidote -- rounded everything, soft pastels, chunky typography, and generous spacing that says "slow down, be comfortable." Born from the intersection of Scandinavian hygge culture, indie web design, and the growing desire for digital spaces that feel like a warm blanket rather than a sterile dashboard, Snug Simple treats every pixel as an opportunity to make the user feel at home. The visual language is deliberately friendly: large border-radius values soften every edge, muted pastel palettes soothe the eyes, bold rounded typefaces feel like handwritten notes from a friend, and abundant whitespace lets content breathe. This is design as a friendly digital companion -- never shouting, never demanding, just quietly present and comforting.

---

## Visual Characteristics

- **Large border-radius everywhere** -- cards, buttons, images, and containers all use generous rounding (16-32px), creating a soft, pillow-like feel across the entire interface
- **Muted pastel color palette** -- sage greens, blush pinks, warm creams, soft lavenders, and dusty roses form the primary palette, never saturated or harsh
- **Chunky bold typography** -- rounded sans-serif typefaces at large sizes with heavy weights (600-800) convey warmth and friendliness without aggression
- **Generous spacing and padding** -- elements breathe with ample margins (2-4rem) and padding (1.5-3rem), resisting the urge to cram content
- **Simple single-column or two-column layouts** -- content flows naturally without complex grid systems or overwhelming information density
- **Soft warm shadows** -- subtle box-shadows with warm color tints replace harsh drop shadows, creating gentle depth
- **Pill-shaped interactive elements** -- buttons, tags, and badges use fully rounded (border-radius: 999px) shapes for a friendly, approachable feel
- **Light paper-like textures** -- subtle off-white and cream backgrounds with gentle grain or noise create tactile warmth
- **Cozy card components** -- content blocks wrapped in softly rounded, lightly bordered cards that feel like sticky notes or recipe cards
- **Playful rounded icons** -- simple, chunky icon styles with rounded strokes and filled shapes rather than thin outlines
- **Subtle warm gradients** -- gentle transitions between adjacent pastels add depth without visual noise
- **Friendly illustration style** -- hand-drawn or softly rendered illustrations with imperfect lines and warm color fills
- **Warm color temperature throughout** -- even neutrals lean warm (oat, cream, warm gray) rather than cool (blue-gray, silver)
- **Minimal decorative complexity** -- ornamentation is limited to soft color blocks, gentle curves, and simple shapes; no sharp angles or intricate patterns

---

## Color Palette

The Snug Simple palette draws from nature's softest moments -- morning light through linen curtains, spring wildflowers, oatmeal in a ceramic bowl, lavender fields at dusk:

- **Warm cream and oat tones** form the background foundation, never stark white
- **Sage green** provides a grounding natural accent, evoking houseplants and herb gardens
- **Blush pink and dusty rose** add gentle warmth and a subtle playfulness
- **Soft lavender** offers a calming cool-leaning accent that still feels warm in context
- **Warm earth tones** for text -- deep brown and espresso rather than pure black, maintaining softness even at high contrast
- **Light sky blue** as a secondary accent for informational elements and links
- **All colors at 30-60% saturation** -- fully saturated colors are avoided; everything should look as if viewed through a light linen curtain
- **Warm neutrals bridge all accent colors** -- oat, warm sand, and soft taupe connect the palette harmoniously

### Suggested Implementation Palette

Based on characteristic Snug Simple warmth and softness:

| Role              | Color           | Hex       |
|-------------------|-----------------|-----------|
| Background Base   | Warm Cream      | `#FFF8F0` |
| Background Alt    | Soft Oat        | `#F5EDE3` |
| Surface Card      | White Linen     | `#FFFFFF` |
| Surface Tinted    | Blush Whisper   | `#FFF0F0` |
| Primary Text      | Espresso Brown  | `#3D3028` |
| Secondary Text    | Warm Umber      | `#5C4A3A` |
| Muted Text        | Soft Clay       | `#9B8A7A` |
| Accent Sage       | Sage Green      | `#B8C9A3` |
| Accent Sage Dark  | Deep Sage       | `#8FAF78` |
| Accent Blush      | Blush Pink      | `#E8B4B8` |
| Accent Rose       | Dusty Rose      | `#D4A0A8` |
| Accent Lavender   | Soft Lavender   | `#C5B8D9` |
| Accent Sky        | Light Sky       | `#B8D4E8` |
| Accent Oat        | Warm Oat        | `#E8DCD0` |
| Border Soft       | Pale Blush      | `#E8D8D0` |
| Shadow Warm       | Tinted Shadow   | `#D4C4B8` |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --snug-bg-base: #FFF8F0;
  --snug-bg-alt: #F5EDE3;
  --snug-bg-card: #FFFFFF;
  --snug-bg-tinted: #FFF0F0;
  --snug-bg-sage: #EEF4E8;
  --snug-bg-lavender: #F0ECF5;

  /* Text */
  --snug-text-primary: #3D3028;
  --snug-text-secondary: #5C4A3A;
  --snug-text-muted: #9B8A7A;
  --snug-text-inverse: #FFFFFF;

  /* Accents */
  --snug-accent-sage: #B8C9A3;
  --snug-accent-sage-dark: #8FAF78;
  --snug-accent-blush: #E8B4B8;
  --snug-accent-rose: #D4A0A8;
  --snug-accent-lavender: #C5B8D9;
  --snug-accent-sky: #B8D4E8;
  --snug-accent-oat: #E8DCD0;
  --snug-accent-peach: #F0D0B8;

  /* Borders */
  --snug-border-soft: #E8D8D0;
  --snug-border-sage: #C8D8B8;
  --snug-border-blush: #E8C8CC;
  --snug-border-lavender: #D0C8E0;

  /* Shadows */
  --snug-shadow-warm: rgba(180, 160, 140, 0.15);
  --snug-shadow-blush: rgba(212, 160, 168, 0.12);
  --snug-shadow-sage: rgba(143, 175, 120, 0.12);

  /* Functional mappings */
  --snug-bg-primary: var(--snug-bg-base);
  --snug-bg-secondary: var(--snug-bg-alt);
  --snug-text-heading: var(--snug-text-primary);
  --snug-text-body: var(--snug-text-secondary);
  --snug-accent-primary: var(--snug-accent-sage);
  --snug-accent-secondary: var(--snug-accent-blush);
  --snug-border: var(--snug-border-soft);
  --snug-radius-sm: 12px;
  --snug-radius-md: 20px;
  --snug-radius-lg: 28px;
  --snug-radius-pill: 999px;
}
```

---

## Typography

### Typeface Characteristics

Snug Simple typography is defined by friendliness and readability -- every letterform should feel like it is smiling:

- **Rounded sans-serif typefaces** -- the defining typographic choice; letter terminals are rounded rather than squared, softening every word
- **Chunky bold weights** -- headings use 700-800 weight for warmth and visual presence without aggression
- **Large comfortable sizes** -- body text at 17-18px, headings generously scaled, nothing feels cramped
- **Generous line-height** -- 1.7 to 2.0 for body text, creating airy readable paragraphs that do not feel dense
- **Slightly positive letter-spacing** -- a touch of extra tracking (0.01-0.03em) on body text keeps things open and friendly
- **No uppercase headings** -- sentence case or title case only; all-caps feels too aggressive for this aesthetic
- **Warm brown text color** -- deep espresso or umber replaces pure black, maintaining softness even at full contrast
- **Playful display fonts for emphasis** -- optional use of bouncy or handwritten-style fonts for callouts and decorative text
- **Comfortable reading rhythm** -- paragraphs are short, sentences are clear, and typography never demands effort

### Recommended Web Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Quicksand** | Rounded geometric sans-serif | Primary headings -- the quintessential snug typeface with perfectly rounded terminals |
| **Nunito** | Rounded neo-grotesque sans-serif | Body text -- excellent readability with soft rounded forms at all sizes |
| **Comfortaa** | Rounded geometric display | Display headings, hero text -- wide and friendly with distinctive round geometry |
| **Baloo 2** | Chunky rounded display | Accent headings, callouts -- playful and bold with a hand-crafted feel |
| **Varela Round** | Rounded grotesque | Secondary text, UI labels -- clean and friendly at small sizes |
| **DM Sans** | Humanist sans-serif | Body text alternative -- slightly more structured while remaining warm |
| **Poppins** | Geometric sans-serif | UI elements, buttons -- clean and modern with rounded geometric forms |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&family=Nunito:wght@400;500;600;700;800&family=Comfortaa:wght@400;600;700&family=Baloo+2:wght@500;600;700;800&display=swap');

/* Primary body text -- warm, readable, friendly */
body {
  font-family: 'Nunito', 'Quicksand', -apple-system, sans-serif;
  font-size: 17px;
  line-height: 1.8;
  letter-spacing: 0.01em;
  color: var(--snug-text-primary);
  font-weight: 400;
  -webkit-font-smoothing: antialiased;
}

/* Headings -- chunky, rounded, warm */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Quicksand', 'Comfortaa', sans-serif;
  color: var(--snug-text-heading);
  font-weight: 700;
  letter-spacing: 0.01em;
  line-height: 1.3;
}

h1 {
  font-size: clamp(2rem, 5vw, 3rem);
  font-weight: 800;
  margin-bottom: 1rem;
}

h2 {
  font-size: clamp(1.5rem, 3.5vw, 2.2rem);
  font-weight: 700;
  margin-bottom: 0.8rem;
  color: var(--snug-accent-sage-dark);
}

h3 {
  font-size: clamp(1.2rem, 2.5vw, 1.6rem);
  font-weight: 600;
  margin-bottom: 0.6rem;
  color: var(--snug-accent-rose);
}

/* Paragraph text -- comfortable reading */
p {
  margin-bottom: 1.2rem;
  color: var(--snug-text-secondary);
  line-height: 1.8;
  max-width: 65ch;
}

/* Display text -- playful emphasis for hero areas */
.snug-display {
  font-family: 'Comfortaa', 'Quicksand', sans-serif;
  font-size: clamp(2.5rem, 6vw, 4rem);
  font-weight: 700;
  color: var(--snug-text-primary);
  line-height: 1.2;
  letter-spacing: -0.01em;
}

/* Accent callout text */
.snug-callout {
  font-family: 'Baloo 2', 'Quicksand', sans-serif;
  font-size: 1.1rem;
  font-weight: 600;
  color: var(--snug-accent-sage-dark);
  letter-spacing: 0.02em;
}

/* Small friendly labels */
.snug-label {
  font-family: 'Quicksand', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  color: var(--snug-text-muted);
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

/* Monospace for code or data (still friendly) */
.snug-mono {
  font-family: 'JetBrains Mono', 'Fira Code', monospace;
  font-size: 0.9em;
  color: var(--snug-accent-sage-dark);
  background: var(--snug-bg-sage);
  padding: 0.15em 0.4em;
  border-radius: var(--snug-radius-sm);
}
```

---

## Key Design Elements and Motifs

### Rounded Cards

The foundational layout element of Snug Simple -- softly rounded containers that organize content like sticky notes on a friendly bulletin board:

- **Large border-radius** (20-28px) on all card containers
- **Subtle warm shadows** that lift cards gently off the background without harsh contrast
- **Light or white backgrounds** with optional pastel tinting (blush, sage, lavender washes)
- **Generous internal padding** (1.5-2.5rem) so content never feels cramped
- **Thin soft borders** in warm tones (1px solid) rather than relying solely on shadows
- **Gentle hover transitions** -- slight lift and shadow expansion on interaction

### Pill Buttons and Tags

- **Fully rounded buttons** (border-radius: 999px) with pastel backgrounds and bold text
- **Chunky padding** -- horizontal padding 1.5-2.5rem, vertical 0.7-1rem for a substantial feel
- **Pastel background fills** that shift to slightly darker tones on hover
- **No sharp outlines** -- borders match or are slightly darker than the fill color
- **Tags and badges** as small pills with muted pastel backgrounds and dark text
- **Gentle scale transform on hover** (1.02-1.05) for playful micro-interaction

### Cozy Color Blocks

- **Full-width pastel background sections** that alternate between cream, sage, blush, and lavender
- **Soft transitions between sections** using subtle gradient fades or gentle wave dividers
- **Color blocks used for emphasis** rather than borders or lines -- a sage-tinted block for tips, a blush block for highlights
- **Pastel accent bars** on the left side of callout boxes (4-6px wide, rounded top and bottom)

### Friendly Icons and Illustrations

- **Rounded stroke icons** with 2-3px stroke width, matching the chunky type aesthetic
- **Filled icon variants** with pastel backgrounds and darker strokes
- **Simple hand-drawn-style illustrations** -- imperfect circles, wobbly lines, warm fills
- **Icon containers** as rounded squares or circles with pastel background fills
- **Emoji as design elements** -- used sparingly in headings or callouts for instant warmth

### Subtle Background Textures

- **Light dot patterns** at very low opacity (3-8%) for tactile paper-like feel
- **Subtle grain/noise overlays** that add organic warmth to flat pastel surfaces
- **Soft grid patterns** barely visible in the background, suggesting graph paper or fabric weave
- **Minimal use** -- textures should be felt rather than seen; if they draw attention, they are too strong

### Generous Whitespace

- **Section margins of 4-6rem** between major content blocks
- **Card margins of 1.5-2rem** between adjacent cards
- **Internal padding of 2-3rem** within containers
- **Line-height of 1.7-2.0** for all body text
- **Max-width constraints** (600-700px for text, 1100px for overall layout) preventing content from stretching too wide

---

## Layout Principles

- **Single-column or simple two-column layouts** -- complexity is the enemy of coziness; grid systems are kept minimal
- **Centered content containers** with comfortable max-widths (1000-1200px), never edge-to-edge
- **Card-based content organization** -- information grouped into discrete, rounded, softly contained blocks
- **Vertical rhythm through generous spacing** -- sections breathe with 4-6rem gaps
- **Asymmetric two-column layouts** where the secondary column is narrower (sidebar for context, main for content)
- **Stacked mobile layout** -- columns collapse gracefully; the single-column mobile view is the purest expression of the aesthetic
- **No hard dividers** -- sections separated by whitespace and alternating pastel background colors rather than lines
- **Content max-width for readability** -- text paragraphs never exceed 65ch for comfortable reading
- **Sticky-but-subtle navigation** -- if navigation is fixed, it uses a soft frosted-glass effect with pastel tint
- **Footer as a cozy landing zone** -- the bottom of the page mirrors the top in warmth, often with a slightly darker pastel background

### Modern Web Adaptation

- Use the **card pattern extensively** -- every content group becomes a rounded, padded, softly shadowed card
- **Alternating pastel section backgrounds** create visual rhythm without harsh dividers
- **Pill-shaped navigation items** and CTAs feel touchable and friendly
- **Large click/tap targets** -- minimum 48px height for interactive elements, generously padded
- **Frosted glass effects** (backdrop-filter) on overlays and sticky headers add depth while maintaining lightness
- **Scroll-triggered animations** should be gentle: fade-in and slight upward float, never bounce or snap
- **Dark mode adaptation** -- warm dark backgrounds (not pure black) with pastel accents at reduced saturation; maintain the cozy feeling

---

## CSS/Design Techniques

### Rounded Card Component

```css
/* The fundamental Snug Simple building block */
.snug-card {
  background: var(--snug-bg-card);
  border: 1px solid var(--snug-border-soft);
  border-radius: var(--snug-radius-lg);
  padding: 2rem 2.2rem;
  box-shadow:
    0 2px 8px var(--snug-shadow-warm),
    0 1px 3px rgba(180, 160, 140, 0.08);
  transition: all 0.3s ease;
}

/* Hover: gentle lift */
.snug-card:hover {
  transform: translateY(-3px);
  box-shadow:
    0 8px 24px var(--snug-shadow-warm),
    0 2px 6px rgba(180, 160, 140, 0.1);
}

/* Tinted card variants */
.snug-card--sage {
  background: var(--snug-bg-sage);
  border-color: var(--snug-border-sage);
}

.snug-card--blush {
  background: var(--snug-bg-tinted);
  border-color: var(--snug-border-blush);
}

.snug-card--lavender {
  background: var(--snug-bg-lavender);
  border-color: var(--snug-border-lavender);
}
```

### Pill Buttons

```css
/* Primary pill button -- the friendliest CTA */
.snug-button {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.75rem 2rem;
  background: var(--snug-accent-sage);
  color: var(--snug-text-primary);
  border: 2px solid transparent;
  border-radius: var(--snug-radius-pill);
  font-family: 'Quicksand', sans-serif;
  font-size: 1rem;
  font-weight: 700;
  letter-spacing: 0.02em;
  text-decoration: none;
  cursor: pointer;
  transition: all 0.25s ease;
}

.snug-button:hover {
  background: var(--snug-accent-sage-dark);
  color: var(--snug-text-inverse);
  transform: scale(1.03);
  box-shadow: 0 4px 16px var(--snug-shadow-sage);
}

.snug-button:active {
  transform: scale(0.98);
}

/* Secondary / outlined variant */
.snug-button--outline {
  background: transparent;
  border-color: var(--snug-accent-sage);
  color: var(--snug-accent-sage-dark);
}

.snug-button--outline:hover {
  background: var(--snug-accent-sage);
  color: var(--snug-text-primary);
}

/* Blush variant */
.snug-button--blush {
  background: var(--snug-accent-blush);
  color: var(--snug-text-primary);
}

.snug-button--blush:hover {
  background: var(--snug-accent-rose);
  color: var(--snug-text-inverse);
  box-shadow: 0 4px 16px var(--snug-shadow-blush);
}

/* Small button for inline actions */
.snug-button--sm {
  padding: 0.45rem 1.2rem;
  font-size: 0.85rem;
  font-weight: 600;
}
```

### Pill Tags and Badges

```css
/* Small pastel pill tags */
.snug-tag {
  display: inline-flex;
  align-items: center;
  padding: 0.3rem 0.9rem;
  background: var(--snug-bg-sage);
  color: var(--snug-accent-sage-dark);
  border-radius: var(--snug-radius-pill);
  font-family: 'Quicksand', sans-serif;
  font-size: 0.78rem;
  font-weight: 600;
  letter-spacing: 0.02em;
  white-space: nowrap;
}

.snug-tag--blush {
  background: var(--snug-bg-tinted);
  color: var(--snug-accent-rose);
}

.snug-tag--lavender {
  background: var(--snug-bg-lavender);
  color: #7B6B9A;
}

.snug-tag--sky {
  background: #EDF4F8;
  color: #5A8AA8;
}

/* Badge with dot indicator */
.snug-badge {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  padding: 0.35rem 1rem;
  background: var(--snug-bg-card);
  border: 1px solid var(--snug-border-soft);
  border-radius: var(--snug-radius-pill);
  font-family: 'Nunito', sans-serif;
  font-size: 0.82rem;
  font-weight: 600;
  color: var(--snug-text-secondary);
}

.snug-badge::before {
  content: '';
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--snug-accent-sage);
}
```

### Cozy Callout Box

```css
/* Callout box with pastel accent bar */
.snug-callout-box {
  background: var(--snug-bg-sage);
  border-left: 5px solid var(--snug-accent-sage);
  border-radius: 0 var(--snug-radius-md) var(--snug-radius-md) 0;
  padding: 1.5rem 2rem;
  margin: 1.5rem 0;
}

.snug-callout-box--blush {
  background: var(--snug-bg-tinted);
  border-left-color: var(--snug-accent-blush);
}

.snug-callout-box--lavender {
  background: var(--snug-bg-lavender);
  border-left-color: var(--snug-accent-lavender);
}

.snug-callout-box p {
  margin-bottom: 0;
  color: var(--snug-text-secondary);
  font-weight: 500;
}

/* Fully rounded callout (alternative) */
.snug-callout-rounded {
  background: var(--snug-bg-card);
  border: 2px solid var(--snug-accent-sage);
  border-radius: var(--snug-radius-lg);
  padding: 1.8rem 2rem;
  margin: 1.5rem 0;
  display: flex;
  gap: 1rem;
  align-items: flex-start;
}

.snug-callout-rounded .callout-icon {
  flex-shrink: 0;
  width: 44px;
  height: 44px;
  background: var(--snug-bg-sage);
  border-radius: var(--snug-radius-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.3rem;
}
```

### Subtle Background Textures

```css
/* Soft dot pattern -- barely perceptible tactile quality */
.snug-texture-dots {
  background-image: radial-gradient(
    circle at 1px 1px,
    var(--snug-text-muted) 0.5px,
    transparent 0.5px
  );
  background-size: 20px 20px;
  background-color: var(--snug-bg-base);
}

/* Reduce dot visibility to a whisper */
.snug-texture-dots::before {
  content: '';
  position: absolute;
  inset: 0;
  background: inherit;
  opacity: 0.04;
  pointer-events: none;
}

/* Soft grid pattern for structured sections */
.snug-texture-grid {
  background-image:
    linear-gradient(var(--snug-border-soft) 1px, transparent 1px),
    linear-gradient(90deg, var(--snug-border-soft) 1px, transparent 1px);
  background-size: 40px 40px;
  background-color: var(--snug-bg-base);
}

/* Paper grain noise (use with a noise SVG or CSS paint) */
.snug-texture-grain {
  position: relative;
}

.snug-texture-grain::after {
  content: '';
  position: absolute;
  inset: 0;
  opacity: 0.03;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='1'/%3E%3C/svg%3E");
  background-repeat: repeat;
  background-size: 256px 256px;
  pointer-events: none;
  mix-blend-mode: multiply;
}
```

### Alternating Section Backgrounds

```css
/* Alternating pastel sections for page rhythm */
.snug-section {
  padding: 4rem 2rem;
}

.snug-section--cream {
  background: var(--snug-bg-base);
}

.snug-section--oat {
  background: var(--snug-bg-alt);
}

.snug-section--sage {
  background: var(--snug-bg-sage);
}

.snug-section--blush {
  background: var(--snug-bg-tinted);
}

.snug-section--lavender {
  background: var(--snug-bg-lavender);
}

/* Soft wave divider between sections */
.snug-divider-wave {
  width: 100%;
  height: 40px;
  background: var(--snug-bg-base);
  clip-path: ellipse(55% 100% at 50% 0%);
  margin-top: -40px;
  position: relative;
  z-index: 1;
}
```

### Frosted Glass Header

```css
/* Sticky navigation with cozy frosted effect */
.snug-header {
  position: sticky;
  top: 0;
  z-index: 100;
  padding: 0.8rem 2rem;
  background: rgba(255, 248, 240, 0.85);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--snug-border-soft);
  box-shadow: 0 1px 8px var(--snug-shadow-warm);
}

/* Nav items as rounded pills */
.snug-nav-item {
  display: inline-flex;
  align-items: center;
  padding: 0.5rem 1.2rem;
  border-radius: var(--snug-radius-pill);
  font-family: 'Quicksand', sans-serif;
  font-size: 0.9rem;
  font-weight: 600;
  color: var(--snug-text-secondary);
  text-decoration: none;
  transition: all 0.2s ease;
}

.snug-nav-item:hover {
  background: var(--snug-bg-alt);
  color: var(--snug-text-primary);
}

.snug-nav-item--active {
  background: var(--snug-accent-sage);
  color: var(--snug-text-primary);
}
```

### Gentle Hover and Interaction Effects

```css
/* Gentle lift on hoverable elements */
.snug-hover-lift {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.snug-hover-lift:hover {
  transform: translateY(-4px);
  box-shadow: 0 10px 30px var(--snug-shadow-warm);
}

/* Subtle scale for buttons and interactive pills */
.snug-hover-grow {
  transition: transform 0.2s ease;
}

.snug-hover-grow:hover {
  transform: scale(1.04);
}

/* Warm color shift on links */
a {
  color: var(--snug-accent-sage-dark);
  text-decoration: underline;
  text-decoration-color: var(--snug-accent-sage);
  text-underline-offset: 3px;
  text-decoration-thickness: 2px;
  transition: color 0.2s ease, text-decoration-color 0.2s ease;
}

a:hover {
  color: var(--snug-accent-rose);
  text-decoration-color: var(--snug-accent-rose);
}

/* Focus ring -- visible and friendly */
:focus-visible {
  outline: 3px solid var(--snug-accent-sage);
  outline-offset: 3px;
  border-radius: var(--snug-radius-sm);
}
```

### Scroll-Triggered Entrance Animation

```css
/* Gentle fade-in-up for scroll-revealed content */
@keyframes snug-fade-in-up {
  from {
    opacity: 0;
    transform: translateY(16px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.snug-animate-in {
  animation: snug-fade-in-up 0.6s ease-out forwards;
}

/* Staggered children entrance */
.snug-stagger > * {
  opacity: 0;
  animation: snug-fade-in-up 0.5s ease-out forwards;
}

.snug-stagger > *:nth-child(1) { animation-delay: 0.05s; }
.snug-stagger > *:nth-child(2) { animation-delay: 0.1s; }
.snug-stagger > *:nth-child(3) { animation-delay: 0.15s; }
.snug-stagger > *:nth-child(4) { animation-delay: 0.2s; }
.snug-stagger > *:nth-child(5) { animation-delay: 0.25s; }
.snug-stagger > *:nth-child(6) { animation-delay: 0.3s; }
```

### Input Fields

```css
/* Friendly rounded input fields */
.snug-input {
  width: 100%;
  padding: 0.8rem 1.4rem;
  background: var(--snug-bg-card);
  border: 2px solid var(--snug-border-soft);
  border-radius: var(--snug-radius-md);
  font-family: 'Nunito', sans-serif;
  font-size: 1rem;
  color: var(--snug-text-primary);
  transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

.snug-input::placeholder {
  color: var(--snug-text-muted);
  font-weight: 400;
}

.snug-input:focus {
  outline: none;
  border-color: var(--snug-accent-sage);
  box-shadow: 0 0 0 4px rgba(184, 201, 163, 0.2);
}

/* Textarea variant */
.snug-textarea {
  min-height: 120px;
  resize: vertical;
  border-radius: var(--snug-radius-lg);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical / Lifestyle Reference | Web Equivalent |
|-------------------------------|----------------|
| Linen fabric texture | Very subtle dot or grain pattern via `radial-gradient` at 3-5% opacity on warm cream background |
| Ceramic mug, rounded pottery | Large `border-radius` (20-28px) on all containers, warm shadow underneath |
| Handmade paper, soft cardstock | Off-white backgrounds (`#FFF8F0`, `#F5EDE3`) with optional SVG noise overlay at 2-4% opacity |
| Wooden table surface | Warm oat/tan accent color (`#E8DCD0`) for secondary backgrounds and borders |
| Knitted blanket texture | Soft repeating grid pattern at low opacity, warm color palette |
| Watercolor washes | Subtle pastel background gradients with soft edges between sections |
| Pressed wildflowers | Simple, flat illustration style with muted natural colors -- hand-drawn icons and decorative elements |
| Cork board | Warm tan surface with cards "pinned" on top using subtle shadows and slight rotation |
| Frosted glass jar | `backdrop-filter: blur()` on overlays and sticky headers with warm-tinted semi-transparency |
| Washi tape strips | Colorful pastel accent bars (4-6px) on the side of callout boxes, slightly uneven if illustrated |
| Round river stones | Pill-shaped buttons and fully rounded badges with smooth pastel fills |
| Soft morning light | Gentle warm gradient overlays (`linear-gradient` from transparent to warm cream) at top of hero sections |

---

## Imagery and Visual Content Guidelines

When creating or sourcing imagery for a Snug Simple styled site:

- **Use soft, warm photography** with natural lighting -- morning light, golden hour, diffused window light; avoid harsh flash or high-contrast studio lighting
- **Feature cozy lifestyle subjects** -- steaming mugs, open books, houseplants, ceramic bowls, knitted textures, wooden surfaces, soft fabrics
- **Apply gentle warmth post-processing** -- slightly increase warmth, reduce contrast, soften highlights; photos should feel like a warm filter has been applied
- **Round image containers** -- always display images in rounded rectangles (16-24px radius) or circles, never sharp rectangles
- **Hand-drawn or softly rendered illustrations** are preferred over polished vector graphics -- imperfect lines and organic shapes reinforce the human-centered feel
- **Icons should be rounded and chunky** -- 2-3px stroke weight with rounded joins and caps; avoid thin or sharp icon sets
- **Avoid stock photography with corporate or sterile settings** -- no glass offices, no suits, no forced smiles; imagery should feel genuine and personal
- **Muted and desaturated color treatment** -- photographs should feel as if they are part of the pastel palette, not visually competing with it
- **Generous padding around images** -- images should never touch the edge of their container; whitespace frames them like a matted print
- **Aspect ratios should feel comfortable** -- prefer 4:3 or 1:1 over extreme widescreen crops; square thumbnails in rounded containers are a signature element
- **Alt text should reflect the warm tone** -- describe imagery conversationally, as if telling a friend what the picture shows

---

## Related Aesthetics

| Aesthetic | Relationship to Snug Simple |
|-----------|----------------------------|
| **Cutecore** | Shares the rounded, friendly visual language and pastel palette; Cutecore pushes further into kawaii territory with more decorative elements and brighter pinks, while Snug Simple stays muted and restrained |
| **Danish Pastel** | Close sibling -- both use soft pastels and rounded forms; Danish Pastel draws more directly from Scandinavian interior design with specific checkered patterns and arched shapes, while Snug Simple is broader and less pattern-dependent |
| **Cottagecore** | Overlapping warmth and comfort focus; Cottagecore is more specifically rural and nature-themed with floral patterns, while Snug Simple is more abstract and typographically driven |
| **Coquette** | Shares softness and pastel pinks but Coquette leans romantic and feminine with bows, ribbons, and lace motifs; Snug Simple is gender-neutral and minimal |
| **Dopamine Design** | Both prioritize friendliness and approachability; Dopamine Design uses saturated bold colors and more visual energy, while Snug Simple deliberately mutes everything for calm |
| **Claymorphism** | Shares rounded containers and soft shadows; Claymorphism uses more dramatic inner shadows and inflated 3D-like effects, while Snug Simple stays flat and lightweight |
| **Coastal Style** | Both emphasize calm, natural palettes and generous spacing; Coastal uses blues and sandy neutrals, while Snug Simple uses a broader pastel range centered on sage and blush |
| **Bento Grid** | Can coexist -- Bento Grid's modular card layout works well when styled with Snug Simple's rounded corners and pastel fills, though Bento tends toward more structured composition |

---

## Implementation Notes

- The core principle of Snug Simple is **comfort through restraint**. Every design decision should ask: "Does this make the user feel more at ease?" If an element creates visual tension, urgency, or complexity, it does not belong.
- **Border-radius is non-negotiable** -- sharp corners immediately break the aesthetic. Every visible rectangle should have a minimum of 12px border-radius. Cards and containers use 20-28px. Buttons and tags use fully rounded (999px). This single property does more to establish the Snug Simple feel than any other.
- **Avoid pure black and pure white** -- use warm off-black (#3D3028 or similar) for text and warm off-white (#FFF8F0) for backgrounds. Pure black/white creates harshness that undermines the cozy atmosphere.
- **Typography weight matters enormously** -- thin or light font weights feel cold and corporate. Use 500 minimum for body text, 600-800 for headings. The type should feel chunky and confident, like letters drawn with a thick marker.
- **Spacing is a feature, not waste** -- resist the impulse to tighten margins and padding. The generous whitespace is what makes Snug Simple feel relaxed. If the page feels "empty," it is working correctly.
- **Pastel saturation must stay low** -- the difference between Snug Simple and childish or garish pastel design is saturation control. Colors should feel dusty, muted, and grown-up. If a color looks like it belongs on a birthday cake, desaturate it by 20-30%.
- **Shadows should be warm, not gray** -- use `rgba()` shadows tinted with warm colors (brown, rose, sage) rather than neutral gray/black. This subtle detail keeps depth feeling cozy.
- **Interaction design should be gentle** -- no snappy, aggressive animations. Transitions use 0.2-0.4s easing. Hover effects are subtle lifts or soft color shifts, never dramatic scale changes or color explosions.
- **Performance note** -- rounded corners on many elements and backdrop-filter can be GPU-intensive on older devices. Test with many cards on screen and consider reducing effects for users who prefer reduced motion.
- **Accessibility** -- the muted palette requires careful contrast checking. Body text on cream backgrounds should maintain WCAG AA (4.5:1 minimum). Espresso brown (#3D3028) on warm cream (#FFF8F0) achieves approximately 9:1 contrast, which is excellent.

---

## Quick-Start: Minimal Snug Simple Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Snug Simple Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&family=Nunito:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --snug-bg-base: #FFF8F0;
      --snug-bg-alt: #F5EDE3;
      --snug-bg-card: #FFFFFF;
      --snug-bg-tinted: #FFF0F0;
      --snug-bg-sage: #EEF4E8;
      --snug-bg-lavender: #F0ECF5;
      --snug-text-primary: #3D3028;
      --snug-text-secondary: #5C4A3A;
      --snug-text-muted: #9B8A7A;
      --snug-text-inverse: #FFFFFF;
      --snug-accent-sage: #B8C9A3;
      --snug-accent-sage-dark: #8FAF78;
      --snug-accent-blush: #E8B4B8;
      --snug-accent-rose: #D4A0A8;
      --snug-accent-lavender: #C5B8D9;
      --snug-accent-sky: #B8D4E8;
      --snug-accent-oat: #E8DCD0;
      --snug-border-soft: #E8D8D0;
      --snug-shadow-warm: rgba(180, 160, 140, 0.15);
      --snug-radius-sm: 12px;
      --snug-radius-md: 20px;
      --snug-radius-lg: 28px;
      --snug-radius-pill: 999px;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--snug-bg-base);
      color: var(--snug-text-primary);
      font-family: 'Nunito', 'Quicksand', -apple-system, sans-serif;
      font-size: 17px;
      line-height: 1.8;
      letter-spacing: 0.01em;
      min-height: 100vh;
      -webkit-font-smoothing: antialiased;
    }

    /* Sticky frosted header */
    .snug-header {
      position: sticky;
      top: 0;
      z-index: 100;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0.8rem 2rem;
      background: rgba(255, 248, 240, 0.85);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--snug-border-soft);
    }

    .snug-logo {
      font-family: 'Quicksand', sans-serif;
      font-size: 1.3rem;
      font-weight: 700;
      color: var(--snug-text-primary);
      text-decoration: none;
    }

    .snug-nav {
      display: flex;
      gap: 0.3rem;
    }

    .snug-nav a {
      padding: 0.5rem 1.2rem;
      border-radius: var(--snug-radius-pill);
      font-family: 'Quicksand', sans-serif;
      font-size: 0.9rem;
      font-weight: 600;
      color: var(--snug-text-secondary);
      text-decoration: none;
      transition: all 0.2s ease;
    }

    .snug-nav a:hover,
    .snug-nav a.active {
      background: var(--snug-accent-sage);
      color: var(--snug-text-primary);
    }

    /* Hero section */
    .snug-hero {
      max-width: 800px;
      margin: 0 auto;
      padding: 5rem 2rem 4rem;
      text-align: center;
    }

    .snug-hero h1 {
      font-family: 'Quicksand', sans-serif;
      font-size: clamp(2.2rem, 5vw, 3.2rem);
      font-weight: 700;
      color: var(--snug-text-primary);
      line-height: 1.25;
      margin-bottom: 1.2rem;
    }

    .snug-hero p {
      font-size: 1.15rem;
      color: var(--snug-text-secondary);
      max-width: 550px;
      margin: 0 auto 2rem;
      line-height: 1.8;
    }

    .snug-hero-actions {
      display: flex;
      gap: 1rem;
      justify-content: center;
      flex-wrap: wrap;
    }

    /* Buttons */
    .snug-button {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.8rem 2rem;
      border: 2px solid transparent;
      border-radius: var(--snug-radius-pill);
      font-family: 'Quicksand', sans-serif;
      font-size: 1rem;
      font-weight: 700;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.25s ease;
    }

    .snug-button--primary {
      background: var(--snug-accent-sage);
      color: var(--snug-text-primary);
    }

    .snug-button--primary:hover {
      background: var(--snug-accent-sage-dark);
      color: var(--snug-text-inverse);
      transform: scale(1.03);
      box-shadow: 0 4px 16px rgba(143, 175, 120, 0.2);
    }

    .snug-button--outline {
      background: transparent;
      border-color: var(--snug-accent-blush);
      color: var(--snug-accent-rose);
    }

    .snug-button--outline:hover {
      background: var(--snug-accent-blush);
      color: var(--snug-text-primary);
      transform: scale(1.03);
    }

    /* Content sections */
    .snug-section {
      padding: 4rem 2rem;
    }

    .snug-section--alt {
      background: var(--snug-bg-alt);
    }

    .snug-section--sage {
      background: var(--snug-bg-sage);
    }

    .snug-container {
      max-width: 1100px;
      margin: 0 auto;
    }

    .snug-section-header {
      text-align: center;
      margin-bottom: 3rem;
    }

    .snug-section-header h2 {
      font-family: 'Quicksand', sans-serif;
      font-size: clamp(1.6rem, 3.5vw, 2.2rem);
      font-weight: 700;
      color: var(--snug-text-primary);
      margin-bottom: 0.6rem;
    }

    .snug-section-header p {
      color: var(--snug-text-muted);
      font-size: 1.05rem;
      max-width: 500px;
      margin: 0 auto;
    }

    /* Card grid */
    .snug-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.8rem;
    }

    .snug-card {
      background: var(--snug-bg-card);
      border: 1px solid var(--snug-border-soft);
      border-radius: var(--snug-radius-lg);
      padding: 2rem 2.2rem;
      box-shadow: 0 2px 8px var(--snug-shadow-warm);
      transition: all 0.3s ease;
    }

    .snug-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 24px var(--snug-shadow-warm);
    }

    .snug-card-icon {
      width: 52px;
      height: 52px;
      border-radius: var(--snug-radius-md);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      margin-bottom: 1.2rem;
    }

    .snug-card-icon--sage { background: var(--snug-bg-sage); }
    .snug-card-icon--blush { background: var(--snug-bg-tinted); }
    .snug-card-icon--lavender { background: var(--snug-bg-lavender); }

    .snug-card h3 {
      font-family: 'Quicksand', sans-serif;
      font-size: 1.25rem;
      font-weight: 700;
      color: var(--snug-text-primary);
      margin-bottom: 0.6rem;
    }

    .snug-card p {
      color: var(--snug-text-secondary);
      font-size: 0.95rem;
      line-height: 1.7;
      margin-bottom: 1.2rem;
    }

    /* Tags */
    .snug-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .snug-tag {
      display: inline-flex;
      padding: 0.3rem 0.9rem;
      border-radius: var(--snug-radius-pill);
      font-family: 'Quicksand', sans-serif;
      font-size: 0.78rem;
      font-weight: 600;
    }

    .snug-tag--sage {
      background: var(--snug-bg-sage);
      color: var(--snug-accent-sage-dark);
    }

    .snug-tag--blush {
      background: var(--snug-bg-tinted);
      color: var(--snug-accent-rose);
    }

    .snug-tag--lavender {
      background: var(--snug-bg-lavender);
      color: #7B6B9A;
    }

    .snug-tag--sky {
      background: #EDF4F8;
      color: #5A8AA8;
    }

    /* Callout box */
    .snug-callout {
      background: var(--snug-bg-sage);
      border-left: 5px solid var(--snug-accent-sage);
      border-radius: 0 var(--snug-radius-md) var(--snug-radius-md) 0;
      padding: 1.5rem 2rem;
      margin: 2rem 0;
    }

    .snug-callout p {
      margin-bottom: 0;
      color: var(--snug-text-secondary);
      font-weight: 500;
    }

    /* Feature list with inline layout */
    .snug-features {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem;
      justify-content: center;
      margin-top: 2rem;
    }

    .snug-feature-pill {
      display: inline-flex;
      align-items: center;
      gap: 0.6rem;
      padding: 0.6rem 1.5rem;
      background: var(--snug-bg-card);
      border: 1px solid var(--snug-border-soft);
      border-radius: var(--snug-radius-pill);
      font-family: 'Quicksand', sans-serif;
      font-size: 0.9rem;
      font-weight: 600;
      color: var(--snug-text-secondary);
      box-shadow: 0 1px 4px var(--snug-shadow-warm);
    }

    .snug-feature-pill .dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;
    }

    .snug-feature-pill .dot--sage { background: var(--snug-accent-sage); }
    .snug-feature-pill .dot--blush { background: var(--snug-accent-blush); }
    .snug-feature-pill .dot--lavender { background: var(--snug-accent-lavender); }
    .snug-feature-pill .dot--sky { background: var(--snug-accent-sky); }

    /* Footer */
    .snug-footer {
      background: var(--snug-bg-alt);
      padding: 3rem 2rem;
      text-align: center;
      border-top: 1px solid var(--snug-border-soft);
    }

    .snug-footer p {
      color: var(--snug-text-muted);
      font-size: 0.9rem;
      max-width: 100%;
    }

    .snug-footer a {
      color: var(--snug-accent-sage-dark);
      text-decoration: underline;
      text-decoration-color: var(--snug-accent-sage);
      text-underline-offset: 3px;
      text-decoration-thickness: 2px;
      transition: color 0.2s ease;
    }

    .snug-footer a:hover {
      color: var(--snug-accent-rose);
    }

    /* Responsive */
    @media (max-width: 768px) {
      .snug-hero { padding: 3rem 1.5rem 2.5rem; }
      .snug-section { padding: 3rem 1.5rem; }
      .snug-grid { grid-template-columns: 1fr; }
      .snug-nav { display: none; }
      .snug-hero-actions { flex-direction: column; align-items: center; }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header class="snug-header">
    <a href="#" class="snug-logo">cozy corner</a>
    <nav class="snug-nav">
      <a href="#" class="active">Home</a>
      <a href="#">About</a>
      <a href="#">Journal</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- Hero -->
  <section class="snug-hero">
    <h1>A warmer kind of digital space</h1>
    <p>Simple tools and gentle ideas for people who want their screen time to feel a little more like a cup of tea and a little less like a spreadsheet.</p>
    <div class="snug-hero-actions">
      <a href="#" class="snug-button snug-button--primary">Get started</a>
      <a href="#" class="snug-button snug-button--outline">Learn more</a>
    </div>
  </section>

  <!-- Cards Section -->
  <section class="snug-section snug-section--alt">
    <div class="snug-container">
      <div class="snug-section-header">
        <h2>What makes it cozy</h2>
        <p>Three small ideas that make a big difference in how a space feels.</p>
      </div>
      <div class="snug-grid">
        <div class="snug-card">
          <div class="snug-card-icon snug-card-icon--sage">&#127807;</div>
          <h3>Breathe easy</h3>
          <p>Generous spacing and soft colors let your eyes rest. Nothing competes for attention here -- content arrives gently.</p>
          <div class="snug-tags">
            <span class="snug-tag snug-tag--sage">Spacing</span>
            <span class="snug-tag snug-tag--lavender">Calm</span>
          </div>
        </div>
        <div class="snug-card">
          <div class="snug-card-icon snug-card-icon--blush">&#128149;</div>
          <h3>Friendly by default</h3>
          <p>Rounded corners, chunky type, and warm pastels create a space that feels approachable from the very first pixel.</p>
          <div class="snug-tags">
            <span class="snug-tag snug-tag--blush">Warm</span>
            <span class="snug-tag snug-tag--sky">Friendly</span>
          </div>
        </div>
        <div class="snug-card">
          <div class="snug-card-icon snug-card-icon--lavender">&#9732;</div>
          <h3>Intentionally simple</h3>
          <p>One column. Clear type. No clutter. Simplicity is not a limitation here -- it is the whole point.</p>
          <div class="snug-tags">
            <span class="snug-tag snug-tag--lavender">Minimal</span>
            <span class="snug-tag snug-tag--sage">Focus</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Callout Section -->
  <section class="snug-section">
    <div class="snug-container" style="max-width: 700px;">
      <div class="snug-callout">
        <p>Good design should feel like a conversation with a friend -- unhurried, clear, and warm. If your screen feels like it is yelling at you, something has gone wrong.</p>
      </div>
    </div>
  </section>

  <!-- Feature Pills -->
  <section class="snug-section snug-section--sage">
    <div class="snug-container">
      <div class="snug-section-header">
        <h2>Built with care</h2>
        <p>Small touches that add up to something comfortable.</p>
      </div>
      <div class="snug-features">
        <div class="snug-feature-pill">
          <span class="dot dot--sage"></span> Rounded everything
        </div>
        <div class="snug-feature-pill">
          <span class="dot dot--blush"></span> Soft pastels
        </div>
        <div class="snug-feature-pill">
          <span class="dot dot--lavender"></span> Chunky type
        </div>
        <div class="snug-feature-pill">
          <span class="dot dot--sky"></span> Generous spacing
        </div>
        <div class="snug-feature-pill">
          <span class="dot dot--sage"></span> Warm shadows
        </div>
        <div class="snug-feature-pill">
          <span class="dot dot--blush"></span> Gentle motion
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="snug-footer">
    <p>Made with warmth and care. Take it slow. <a href="#">Say hello</a>.</p>
  </footer>

</body>
</html>
```
