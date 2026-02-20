# Kinetic Typography Design Reference

Kinetic Typography is a motion-driven design aesthetic where animated text serves as the primary visual element, transforming words from static information carriers into expressive, dynamic experiences. Rooted in the opening title sequences of 1950s cinema -- most notably Saul Bass's work on Alfred Hitchcock's *North by Northwest* (1959) -- kinetic typography treats letterforms as choreographed performers: they scale, rotate, split, morph, bounce, fade, and flow across the screen in rhythm with narrative or user interaction. In web and UI design, this aesthetic translates to scroll-triggered text reveals, variable font animations, letter-by-letter staggered entrances, headline text that "breathes" on hover, and layouts where typography itself is the hero imagery. The philosophy is clear: when words move with purpose, they communicate emotion, hierarchy, and energy far beyond what static text can achieve.

---

## Visual Characteristics

### Core Design Traits

- **Motion as primary visual language** -- text animation replaces static imagery as the dominant design element; words are the hero, not decoration
- **Staggered letter entrances** -- individual characters animate into view with calculated delays, creating a rhythmic cascade effect
- **Scroll-triggered text reveals** -- headlines, paragraphs, and display text animate in response to scroll position, turning the page into a cinematic sequence
- **Variable font axis transitions** -- weight, width, slant, and optical size shift fluidly through CSS or JavaScript, making type feel alive
- **Split-text decomposition** -- words broken into individual characters or lines, each independently animated for granular motion control
- **High-contrast type on dark canvases** -- bold white or accent-colored text on deep black or near-black backgrounds for maximum visual impact
- **Generous whitespace** -- large empty areas surrounding animated text ensure focus remains on the motion and the message
- **Oversized display type** -- headlines at extreme scale (often 10-20vw) that dominate the viewport and command attention
- **Minimal ornamentation** -- imagery, icons, and decorative elements are reduced or eliminated so that the typography carries the full visual weight
- **Rhythmic pacing** -- animation timing follows deliberate cadences with easing curves that feel natural and intentional, not mechanical
- **Clip-path and mask reveals** -- text revealed through animated masks, sliding panels, or geometric clip-paths that create theatrical unveiling effects
- **Horizontal scroll marquees** -- continuous text tickers running across the screen, often at large scale, as a background texture or navigation element

### Design Principles

- Type is the hero -- every design decision should serve the legibility, impact, and expressiveness of the text
- Motion must have purpose -- every animation should convey meaning, establish hierarchy, or guide the user's eye; never animate for decoration alone
- Timing is everything -- the rhythm, duration, and easing of animations are as important as the visual design itself
- Balance motion with rest -- provide static moments and visual pauses so constant movement does not overwhelm the viewer
- Dark backgrounds amplify text presence -- deep, neutral canvases let animated letterforms command the full visual field
- Respect readability -- no matter how dramatic the animation, the text must be legible at the moment it matters most
- Performance is a design constraint -- animations must run at 60fps; favor GPU-accelerated properties (transform, opacity) over layout-triggering ones
- Honor user preferences -- always implement `prefers-reduced-motion` to provide a static fallback for users who are sensitive to animation
- Less content, more impact -- kinetic typography thrives with concise, punchy copy; fewer words animated well outperform many words animated poorly
- Create a sense of narrative -- sequences of animated text should feel like a story unfolding, with beginning, development, and resolution

---

## Color Palette

