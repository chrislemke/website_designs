# Duotone Design Reference

Duotone is a graphic design technique that reduces an image or composition to just two colors, mapping one to the shadows and another to the highlights. Rooted in the economics of print production -- where two-ink halftone processes could create striking, cost-effective reproductions -- duotone has evolved from a practical printing constraint into a deliberate, high-impact aesthetic choice. The technique gained modern digital prominence through Spotify's 2015 rebrand (designed by Collins), which applied bold, two-color overlays to artist photography and made the effect synonymous with contemporary music culture. In web and UI design, Duotone translates to dramatic color-washed imagery, high-contrast photography treatments, bold two-color palettes that unify disparate visual content under a single cohesive brand mood, and a graphic boldness that immediately commands attention. The power of duotone lies in subtraction: by removing color complexity, you amplify visual impact, create instant brand recognition, and force the viewer to engage with shape, contrast, and composition rather than photographic detail.

---

## Visual Characteristics

### Core Design Traits

- **Two-color image overlays** -- photographs processed so shadows map to one color and highlights to another, eliminating all other hues
- **High-contrast photography treatment** -- grayscale conversion followed by color mapping creates dramatic light-to-dark transitions
- **Bold graphic impact** -- the reduction to two colors transforms ordinary photos into poster-like graphic statements
- **Color-washed hero imagery** -- full-bleed background images drenched in a two-color gradient, unifying content and imagery
- **Complementary or analogous pairings** -- classic duotone palettes use colors with strong contrast (deep blue + bright coral) or tonal harmony (navy + teal)
- **Flat color fields alongside treated images** -- solid blocks of the two palette colors used for cards, sections, and UI elements
- **Strong silhouette emphasis** -- the removal of photographic detail forces attention onto the shapes and outlines of subjects
- **Gradient transitions between the two tones** -- smooth gradients flowing from the shadow color to the highlight color used in backgrounds and overlays
- **Halftone and dot-pattern textures** -- nods to the print origins of duotone, where the effect was created through halftone screening
- **Minimal additional color** -- white, black, or a single neutral may appear for text and UI chrome, but the two primary colors dominate everything

### Design Principles

- Restrict the palette ruthlessly -- the power of duotone comes from limitation, not variety
- Choose two colors with enough contrast to maintain legibility and visual depth across the full tonal range
- Use duotone treatment to unify visually diverse content (different photographs, illustrations) under one cohesive brand look
- Let the color pairing carry emotional weight -- warm pairs (orange + magenta) feel energetic, cool pairs (navy + cyan) feel sophisticated
- Preserve strong shapes and silhouettes in treated imagery; photos with clear subjects and good contrast work best
- Balance treated photography with clean typography and generous white space
- The two colors should serve distinct roles: one anchors the darks (grounding), the other illuminates the lights (energy)
- Avoid competing with the duotone effect -- keep UI elements simple so the color treatment remains the hero
- Gradients between the two colors are natural and encouraged; they are the visual signature of the technique
- Consider accessibility: ensure sufficient contrast ratios between the two colors for text overlays

---

## Color Palette

### Classic Duotone Palettes

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Midnight Indigo** | `#1A0533` | Primary dark / shadow mapping color |
| **Electric Coral** | `#FF6B6B` | Primary light / highlight mapping color |
| **Deep Navy** | `#0D1B3E` | Dark background, shadow tone alternative |
| **Vivid Magenta** | `#E91E8C` | Bright highlight, accent, CTA emphasis |
| **Ocean Teal** | `#0A7E8C` | Cool shadow tone for sophisticated palettes |
| **Sunlit Gold** | `#FFB347` | Warm highlight, optimistic energy |
| **Royal Purple** | `#6B2FA0` | Rich shadow, creative and luxurious feel |
| **Hot Pink** | `#FF3CAC` | Vibrant highlight, energetic and youthful |
| **Charcoal Slate** | `#2D2D3A` | Neutral dark for UI surfaces and panels |
| **Bone White** | `#F5F0EB` | Light background, text on dark surfaces |
| **Pure White** | `#FFFFFF` | Maximum highlight, text, chrome elements |
| **Near Black** | `#0A0A12` | Deepest background, footer, modal overlays |
| **Muted Lavender** | `#8B7FA8` | Secondary text, captions, subtle UI elements |
| **Soft Coral Tint** | `#FFD4D4` | Light accent, hover states, subtle highlights |

### CSS Custom Properties

