# Fitness Splatter Design Reference

Fitness Splatter (c. 2012--2017) is a graphic design aesthetic defined by the **visual deconstruction of human subjects -- typically dancers or athletes -- into geometric shards, low-poly triangles, and liquid ink splatters**. The style emerged during the global EDM boom and the gamification of fitness culture, becoming the default visual language for Zumba marketing, gym flyers, street dance competition posters, and high-tempo electronic music packaging (Hands Up, UK Hardcore, J-Core). The overall effect conveys movement so rapid that subjects appear to be "breaking the sound barrier or shedding their physical form." Fitness Splatter strategically bridges **corporate polish and street culture** -- vector-based and crisp elements (Adobe Illustrator-style) that mimic "messy" real-world textures, but with grit that is **sanitized, bright, and precisely placed for marketing impact**.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Low-poly shattering effect** -- human figures rendered as hundreds of geometric triangles across skin and clothing, creating a crystalline fragmentation
- **Liquid ink splatters** -- motion trails transformed into liquid drips, spray paint burns, or ink blots suggesting extreme velocity and kinetic energy
- **Chevrons and directional arrows** -- bold geometric directional indicators conveying forward motion and energy
- **Tech lines and circuit traces** -- thin geometric lines layered behind subjects to add depth and a digital/futuristic edge
- **Halftone dot patterns** -- screened overlays adding texture and a print-production feel to digital compositions
- **Grunge brushes and spray paint drips** -- urban texture elements applied with vector precision rather than true analog chaos
- **Sharp angular vector shapes** -- jagged, aggressive geometric fragments radiating outward from subjects
- **Speed lines and motion trails** -- directional streaks suggesting rapid movement and explosive energy
- **Particle dispersion** -- subjects dissolving at their edges into scattered geometric fragments or paint droplets

### Design Principles

- **Maximalist density** -- pack the maximum amount of visual noise (shards, colors, splatters) into the frame; more is more
- **Controlled chaos** -- every element appears wild and spontaneous but is precisely positioned for marketing impact and visual balance
- **Central figure dominance** -- a human subject (athlete, dancer) always anchors the composition at center or slight off-center
- **Radial energy explosion** -- visual elements radiate outward from the central figure, creating a "detonation" composition
- **Corporate-clean street grit** -- all grunge and splatter elements are vector-based, crisp, and deliberately placed rather than authentically messy
- **High contrast and visual urgency** -- neon hues against stark black or white backgrounds demand immediate attention
- **Layered depth planes** -- background tech lines, midground splatters, foreground subject, and top-layer geometric fragments create z-depth
- **Dynamic asymmetry** -- compositions lean into directional energy rather than static symmetry, suggesting movement frozen mid-explosion

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Background** | Pure black, near-black, stark white |
| **Primary neon accents** | Cyan, magenta, hot pink |
| **Secondary neon accents** | Lime green, electric yellow, hot orange |
| **Splatter/fragment tones** | Full CMYK neon spectrum in high saturation |
| **Text** | White on dark, black on light, neon accent for emphasis |

### Detailed Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Void Black | `#000000` | Primary dark background |
| Carbon Black | `#0A0A0A` | Slightly lifted dark backgrounds |
| Near Black | `#111111` | Card backgrounds, elevated dark surfaces |
| Pure White | `#FFFFFF` | Light backgrounds, high-contrast text |
| Off White | `#F5F5F5` | Softened light backgrounds |
| Neon Cyan | `#00E5FF` | Primary cool accent, shattering fragments |
| Electric Blue | `#2979FF` | Secondary cool accent, tech lines |
| Hot Magenta | `#FF00FF` | Primary warm-cool accent, splatter elements |
| Vivid Pink | `#FF1493` | High-energy accent, overlays |
| Hot Pink | `#FF0066` | Aggressive accent, call-to-action elements |
| Neon Lime | `#76FF03` | Primary green accent, energy indicators |
| Electric Yellow | `#FFEA00` | Bright accent, highlight fragments |
| Hot Orange | `#FF6D00` | Warm energy accent, secondary splatters |
| Laser Red | `#FF1744` | Aggressive warm accent, urgency elements |
| Deep Purple | `#AA00FF` | Supplemental accent, glow effects |
| Charcoal Gray | `#2A2A2A` | Subtle structural elements, muted backgrounds |
| Medium Gray | `#666666` | Secondary text, tech line details |
| Light Gray | `#CCCCCC` | Tertiary text, subtle borders |

