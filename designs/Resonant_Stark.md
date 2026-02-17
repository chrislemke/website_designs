# Resonant Stark -- Design Reference

Resonant Stark is a purpose-driven minimalism with emotional subtlety -- ultra-clean layouts where every element earns its place, with warmth injected through micro-interactions and tonal shifts. It draws from the lineage of Swiss/International design and Japanese Ma (negative space philosophy) but rejects the coldness often associated with minimalism. The defining quality is resonance: a sense that the sparse visual field vibrates with intention, that the whitespace is not empty but charged. Ultra-thin typography floats in vast fields of near-white, borders dissolve to single pixels or vanish entirely, and color appears only as a whisper -- a muted terracotta link, a sage hover state. Movement is the emotional medium: elements fade in on scroll with glacial smoothness, letter-spacing expands imperceptibly on hover, opacity shifts hint at depth beneath the surface. The result is design that feels like a held breath -- still, precise, and quietly alive.

---

## Visual Characteristics

- **Vast whitespace** -- 80% or more of the page is negative space; content floats in open fields with deliberate, asymmetric placement
- **Ultra-thin typography** -- font weights of 100-300 dominate, with large display sizes (4-8rem) that make thinness feel monumental rather than fragile
- **Near-monochrome palette** -- backgrounds range from #FAFAFA to #F5F5F0, text from #1A1A18 to #4A4A48, with color nearly absent
- **Single muted accent color** -- one understated warm tone (terracotta, sage, dusty rose) used sparingly for links, hover states, and focal points
- **Micro-interactions on hover** -- subtle opacity shifts, gentle translates, letter-spacing expansion, and color transitions that reward attention
- **Smooth animation reveals** -- scroll-triggered fade-ins with long durations (0.6-1.2s), content emerging rather than appearing
- **Minimal or absent borders** -- single-pixel lines used rarely, replaced by whitespace as the primary structural divider
- **Soft gradient fades** -- barely perceptible gradients between near-white tones (#FAFAFA to #F5F5F0) creating depth without visible color
- **Generous line-height** -- body text at 1.6-2.0 line-height, headings with expansive leading that allows each word to breathe
- **Wide letter-spacing** -- 0.05-0.15em tracking on headings and labels, creating an airy, unhurried typographic rhythm
- **Content that breathes** -- every text block, image, and element surrounded by disproportionately large margins and padding
- **Emotional restraint with warmth** -- the palette leans warm (cream whites, warm grays) rather than clinical blue-whites, maintaining human presence in the minimalism

---

## Color Palette

The Resonant Stark palette is defined by extreme restraint -- near-whites and warm grays dominate, with color appearing only as a momentary accent:

- **Near-white backgrounds** -- not pure #FFFFFF but warm off-whites (#FAFAFA, #F8F8F5, #F5F5F0) that soften the screen and reduce harshness
- **Warm gray spectrum** -- light grays with warm undertones (#E8E4E0, #D4D0CC, #B8B4B0) for secondary elements and subtle borders
- **Near-black text** -- #1A1A18 for primary text, warm enough to avoid the starkness of pure black while maintaining strong contrast
- **Muted accent colors** -- a single accent chosen per project: terracotta (#C4836A), sage (#8BA888), dusty rose (#B89090), or warm clay (#A08060)
- **No saturated colors** -- even the accent is desaturated and muted, blending into the warm gray world
- **Gradient subtlety** -- backgrounds use gradients between near-whites so faint they register more as atmosphere than visible color
- **Hover-state color shifts** -- accent colors appear primarily on interaction, reinforcing the "resonance" quality

### Suggested Implementation Palette

Based on characteristic Resonant Stark visual compositions:

| Role                | Color             | Hex       |
|---------------------|-------------------|-----------|
| Background Primary  | Warm White        | `#FAFAFA` |
| Background Alt      | Cream White       | `#F5F5F0` |
| Background Subtle   | Warm Snow         | `#F0EEEB` |
| Surface             | Light Warm Gray   | `#E8E4E0` |
| Surface Muted       | Mid Warm Gray     | `#D4D0CC` |
| Border Subtle       | Pale Gray         | `#D0CCC8` |
| Text Primary        | Near Black        | `#1A1A18` |
| Text Secondary      | Dark Warm Gray    | `#6A6864` |
| Text Tertiary       | Mid Gray          | `#9A9894` |
| Accent Warm         | Muted Terracotta  | `#C4836A` |
| Accent Cool         | Sage Green        | `#8BA888` |
| Accent Neutral      | Warm Clay         | `#A08060` |
| Hover Glow          | Faded Terracotta  | `#C4836A20`|
| Gradient Start      | Warm White        | `#FAFAFA` |
| Gradient End        | Cream             | `#F5F5F0` |
| Focus Ring          | Light Terracotta  | `#C4836A40`|

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --stark-bg-primary: #FAFAFA;
  --stark-bg-alt: #F5F5F0;
  --stark-bg-subtle: #F0EEEB;
  --stark-bg-surface: #E8E4E0;
  --stark-bg-muted: #D4D0CC;

  /* Text */
  --stark-text-primary: #1A1A18;
  --stark-text-secondary: #6A6864;
  --stark-text-tertiary: #9A9894;
  --stark-text-faint: #B8B4B0;

  /* Accent -- Terracotta (swap for project-specific accent) */
  --stark-accent: #C4836A;
  --stark-accent-hover: #B07058;
  --stark-accent-faded: rgba(196, 131, 106, 0.12);
  --stark-accent-glow: rgba(196, 131, 106, 0.06);

  /* Alternate accent -- Sage */
  --stark-accent-sage: #8BA888;
  --stark-accent-sage-hover: #7A9A78;
  --stark-accent-sage-faded: rgba(139, 168, 136, 0.12);

  /* Borders */
  --stark-border: #E8E4E0;
  --stark-border-faint: #F0EEEB;
  --stark-border-visible: #D0CCC8;

  /* Shadows */
  --stark-shadow-subtle: rgba(26, 26, 24, 0.04);
  --stark-shadow-medium: rgba(26, 26, 24, 0.08);

  /* Transitions */
  --stark-transition-fast: 0.3s ease;
  --stark-transition-base: 0.5s ease;
  --stark-transition-slow: 0.8s ease;
  --stark-transition-glacial: 1.2s ease;

  /* Spacing scale */
  --stark-space-xs: 0.5rem;
  --stark-space-sm: 1rem;
  --stark-space-md: 2rem;
  --stark-space-lg: 4rem;
  --stark-space-xl: 8rem;
  --stark-space-2xl: 12rem;

  /* Functional mappings */
  --stark-bg-page: var(--stark-bg-primary);
  --stark-bg-section: var(--stark-bg-alt);
  --stark-text-heading: var(--stark-text-primary);
  --stark-text-body: var(--stark-text-secondary);
  --stark-accent-primary: var(--stark-accent);
  --stark-border-default: var(--stark-border);
}
```

---

## Typography

### Typeface Characteristics

Resonant Stark typography relies on extreme thinness at large scale -- the contradiction between fragility and monumentality creates visual tension:

- **Ultra-thin weights** -- font-weight 100-300 for all display and heading text; body text at 300-400 for readability
- **Large display sizes** -- hero headings at 4-8rem, section headings at 2-3rem; the thinness demands size to maintain legibility and presence
- **Wide letter-spacing** -- 0.05-0.15em on headings and labels; text feels unhurried and deliberately placed
- **High line-height** -- 1.6 minimum for body text, 1.2-1.4 for large headings where the vertical space between lines becomes a design element
- **Single font family** -- typically one sans-serif family at most two weights (thin for display, light/regular for body)
- **No bold text** -- emphasis achieved through size, spacing, opacity, or accent color rather than weight
- **Uppercase sparingly** -- section labels and navigation may use uppercase with wide tracking, but body text remains sentence case
- **Restrained font palette** -- one family, two weights maximum; additional hierarchy comes from size, color, and spacing alone
- **Text as sculpture** -- headings treated as visual elements occupying space, not just carrying meaning

### Recommended Web Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Inter** | Geometric sans-serif (Thin 100, Light 300) | Primary choice -- excellent thin weights, wide character set, clean geometry |
| **Outfit** | Geometric sans with warmth (Thin 100, Light 300) | Slightly softer than Inter, warmer curves at thin weights |
| **Instrument Sans** | Contemporary sans (Regular 400) | Body text alternative with humanist touches |
| **Sora** | Geometric sans (Thin 100, ExtraLight 200, Light 300) | Excellent ultra-thin display font with distinctive character |
| **Jost** | Futura-inspired geometric (Thin 100, Light 300) | Classic geometric proportions, beautiful at large thin sizes |
| **Work Sans** | Humanist sans (Thin 100, ExtraLight 200, Light 300) | Warmth in thin weights, good for accessible thin typography |
| **Libre Franklin** | Franklin Gothic revival (Thin 100, ExtraLight 200) | Traditional American sans proportions, stable at thin weights |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400&display=swap');

/* Body -- light weight, generous spacing */
body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  font-weight: 300;
  font-size: 17px;
  line-height: 1.8;
  letter-spacing: 0.01em;
  color: var(--stark-text-secondary);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* Display heading -- ultra-thin, monumental */
h1 {
  font-weight: 100;
  font-size: clamp(3rem, 8vw, 7rem);
  line-height: 1.1;
  letter-spacing: -0.02em;
  color: var(--stark-text-primary);
  margin-bottom: var(--stark-space-lg);
}

/* Section heading -- thin, wide-tracked */
h2 {
  font-weight: 200;
  font-size: clamp(1.8rem, 4vw, 3rem);
  line-height: 1.2;
  letter-spacing: 0.04em;
  color: var(--stark-text-primary);
  margin-bottom: var(--stark-space-md);
}

/* Subsection heading */
h3 {
  font-weight: 300;
  font-size: clamp(1.2rem, 2.5vw, 1.6rem);
  line-height: 1.4;
  letter-spacing: 0.03em;
  color: var(--stark-text-primary);
  margin-bottom: var(--stark-space-sm);
}

/* Label text -- uppercase, wide tracking */
.stark-label {
  font-weight: 300;
  font-size: 0.75rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--stark-text-tertiary);
}

/* Body text -- light, readable */
p {
  font-weight: 300;
  font-size: 1.0625rem;
  line-height: 1.8;
  color: var(--stark-text-secondary);
  max-width: 38em;
  margin-bottom: 1.5em;
}

/* Lead paragraph -- slightly larger, thinner */
.stark-lead {
  font-weight: 200;
  font-size: 1.25rem;
  line-height: 1.9;
  color: var(--stark-text-secondary);
  max-width: 32em;
}

/* Link -- accent color, understated underline */
a {
  color: var(--stark-accent);
  text-decoration: none;
  border-bottom: 0.5px solid var(--stark-accent-faded);
  transition: border-color var(--stark-transition-base),
              color var(--stark-transition-fast);
}

a:hover {
  color: var(--stark-accent-hover);
  border-bottom-color: var(--stark-accent);
}
```

---

## Key Design Elements and Motifs

### Whitespace as Primary Material

The defining element of Resonant Stark -- whitespace is not absence but the dominant design material:

- **80%+ negative space** in any given viewport; content occupies the minority of the screen
- **Asymmetric placement** -- elements positioned off-center, with unequal margins creating visual tension and movement
- **Vertical rhythm through space** -- sections separated by 6-12rem of whitespace rather than borders or background changes
- **Breathing room around text** -- paragraphs set with generous padding, max-width constraints (32-40em), and high line-height
- **Intentional emptiness** -- every area of whitespace is a deliberate design decision, not leftover space

### Micro-Interactions

Subtle hover and focus effects that create the "resonance" quality -- the sense that the interface responds to attention:

- **Opacity shifts on hover** -- elements transition from 0.7 to 1.0 opacity, revealing full presence on interaction
- **Gentle translate movements** -- 2-4px upward shifts on card hover, suggesting weightlessness
- **Letter-spacing expansion** -- navigation items or headings that breathe wider on hover (0.05em to 0.12em)
- **Color emergence** -- accent color appears on hover from an initially colorless state (gray to terracotta)
- **Underline animations** -- links grow a subtle underline from left to right on hover
- **Transition timing** -- all interactions use 0.3-0.8s ease transitions, never instant or jarring

### Scroll-Triggered Reveals

Content emerges into view with restrained, purposeful animations:

- **Fade-in from below** -- elements translate 20-30px upward while fading from 0 to 1 opacity
- **Staggered timing** -- multiple elements in a section animate sequentially with 100-150ms delays
- **Long durations** -- reveal animations take 0.6-1.2s, creating a meditative pace
- **Once-only animation** -- elements animate into their final position and remain; no repeated or looping animations
- **No bounce or overshoot** -- easing is always smooth (ease, ease-out), never elastic or spring-based

### Understated Typography Treatments

Text itself becomes a visual element through scale and spacing:

- **Display headings as landmarks** -- 4-8rem thin text that anchors the page visually, readable across a room
- **Numeral styling** -- large thin numerals (for lists, stats, dates) used as decorative anchors
- **Subtle text color hierarchy** -- primary (#1A1A18), secondary (#6A6864), tertiary (#9A9894) creating depth through value alone
- **No text decoration** -- no underlines, no bold, no italic except for semantic emphasis; hierarchy comes from size and weight

### Single-Pixel Borders and Dividers

When structural lines appear at all, they are whisper-thin:

- **0.5-1px borders** -- the thinnest renderable line, often in a color barely distinguishable from the background
- **Partial dividers** -- horizontal rules that span only 30-50% of the container width, centered or left-aligned
- **Borders as last resort** -- whitespace is always preferred; borders appear only when spatial separation alone is insufficient
- **Border color near-invisible** -- #E8E4E0 or #F0EEEB on a #FAFAFA background, a shadow of a line

---

## Layout Principles

- **Single-column dominance** -- content flows in one column, typically 600-800px wide, centered or offset on the page
- **Vast vertical spacing** -- sections separated by 8-16rem, creating a rhythm of content and emptiness
- **Asymmetric placement** -- content containers offset from center (60/40 or 70/30 splits), avoiding symmetry's static quality
- **Max-width constraints** -- text blocks limited to 32-40em for optimal reading line length
- **Full-viewport hero sections** -- opening sections use 100vh with content placed in the lower third or center
- **Grid as invisible structure** -- underlying grid exists but is never visible; no grid lines, gutters, or explicit column markers
- **Minimal navigation** -- navigation reduced to essential links, often a single word or logo, positioned with vast surrounding space
- **Progressive disclosure** -- content reveals through scrolling rather than being presented all at once
- **Horizontal elements rare** -- horizontal layouts (multi-column grids) used sparingly and always with generous gaps (4-8rem)
- **Mobile: even more space** -- on smaller screens, whitespace proportions are maintained or increased, not compressed

### Modern Web Adaptation

- Use **CSS Grid with large gap values** (4-8rem) for section spacing
- **Scroll-driven animations** with Intersection Observer for fade-in reveals
- **clamp()** for responsive typography that scales fluidly between mobile and desktop
- **Container queries** for components that adapt to available space
- **prefers-reduced-motion** media query to disable animations for accessibility
- **Light mode only** -- dark mode undermines the vast whitespace effect; if dark mode is required, use very dark near-blacks (#0A0A0A) with the same spatial principles

---

## CSS/Design Techniques

### Micro-Interaction: Hover Fade and Lift

```css
/* Card or content block with subtle hover response */
.stark-card {
  padding: var(--stark-space-lg);
  opacity: 0.85;
  transform: translateY(0);
  transition:
    opacity var(--stark-transition-base),
    transform var(--stark-transition-base),
    box-shadow var(--stark-transition-base);
}

.stark-card:hover {
  opacity: 1;
  transform: translateY(-3px);
  box-shadow: 0 8px 40px var(--stark-shadow-subtle);
}
```

### Scroll-Triggered Fade-In Reveal

```css
/* Elements start hidden and animate in when scrolled into view */
.stark-reveal {
  opacity: 0;
  transform: translateY(24px);
  transition:
    opacity var(--stark-transition-slow),
    transform var(--stark-transition-slow);
}

.stark-reveal.is-visible {
  opacity: 1;
  transform: translateY(0);
}

/* Staggered children */
.stark-reveal-group .stark-reveal:nth-child(1) { transition-delay: 0s; }
.stark-reveal-group .stark-reveal:nth-child(2) { transition-delay: 0.12s; }
.stark-reveal-group .stark-reveal:nth-child(3) { transition-delay: 0.24s; }
.stark-reveal-group .stark-reveal:nth-child(4) { transition-delay: 0.36s; }
.stark-reveal-group .stark-reveal:nth-child(5) { transition-delay: 0.48s; }

/* Respect reduced motion preference */
@media (prefers-reduced-motion: reduce) {
  .stark-reveal {
    opacity: 1;
    transform: none;
    transition: none;
  }
}
```

### Scroll-Triggered Fade-In (JavaScript)

```javascript
/* Intersection Observer for scroll-triggered reveals */
const observer = new IntersectionObserver(
  (entries) => {
    entries.forEach((entry) => {
      if (entry.isIntersecting) {
        entry.target.classList.add('is-visible');
        observer.unobserve(entry.target);
      }
    });
  },
  { threshold: 0.15, rootMargin: '0px 0px -40px 0px' }
);

document.querySelectorAll('.stark-reveal').forEach((el) => {
  observer.observe(el);
});
```

### Letter-Spacing Hover Animation

```css
/* Navigation or heading with expanding letter-spacing on hover */
.stark-nav-link {
  font-weight: 200;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--stark-text-tertiary);
  text-decoration: none;
  border: none;
  transition:
    letter-spacing var(--stark-transition-base),
    color var(--stark-transition-fast);
}

.stark-nav-link:hover {
  letter-spacing: 0.16em;
  color: var(--stark-text-primary);
}

.stark-nav-link:focus-visible {
  outline: 1px solid var(--stark-accent-faded);
  outline-offset: 8px;
}
```

### Understated Underline Link Animation

```css
/* Link with animated underline that grows from left on hover */
.stark-link {
  color: var(--stark-text-secondary);
  text-decoration: none;
  position: relative;
  transition: color var(--stark-transition-fast);
}

.stark-link::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 0.5px;
  background: var(--stark-accent);
  transition: width var(--stark-transition-base);
}

.stark-link:hover {
  color: var(--stark-accent);
}

.stark-link:hover::after {
  width: 100%;
}
```

### Near-Invisible Gradient Background

```css
/* Barely perceptible gradient that creates subtle depth */
.stark-gradient-bg {
  background: linear-gradient(
    180deg,
    var(--stark-bg-primary) 0%,
    var(--stark-bg-alt) 50%,
    var(--stark-bg-primary) 100%
  );
}

/* Radial glow -- extremely subtle warmth behind content */
.stark-glow {
  background: radial-gradient(
    ellipse 60% 50% at 50% 40%,
    var(--stark-accent-glow) 0%,
    transparent 70%
  );
}

/* Section divider gradient -- horizontal fade line */
.stark-divider {
  height: 0.5px;
  border: none;
  background: linear-gradient(
    90deg,
    transparent 0%,
    var(--stark-border-visible) 20%,
    var(--stark-border-visible) 80%,
    transparent 100%
  );
  margin: var(--stark-space-xl) auto;
  max-width: 40%;
}
```

### Massive Whitespace Spacing

```css
/* Section spacing for the breath-filled layout */
.stark-section {
  padding: var(--stark-space-xl) var(--stark-space-md);
  max-width: 1200px;
  margin: 0 auto;
}

/* Hero section -- full viewport with bottom-weighted content */
.stark-hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding-bottom: var(--stark-space-xl);
  padding-left: var(--stark-space-lg);
  padding-right: var(--stark-space-lg);
}

/* Content block with breathing room */
.stark-content {
  max-width: 36em;
  margin-left: 10%;
  padding: var(--stark-space-lg) 0;
}

/* Wide spacing between grid items */
.stark-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: var(--stark-space-lg);
  padding: var(--stark-space-lg) 0;
}
```

### Thin Border and Divider Treatments

```css
/* Single-pixel border card */
.stark-bordered {
  border: 0.5px solid var(--stark-border);
  padding: var(--stark-space-lg);
  transition: border-color var(--stark-transition-base);
}

.stark-bordered:hover {
  border-color: var(--stark-border-visible);
}

/* Partial horizontal divider */
.stark-rule {
  width: 40px;
  height: 0.5px;
  background: var(--stark-border-visible);
  border: none;
  margin: var(--stark-space-lg) 0;
}

/* Vertical thin line accent */
.stark-vertical-accent {
  border-left: 0.5px solid var(--stark-accent-faded);
  padding-left: var(--stark-space-md);
}
```

### Button -- Minimal and Understated

```css
/* Resonant Stark button -- barely there until hovered */
.stark-button {
  display: inline-block;
  padding: 0.75rem 2.5rem;
  font-family: inherit;
  font-weight: 300;
  font-size: 0.8rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--stark-text-secondary);
  background: transparent;
  border: 0.5px solid var(--stark-border-visible);
  cursor: pointer;
  transition:
    color var(--stark-transition-fast),
    border-color var(--stark-transition-base),
    background var(--stark-transition-base),
    letter-spacing var(--stark-transition-base);
}

.stark-button:hover {
  color: var(--stark-accent);
  border-color: var(--stark-accent);
  background: var(--stark-accent-glow);
  letter-spacing: 0.14em;
}

.stark-button:active {
  background: var(--stark-accent-faded);
}

.stark-button:focus-visible {
  outline: 1px solid var(--stark-accent-faded);
  outline-offset: 4px;
}
```

### Smooth Number/Stat Display

```css
/* Large numeral as decorative anchor */
.stark-stat-number {
  font-weight: 100;
  font-size: clamp(4rem, 10vw, 8rem);
  line-height: 1;
  color: var(--stark-text-primary);
  letter-spacing: -0.03em;
  opacity: 0.9;
}

.stark-stat-label {
  font-weight: 300;
  font-size: 0.75rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--stark-text-tertiary);
  margin-top: var(--stark-space-xs);
}
```

### Subtle Image Treatment

```css
/* Images blend into the whitespace rather than demanding attention */
.stark-image {
  width: 100%;
  display: block;
  filter: grayscale(0.3) brightness(1.05) contrast(0.95);
  opacity: 0.9;
  transition:
    filter var(--stark-transition-slow),
    opacity var(--stark-transition-slow);
}

.stark-image:hover {
  filter: grayscale(0) brightness(1) contrast(1);
  opacity: 1;
}

/* Image with vast surrounding whitespace */
.stark-image-container {
  padding: var(--stark-space-xl) var(--stark-space-lg);
  max-width: 800px;
  margin: 0 auto;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical / Design Reference | Web Equivalent |
|------------------------------|----------------|
| Matte white museum wall | Near-white background (#FAFAFA) with no texture, gradient, or pattern; content floats on pure surface |
| Thin pencil line on paper | 0.5px borders in #E8E4E0 or #D4D0CC; barely visible structural lines that suggest rather than define |
| Natural linen or cotton | Warm off-white backgrounds (#F5F5F0) with optional subtle noise texture at 1-2% opacity |
| Japanese Ma (negative space) | Vast padding and margin (8-16rem between sections); whitespace as active design element |
| Gallery exhibition labels | Small uppercase text (0.75rem, 300 weight, 0.12em tracking) in tertiary gray for metadata and captions |
| Frosted glass panel | Background with `backdrop-filter: blur(20px)` and near-white semi-transparent fill for overlay elements |
| Hairline metal wire | Single-pixel accent lines in muted terracotta or sage; architectural rather than decorative |
| Warm halogen gallery light | Subtle radial gradient glow (`radial-gradient`) in faint accent color behind focal content |
| Pressed letterpress impression | Text in near-black (#1A1A18) at thin weight that feels subtly pressed into the white surface |
| Silk ribbon bookmark | Accent color (#C4836A) used as a single thin vertical or horizontal line marking a focal point |

---

## Imagery and Visual Content Guidelines

When creating or sourcing imagery for a Resonant Stark styled site:

- **Muted, desaturated photography** -- images should feel quiet; reduce saturation by 20-40% and slightly increase brightness
- **Generous whitespace around images** -- never edge-to-edge; images float in large padding containers
- **Minimal subjects** -- photographs of single objects, quiet landscapes, architectural details, or negative space compositions
- **Warm tone grading** -- slight warm color cast to match the cream-white palette; avoid cool blue tones
- **Grayscale or near-grayscale** -- many images work best in black-and-white or with heavy desaturation, with color reserved for hover states
- **No busy patterns or clutter** -- imagery should echo the whitespace philosophy; avoid crowded compositions
- **Soft focus and shallow depth of field** -- backgrounds blurred, single focal point, creating visual calm
- **Abstract and textural** -- surfaces, materials, light patterns, and shadows preferred over complex narrative scenes
- **Consistent aspect ratios** -- use a single aspect ratio (16:9 or 3:2) throughout for visual consistency
- **Hover-to-reveal color** -- images can display desaturated by default and transition to full color on hover, rewarding interaction
- **No decorative borders on images** -- images are bounded only by their own edges and surrounding whitespace

---

## Related Aesthetics

| Aesthetic | Relationship to Resonant Stark |
|-----------|-------------------------------|
| **Minimalism** | Direct ancestor; Resonant Stark adds emotional warmth and micro-interaction to minimalism's structural restraint |
| **Flat Design** | Shares rejection of ornamentation and skeuomorphism, but Resonant Stark uses depth through subtle shadow and animation rather than pure flatness |
| **Japandi** | Parallel philosophy combining Japanese Ma (negative space) with Scandinavian warmth; Resonant Stark is the digital expression |
| **Swiss/International** | Shares grid discipline and typographic focus, but Resonant Stark softens the rationalism with warm tones and organic animation |
| **Wabi-sabi** | Both find beauty in restraint and imperfection; Resonant Stark allows slight asymmetry and organic warmth within its precision |
| **Kinfolk** | Shares warm minimalist photography and generous whitespace, but Resonant Stark is more architecturally rigorous |

---

## Implementation Notes

- Resonant Stark is **warm minimalism, not cold minimalism**. Avoid pure white (#FFFFFF) backgrounds, blue-gray palettes, or sharp geometric precision. The warmth comes from off-white tones, warm grays, and organic transition timing. If the result feels clinical or corporate, add warmth.
- **Whitespace is the primary design element** -- resist the urge to fill empty space with content, decorations, or visual noise. If a layout does not feel uncomfortably sparse during development, there is not enough whitespace. The vast emptiness is what creates the emotional resonance.
- **Micro-interactions are essential** -- without hover effects and scroll reveals, the aesthetic collapses into plain emptiness. The subtle animations are what make the design feel alive rather than abandoned. Every interactive element should respond to attention.
- **Ultra-thin fonts require anti-aliasing** -- always use `-webkit-font-smoothing: antialiased` and `-moz-osx-font-smoothing: grayscale` to prevent thin type from appearing jagged. Test at multiple screen densities; thin fonts can vanish on low-DPI displays.
- **One accent color maximum** -- using multiple accent colors destroys the near-monochrome restraint. Choose one muted warm tone and use it sparingly (links, hover states, a single decorative line). If the accent feels prominent, it is overused.
- **Respect `prefers-reduced-motion`** -- the scroll and hover animations are central to the aesthetic, but accessibility requires honoring motion preferences. All animations must have reduced-motion fallbacks that show content immediately.
- **Performance matters** -- thin fonts, smooth transitions, and vast whitespace create an expectation of speed and polish. Any layout shift, font flash (FOUT), or janky animation shatters the illusion. Use `font-display: swap`, preload critical fonts, and ensure 60fps transitions.
- **Dark mode is challenging** -- the aesthetic is built on vast whitespace, which does not translate directly to dark backgrounds. If dark mode is required, use near-black (#0A0A08) with the same spatial principles, warm dark grays (#2A2A28), and the same muted accent. The result will feel different but can maintain the spatial philosophy.

---

## Quick-Start: Minimal Resonant Stark Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Resonant Stark</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400&display=swap" rel="stylesheet">
  <style>
    :root {
      --stark-bg-primary: #FAFAFA;
      --stark-bg-alt: #F5F5F0;
      --stark-bg-subtle: #F0EEEB;
      --stark-bg-surface: #E8E4E0;
      --stark-text-primary: #1A1A18;
      --stark-text-secondary: #6A6864;
      --stark-text-tertiary: #9A9894;
      --stark-text-faint: #B8B4B0;
      --stark-accent: #C4836A;
      --stark-accent-hover: #B07058;
      --stark-accent-faded: rgba(196, 131, 106, 0.12);
      --stark-accent-glow: rgba(196, 131, 106, 0.06);
      --stark-border: #E8E4E0;
      --stark-border-visible: #D0CCC8;
      --stark-shadow-subtle: rgba(26, 26, 24, 0.04);
      --stark-transition-fast: 0.3s ease;
      --stark-transition-base: 0.5s ease;
      --stark-transition-slow: 0.8s ease;
      --stark-space-xs: 0.5rem;
      --stark-space-sm: 1rem;
      --stark-space-md: 2rem;
      --stark-space-lg: 4rem;
      --stark-space-xl: 8rem;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--stark-bg-primary);
      color: var(--stark-text-secondary);
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      font-weight: 300;
      font-size: 17px;
      line-height: 1.8;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      overflow-x: hidden;
    }

    /* Navigation -- minimal, vast space */
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: var(--stark-space-md) var(--stark-space-lg);
      max-width: 1400px;
      margin: 0 auto;
    }

    .nav-logo {
      font-weight: 200;
      font-size: 0.85rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--stark-text-primary);
    }

    .nav-links {
      display: flex;
      gap: var(--stark-space-md);
      list-style: none;
    }

    .nav-links a {
      font-weight: 300;
      font-size: 0.75rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--stark-text-tertiary);
      text-decoration: none;
      border: none;
      transition:
        letter-spacing var(--stark-transition-base),
        color var(--stark-transition-fast);
    }

    .nav-links a:hover {
      letter-spacing: 0.14em;
      color: var(--stark-text-primary);
    }

    /* Hero -- full viewport, content at bottom */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      padding: 0 var(--stark-space-lg) var(--stark-space-xl);
      max-width: 1400px;
      margin: 0 auto;
    }

    .hero h1 {
      font-weight: 100;
      font-size: clamp(3.5rem, 8vw, 7rem);
      line-height: 1.08;
      letter-spacing: -0.02em;
      color: var(--stark-text-primary);
      max-width: 12em;
      margin-bottom: var(--stark-space-md);
    }

    .hero p {
      font-weight: 300;
      font-size: 1.1rem;
      line-height: 1.9;
      color: var(--stark-text-tertiary);
      max-width: 30em;
      margin-bottom: var(--stark-space-lg);
    }

    /* Divider -- partial width gradient line */
    .divider {
      height: 0.5px;
      border: none;
      background: linear-gradient(
        90deg,
        transparent 0%,
        var(--stark-border-visible) 20%,
        var(--stark-border-visible) 80%,
        transparent 100%
      );
      max-width: 30%;
      margin: var(--stark-space-xl) auto;
    }

    /* Section -- vast padding */
    .section {
      padding: var(--stark-space-xl) var(--stark-space-lg);
      max-width: 1400px;
      margin: 0 auto;
    }

    .section-label {
      font-weight: 300;
      font-size: 0.7rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--stark-text-faint);
      margin-bottom: var(--stark-space-lg);
    }

    .section h2 {
      font-weight: 200;
      font-size: clamp(2rem, 4.5vw, 3.2rem);
      line-height: 1.2;
      letter-spacing: 0.02em;
      color: var(--stark-text-primary);
      max-width: 16em;
      margin-bottom: var(--stark-space-md);
    }

    .section p {
      font-weight: 300;
      font-size: 1.0625rem;
      line-height: 1.85;
      color: var(--stark-text-secondary);
      max-width: 36em;
    }

    /* Card grid */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: var(--stark-space-lg);
      padding: var(--stark-space-lg) 0;
    }

    .card {
      padding: var(--stark-space-lg);
      border: 0.5px solid var(--stark-border);
      opacity: 0.8;
      transform: translateY(0);
      transition:
        opacity var(--stark-transition-base),
        transform var(--stark-transition-base),
        border-color var(--stark-transition-base);
    }

    .card:hover {
      opacity: 1;
      transform: translateY(-3px);
      border-color: var(--stark-border-visible);
    }

    .card-number {
      font-weight: 100;
      font-size: 3.5rem;
      line-height: 1;
      color: var(--stark-text-faint);
      margin-bottom: var(--stark-space-sm);
      transition: color var(--stark-transition-base);
    }

    .card:hover .card-number {
      color: var(--stark-accent);
    }

    .card h3 {
      font-weight: 300;
      font-size: 1.1rem;
      letter-spacing: 0.02em;
      color: var(--stark-text-primary);
      margin-bottom: var(--stark-space-xs);
    }

    .card p {
      font-size: 0.9rem;
      line-height: 1.7;
      color: var(--stark-text-tertiary);
      max-width: none;
    }

    /* Feature section with offset layout */
    .feature {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: var(--stark-space-xl);
      align-items: center;
      padding: var(--stark-space-xl) 0;
    }

    .feature-text {
      padding-right: var(--stark-space-lg);
    }

    .feature-visual {
      aspect-ratio: 4 / 3;
      background: linear-gradient(
        135deg,
        var(--stark-bg-alt) 0%,
        var(--stark-bg-subtle) 100%
      );
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .feature-visual span {
      font-weight: 100;
      font-size: 5rem;
      color: var(--stark-text-faint);
      opacity: 0.4;
    }

    /* Accent link */
    .accent-link {
      display: inline-block;
      font-weight: 300;
      font-size: 0.8rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--stark-accent);
      text-decoration: none;
      border: none;
      position: relative;
      margin-top: var(--stark-space-md);
      transition: letter-spacing var(--stark-transition-base);
    }

    .accent-link::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 0.5px;
      background: var(--stark-accent);
      transition: width var(--stark-transition-base);
    }

    .accent-link:hover {
      letter-spacing: 0.14em;
    }

    .accent-link:hover::after {
      width: 100%;
    }

    /* Footer -- minimal */
    footer {
      padding: var(--stark-space-xl) var(--stark-space-lg) var(--stark-space-lg);
      max-width: 1400px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      border-top: 0.5px solid var(--stark-border);
    }

    footer p {
      font-size: 0.75rem;
      color: var(--stark-text-faint);
      max-width: none;
    }

    /* Scroll reveal animations */
    .reveal {
      opacity: 0;
      transform: translateY(24px);
      transition:
        opacity 0.8s ease,
        transform 0.8s ease;
    }

    .reveal.is-visible {
      opacity: 1;
      transform: translateY(0);
    }

    .reveal-delay-1 { transition-delay: 0.1s; }
    .reveal-delay-2 { transition-delay: 0.2s; }
    .reveal-delay-3 { transition-delay: 0.3s; }

    /* Subtle background gradient for sections */
    .bg-gradient {
      background: linear-gradient(
        180deg,
        var(--stark-bg-primary) 0%,
        var(--stark-bg-alt) 50%,
        var(--stark-bg-primary) 100%
      );
    }

    /* Button */
    .stark-button {
      display: inline-block;
      padding: 0.8rem 2.8rem;
      font-family: inherit;
      font-weight: 300;
      font-size: 0.75rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--stark-text-secondary);
      background: transparent;
      border: 0.5px solid var(--stark-border-visible);
      cursor: pointer;
      text-decoration: none;
      transition:
        color var(--stark-transition-fast),
        border-color var(--stark-transition-base),
        background var(--stark-transition-base),
        letter-spacing var(--stark-transition-base);
    }

    .stark-button:hover {
      color: var(--stark-accent);
      border-color: var(--stark-accent);
      background: var(--stark-accent-glow);
      letter-spacing: 0.14em;
    }

    /* Reduced motion */
    @media (prefers-reduced-motion: reduce) {
      .reveal {
        opacity: 1;
        transform: none;
        transition: none;
      }
      *, *::before, *::after {
        transition-duration: 0.01ms !important;
        animation-duration: 0.01ms !important;
      }
    }

    /* Responsive */
    @media (max-width: 768px) {
      nav { padding: var(--stark-space-sm) var(--stark-space-md); }
      .hero { padding: 0 var(--stark-space-md) var(--stark-space-lg); }
      .section { padding: var(--stark-space-lg) var(--stark-space-md); }
      .feature { grid-template-columns: 1fr; gap: var(--stark-space-lg); }
      .feature-text { padding-right: 0; }
      footer { flex-direction: column; gap: var(--stark-space-sm); align-items: flex-start; }
    }
  </style>
</head>
<body>

  <nav>
    <span class="nav-logo">Resonant</span>
    <ul class="nav-links">
      <li><a href="#work">Work</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <h1 class="reveal">Clarity with feeling</h1>
    <p class="reveal reveal-delay-1">Purpose-driven minimalism where every element earns its place. Warmth lives in the whitespace, emotion in the quiet transitions between stillness and response.</p>
    <div class="reveal reveal-delay-2">
      <a href="#work" class="accent-link">Explore</a>
    </div>
  </section>

  <hr class="divider">

  <section class="section" id="work">
    <span class="section-label reveal">Selected Work</span>
    <h2 class="reveal">Designed to resonate,<br>built to endure</h2>

    <div class="card-grid">
      <div class="card reveal">
        <div class="card-number">01</div>
        <h3>Spatial Awareness</h3>
        <p>Understanding that what you remove matters more than what you add. Emptiness as the primary compositional tool.</p>
      </div>
      <div class="card reveal reveal-delay-1">
        <div class="card-number">02</div>
        <h3>Emotional Precision</h3>
        <p>Micro-interactions that reward attention. A shift in opacity, an expanding letter, a color that appears only when you look.</p>
      </div>
      <div class="card reveal reveal-delay-2">
        <div class="card-number">03</div>
        <h3>Tonal Warmth</h3>
        <p>Near-whites that lean cream rather than blue. Grays with warmth underneath. A palette that feels human despite its restraint.</p>
      </div>
    </div>
  </section>

  <section class="section bg-gradient">
    <div class="feature">
      <div class="feature-text reveal">
        <span class="section-label">Approach</span>
        <h2>Less, but with intention</h2>
        <p>Every element is questioned. Does it serve purpose? Does it earn its space? The result is not absence but presence -- each remaining element amplified by the silence surrounding it.</p>
        <a href="#" class="accent-link">Read more</a>
      </div>
      <div class="feature-visual reveal reveal-delay-1">
        <span>&mdash;</span>
      </div>
    </div>
  </section>

  <hr class="divider">

  <section class="section" id="about">
    <span class="section-label reveal">About</span>
    <h2 class="reveal">Stillness is not<br>the absence of life</h2>
    <p class="reveal reveal-delay-1">Resonant Stark finds the space between austerity and emotion. It is the held breath before speaking, the pause that gives weight to what follows. Design that trusts silence.</p>
    <div class="reveal reveal-delay-2" style="margin-top: var(--stark-space-lg);">
      <a href="#contact" class="stark-button">Get in touch</a>
    </div>
  </section>

  <footer>
    <p>&copy; 2026 Resonant Stark</p>
    <p>Purpose-driven minimalism</p>
  </footer>

  <script>
    // Scroll-triggered reveal animation
    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach((entry) => {
          if (entry.isIntersecting) {
            entry.target.classList.add('is-visible');
            observer.unobserve(entry.target);
          }
        });
      },
      { threshold: 0.15, rootMargin: '0px 0px -40px 0px' }
    );

    document.querySelectorAll('.reveal').forEach((el) => {
      observer.observe(el);
    });
  </script>

</body>
</html>
```