### Motion Type Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Void Black** | `#0A0A0A` | Primary background, deepest canvas |
| **Deep Charcoal** | `#141414` | Secondary background, elevated surfaces |
| **Carbon** | `#1E1E1E` | Card backgrounds, panel surfaces |
| **Graphite** | `#2A2A2A` | Tertiary surfaces, subtle contrast |
| **Pure White** | `#FFFFFF` | Primary display text, maximum contrast |
| **Soft White** | `#E8E8E8` | Body text, readable content |
| **Silver** | `#A0A0A0` | Secondary text, captions, muted content |
| **Medium Gray** | `#666666` | Tertiary text, timestamps, metadata |
| **Electric Blue** | `#2D5BFF` | Primary accent, interactive elements, CTAs |
| **Vivid Coral** | `#FF4D4D` | Secondary accent, emphasis, alerts |
| **Neon Green** | `#00FF88` | Success states, highlight accents |
| **Amber** | `#FFB800` | Warning states, warm accents |
| **Deep Indigo** | `#1A1A3E` | Dark accent background, gradient base |
| **Faded Lavender** | `#8888AA` | Decorative text, watermarks, ghost elements |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --kt-bg-void: #0a0a0a;
  --kt-bg-deep: #141414;
  --kt-bg-carbon: #1e1e1e;
  --kt-bg-graphite: #2a2a2a;

  /* Text */
  --kt-text-primary: #ffffff;
  --kt-text-body: #e8e8e8;
  --kt-text-secondary: #a0a0a0;
  --kt-text-muted: #666666;

  /* Accents */
  --kt-accent-blue: #2d5bff;
  --kt-accent-coral: #ff4d4d;
  --kt-accent-green: #00ff88;
  --kt-accent-amber: #ffb800;

  /* Decorative */
  --kt-deep-indigo: #1a1a3e;
  --kt-faded-lavender: #8888aa;

  /* Gradients */
  --kt-gradient-text: linear-gradient(135deg, #ffffff 0%, #a0a0a0 100%);
  --kt-gradient-accent: linear-gradient(135deg, #2d5bff 0%, #ff4d4d 100%);
  --kt-gradient-dark: linear-gradient(180deg, #0a0a0a 0%, #1a1a3e 100%);
  --kt-gradient-reveal: linear-gradient(90deg, transparent 0%, #0a0a0a 100%);

  /* Animation timing */
  --kt-ease-out-expo: cubic-bezier(0.16, 1, 0.3, 1);
  --kt-ease-out-back: cubic-bezier(0.34, 1.56, 0.64, 1);
  --kt-ease-in-out: cubic-bezier(0.65, 0, 0.35, 1);
  --kt-duration-fast: 0.3s;
  --kt-duration-normal: 0.6s;
  --kt-duration-slow: 1.2s;
  --kt-stagger-delay: 0.05s;
}
```

---

## Typography

### Typeface Characteristics

Kinetic Typography typefaces are:

- **High contrast and bold** -- display faces with strong visual weight that remain legible during motion and at extreme scales
- **Variable font enabled** -- typefaces with multiple axes (weight, width, slant, optical size) that can be animated fluidly through CSS transitions
- **Geometric or grotesque sans-serifs** -- clean, modern faces that look crisp during transformation and hold their form across animation states
- **Generous x-height** -- tall lowercase letters remain readable even when text is animating or partially revealed
- **Tight or dramatic spacing** -- letter-spacing is often compressed for display text to create visual density, or widely tracked for cinematic effect
- **Mixed case for expression** -- unlike all-caps-heavy aesthetics, kinetic typography leverages case contrast (uppercase headlines, sentence-case body) for rhythmic variety
- **Monospaced for code-like rhythm** -- fixed-width fonts occasionally used for staggered character animations where uniform spacing amplifies the mechanical, letter-by-letter cadence

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Inter** | Variable, geometric sans | Body text, UI elements, versatile workhorse |
| **Space Grotesk** | Geometric, contemporary | Headlines, display, modern kinetic layouts |
| **Syne** | Variable, expressive | Display text, bold headlines, artistic layouts |
| **DM Sans** | Geometric, clean | Body text, readable content at all sizes |
| **Unbounded** | Variable, rounded display | Large animated headlines, playful motion |
| **Plus Jakarta Sans** | Modern geometric | Subheadings, body, clean professional feel |
| **JetBrains Mono** | Monospaced, clear | Code-style text, staggered letter animations |
| **Instrument Sans** | Variable, refined | Body text, editorial layouts, subtle motion |
| **Bricolage Grotesque** | Variable, characterful | Display headlines, expressive kinetic sequences |
| **Archivo** | Variable, wide range | Versatile display and body, weight animations |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Space Grotesk** (700) | **Inter** (400) | Modern, clean, tech-forward kinetic design |
| **Syne** (700) | **DM Sans** (400) | Expressive headlines with calm, readable body |
| **Unbounded** (700) | **Plus Jakarta Sans** (400) | Playful, bold display with professional body |
| **Bricolage Grotesque** (800) | **Instrument Sans** (400) | Characterful headlines, refined body text |
| **Archivo** (900) | **JetBrains Mono** (400) | Maximum weight contrast, technical body feel |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  color: var(--kt-text-primary);
  line-height: 1.05;
  letter-spacing: -0.03em;
}

/* Display / Hero text -- oversized and commanding */
.kt-display {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(3rem, 12vw, 10rem);
  font-weight: 700;
  letter-spacing: -0.04em;
  line-height: 0.95;
  color: var(--kt-text-primary);
}

/* Gradient text for display headings */
.kt-gradient-text {
  background: var(--kt-gradient-text);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Body text */
body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--kt-text-body);
}

/* Monospaced accent text */
.kt-mono {
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.85rem;
  letter-spacing: 0.02em;
  color: var(--kt-text-secondary);
}

/* Label / overline text */
.kt-label {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--kt-text-muted);
}
```

---

## Layout Principles

### Grid and Structure

- **Full-viewport sections** -- each major content block occupies 100vh to create distinct "scenes" for scroll-triggered animations
- **Extreme horizontal padding** -- generous side margins (10-15% of viewport width) frame text centrally and create cinematic letterboxing
- **Single-column dominance** -- content flows in a single column to keep focus on sequential, animated text reveals
- **Oversized type as layout** -- headlines at 10-20vw become the structural grid themselves; the type IS the layout
- **Sticky and pinned sections** -- scrollable containers where text elements are position:sticky, animating in place while the user scrolls through content
- **Layered z-index compositions** -- foreground animated text layered over background marquee text or ghost typography
- **Asymmetric text placement** -- text blocks positioned off-center or anchored to edges for dynamic tension
- **Viewport-relative sizing** -- heavy use of vw, vh, and clamp() units so type scales proportionally with the screen

### Section Organization

- **Navigation**: Minimal, often a single logo and hamburger menu or inline text links; transparent overlay on content
- **Hero**: Full-viewport section with oversized animated headline, staggered character entrance, minimal supporting text
- **Manifesto / Statement**: Scroll-triggered paragraph where each line or word animates into view as the user scrolls
- **Marquee band**: Full-width continuous scrolling text ticker, often in large display type, acting as a visual divider
- **Feature blocks**: Text-dominant cards or sections where each feature headline animates on scroll intersection
- **Split-screen type**: Left/right or top/bottom divided layouts where text on each side animates independently
- **CTA section**: Centered, simple call-to-action with a single animated headline and button
- **Footer**: Minimal dark footer with muted text; may include a final animation flourish

### Responsive Approach

- Scale display text aggressively with `clamp()` -- headlines that are 10vw on desktop should reduce to 8-12vw on mobile with appropriate minimums
- Maintain full-viewport section heights on mobile to preserve the "scene" structure
- Simplify stagger animations on mobile -- reduce the number of individually animated elements to preserve performance
- Keep marquee tickers but reduce font size and speed
- Switch from multi-column layouts to stacked single-column on mobile
- Reduce animation complexity and duration for mobile; favor simpler fade/slide over complex transforms
- Always implement `prefers-reduced-motion` at all breakpoints

---

## CSS / Design Techniques

### Kinetic Typography Card Component

```css
.kt-card {
  background: var(--kt-bg-carbon);
  border: 1px solid rgba(255, 255, 255, 0.06);
  border-radius: 8px;
  padding: 40px 32px;
  position: relative;
  overflow: hidden;
  transition: border-color var(--kt-duration-fast) ease;
}

.kt-card:hover {
  border-color: rgba(255, 255, 255, 0.15);
}

/* Animated underline reveal on card heading */
.kt-card h3 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 1.25rem;
  font-weight: 600;
  margin-bottom: 12px;
  display: inline-block;
  position: relative;
}

.kt-card h3::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--kt-accent-blue);
  transition: width var(--kt-duration-normal) var(--kt-ease-out-expo);
}

.kt-card:hover h3::after {
  width: 100%;
}

.kt-card p {
  color: var(--kt-text-secondary);
  font-size: 0.95rem;
  line-height: 1.6;
}

/* Card grid */
.kt-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 24px;
}
```

### Kinetic Typography Button

```css
.kt-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: var(--kt-text-primary);
  color: var(--kt-bg-void);
  border: none;
  border-radius: 6px;
  padding: 16px 36px;
  font-family: 'Space Grotesk', sans-serif;
  font-size: 0.9rem;
  font-weight: 600;
  letter-spacing: 0.02em;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: transform var(--kt-duration-fast) var(--kt-ease-out-expo),
              box-shadow var(--kt-duration-fast) ease;
  text-decoration: none;
}

/* Text slide-up effect on hover */
.kt-button span {
  display: inline-block;
  transition: transform var(--kt-duration-normal) var(--kt-ease-out-expo);
}

.kt-button:hover span {
  transform: translateY(-100%);
}

.kt-button::after {
  content: attr(data-text);
  position: absolute;
  top: 100%;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: top var(--kt-duration-normal) var(--kt-ease-out-expo);
}

.kt-button:hover::after {
  top: 0;
}

.kt-button:hover {
  box-shadow: 0 4px 24px rgba(0, 0, 0, 0.3);
}

/* Outline variant */
.kt-button--outline {
  background: transparent;
  color: var(--kt-text-primary);
  border: 1.5px solid rgba(255, 255, 255, 0.25);
}

.kt-button--outline:hover {
  border-color: var(--kt-text-primary);
  background: rgba(255, 255, 255, 0.05);
}

/* Accent variant */
.kt-button--accent {
  background: var(--kt-accent-blue);
  color: #ffffff;
}
```

### Navigation Bar

```css
.kt-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1400px;
  margin: 0 auto;
  padding: 24px 48px;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  mix-blend-mode: difference;
}

.kt-nav__logo {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 1.1rem;
  font-weight: 700;
  color: var(--kt-text-primary);
  text-decoration: none;
  letter-spacing: -0.02em;
}

.kt-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.kt-nav__links a {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--kt-text-primary);
  text-decoration: none;
  position: relative;
  transition: opacity var(--kt-duration-fast) ease;
}

.kt-nav__links a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  width: 0;
  height: 1.5px;
  background: var(--kt-text-primary);
  transition: width var(--kt-duration-normal) var(--kt-ease-out-expo);
}

.kt-nav__links a:hover::after {
  width: 100%;
}

.kt-nav__links a:hover {
  opacity: 0.7;
}
```

### Hero Section with Animated Text

```css
.kt-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 10vw;
  background: var(--kt-bg-void);
  overflow: hidden;
}

.kt-hero__content {
  position: relative;
  z-index: 5;
  max-width: 1000px;
}

.kt-hero__headline {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(3rem, 12vw, 9rem);
  font-weight: 700;
  line-height: 0.95;
  letter-spacing: -0.04em;
  color: var(--kt-text-primary);
  margin-bottom: 2rem;
}

/* Individual character animation */
.kt-hero__headline .char {
  display: inline-block;
  opacity: 0;
  transform: translateY(60px) rotateX(-40deg);
  animation: kt-char-enter var(--kt-duration-slow) var(--kt-ease-out-expo) forwards;
}

@keyframes kt-char-enter {
  to {
    opacity: 1;
    transform: translateY(0) rotateX(0deg);
  }
}

/* Stagger each character */
.kt-hero__headline .char:nth-child(1) { animation-delay: 0.05s; }
.kt-hero__headline .char:nth-child(2) { animation-delay: 0.10s; }
.kt-hero__headline .char:nth-child(3) { animation-delay: 0.15s; }
.kt-hero__headline .char:nth-child(4) { animation-delay: 0.20s; }
.kt-hero__headline .char:nth-child(5) { animation-delay: 0.25s; }
.kt-hero__headline .char:nth-child(6) { animation-delay: 0.30s; }
.kt-hero__headline .char:nth-child(7) { animation-delay: 0.35s; }
.kt-hero__headline .char:nth-child(8) { animation-delay: 0.40s; }
.kt-hero__headline .char:nth-child(9) { animation-delay: 0.45s; }
.kt-hero__headline .char:nth-child(10) { animation-delay: 0.50s; }

.kt-hero__subtitle {
  font-size: 1.15rem;
  color: var(--kt-text-secondary);
  margin-bottom: 2.5rem;
  opacity: 0;
  animation: kt-fade-up 0.8s var(--kt-ease-out-expo) 0.8s forwards;
}

@keyframes kt-fade-up {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Background ghost text */
.kt-hero__ghost {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(8rem, 25vw, 20rem);
  font-weight: 700;
  color: rgba(255, 255, 255, 0.03);
  white-space: nowrap;
  pointer-events: none;
  z-index: 1;
}

@media (max-width: 768px) {
  .kt-hero { padding: 60px 6vw; }
}
```

### CSS Text Reveal Animation (Clip-Path)

```css
/* Line-by-line text reveal using clip-path */
.kt-reveal {
  overflow: hidden;
}

.kt-reveal__line {
  display: block;
  clip-path: inset(0 100% 0 0);
  animation: kt-clip-reveal var(--kt-duration-slow) var(--kt-ease-out-expo) forwards;
}

@keyframes kt-clip-reveal {
  to {
    clip-path: inset(0 0 0 0);
  }
}

.kt-reveal__line:nth-child(1) { animation-delay: 0.0s; }
.kt-reveal__line:nth-child(2) { animation-delay: 0.15s; }
.kt-reveal__line:nth-child(3) { animation-delay: 0.30s; }
.kt-reveal__line:nth-child(4) { animation-delay: 0.45s; }

/* Vertical slide reveal variant */
.kt-reveal--slide .kt-reveal__line {
  clip-path: none;
  transform: translateY(100%);
  opacity: 0;
  animation: kt-slide-reveal var(--kt-duration-normal) var(--kt-ease-out-expo) forwards;
}

@keyframes kt-slide-reveal {
  to {
    transform: translateY(0);
    opacity: 1;
  }
}
```

### Infinite Marquee / Text Ticker

```css
/* Continuous horizontal scrolling text */
.kt-marquee {
  overflow: hidden;
  white-space: nowrap;
  padding: 24px 0;
  border-top: 1px solid rgba(255, 255, 255, 0.06);
  border-bottom: 1px solid rgba(255, 255, 255, 0.06);
}

.kt-marquee__track {
  display: inline-flex;
  animation: kt-scroll-left 20s linear infinite;
}

.kt-marquee__text {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(2rem, 5vw, 4rem);
  font-weight: 700;
  color: var(--kt-text-primary);
  text-transform: uppercase;
  letter-spacing: -0.02em;
  padding: 0 24px;
  flex-shrink: 0;
}

/* Separator dot between repeated items */
.kt-marquee__text::after {
  content: '\2022';
  margin-left: 24px;
  color: var(--kt-accent-blue);
}

@keyframes kt-scroll-left {
  from { transform: translateX(0); }
  to { transform: translateX(-50%); }
}

/* Outlined / stroke variant */
.kt-marquee--outline .kt-marquee__text {
  color: transparent;
  -webkit-text-stroke: 1.5px var(--kt-text-primary);
}

/* Reverse direction variant */
.kt-marquee--reverse .kt-marquee__track {
  animation-direction: reverse;
}

/* Hover pause */
.kt-marquee:hover .kt-marquee__track {
  animation-play-state: paused;
}

@media (prefers-reduced-motion: reduce) {
  .kt-marquee__track { animation: none; }
}
```

### Variable Font Weight Animation

```css
/* Animate variable font weight on hover */
@supports (font-variation-settings: normal) {
  .kt-variable {
    font-family: 'Inter', sans-serif;
    font-variation-settings: 'wght' 400;
    transition: font-variation-settings var(--kt-duration-normal) var(--kt-ease-out-expo);
  }

  .kt-variable:hover {
    font-variation-settings: 'wght' 900;
  }

  /* Per-character weight wave animation */
  .kt-variable-wave .char {
    display: inline-block;
    font-variation-settings: 'wght' 300;
    animation: kt-weight-wave 2s ease-in-out infinite;
  }

  @keyframes kt-weight-wave {
    0%, 100% { font-variation-settings: 'wght' 300; }
    50% { font-variation-settings: 'wght' 900; }
  }

  /* Stagger the wave across characters */
  .kt-variable-wave .char:nth-child(1) { animation-delay: 0.0s; }
  .kt-variable-wave .char:nth-child(2) { animation-delay: 0.08s; }
  .kt-variable-wave .char:nth-child(3) { animation-delay: 0.16s; }
  .kt-variable-wave .char:nth-child(4) { animation-delay: 0.24s; }
  .kt-variable-wave .char:nth-child(5) { animation-delay: 0.32s; }
  .kt-variable-wave .char:nth-child(6) { animation-delay: 0.40s; }
  .kt-variable-wave .char:nth-child(7) { animation-delay: 0.48s; }
  .kt-variable-wave .char:nth-child(8) { animation-delay: 0.56s; }
  .kt-variable-wave .char:nth-child(9) { animation-delay: 0.64s; }
  .kt-variable-wave .char:nth-child(10) { animation-delay: 0.72s; }
}
```

### Scroll-Triggered Text Animation (Intersection Observer)

```css
/* Base state for scroll-animated elements */
.kt-scroll-animate {
  opacity: 0;
  transform: translateY(40px);
  transition: opacity var(--kt-duration-slow) var(--kt-ease-out-expo),
              transform var(--kt-duration-slow) var(--kt-ease-out-expo);
}

/* Revealed state -- toggled via Intersection Observer */
.kt-scroll-animate.is-visible {
  opacity: 1;
  transform: translateY(0);
}

/* Slide from left variant */
.kt-scroll-animate--left {
  transform: translateX(-60px);
}

.kt-scroll-animate--left.is-visible {
  transform: translateX(0);
}

/* Slide from right variant */
.kt-scroll-animate--right {
  transform: translateX(60px);
}

.kt-scroll-animate--right.is-visible {
  transform: translateX(0);
}

/* Scale up variant */
.kt-scroll-animate--scale {
  transform: scale(0.85);
}

.kt-scroll-animate--scale.is-visible {
  transform: scale(1);
}

/* Stagger children inside a container */
.kt-scroll-stagger .kt-scroll-animate:nth-child(1) { transition-delay: 0.0s; }
.kt-scroll-stagger .kt-scroll-animate:nth-child(2) { transition-delay: 0.1s; }
.kt-scroll-stagger .kt-scroll-animate:nth-child(3) { transition-delay: 0.2s; }
.kt-scroll-stagger .kt-scroll-animate:nth-child(4) { transition-delay: 0.3s; }
.kt-scroll-stagger .kt-scroll-animate:nth-child(5) { transition-delay: 0.4s; }

@media (prefers-reduced-motion: reduce) {
  .kt-scroll-animate {
    opacity: 1;
    transform: none;
    transition: none;
  }
}
```

### Typewriter Effect

```css
/* CSS-only typewriter animation */
.kt-typewriter {
  font-family: 'JetBrains Mono', monospace;
  font-size: 1.25rem;
  color: var(--kt-text-primary);
  overflow: hidden;
  border-right: 2px solid var(--kt-accent-blue);
  white-space: nowrap;
  width: 0;
  animation:
    kt-typing 3s steps(30, end) forwards,
    kt-blink-cursor 0.7s step-end infinite;
}

@keyframes kt-typing {
  from { width: 0; }
  to { width: 100%; }
}

@keyframes kt-blink-cursor {
  from, to { border-color: transparent; }
  50% { border-color: var(--kt-accent-blue); }
}

@media (prefers-reduced-motion: reduce) {
  .kt-typewriter {
    width: 100%;
    animation: none;
    border-right: none;
  }
}
```

---

## Design Do's and Don'ts

### Do

- Use motion to establish visual hierarchy -- the most important text should animate first or most prominently
- Implement `prefers-reduced-motion: reduce` on every animation to respect accessibility preferences
- Favor GPU-accelerated properties (`transform`, `opacity`) for smooth 60fps performance
- Use `clamp()` for display text so oversized type scales gracefully across all viewports
- Keep animation durations deliberate -- 0.4s to 1.2s is the sweet spot for most text reveals
- Apply staggered delays across characters or lines for natural, rhythmic entrances
- Maintain high contrast (WCAG AAA: 7:1 ratio minimum) between animated text and backgrounds
- Pair bold, expressive headline fonts with clean, readable body fonts
- Use generous whitespace to let animated text breathe and command attention
- Test on low-powered devices -- mobile performance is a critical constraint for motion-heavy design
- Provide meaningful easing curves (`cubic-bezier`) rather than default `linear` or `ease`
- Use the Intersection Observer API for scroll-triggered animations instead of scroll event listeners

### Don't

- Animate every piece of text on the page -- reserve motion for headlines, key statements, and transitions
- Use animation durations longer than 2 seconds for text reveals -- users will lose patience
- Forget to provide static content for users who disable motion -- the content must be readable without animation
- Rely on JavaScript frameworks when CSS animations can achieve the effect -- simpler is more performant
- Use bright or colorful backgrounds that compete with animated text for attention
- Apply complex motion to body text or long paragraphs -- these should remain static and readable
- Ignore mobile viewport -- oversized text that works at 1920px may break entirely at 375px
- Mix too many animation styles in one section -- consistency in timing and easing creates coherence
- Use `animation-delay` values so large that users might scroll past before the animation triggers
- Apply text-shadow or filter effects during active animations -- they are expensive and cause frame drops
- Create animations that block content access -- text should be readable even if the animation is interrupted

---

## Related Aesthetics

| Aesthetic | Relationship to Kinetic Typography |
|-----------|-----------------------------------|
| **Brutalist** | Both favor oversized typography and bold visual impact; Brutalist uses type as raw structure while Kinetic Typography adds expressive motion |
| **Swiss / International** | Shares the emphasis on typographic hierarchy and grid discipline; Kinetic Typography animates what Swiss design composes statically |
| **Motion Design** | Kinetic Typography is a subset of motion design focused specifically on text; broader motion design includes shapes, illustrations, and transitions |
| **Editorial / Magazine** | Both treat typography as a primary visual element; Editorial layouts are static compositions while Kinetic Typography brings them to life through animation |
| **Minimalism** | Kinetic Typography often adopts minimalist layouts -- dark backgrounds, whitespace, limited elements -- to spotlight animated text |
| **Cyberpunk** | Both can feature dramatic, screen-filling text; Cyberpunk adds dystopian glitch and neon effects, Kinetic Typography keeps focus on fluid motion |
| **Parallax Design** | Shares scroll-driven animation techniques; Parallax focuses on depth layers of imagery while Kinetic Typography focuses on text behavior |
| **Variable Font Art** | Directly related -- variable font art explores the artistic potential of font axis animation, a core technique in Kinetic Typography |
| **Data Visualization** | Both use motion to communicate meaning; data viz animates charts and numbers while Kinetic Typography animates words and letterforms |

---

## Quick-Start: Minimal Kinetic Typography Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kinetic Typography Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400&display=swap" rel="stylesheet">
  <style>
    :root {
      --kt-bg-void: #0a0a0a;
      --kt-bg-deep: #141414;
      --kt-bg-carbon: #1e1e1e;
      --kt-text-primary: #ffffff;
      --kt-text-body: #e8e8e8;
      --kt-text-secondary: #a0a0a0;
      --kt-text-muted: #666666;
      --kt-accent-blue: #2d5bff;
      --kt-accent-coral: #ff4d4d;
      --kt-ease-out-expo: cubic-bezier(0.16, 1, 0.3, 1);
      --kt-duration-slow: 1.2s;
      --kt-duration-normal: 0.6s;
      --kt-duration-fast: 0.3s;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--kt-bg-void);
      color: var(--kt-text-body);
      font-family: 'Inter', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      color: var(--kt-text-primary);
      line-height: 1.05;
      letter-spacing: -0.03em;
    }

    /* -- Navigation -- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 24px 48px;
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 100;
      mix-blend-mode: difference;
    }

    nav a.logo {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 1.1rem;
      font-weight: 700;
      color: var(--kt-text-primary);
      text-decoration: none;
      letter-spacing: -0.02em;
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'Inter', sans-serif;
      font-weight: 500;
      font-size: 0.85rem;
      color: var(--kt-text-primary);
      text-decoration: none;
      position: relative;
      transition: opacity var(--kt-duration-fast) ease;
    }

    nav ul a::after {
      content: '';
      position: absolute;
      bottom: -4px; left: 0;
      width: 0; height: 1.5px;
      background: var(--kt-text-primary);
      transition: width var(--kt-duration-normal) var(--kt-ease-out-expo);
    }

    nav ul a:hover::after { width: 100%; }
    nav ul a:hover { opacity: 0.7; }

    /* -- Hero -- */
    .hero {
      position: relative;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 80px 10vw;
      overflow: hidden;
    }

    .hero__ghost {
      position: absolute;
      top: 50%; left: 50%;
      transform: translate(-50%, -50%);
      font-family: 'Space Grotesk', sans-serif;
      font-size: clamp(8rem, 25vw, 20rem);
      font-weight: 700;
      color: rgba(255, 255, 255, 0.025);
      white-space: nowrap;
      pointer-events: none;
      z-index: 1;
    }

    .hero__content {
      position: relative;
      z-index: 5;
      max-width: 900px;
    }

    .hero h1 {
      font-size: clamp(3rem, 11vw, 8rem);
      letter-spacing: -0.04em;
      line-height: 0.95;
      margin-bottom: 2rem;
    }

    .hero h1 .char {
      display: inline-block;
      opacity: 0;
      transform: translateY(50px);
      animation: char-enter var(--kt-duration-slow) var(--kt-ease-out-expo) forwards;
    }

    @keyframes char-enter {
      to { opacity: 1; transform: translateY(0); }
    }

    .hero h1 .word { display: inline-block; white-space: nowrap; }
    .hero h1 .space { display: inline-block; width: 0.3em; }

    .hero p {
      font-size: 1.15rem;
      color: var(--kt-text-secondary);
      margin-bottom: 2.5rem;
      opacity: 0;
      animation: fade-up 0.8s var(--kt-ease-out-expo) 1s forwards;
    }

    .hero .label {
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.75rem;
      color: var(--kt-text-muted);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      margin-bottom: 1.5rem;
      opacity: 0;
      animation: fade-up 0.6s var(--kt-ease-out-expo) 0.4s forwards;
    }

    @keyframes fade-up {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .btn {
      display: inline-block;
      background: var(--kt-text-primary);
      color: var(--kt-bg-void);
      border: none;
      border-radius: 6px;
      padding: 16px 36px;
      font-family: 'Space Grotesk', sans-serif;
      font-size: 0.9rem;
      font-weight: 600;
      cursor: pointer;
      text-decoration: none;
      transition: transform var(--kt-duration-fast) var(--kt-ease-out-expo),
                  box-shadow var(--kt-duration-fast) ease;
      opacity: 0;
      animation: fade-up 0.8s var(--kt-ease-out-expo) 1.2s forwards;
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.4);
    }

    .btn--outline {
      background: transparent;
      color: var(--kt-text-primary);
      border: 1.5px solid rgba(255, 255, 255, 0.25);
    }

    .btn--outline:hover {
      border-color: var(--kt-text-primary);
      background: rgba(255, 255, 255, 0.05);
    }

    /* -- Marquee -- */
    .marquee {
      overflow: hidden;
      white-space: nowrap;
      padding: 28px 0;
      border-top: 1px solid rgba(255, 255, 255, 0.06);
      border-bottom: 1px solid rgba(255, 255, 255, 0.06);
    }

    .marquee__track {
      display: inline-flex;
      animation: scroll-left 18s linear infinite;
    }

    .marquee__item {
      font-family: 'Space Grotesk', sans-serif;
      font-size: clamp(1.5rem, 4vw, 3rem);
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: -0.02em;
      padding: 0 20px;
      flex-shrink: 0;
    }

    .marquee__item--filled { color: var(--kt-text-primary); }

    .marquee__item--outline {
      color: transparent;
      -webkit-text-stroke: 1px var(--kt-text-primary);
    }

    .marquee__item::after {
      content: '\2022';
      margin-left: 20px;
      color: var(--kt-accent-blue);
    }

    @keyframes scroll-left {
      from { transform: translateX(0); }
      to { transform: translateX(-50%); }
    }

    .marquee:hover .marquee__track {
      animation-play-state: paused;
    }

    /* -- Scroll reveal sections -- */
    .scroll-section {
      padding: 120px 10vw;
      max-width: 1400px;
      margin: 0 auto;
    }

    .scroll-animate {
      opacity: 0;
      transform: translateY(40px);
      transition: opacity var(--kt-duration-slow) var(--kt-ease-out-expo),
                  transform var(--kt-duration-slow) var(--kt-ease-out-expo);
    }

    .scroll-animate.is-visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* Staggered children */
    .stagger-group .scroll-animate:nth-child(1) { transition-delay: 0.0s; }
    .stagger-group .scroll-animate:nth-child(2) { transition-delay: 0.1s; }
    .stagger-group .scroll-animate:nth-child(3) { transition-delay: 0.2s; }
    .stagger-group .scroll-animate:nth-child(4) { transition-delay: 0.3s; }

    /* -- Statement section -- */
    .statement {
      padding: 160px 10vw;
      text-align: center;
    }

    .statement h2 {
      font-size: clamp(2rem, 6vw, 4.5rem);
      letter-spacing: -0.03em;
      line-height: 1.1;
      max-width: 900px;
      margin: 0 auto;
    }

    .statement h2 .line {
      display: block;
      overflow: hidden;
    }

    .statement h2 .line-inner {
      display: block;
      transform: translateY(100%);
      transition: transform var(--kt-duration-slow) var(--kt-ease-out-expo);
    }

    .statement h2.is-visible .line-inner {
      transform: translateY(0);
    }

    .statement h2.is-visible .line:nth-child(2) .line-inner { transition-delay: 0.12s; }
    .statement h2.is-visible .line:nth-child(3) .line-inner { transition-delay: 0.24s; }

    /* -- Features -- */
    .features {
      padding: 100px 0;
    }

    .features__header {
      text-align: center;
      margin-bottom: 64px;
      padding: 0 10vw;
    }

    .features__header .label {
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.7rem;
      color: var(--kt-accent-blue);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      margin-bottom: 16px;
    }

    .features__header h2 {
      font-size: clamp(1.8rem, 4vw, 3rem);
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1px;
      background: rgba(255, 255, 255, 0.06);
      max-width: 1200px;
      margin: 0 auto;
    }

    .feature {
      background: var(--kt-bg-void);
      padding: 48px 36px;
      position: relative;
      transition: background var(--kt-duration-fast) ease;
    }

    .feature:hover {
      background: var(--kt-bg-deep);
    }

    .feature__number {
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.7rem;
      color: var(--kt-text-muted);
      margin-bottom: 20px;
      letter-spacing: 0.1em;
    }

    .feature h3 {
      font-size: 1.25rem;
      margin-bottom: 12px;
      position: relative;
      display: inline-block;
    }

    .feature h3::after {
      content: '';
      position: absolute;
      bottom: -2px; left: 0;
      width: 0; height: 2px;
      background: var(--kt-accent-blue);
      transition: width var(--kt-duration-normal) var(--kt-ease-out-expo);
    }

    .feature:hover h3::after { width: 100%; }

    .feature p {
      color: var(--kt-text-secondary);
      font-size: 0.9rem;
      line-height: 1.65;
    }

    /* -- CTA -- */
    .cta {
      text-align: center;
      padding: 160px 10vw;
      position: relative;
    }

    .cta h2 {
      font-size: clamp(2.5rem, 8vw, 6rem);
      letter-spacing: -0.04em;
      margin-bottom: 1.5rem;
    }

    .cta p {
      color: var(--kt-text-secondary);
      font-size: 1.05rem;
      margin-bottom: 2.5rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    /* -- Divider -- */
    .divider {
      border: none;
      height: 1px;
      background: rgba(255, 255, 255, 0.06);
      max-width: 1200px;
      margin: 0 auto;
    }

    /* -- Footer -- */
    footer {
      background: var(--kt-bg-void);
      border-top: 1px solid rgba(255, 255, 255, 0.06);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 28px 48px;
    }

    footer p {
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.75rem;
      color: var(--kt-text-muted);
      letter-spacing: 0.05em;
    }

    footer a {
      color: var(--kt-text-secondary);
      text-decoration: none;
      font-size: 0.8rem;
      transition: color var(--kt-duration-fast) ease;
    }

    footer a:hover { color: var(--kt-text-primary); }

    /* -- Reduced motion -- */
    @media (prefers-reduced-motion: reduce) {
      .hero h1 .char {
        opacity: 1;
        transform: none;
        animation: none;
      }
      .hero p,
      .hero .label,
      .btn {
        opacity: 1;
        animation: none;
      }
      .marquee__track { animation: none; }
      .scroll-animate {
        opacity: 1;
        transform: none;
        transition: none;
      }
      .statement h2 .line-inner {
        transform: none;
        transition: none;
      }
    }

    /* -- Mobile -- */
    @media (max-width: 768px) {
      nav { padding: 16px 24px; }
      nav ul { gap: 16px; }
      .hero { padding: 60px 6vw; }
      .scroll-section { padding: 80px 6vw; }
      .statement { padding: 100px 6vw; }
      .cta { padding: 100px 6vw; }
      footer { flex-direction: column; gap: 12px; text-align: center; padding: 24px; }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <a href="#" class="logo">Motion</a>
    <ul>
      <li><a href="#">Work</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Process</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="hero__ghost">MOTION</div>
    <div class="hero__content">
      <p class="label">Design Studio / Est. 2024</p>
      <h1>
        <span class="word">
          <span class="char" style="animation-delay:0.05s">W</span><span class="char" style="animation-delay:0.08s">o</span><span class="char" style="animation-delay:0.11s">r</span><span class="char" style="animation-delay:0.14s">d</span><span class="char" style="animation-delay:0.17s">s</span>
        </span>
        <span class="space"></span>
        <span class="word">
          <span class="char" style="animation-delay:0.24s">i</span><span class="char" style="animation-delay:0.27s">n</span>
        </span>
        <br>
        <span class="word">
          <span class="char" style="animation-delay:0.36s">M</span><span class="char" style="animation-delay:0.39s">o</span><span class="char" style="animation-delay:0.42s">t</span><span class="char" style="animation-delay:0.45s">i</span><span class="char" style="animation-delay:0.48s">o</span><span class="char" style="animation-delay:0.51s">n</span>
        </span>
      </h1>
      <p>We craft typographic experiences that move, breathe, and resonate. Every letter has a story to tell.</p>
      <a href="#" class="btn">Explore Our Work</a>
    </div>
  </section>

  <!-- Marquee -->
  <div class="marquee">
    <div class="marquee__track">
      <span class="marquee__item marquee__item--filled">Typography</span>
      <span class="marquee__item marquee__item--outline">Animation</span>
      <span class="marquee__item marquee__item--filled">Expression</span>
      <span class="marquee__item marquee__item--outline">Rhythm</span>
      <span class="marquee__item marquee__item--filled">Typography</span>
      <span class="marquee__item marquee__item--outline">Animation</span>
      <span class="marquee__item marquee__item--filled">Expression</span>
      <span class="marquee__item marquee__item--outline">Rhythm</span>
    </div>
  </div>

  <!-- Statement -->
  <section class="statement">
    <h2>
      <span class="line"><span class="line-inner">We believe that words</span></span>
      <span class="line"><span class="line-inner">deserve to be felt,</span></span>
      <span class="line"><span class="line-inner">not just read.</span></span>
    </h2>
  </section>

  <hr class="divider">

  <!-- Features -->
  <section class="features">
    <div class="features__header">
      <p class="label scroll-animate">What we do</p>
      <h2 class="scroll-animate">Text that transforms</h2>
    </div>
    <div class="features-grid stagger-group">
      <div class="feature scroll-animate">
        <p class="feature__number">01</p>
        <h3>Scroll Sequences</h3>
        <p>Typography that reveals itself in rhythm with the user's journey, turning every scroll into a moment of discovery.</p>
      </div>
      <div class="feature scroll-animate">
        <p class="feature__number">02</p>
        <h3>Variable Dynamics</h3>
        <p>Fluid transitions across font weight, width, and slant axes, creating letterforms that breathe and shift before your eyes.</p>
      </div>
      <div class="feature scroll-animate">
        <p class="feature__number">03</p>
        <h3>Character Choreography</h3>
        <p>Each letter animated independently with precise timing and easing, orchestrated into sequences that feel alive.</p>
      </div>
      <div class="feature scroll-animate">
        <p class="feature__number">04</p>
        <h3>Reveal Transitions</h3>
        <p>Clip-path masks, sliding panels, and geometric reveals that turn the appearance of text into a theatrical event.</p>
      </div>
      <div class="feature scroll-animate">
        <p class="feature__number">05</p>
        <h3>Marquee Systems</h3>
        <p>Continuous horizontal text tickers at scale -- bold, rhythmic, and hypnotic -- serving as both content and texture.</p>
      </div>
      <div class="feature scroll-animate">
        <p class="feature__number">06</p>
        <h3>Accessible Motion</h3>
        <p>Every animation respects user preferences with reduced-motion fallbacks, ensuring the message reaches everyone.</p>
      </div>
    </div>
  </section>

  <!-- CTA -->
  <section class="cta">
    <h2 class="scroll-animate">Let's move.</h2>
    <p class="scroll-animate">Start a conversation about bringing your words to life through motion and rhythm.</p>
    <a href="#" class="btn btn--outline scroll-animate">Get in Touch</a>
  </section>

  <!-- Footer -->
  <footer>
    <p>MOTION STUDIO // Type in perpetual motion</p>
    <a href="#">hello@motionstudio.design</a>
  </footer>

  <!-- Scroll animation script -->
  <script>
    // Intersection Observer for scroll-triggered animations
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('is-visible');
        }
      });
    }, {
      threshold: 0.15,
      rootMargin: '0px 0px -50px 0px'
    });

    // Observe all scroll-animated elements
    document.querySelectorAll('.scroll-animate, .statement h2').forEach(el => {
      observer.observe(el);
    });
  </script>

</body>
</html>
```