### Suggested CSS Custom Properties

```css
:root {
  /* Base tones */
  --splatter-black: #000000;
  --splatter-carbon: #0a0a0a;
  --splatter-dark: #111111;
  --splatter-charcoal: #2a2a2a;
  --splatter-gray: #666666;
  --splatter-light-gray: #cccccc;
  --splatter-white: #ffffff;
  --splatter-off-white: #f5f5f5;

  /* Neon accents -- CMYK-adjacent */
  --splatter-cyan: #00e5ff;
  --splatter-blue: #2979ff;
  --splatter-magenta: #ff00ff;
  --splatter-pink: #ff1493;
  --splatter-hot-pink: #ff0066;
  --splatter-lime: #76ff03;
  --splatter-yellow: #ffea00;
  --splatter-orange: #ff6d00;
  --splatter-red: #ff1744;
  --splatter-purple: #aa00ff;

  /* Glow variants (semi-transparent for box-shadow/text-shadow) */
  --splatter-glow-cyan: rgba(0, 229, 255, 0.6);
  --splatter-glow-magenta: rgba(255, 0, 255, 0.6);
  --splatter-glow-lime: rgba(118, 255, 3, 0.6);
  --splatter-glow-pink: rgba(255, 0, 102, 0.6);

  /* Functional mappings */
  --splatter-bg-primary: var(--splatter-black);
  --splatter-bg-secondary: var(--splatter-dark);
  --splatter-bg-surface: var(--splatter-charcoal);
  --splatter-text-primary: var(--splatter-white);
  --splatter-text-secondary: var(--splatter-light-gray);
  --splatter-text-muted: var(--splatter-gray);
  --splatter-accent-1: var(--splatter-cyan);
  --splatter-accent-2: var(--splatter-magenta);
  --splatter-accent-3: var(--splatter-lime);
  --splatter-border: var(--splatter-charcoal);
}
```

### Palette Approaches

- **Neon-on-black dominance** -- the signature look pairs blazing neon hues against pitch-black backgrounds for maximum "color vibration"
- **CMYK trio core** -- cyan, magenta, and yellow form the foundational accent triad, referencing commercial print while reading as electric and digital
- **Full saturation, no pastels** -- colors are pushed to 100% saturation; muted or desaturated tones are avoided entirely
- **Multi-accent freedom** -- unlike minimal design, Fitness Splatter uses 3--5 neon accent colors simultaneously without restraint
- **Color as energy metaphor** -- brighter, more saturated colors concentrate around the central subject; fragments and splatters at the edges can shift hue
- **Stark contrast pairs** -- neon cyan on black, hot pink on white, lime on charcoal -- always high-contrast, never low-key

---

## Typography

### Typeface Characteristics

Fitness Splatter typography is bold, aggressive, and unapologetically loud:

- **Ultra-bold condensed sans-serifs** -- heavy, compressed display faces dominating the composition
- **All-caps everything** -- uppercase text is the default for all headings, taglines, and calls to action
- **Tight tracking, aggressive kerning** -- letters are packed close together, sometimes overlapping
- **Italic/slanted variants** -- forward-leaning text reinforcing the sense of speed and dynamic motion
- **Geometric/angular letterforms** -- typefaces with sharp corners and clean geometric construction
- **Text integrated with imagery** -- type placed over, under, and between the shattered figure elements
- **Neon-glow text treatments** -- text-shadow effects creating the impression of glowing signage
- **Stacked word compositions** -- multiple short words stacked vertically in different sizes for visual impact
- **Distressed or fragmented text** -- letterforms with pieces missing or edges dissolving into fragments, matching the shattered subject

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Bebas Neue** | Ultra-condensed bold sans | Hero titles, primary display text, event names |
| **Oswald** | Condensed sans-serif | Section headings, subheadings, navigation |
| **Anton** | Bold condensed display | Impact headlines, single-word callouts |
| **Black Ops One** | Military stencil display | Aggressive display headers, "extreme" emphasis |
| **Teko** | Condensed geometric sans | Secondary headings, stats, counters |
| **Rajdhani** | Semi-condensed tech sans | Body text, UI labels, metadata |
| **Orbitron** | Geometric/tech display | Futuristic accent text, tech-themed headings |
| **Saira Extra Condensed** | Ultra-narrow sans | Stacked word compositions, compact headlines |
| **Russo One** | Bold geometric display | Strong callout text, athletic branding |
| **Share Tech** | Technical sans-serif | Body text, descriptions, small print |