```css
:root {
  /* Primary duotone pair (Dark + Light) */
  --duo-shadow: #1a0533;
  --duo-highlight: #ff6b6b;

  /* Alternative duotone pairs */
  --duo-pair2-shadow: #0d1b3e;
  --duo-pair2-highlight: #e91e8c;
  --duo-pair3-shadow: #0a7e8c;
  --duo-pair3-highlight: #ffb347;
  --duo-pair4-shadow: #6b2fa0;
  --duo-pair4-highlight: #ff3cac;

  /* Neutral foundations */
  --duo-bg-dark: #0a0a12;
  --duo-bg-surface: #2d2d3a;
  --duo-bg-light: #f5f0eb;
  --duo-white: #ffffff;

  /* Text */
  --duo-text-on-dark: #f5f0eb;
  --duo-text-on-light: #1a0533;
  --duo-text-muted: #8b7fa8;

  /* Gradients */
  --duo-gradient-primary: linear-gradient(135deg, #1a0533 0%, #ff6b6b 100%);
  --duo-gradient-vivid: linear-gradient(135deg, #0d1b3e 0%, #e91e8c 100%);
  --duo-gradient-warm: linear-gradient(135deg, #6b2fa0 0%, #ffb347 100%);
  --duo-gradient-cool: linear-gradient(135deg, #0a7e8c 0%, #ff6b6b 100%);

  /* Overlays */
  --duo-overlay-shadow: rgba(26, 5, 51, 0.85);
  --duo-overlay-highlight: rgba(255, 107, 107, 0.6);
}
```

---

## Typography

### Typeface Characteristics

Duotone typography is:

- **Bold and high-impact** -- large-scale headlines that match the graphic boldness of duotone imagery
- **Clean and geometric** -- sans-serif faces that do not compete with the color treatment for visual attention
- **High-contrast weight pairing** -- very bold headings against light-weight body text, echoing the two-tone contrast philosophy
- **Often uppercase for display** -- all-caps headlines with generous tracking for a poster-like presence
- **Minimal ornamentation** -- no serifs, scripts, or decorative faces; the color does the work, not the letterforms
- **Strong hierarchy** -- clear visual steps between heading sizes, using weight and scale rather than color variation

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Space Grotesk** | Geometric, contemporary | Headlines, hero text, strong display |
| **Sora** | Geometric, clean | Headlines, subheadings, modern feel |
| **Inter** | Neutral, highly legible | Body text, UI elements, versatile |
| **Manrope** | Geometric, friendly | Subheadings, body, approachable tone |
| **DM Sans** | Geometric, low contrast | Body text, labels, clean reading |
| **Plus Jakarta Sans** | Modern geometric | Headlines, subheadings, premium feel |
| **Archivo Black** | Ultra bold display | Large hero headlines, maximum impact |
| **Bebas Neue** | Condensed, tall display | Poster-style headlines, all-caps titles |
| **Work Sans** | Geometric, workmanlike | Body text, paragraphs, utility text |
| **Albert Sans** | Geometric, contemporary | Navigation, labels, small text |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Archivo Black** (400) | **Inter** (400) | Maximum graphic impact, clean body |
| **Bebas Neue** (400) | **DM Sans** (400) | Poster-bold headlines, elegant body |
| **Space Grotesk** (700) | **Manrope** (400) | Contemporary, geometric harmony |
| **Sora** (800) | **Work Sans** (400) | Modern boldness, readable body |
| **Plus Jakarta Sans** (800) | **Albert Sans** (400) | Premium, polished, startup aesthetic |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;700&family=Inter:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  color: var(--duo-text-on-dark);
  text-transform: uppercase;
  letter-spacing: 0.02em;
  line-height: 1.1;
}

/* Display / Hero text with duotone gradient */
.duo-display {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: -0.02em;
  line-height: 0.95;
  background: var(--duo-gradient-primary);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Solid color heading */
.duo-heading-highlight {
  font-family: 'Space Grotesk', sans-serif;
  color: var(--duo-highlight);
}

/* Body text */
body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--duo-text-on-dark);
}

/* Muted label */
.duo-label {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--duo-text-muted);
}