### Typography CSS Example

```css
/* Import Fitness Splatter fonts */
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Oswald:wght@400;500;600;700&family=Anton&family=Black+Ops+One&family=Teko:wght@400;500;600;700&family=Rajdhani:wght@400;500;600;700&family=Share+Tech&display=swap');

/* Hero / Display text -- maximum impact */
h1 {
  font-family: 'Bebas Neue', 'Anton', 'Arial Black', sans-serif;
  font-size: clamp(3rem, 10vw, 8rem);
  letter-spacing: 0.02em;
  line-height: 0.9;
  text-transform: uppercase;
  color: var(--splatter-white);
  text-shadow:
    0 0 10px var(--splatter-glow-cyan),
    0 0 40px var(--splatter-glow-cyan),
    0 0 80px rgba(0, 229, 255, 0.2);
}

/* Section headings -- condensed, bold, forward-leaning */
h2 {
  font-family: 'Oswald', 'Teko', sans-serif;
  font-weight: 700;
  font-size: clamp(1.8rem, 4vw, 3rem);
  text-transform: uppercase;
  letter-spacing: 0.05em;
  color: var(--splatter-white);
}

/* Subheadings with accent color */
h3 {
  font-family: 'Teko', 'Oswald', sans-serif;
  font-weight: 500;
  font-size: clamp(1.2rem, 2.5vw, 1.8rem);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--splatter-cyan);
}

/* Body text -- clean, technical, readable */
body {
  font-family: 'Rajdhani', 'Share Tech', 'Arial', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--splatter-text-secondary);
}

/* Aggressive callout / stat number */
.splatter-stat {
  font-family: 'Anton', 'Bebas Neue', sans-serif;
  font-size: clamp(4rem, 12vw, 10rem);
  text-transform: uppercase;
  color: var(--splatter-magenta);
  text-shadow:
    0 0 20px var(--splatter-glow-magenta),
    0 0 60px rgba(255, 0, 255, 0.3);
  line-height: 0.85;
}

/* Technical label / metadata */
.splatter-label {
  font-family: 'Share Tech', 'Rajdhani', sans-serif;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.25em;
  color: var(--splatter-gray);
}
```

---

## Layout Principles

### Grid and Structure

- **Edge-to-edge full-bleed** -- backgrounds and splatter elements extend to all viewport edges with no visible margin or frame
- **Central focal anchor** -- the hero figure or primary content element is positioned at center, with all energy radiating outward
- **Maximalist fill** -- every region of the layout is populated with fragments, splatters, tech lines, or color; empty space is minimal
- **Layered z-depth stacking** -- backgrounds, midground textures, subjects, foreground fragments, and UI text each occupy distinct visual planes
- **Responsive scaling through fluid typography** -- oversized display text uses `clamp()` for aggressive scaling from mobile to widescreen
- **Diagonal energy lines** -- layout elements, dividers, and decorative elements follow diagonal angles (typically 15--45 degrees) rather than pure horizontal/vertical
- **Overlapping elements** -- content panels, images, and text blocks deliberately overlap to create a collaged, energetic composition

### Section Organization

- Use **angular/diagonal dividers** between sections -- clip-path polygon dividers angled at 5--15 degrees rather than horizontal lines
- Apply **alternating color temperature** per section -- swap between cyan-dominant and magenta-dominant palettes to maintain visual energy
- Create **hierarchy through scale and glow** -- primary elements are massive and glow; secondary elements are smaller and matte
- Employ **fragmented section transitions** -- sections appear to shatter into one another with polygon clip-path effects
- Use **full-viewport hero sections** -- primary content areas take up 100vh with the subject figure and splatters filling the space
- Apply **tight vertical stacking** -- sections pack closely together with minimal padding, keeping energy levels high

---

## CSS/Design Techniques

### Neon Glow Text Effect

```css
/* Neon glow heading with multi-layered text-shadow */
.splatter-neon {
  color: var(--splatter-white);
  text-shadow:
    0 0 7px var(--splatter-cyan),
    0 0 10px var(--splatter-cyan),
    0 0 21px var(--splatter-cyan),
    0 0 42px var(--splatter-cyan),
    0 0 82px rgba(0, 229, 255, 0.4),
    0 0 92px rgba(0, 229, 255, 0.2);
}

/* Alternating neon color for emphasis words */
.splatter-neon-magenta {
  color: var(--splatter-white);
  text-shadow:
    0 0 7px var(--splatter-magenta),
    0 0 10px var(--splatter-magenta),
    0 0 21px var(--splatter-magenta),
    0 0 42px var(--splatter-magenta),
    0 0 82px rgba(255, 0, 255, 0.4);
}
```