/* Large stat number */
.duo-stat-number {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(3rem, 6vw, 5rem);
  font-weight: 700;
  color: var(--duo-highlight);
  line-height: 1;
}
```

---

## Layout Principles

### Grid and Structure

- **Full-bleed duotone imagery** -- hero images span the entire viewport; the color treatment ties them seamlessly to the brand palette
- **Clean grid systems** -- 12-column or simple symmetric grids; the aesthetic favors order and structure over chaos
- **Generous white space** -- let the duotone images and bold typography breathe; avoid crowding
- **Large hero sections** -- 80-100vh hero areas with treated photography as the dominant visual
- **Alternating dark/light sections** -- sections alternate between the shadow color background and the highlight color or white, creating rhythm
- **Overlay text on images** -- duotone treatment reduces visual noise in photos enough to allow text directly on images with good legibility
- **Strong horizontal bands** -- content organized in clear, wide horizontal sections rather than complex multi-column layouts
- **Centered compositions** -- headlines and CTAs centered for maximum poster-like impact

### Section Organization

- **Navigation**: Clean, minimal bar with the two brand colors; logo in one tone, links in the other or in neutral
- **Hero**: Full-viewport duotone-treated photograph with large overlay headline and CTA button
- **Introduction**: Solid color background (shadow or highlight) with centered text block
- **Feature grid**: Cards or columns on a contrasting background; icons or images treated in the duotone palette
- **Image gallery**: Multiple photographs all processed with the same duotone filter for visual unity
- **Stats/Metrics**: Large numbers in the highlight color on the shadow color background
- **CTA section**: Gradient band flowing between the two tones with white text and a contrasting button
- **Footer**: Deepest shadow color background with muted text

### Responsive Approach

- Maintain duotone image treatments at all breakpoints -- they are CSS-driven and resolution-independent
- Scale hero text aggressively with `clamp()` for mobile readability
- Stack feature cards vertically on mobile; maintain consistent duotone styling
- Simplify gradient overlays on mobile if performance requires it
- Ensure the two-color palette reads clearly on small screens with sufficient contrast

---

## CSS / Design Techniques

### Duotone Card Component

```css
.duo-card {
  background: var(--duo-bg-surface);
  border: 1px solid rgba(255, 107, 107, 0.1);
  border-radius: 8px;
  padding: 32px;
  position: relative;
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.duo-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 20px 40px rgba(26, 5, 51, 0.4);
}

/* Accent gradient bar at top */
.duo-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: var(--duo-gradient-primary);
}

.duo-card__title {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  font-size: 1.15rem;
  color: var(--duo-highlight);
  margin-bottom: 12px;
}

.duo-card__text {
  color: var(--duo-text-muted);
  font-size: 0.95rem;
  line-height: 1.6;
}

/* Card grid layout */
.duo-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
}
```

### Duotone Button

```css
.duo-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--duo-highlight);
  color: var(--duo-shadow);
  border: none;
  border-radius: 6px;
  padding: 14px 36px;
  font-family: 'Space Grotesk', sans-serif;
  font-size: 0.9rem;
  font-weight: 700;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.25s ease;
  text-decoration: none;
}

.duo-button:hover {
  background: var(--duo-white);
  color: var(--duo-shadow);
  box-shadow: 0 8px 24px rgba(255, 107, 107, 0.3);
}

/* Outline variant */
.duo-button--outline {
  background: transparent;
  color: var(--duo-highlight);
  border: 2px solid var(--duo-highlight);
}

.duo-button--outline:hover {
  background: var(--duo-highlight);
  color: var(--duo-shadow);
}

/* Gradient variant */
.duo-button--gradient {
  background: var(--duo-gradient-primary);
  color: var(--duo-white);
  border: none;
}

.duo-button--gradient:hover {
  filter: brightness(1.15);
  box-shadow: 0 8px 24px rgba(26, 5, 51, 0.4);
}
```

### Navigation Bar

```css
.duo-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  position: relative;
  z-index: 10;
}

.duo-nav__logo {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 1.4rem;
  font-weight: 700;
  color: var(--duo-highlight);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.04em;
}

.duo-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.duo-nav__links a {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--duo-text-muted);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  transition: color 0.2s ease;
}

.duo-nav__links a:hover {
  color: var(--duo-highlight);
}

.duo-nav__links a.active {
  color: var(--duo-highlight);
}
```

### Hero Section with Duotone Image Overlay

```css
.duo-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 40px;
  overflow: hidden;
}

/* Background image (set via inline style or additional class) */
.duo-hero__image {
  position: absolute;
  inset: 0;
  background-size: cover;
  background-position: center;
  filter: grayscale(100%) contrast(1.2);
  z-index: 1;
}

/* Duotone color overlay using blend modes */
.duo-hero__overlay {
  position: absolute;
  inset: 0;
  background: var(--duo-gradient-primary);
  mix-blend-mode: color;
  z-index: 2;
}

/* Darkening layer for text legibility */
.duo-hero__darken {
  position: absolute;
  inset: 0;
  background: rgba(26, 5, 51, 0.3);
  z-index: 3;
}

.duo-hero__content {
  position: relative;
  z-index: 5;
  max-width: 800px;
}