### Shattered / Low-Poly Fragment Effect (CSS Clip-Path)

```css
/* Geometric fragment that appears to break off from content */
.splatter-fragment {
  position: absolute;
  width: 80px;
  height: 80px;
  background: linear-gradient(135deg, var(--splatter-cyan), var(--splatter-blue));
  clip-path: polygon(50% 0%, 100% 38%, 82% 100%, 18% 100%, 0% 38%);
  opacity: 0.7;
  transform: rotate(15deg);
  filter: blur(0.5px);
}

/* Triangular shard */
.splatter-shard {
  position: absolute;
  width: 60px;
  height: 60px;
  background: var(--splatter-magenta);
  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
  opacity: 0.5;
}

/* Diamond fragment */
.splatter-diamond {
  position: absolute;
  width: 40px;
  height: 40px;
  background: var(--splatter-lime);
  clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%);
  opacity: 0.6;
  transform: rotate(22deg);
}

/* Scatter multiple fragments around a container */
.splatter-scatter {
  position: relative;
  overflow: visible;
}

.splatter-scatter .splatter-shard:nth-child(1) { top: -20px; left: 10%; transform: rotate(25deg); }
.splatter-scatter .splatter-shard:nth-child(2) { top: 15%; right: -15px; transform: rotate(-40deg); }
.splatter-scatter .splatter-shard:nth-child(3) { bottom: -10px; left: 30%; transform: rotate(60deg); }
.splatter-scatter .splatter-diamond:nth-child(4) { top: 5%; left: -20px; transform: rotate(12deg); }
.splatter-scatter .splatter-diamond:nth-child(5) { bottom: 20%; right: 5%; transform: rotate(-30deg); }
```

### Diagonal Section Divider

```css
/* Angled section divider using clip-path */
.splatter-angle-divider {
  position: relative;
  margin-top: -5vw;
  padding-top: 5vw;
  clip-path: polygon(0 5vw, 100% 0, 100% 100%, 0 100%);
}

/* Double-angle zigzag divider */
.splatter-zigzag-divider {
  position: relative;
}

.splatter-zigzag-divider::before {
  content: '';
  position: absolute;
  top: -30px;
  left: 0;
  right: 0;
  height: 30px;
  background: var(--splatter-black);
  clip-path: polygon(
    0% 100%, 5% 0%, 10% 100%, 15% 0%, 20% 100%, 25% 0%,
    30% 100%, 35% 0%, 40% 100%, 45% 0%, 50% 100%, 55% 0%,
    60% 100%, 65% 0%, 70% 100%, 75% 0%, 80% 100%, 85% 0%,
    90% 100%, 95% 0%, 100% 100%
  );
}
```

### Ink Splatter / Paint Splash Effect (CSS Only)

```css
/* Paint splatter using layered radial gradients and box-shadows */
.splatter-ink {
  position: absolute;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: var(--splatter-cyan);
  box-shadow:
    /* Main splash */
    15px -8px 0 12px var(--splatter-cyan),
    -10px 15px 0 8px var(--splatter-cyan),
    25px 20px 0 5px var(--splatter-cyan),
    -20px -5px 0 10px var(--splatter-cyan),
    /* Secondary drips */
    40px 10px 0 3px var(--splatter-cyan),
    -35px 25px 0 4px var(--splatter-cyan),
    10px 40px 0 2px var(--splatter-cyan),
    -15px -30px 0 6px var(--splatter-cyan),
    /* Fine spray */
    50px -15px 0 1px var(--splatter-cyan),
    -45px 5px 0 2px var(--splatter-cyan),
    30px 35px 0 1px var(--splatter-cyan),
    -25px -25px 0 1px var(--splatter-cyan);
  filter: blur(0.5px);
}

/* Magenta splatter variant */
.splatter-ink-magenta {
  background: var(--splatter-magenta);
  box-shadow:
    12px -15px 0 8px var(--splatter-magenta),
    -18px 10px 0 12px var(--splatter-magenta),
    30px 5px 0 6px var(--splatter-magenta),
    -8px 25px 0 4px var(--splatter-magenta),
    22px -22px 0 3px var(--splatter-magenta),
    -30px -10px 0 7px var(--splatter-magenta),
    5px 35px 0 2px var(--splatter-magenta),
    -40px 20px 0 1px var(--splatter-magenta);
  filter: blur(0.5px);
}
```