.duo-hero__content h1 {
  font-size: clamp(3rem, 8vw, 6.5rem);
  margin-bottom: 1.5rem;
  color: var(--duo-white);
  letter-spacing: -0.02em;
}

.duo-hero__content p {
  font-size: 1.15rem;
  color: rgba(245, 240, 235, 0.8);
  margin-bottom: 2.5rem;
  max-width: 560px;
  margin-left: auto;
  margin-right: auto;
}

@media (max-width: 768px) {
  .duo-hero { min-height: auto; padding: 80px 20px; }
}
```

### CSS Blend Mode Duotone Effect

This technique uses CSS `mix-blend-mode` to create a duotone effect on any image without SVG filters. It layers a gradient over a grayscale image.

```css
/* Container for the duotone effect */
.duo-image-wrapper {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
}

/* The image itself, converted to grayscale and boosted contrast */
.duo-image-wrapper img {
  display: block;
  width: 100%;
  height: auto;
  filter: grayscale(100%) contrast(1.1);
}

/* Color overlay that creates the duotone effect */
.duo-image-wrapper::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(135deg, var(--duo-shadow) 0%, var(--duo-highlight) 100%);
  mix-blend-mode: color;
  pointer-events: none;
}

/* Alternative: single-color tint using multiply */
.duo-image-wrapper--multiply::after {
  background: var(--duo-highlight);
  mix-blend-mode: multiply;
}

/* Alternative: using screen blend for lighter effect */
.duo-image-wrapper--screen::after {
  background: var(--duo-shadow);
  mix-blend-mode: screen;
}

/* Hover reveal: show original image on hover */
.duo-image-wrapper--reveal img {
  transition: filter 0.4s ease;
}

.duo-image-wrapper--reveal:hover img {
  filter: grayscale(0%) contrast(1);
}

.duo-image-wrapper--reveal::after {
  transition: opacity 0.4s ease;
}

.duo-image-wrapper--reveal:hover::after {
  opacity: 0;
}
```

### SVG Filter Duotone Effect

This technique uses inline SVG filters with `feComponentTransfer` to create a true duotone mapping. This is the most accurate duotone method and mirrors how print duotone works -- mapping the grayscale range to two specific colors.

```html
<!-- Define the SVG filter (place once in the HTML, hidden) -->
<svg style="display: none;">
  <defs>
    <!-- Duotone: Midnight Indigo (#1A0533) to Electric Coral (#FF6B6B) -->
    <filter id="duotone-indigo-coral">
      <!-- Step 1: Convert to grayscale using luminance values -->
      <feColorMatrix type="matrix"
        values="0.33 0.33 0.33 0 0
                0.33 0.33 0.33 0 0
                0.33 0.33 0.33 0 0
                0    0    0    1 0" />
      <!-- Step 2: Map grayscale to two-color range -->
      <!-- Shadow: #1A0533 = rgb(26,5,51)  => 0.102, 0.020, 0.200 -->
      <!-- Highlight: #FF6B6B = rgb(255,107,107) => 1.000, 0.420, 0.420 -->
      <feComponentTransfer color-interpolation-filters="sRGB">
        <feFuncR type="table" tableValues="0.102 1.000" />
        <feFuncG type="table" tableValues="0.020 0.420" />
        <feFuncB type="table" tableValues="0.200 0.420" />
      </feComponentTransfer>
    </filter>

    <!-- Duotone: Deep Navy (#0D1B3E) to Vivid Magenta (#E91E8C) -->
    <filter id="duotone-navy-magenta">
      <feColorMatrix type="matrix"
        values="0.33 0.33 0.33 0 0
                0.33 0.33 0.33 0 0
                0.33 0.33 0.33 0 0
                0    0    0    1 0" />
      <feComponentTransfer color-interpolation-filters="sRGB">
        <feFuncR type="table" tableValues="0.051 0.914" />
        <feFuncG type="table" tableValues="0.106 0.118" />
        <feFuncB type="table" tableValues="0.243 0.549" />
      </feComponentTransfer>
    </filter>

    <!-- Duotone: Royal Purple (#6B2FA0) to Sunlit Gold (#FFB347) -->
    <filter id="duotone-purple-gold">
      <feColorMatrix type="matrix"
        values="0.33 0.33 0.33 0 0
                0.33 0.33 0.33 0 0
                0.33 0.33 0.33 0 0
                0    0    0    1 0" />
      <feComponentTransfer color-interpolation-filters="sRGB">
        <feFuncR type="table" tableValues="0.420 1.000" />
        <feFuncG type="table" tableValues="0.184 0.702" />
        <feFuncB type="table" tableValues="0.627 0.278" />
      </feComponentTransfer>
    </filter>
  </defs>
</svg>
```

```css
/* Apply SVG filter to images via CSS */
.duo-filter-indigo-coral {
  filter: url(#duotone-indigo-coral);
}

.duo-filter-navy-magenta {
  filter: url(#duotone-navy-magenta);
}

.duo-filter-purple-gold {
  filter: url(#duotone-purple-gold);
}

/* Hover to reveal original */
.duo-filter-reveal {
  transition: filter 0.4s ease;
}

.duo-filter-reveal:hover {
  filter: none;
}
```

### Duotone Gradient Text

```css
/* Gradient text using the duotone palette */
.duo-gradient-text {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  text-transform: uppercase;
  background: var(--duo-gradient-primary);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Animated gradient text */
.duo-gradient-text--animated {
  background-size: 200% 200%;
  animation: duo-text-shift 4s ease infinite;
}

@keyframes duo-text-shift {
  0%, 100% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
}
```

### Duotone Section Divider

```css
.duo-divider {
  border: none;
  height: 3px;
  background: var(--duo-gradient-primary);
  margin: 60px auto;
  max-width: 1200px;
}

/* Thin centered accent line */
.duo-divider--accent {
  max-width: 80px;
  height: 4px;
  border-radius: 2px;
  background: var(--duo-highlight);
  margin: 32px auto;
}
```

### Halftone Dot Pattern Overlay

A nod to the print origins of duotone, this creates a halftone dot texture using radial gradients.

```css
.duo-halftone {
  position: relative;
}

.duo-halftone::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: radial-gradient(
    circle,
    var(--duo-shadow) 1px,
    transparent 1px
  );
  background-size: 6px 6px;
  opacity: 0.15;
  pointer-events: none;
  mix-blend-mode: multiply;
}

/* Larger dot pattern for more visible texture */
.duo-halftone--large::after {
  background-image: radial-gradient(
    circle,
    var(--duo-shadow) 2px,
    transparent 2px
  );
  background-size: 10px 10px;
  opacity: 0.1;
}
```

### Palette Switcher (CSS-Only Theme Variations)

Since duotone is defined by its color pair, switching palettes is as simple as overriding two custom properties. This allows a single page to support multiple duotone moods.

```css
/* Default: Indigo + Coral */
:root {
  --duo-shadow: #1a0533;
  --duo-highlight: #ff6b6b;
}

/* Pair 2: Navy + Magenta */
[data-duo-theme="navy-magenta"] {
  --duo-shadow: #0d1b3e;
  --duo-highlight: #e91e8c;
  --duo-gradient-primary: linear-gradient(135deg, #0d1b3e 0%, #e91e8c 100%);
}

/* Pair 3: Purple + Gold */
[data-duo-theme="purple-gold"] {
  --duo-shadow: #6b2fa0;
  --duo-highlight: #ffb347;
  --duo-gradient-primary: linear-gradient(135deg, #6b2fa0 0%, #ffb347 100%);
}

/* Pair 4: Teal + Coral */
[data-duo-theme="teal-coral"] {
  --duo-shadow: #0a7e8c;
  --duo-highlight: #ff6b6b;
  --duo-gradient-primary: linear-gradient(135deg, #0a7e8c 0%, #ff6b6b 100%);
}

/* Pair 5: Charcoal + Electric Blue */
[data-duo-theme="charcoal-blue"] {
  --duo-shadow: #1a1a2e;
  --duo-highlight: #00d4ff;
  --duo-gradient-primary: linear-gradient(135deg, #1a1a2e 0%, #00d4ff 100%);
}
```

---

## Design Do's and Don'ts

### Do

- Limit your palette to exactly two colors (plus neutrals like white, black, or gray for text and UI chrome)
- Choose color pairs with strong tonal contrast so that shadows and highlights remain distinct and readable
- Apply duotone treatment consistently across all imagery to create visual cohesion
- Use CSS blend modes (`mix-blend-mode: color`) or SVG filters (`feComponentTransfer`) for scalable, resolution-independent effects
- Pair bold, geometric sans-serif typography with duotone imagery for maximum graphic impact
- Use the gradient between your two colors as a design element in backgrounds, dividers, and buttons
- Allow generous white space around duotone elements so the color treatment can breathe
- Select photographs with strong shapes, clear silhouettes, and good tonal range for the best duotone results
- Consider hover interactions that reveal the original full-color image, creating a satisfying contrast moment
- Test your two-color palette for WCAG accessibility -- text must remain legible on both tones

### Don't

- Introduce a third dominant color -- doing so breaks the duotone discipline and dilutes the visual impact
- Apply duotone to images with poor contrast or overly complex compositions -- the effect needs clear shapes to read well
- Use the same color for both shadows and highlights -- there must be sufficient contrast between the two
- Rely solely on `mix-blend-mode` without a grayscale base -- the image must be desaturated first for a true duotone
- Choose colors that are too similar in lightness -- the tonal mapping needs a clear light and dark pole
- Add heavy textures, patterns, or effects that compete with the duotone color treatment
- Use decorative, script, or serif typefaces that clash with the graphic boldness of the aesthetic
- Overuse halftone patterns -- they should be subtle textural accents, not dominant visual noise
- Forget to provide full-color alternatives for contexts where color accuracy matters (product photos, medical images)
- Apply duotone treatment inconsistently -- some images treated, others not -- within the same layout section

---

## Related Aesthetics

| Aesthetic | Relationship to Duotone |
|-----------|------------------------|
| **Monochrome** | Shares the limited palette philosophy; Monochrome uses one color plus black/white, Duotone uses exactly two |
| **Gradient Design** | Both rely on color transitions; Gradient design uses full spectrum, Duotone limits to a two-color gradient |
| **Swiss/International** | Shares clean grids and typographic boldness; Swiss design is color-neutral, Duotone is color-forward |
| **Pop Art** | Both use bold, limited color for graphic punch; Pop Art is playful and referential, Duotone is more refined |
| **Risograph** | Both reference limited-color print processes; Risograph embraces misregistration and texture, Duotone is clean and precise |
| **Brutalist Web** | Both favor bold visual impact; Brutalist is deliberately raw and chaotic, Duotone is controlled and polished |
| **Minimal** | Shares the principle of reduction; Minimalism reduces everything, Duotone specifically reduces color while amplifying it |
| **Vaporwave** | Both use color-processed imagery; Vaporwave is nostalgic and ironic with pastels, Duotone is contemporary and sincere |
| **Editorial** | Both favor strong typography and image treatment; Editorial uses full photography, Duotone transforms it |

---

## Quick-Start: Minimal Duotone Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Duotone Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --duo-shadow: #1a0533;
      --duo-highlight: #ff6b6b;
      --duo-bg-dark: #0a0a12;
      --duo-bg-surface: #2d2d3a;
      --duo-bg-light: #f5f0eb;
      --duo-white: #ffffff;
      --duo-text-on-dark: #f5f0eb;
      --duo-text-muted: #8b7fa8;
      --duo-gradient-primary: linear-gradient(135deg, #1a0533 0%, #ff6b6b 100%);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--duo-bg-dark);
      color: var(--duo-text-on-dark);
      font-family: 'Inter', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.02em;
      line-height: 1.1;
    }

    /* ---------- SVG Duotone Filters ---------- */
    .svg-filters { display: none; }

    /* ---------- Navigation ---------- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
      position: relative;
      z-index: 10;
    }

    nav a.logo {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 1.3rem;
      font-weight: 700;
      color: var(--duo-highlight);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.04em;
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'Inter', sans-serif;
      font-weight: 500;
      font-size: 0.9rem;
      color: var(--duo-text-muted);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      transition: color 0.2s ease;
    }

    nav ul a:hover { color: var(--duo-highlight); }

    /* ---------- Hero ---------- */
    .hero {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 92vh;
      padding: 80px 40px;
      overflow: hidden;
      background: var(--duo-bg-dark);
    }

    /* Abstract duotone background using layered gradients */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse 80% 60% at 30% 40%, rgba(26, 5, 51, 0.9) 0%, transparent 70%),
        radial-gradient(ellipse 70% 50% at 70% 60%, rgba(255, 107, 107, 0.4) 0%, transparent 70%),
        radial-gradient(ellipse 90% 70% at 50% 50%, rgba(26, 5, 51, 0.6) 0%, transparent 80%);
      z-index: 1;
    }

    /* Halftone texture overlay */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background-image: radial-gradient(circle, var(--duo-shadow) 1px, transparent 1px);
      background-size: 8px 8px;
      opacity: 0.08;
      pointer-events: none;
      z-index: 2;
    }

    .hero-content {
      position: relative;
      z-index: 5;
      max-width: 800px;
    }

    .hero h1 {
      font-size: clamp(3rem, 8vw, 6.5rem);
      margin-bottom: 1.5rem;
      color: var(--duo-white);
      letter-spacing: -0.02em;
    }

    .hero h1 span {
      background: var(--duo-gradient-primary);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero p {
      font-size: 1.15rem;
      color: rgba(245, 240, 235, 0.7);
      margin-bottom: 2.5rem;
      max-width: 540px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn {
      display: inline-block;
      background: var(--duo-highlight);
      color: var(--duo-shadow);
      border: none;
      border-radius: 6px;
      padding: 14px 36px;
      font-family: 'Space Grotesk', sans-serif;
      font-size: 0.9rem;
      font-weight: 700;
      letter-spacing: 0.04em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.25s ease;
    }

    .btn:hover {
      background: var(--duo-white);
      box-shadow: 0 8px 24px rgba(255, 107, 107, 0.3);
    }

    .btn--outline {
      background: transparent;
      color: var(--duo-highlight);
      border: 2px solid var(--duo-highlight);
      margin-left: 12px;
    }

    .btn--outline:hover {
      background: var(--duo-highlight);
      color: var(--duo-shadow);
    }

    /* ---------- Divider ---------- */
    .divider {
      border: none;
      height: 3px;
      background: var(--duo-gradient-primary);
      max-width: 1200px;
      margin: 0 auto;
    }

    /* ---------- Gallery (Duotone Images) ---------- */
    .gallery {
      padding: 80px 40px;
      background: var(--duo-shadow);
    }

    .gallery h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--duo-highlight);
      margin-bottom: 48px;
    }

    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .gallery-item {
      position: relative;
      overflow: hidden;
      border-radius: 8px;
      aspect-ratio: 4 / 3;
      background: var(--duo-bg-surface);
    }

    .gallery-item img {
      display: block;
      width: 100%;
      height: 100%;
      object-fit: cover;
      filter: url(#duotone-filter);
      transition: filter 0.4s ease;
    }

    .gallery-item:hover img {
      filter: none;
    }

    .gallery-item__label {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      padding: 16px 20px;
      background: linear-gradient(transparent, rgba(10, 10, 18, 0.8));
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      font-size: 0.85rem;
      color: var(--duo-white);
      text-transform: uppercase;
      letter-spacing: 0.04em;
      transform: translateY(100%);
      transition: transform 0.3s ease;
    }

    .gallery-item:hover .gallery-item__label {
      transform: translateY(0);
    }

    /* Placeholder gradient for demo (replaces actual images) */
    .gallery-placeholder {
      width: 100%;
      height: 100%;
      background: linear-gradient(135deg, var(--duo-shadow), var(--duo-highlight));
      opacity: 0.7;
    }

    /* ---------- Features ---------- */
    .features {
      padding: 80px 40px;
      background: var(--duo-bg-dark);
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--duo-white);
      margin-bottom: 12px;
    }

    .features .subtitle {
      text-align: center;
      color: var(--duo-text-muted);
      margin-bottom: 48px;
      font-size: 1rem;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .feature {
      background: var(--duo-bg-surface);
      border: 1px solid rgba(255, 107, 107, 0.08);
      border-radius: 8px;
      padding: 32px;
      position: relative;
      overflow: hidden;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .feature::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 3px;
      background: var(--duo-gradient-primary);
    }

    .feature:hover {
      transform: translateY(-4px);
      box-shadow: 0 16px 32px rgba(26, 5, 51, 0.4);
    }

    .feature-icon {
      width: 48px;
      height: 48px;
      border-radius: 12px;
      background: var(--duo-gradient-primary);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4rem;
      margin-bottom: 20px;
    }

    .feature h3 {
      font-size: 1.1rem;
      color: var(--duo-highlight);
      margin-bottom: 12px;
    }

    .feature p {
      color: var(--duo-text-muted);
      font-size: 0.95rem;
      line-height: 1.6;
    }

    /* ---------- Stats ---------- */
    .stats {
      padding: 60px 40px;
      background: var(--duo-shadow);
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 40px;
      max-width: 1000px;
      margin: 0 auto;
      text-align: center;
    }

    .stat-number {
      font-family: 'Space Grotesk', sans-serif;
      font-size: clamp(2.5rem, 5vw, 3.5rem);
      font-weight: 700;
      color: var(--duo-highlight);
      line-height: 1;
      margin-bottom: 8px;
    }

    .stat-label {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 0.75rem;
      font-weight: 500;
      color: var(--duo-text-muted);
      text-transform: uppercase;
      letter-spacing: 0.12em;
    }

    /* ---------- CTA ---------- */
    .cta {
      text-align: center;
      padding: 80px 40px;
      background: var(--duo-bg-dark);
      position: relative;
      overflow: hidden;
    }

    /* Gradient glow behind CTA */
    .cta::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 600px;
      height: 400px;
      background: radial-gradient(ellipse, rgba(255, 107, 107, 0.15) 0%, transparent 70%);
      pointer-events: none;
    }

    .cta h2 {
      font-size: clamp(1.8rem, 4vw, 2.5rem);
      color: var(--duo-white);
      margin-bottom: 1rem;
      position: relative;
    }

    .cta p {
      color: var(--duo-text-muted);
      margin-bottom: 2rem;
      max-width: 480px;
      margin-left: auto;
      margin-right: auto;
      position: relative;
    }

    /* ---------- Footer ---------- */
    footer {
      background: #06060c;
      text-align: center;
      padding: 30px 40px;
      color: var(--duo-text-muted);
      font-size: 0.85rem;
      border-top: 1px solid rgba(255, 107, 107, 0.08);
    }

    footer a {
      color: var(--duo-highlight);
      text-decoration: none;
    }

    /* ---------- Responsive ---------- */
    @media (max-width: 768px) {
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
      .hero { min-height: auto; padding: 60px 20px; }
      .gallery { padding: 60px 20px; }
      .features { padding: 60px 20px; }
      .stats { padding: 40px 20px; }
      .cta { padding: 60px 20px; }
    }
  </style>
</head>
<body>

  <!-- SVG Duotone Filter Definition -->
  <svg class="svg-filters">
    <defs>
      <filter id="duotone-filter">
        <feColorMatrix type="matrix"
          values="0.33 0.33 0.33 0 0
                  0.33 0.33 0.33 0 0
                  0.33 0.33 0.33 0 0
                  0    0    0    1 0" />
        <feComponentTransfer color-interpolation-filters="sRGB">
          <feFuncR type="table" tableValues="0.102 1.000" />
          <feFuncG type="table" tableValues="0.020 0.420" />
          <feFuncB type="table" tableValues="0.200 0.420" />
        </feComponentTransfer>
      </filter>
    </defs>
  </svg>

  <nav>
    <a href="#" class="logo">Chromatic</a>
    <ul>
      <li><a href="#">Work</a></li>
      <li><a href="#">Studio</a></li>
      <li><a href="#">Process</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Two Colors.<br><span>Infinite Impact.</span></h1>
      <p>Strip away the noise. Reduce to two tones. Watch everything come alive with bold, graphic clarity.</p>
      <a href="#" class="btn">Explore</a>
      <a href="#" class="btn btn--outline">Learn More</a>
    </div>
  </section>

  <hr class="divider">

  <section class="gallery">
    <h2>Selected Work</h2>
    <div class="gallery-grid">
      <div class="gallery-item">
        <div class="gallery-placeholder"></div>
        <div class="gallery-item__label">Brand Identity</div>
      </div>
      <div class="gallery-item">
        <div class="gallery-placeholder" style="background: linear-gradient(225deg, var(--duo-shadow), var(--duo-highlight));"></div>
        <div class="gallery-item__label">Editorial Design</div>
      </div>
      <div class="gallery-item">
        <div class="gallery-placeholder" style="background: linear-gradient(45deg, var(--duo-shadow), var(--duo-highlight));"></div>
        <div class="gallery-item__label">Campaign Art</div>
      </div>
    </div>
  </section>

  <section class="features">
    <h2>Our Process</h2>
    <p class="subtitle">Every project follows the same disciplined approach to color and contrast.</p>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon">01</div>
        <h3>Distill</h3>
        <p>We analyze your visual content and identify the two colors that best express your brand's emotional core and tonal range.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">02</div>
        <h3>Transform</h3>
        <p>Every image is processed through our duotone pipeline, mapping shadows and highlights to your chosen palette with precision.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">03</div>
        <h3>Unify</h3>
        <p>Disparate photography, illustration, and graphic elements merge into one cohesive visual language through shared color constraint.</p>
      </div>
    </div>
  </section>

  <section class="stats">
    <div class="stats-grid">
      <div>
        <div class="stat-number">2</div>
        <div class="stat-label">Colors. That's It.</div>
      </div>
      <div>
        <div class="stat-number">147</div>
        <div class="stat-label">Projects Delivered</div>
      </div>
      <div>
        <div class="stat-number">98%</div>
        <div class="stat-label">Brand Recall Rate</div>
      </div>
      <div>
        <div class="stat-number">3.2s</div>
        <div class="stat-label">Avg. Attention Hold</div>
      </div>
    </div>
  </section>

  <hr class="divider">

  <section class="cta">
    <h2>Ready to Reduce, Amplify, and Stand Out?</h2>
    <p>Two colors is all it takes to make an unforgettable impression. Let's find yours.</p>
    <a href="#" class="btn">Start a Project</a>
  </section>

  <footer>
    <p>Chromatic Studio &mdash; Bold design through disciplined color. <a href="#">hello@chromatic.studio</a></p>
  </footer>

</body>
</html>
```