### Halftone Dot Overlay

```css
/* Halftone screen overlay for sections */
.splatter-halftone::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: radial-gradient(circle, var(--splatter-white) 1px, transparent 1px);
  background-size: 6px 6px;
  opacity: 0.04;
  mix-blend-mode: overlay;
  pointer-events: none;
}
```

### Speed Lines / Motion Trail

```css
/* Horizontal speed lines behind content */
.splatter-speed-lines {
  position: relative;
}

.splatter-speed-lines::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 8px,
      rgba(0, 229, 255, 0.03) 8px,
      rgba(0, 229, 255, 0.03) 9px
    ),
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 22px,
      rgba(255, 0, 255, 0.02) 22px,
      rgba(255, 0, 255, 0.02) 23px
    );
  pointer-events: none;
}

/* Diagonal tech lines */
.splatter-tech-lines::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    repeating-linear-gradient(
      -30deg,
      transparent,
      transparent 40px,
      rgba(0, 229, 255, 0.05) 40px,
      rgba(0, 229, 255, 0.05) 41px
    ),
    repeating-linear-gradient(
      30deg,
      transparent,
      transparent 60px,
      rgba(255, 0, 255, 0.03) 60px,
      rgba(255, 0, 255, 0.03) 61px
    );
  pointer-events: none;
}
```

### Particle Explosion Animation

```css
/* Particle explosion effect using keyframes */
@keyframes splatter-explode {
  0% {
    transform: translate(0, 0) scale(1);
    opacity: 1;
  }
  100% {
    transform: translate(var(--tx, 100px), var(--ty, -80px)) scale(0.3);
    opacity: 0;
  }
}

.splatter-particle {
  position: absolute;
  width: 8px;
  height: 8px;
  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
  animation: splatter-explode 2s ease-out infinite;
}

.splatter-particle:nth-child(1) { --tx: 120px; --ty: -90px; background: var(--splatter-cyan); animation-delay: 0s; }
.splatter-particle:nth-child(2) { --tx: -80px; --ty: -120px; background: var(--splatter-magenta); animation-delay: 0.2s; }
.splatter-particle:nth-child(3) { --tx: 150px; --ty: 40px; background: var(--splatter-lime); animation-delay: 0.4s; }
.splatter-particle:nth-child(4) { --tx: -130px; --ty: 60px; background: var(--splatter-yellow); animation-delay: 0.1s; }
.splatter-particle:nth-child(5) { --tx: 60px; --ty: -150px; background: var(--splatter-orange); animation-delay: 0.3s; }
.splatter-particle:nth-child(6) { --tx: -100px; --ty: -50px; background: var(--splatter-pink); animation-delay: 0.5s; }
```

### Chevron / Arrow Accent

```css
/* Directional chevron accent */
.splatter-chevron {
  display: inline-block;
  width: 0;
  height: 0;
  border-left: 15px solid transparent;
  border-right: 15px solid transparent;
  border-bottom: 25px solid var(--splatter-cyan);
  transform: rotate(-90deg);
  opacity: 0.6;
}

/* Stacked repeating chevrons */
.splatter-chevrons {
  display: flex;
  gap: 4px;
}

.splatter-chevrons::before,
.splatter-chevrons::after {
  content: '';
  display: block;
  width: 20px;
  height: 20px;
  border-right: 3px solid var(--splatter-cyan);
  border-bottom: 3px solid var(--splatter-cyan);
  transform: rotate(-45deg);
}

.splatter-chevrons::after {
  border-color: rgba(0, 229, 255, 0.4);
}
```

### Neon Glow Card / Panel

```css
.splatter-card {
  background: var(--splatter-dark);
  border: 1px solid rgba(0, 229, 255, 0.2);
  padding: 2rem;
  position: relative;
  overflow: hidden;
  clip-path: polygon(0 0, calc(100% - 20px) 0, 100% 20px, 100% 100%, 20px 100%, 0 calc(100% - 20px));
  box-shadow:
    0 0 15px rgba(0, 229, 255, 0.1),
    inset 0 0 30px rgba(0, 0, 0, 0.5);
  transition: border-color 0.3s, box-shadow 0.3s;
}

.splatter-card:hover {
  border-color: rgba(0, 229, 255, 0.5);
  box-shadow:
    0 0 25px rgba(0, 229, 255, 0.2),
    inset 0 0 30px rgba(0, 0, 0, 0.5);
}

/* Corner accent marks */
.splatter-card::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 20px;
  height: 20px;
  background: var(--splatter-cyan);
  clip-path: polygon(100% 0, 0 0, 100% 100%);
  opacity: 0.4;
}
```

### Splatter Button

```css
.splatter-button {
  display: inline-block;
  padding: 0.8rem 2.5rem;
  font-family: 'Bebas Neue', 'Oswald', sans-serif;
  font-size: 1.1rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--splatter-white);
  background: transparent;
  border: 2px solid var(--splatter-cyan);
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: all 0.2s ease;
  clip-path: polygon(0 0, calc(100% - 12px) 0, 100% 12px, 100% 100%, 12px 100%, 0 calc(100% - 12px));
}

.splatter-button:hover {
  background: var(--splatter-cyan);
  color: var(--splatter-black);
  box-shadow:
    0 0 20px var(--splatter-glow-cyan),
    0 0 40px rgba(0, 229, 255, 0.2);
}

.splatter-button:active {
  transform: scale(0.97);
  box-shadow: 0 0 10px var(--splatter-glow-cyan);
}

/* Magenta variant */
.splatter-button--magenta {
  border-color: var(--splatter-magenta);
}

.splatter-button--magenta:hover {
  background: var(--splatter-magenta);
  box-shadow:
    0 0 20px var(--splatter-glow-magenta),
    0 0 40px rgba(255, 0, 255, 0.2);
}
```

### Color Blend / Overlay Effect for Images

```css
/* Apply neon color overlay to grayscale images */
.splatter-image-overlay {
  position: relative;
  display: inline-block;
}

.splatter-image-overlay img {
  display: block;
  filter: grayscale(1) contrast(1.3) brightness(0.8);
}

.splatter-image-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(
    135deg,
    rgba(0, 229, 255, 0.3) 0%,
    rgba(255, 0, 255, 0.3) 50%,
    rgba(118, 255, 3, 0.2) 100%
  );
  mix-blend-mode: color;
  pointer-events: none;
}

/* High-contrast duotone treatment */
.splatter-duotone {
  filter: grayscale(1) contrast(1.5) brightness(1.1);
  mix-blend-mode: luminosity;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Fitness Splatter elements and their web equivalents:

| Physical Element | Web Equivalent |
|------------------|----------------|
| Shattered glass / crystal | CSS `clip-path: polygon()` fragments with semi-transparent neon fills and `backdrop-filter: blur()` |
| Spray paint splatters | Layered `box-shadow` clusters with `border-radius: 50%` on small elements, varying sizes |
| Low-poly mesh | SVG polygon fills with adjacent triangles in shifting hue values |
| Neon signage glow | Multi-layered `text-shadow` with increasing blur radius on neon color values |
| Ink drips and runs | CSS gradients with irregular `clip-path` or SVG paths along vertical axis |
| Halftone print screen | `radial-gradient` dot patterns at small `background-size` with low opacity overlay |
| Tech circuitry lines | Thin `border` or `outline` elements at 30-60 degree angles using `transform: rotate()` |
| Holographic foil | `background: linear-gradient()` with multiple color stops animating `background-position` |
| Smoke / fog trails | Large `box-shadow` with heavy blur and low opacity on neon-colored pseudo-elements |
| Energy burst / flare | `radial-gradient` from neon center to transparent, combined with `mix-blend-mode: screen` |

---

## Cultural References and Influences

The following define the Fitness Splatter visual language and serve as design references:

- **Zumba Fitness marketing materials** (2012--2017) -- the canonical Fitness Splatter application; neon-drenched dancers exploding into geometric fragments
- **Ravemania Speed compilation covers** (2016--2017) -- album artwork featuring shattered dancers with maximum color density
- **Street dance competition posters** -- high-energy promotional materials for breakdance, hip-hop, and freestyle events
- **Gym and dance studio flyers** -- mass-produced using stock Envato/GraphicRiver templates with customizable splatter effects
- **UK Hardcore and J-Core album covers** -- high-tempo electronic music packaging pushing the fragmented-figure aesthetic to its extreme
- **EDM YouTube thumbnail art** -- high-saturation, attention-grabbing compositions designed for small-format visibility
- **Nike/Adidas athletic marketing** (2013--2016) -- commercial sports advertising borrowing the shattered-athlete visual language

### Design Tool Context

Fitness Splatter was produced almost exclusively using:

- **Adobe Illustrator** -- vector-based geometric shards, clean polygon construction, crisp splatter brushes
- **Adobe Photoshop** -- compositing, layer blending modes, halftone filters, glow effects
- **Envato GraphicRiver templates** -- pre-made action/template packs democratized the style for small gyms and event promoters

---

## Related Aesthetics

| Aesthetic | Relationship to Fitness Splatter |
|-----------|----------------------------------|
| **Vectordelia** | Predecessor focusing on smooth, organic curves and gradients; Fitness Splatter replaces organic curves with angular shattering |
| **Avantropop** | Shares the neon-bright, high-energy sensibility but with more pop-art influence and less geometric fragmentation |
| **Colorful Pop** | Similar maximum-saturation palette philosophy; Colorful Pop is flatter and more illustrative while Fitness Splatter is photographic and dimensional |
| **Hands Up** | Musical genre counterpart; the Hands Up EDM scene uses Fitness Splatter visuals extensively for album and event art |
| **Hexatron** | Shares geometric/hexagonal fragmentation; Hexatron is more sci-fi and digital, less athletic and kinetic |
| **Corporate Memphis** | Opposite design philosophy; where Corporate Memphis is flat, minimal, and muted, Fitness Splatter is textured, maximal, and neon |
| **Vaporwave** | Both use neon colors but for completely different purposes; Vaporwave is nostalgic and ironic, Fitness Splatter is earnest and high-energy |

---

## Quick-Start: Minimal Fitness Splatter Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fitness Splatter Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Oswald:wght@400;600;700&family=Anton&family=Teko:wght@400;500;600&family=Rajdhani:wght@400;500;600&family=Share+Tech&display=swap" rel="stylesheet">
  <style>
    :root {
      --splatter-black: #000000;
      --splatter-dark: #111111;
      --splatter-charcoal: #2a2a2a;
      --splatter-gray: #666666;
      --splatter-light-gray: #cccccc;
      --splatter-white: #ffffff;
      --splatter-cyan: #00e5ff;
      --splatter-magenta: #ff00ff;
      --splatter-lime: #76ff03;
      --splatter-yellow: #ffea00;
      --splatter-orange: #ff6d00;
      --splatter-pink: #ff0066;
      --splatter-glow-cyan: rgba(0, 229, 255, 0.6);
      --splatter-glow-magenta: rgba(255, 0, 255, 0.6);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--splatter-black);
      color: var(--splatter-light-gray);
      font-family: 'Rajdhani', 'Share Tech', Arial, sans-serif;
      font-weight: 400;
      line-height: 1.6;
      overflow-x: hidden;
    }

    /* Tech line background overlay */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background:
        repeating-linear-gradient(
          -30deg,
          transparent,
          transparent 60px,
          rgba(0, 229, 255, 0.03) 60px,
          rgba(0, 229, 255, 0.03) 61px
        ),
        repeating-linear-gradient(
          30deg,
          transparent,
          transparent 80px,
          rgba(255, 0, 255, 0.02) 80px,
          rgba(255, 0, 255, 0.02) 81px
        );
      pointer-events: none;
      z-index: 1;
    }

    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 4rem 2rem;
      position: relative;
      background:
        radial-gradient(ellipse at 30% 50%, rgba(0, 229, 255, 0.08) 0%, transparent 50%),
        radial-gradient(ellipse at 70% 50%, rgba(255, 0, 255, 0.08) 0%, transparent 50%),
        var(--splatter-black);
    }

    .hero h1 {
      font-family: 'Bebas Neue', 'Anton', sans-serif;
      font-size: clamp(4rem, 12vw, 10rem);
      letter-spacing: 0.02em;
      line-height: 0.9;
      text-transform: uppercase;
      color: var(--splatter-white);
      text-shadow:
        0 0 10px var(--splatter-glow-cyan),
        0 0 40px var(--splatter-glow-cyan),
        0 0 80px rgba(0, 229, 255, 0.15);
      position: relative;
      z-index: 2;
    }

    .hero h1 span {
      color: var(--splatter-magenta);
      text-shadow:
        0 0 10px var(--splatter-glow-magenta),
        0 0 40px var(--splatter-glow-magenta);
    }

    .hero p {
      font-family: 'Share Tech', sans-serif;
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.3em;
      color: var(--splatter-gray);
      margin-top: 1.5rem;
      position: relative;
      z-index: 2;
    }

    /* Decorative fragments in hero */
    .fragment {
      position: absolute;
      opacity: 0.4;
      z-index: 0;
    }
    .fragment--1 {
      top: 15%; left: 8%;
      width: 50px; height: 50px;
      background: var(--splatter-cyan);
      clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
      transform: rotate(20deg);
    }
    .fragment--2 {
      top: 25%; right: 12%;
      width: 35px; height: 35px;
      background: var(--splatter-magenta);
      clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%);
      transform: rotate(-15deg);
    }
    .fragment--3 {
      bottom: 20%; left: 15%;
      width: 60px; height: 60px;
      background: var(--splatter-lime);
      clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
      transform: rotate(35deg);
      opacity: 0.3;
    }
    .fragment--4 {
      bottom: 30%; right: 8%;
      width: 40px; height: 40px;
      background: var(--splatter-yellow);
      clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
      transform: rotate(-40deg);
      opacity: 0.25;
    }

    /* Angled section divider */
    .angle-divider {
      height: 5vw;
      background: var(--splatter-dark);
      clip-path: polygon(0 0, 100% 100%, 0 100%);
      margin-top: -1px;
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      position: relative;
      z-index: 2;
    }

    section h2 {
      font-family: 'Oswald', 'Teko', sans-serif;
      font-weight: 700;
      font-size: clamp(1.8rem, 4vw, 3rem);
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--splatter-white);
      margin-bottom: 1.5rem;
      padding-left: 1rem;
      border-left: 4px solid var(--splatter-cyan);
    }

    .splatter-card {
      background: var(--splatter-dark);
      border: 1px solid rgba(0, 229, 255, 0.15);
      padding: 2rem;
      margin: 1.5rem 0;
      position: relative;
      clip-path: polygon(0 0, calc(100% - 16px) 0, 100% 16px, 100% 100%, 16px 100%, 0 calc(100% - 16px));
      box-shadow: 0 0 15px rgba(0, 229, 255, 0.05);
    }

    .splatter-card h3 {
      font-family: 'Teko', sans-serif;
      font-weight: 500;
      font-size: 1.4rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--splatter-cyan);
      margin-bottom: 0.5rem;
    }

    .splatter-button {
      display: inline-block;
      padding: 0.8rem 2.5rem;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.1rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      text-decoration: none;
      color: var(--splatter-white);
      background: transparent;
      border: 2px solid var(--splatter-cyan);
      cursor: pointer;
      transition: all 0.2s ease;
      clip-path: polygon(0 0, calc(100% - 10px) 0, 100% 10px, 100% 100%, 10px 100%, 0 calc(100% - 10px));
    }

    .splatter-button:hover {
      background: var(--splatter-cyan);
      color: var(--splatter-black);
      box-shadow: 0 0 20px var(--splatter-glow-cyan);
    }

    a {
      color: var(--splatter-cyan);
      text-decoration: none;
      border-bottom: 1px solid rgba(0, 229, 255, 0.3);
      transition: color 0.15s;
    }

    a:hover {
      color: var(--splatter-magenta);
      border-bottom-color: rgba(255, 0, 255, 0.3);
    }

    .label {
      font-family: 'Share Tech', sans-serif;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.25em;
      color: var(--splatter-gray);
    }
  </style>
</head>
<body>
  <div class="hero">
    <div class="fragment fragment--1"></div>
    <div class="fragment fragment--2"></div>
    <div class="fragment fragment--3"></div>
    <div class="fragment fragment--4"></div>
    <h1>Break <span>Limits</span></h1>
    <p>Shatter every boundary</p>
  </div>
  <div class="angle-divider"></div>
  <section>
    <h2>Maximum Energy</h2>
    <div class="splatter-card">
      <span class="label">High intensity</span>
      <h3>Explosive Performance</h3>
      <p>Content styled with the Fitness Splatter aesthetic. Neon accents, geometric fragments, high-contrast urgency against a dark void.</p>
      <br>
      <a href="#" class="splatter-button">Engage</a>
    </div>
  </section>
</body>
</html>
```
