# Glitch Art Design Reference

Glitch Art is a digital aesthetic rooted in the deliberate exploitation of technological errors, data corruption, and signal malfunction to produce visually striking compositions. Emerging from net art and new media art communities in the mid-2000s -- with theoretical grounding established by Rosa Menkman's *Glitch Studies Manifesto* (2010) and *The Glitch Moment(um)* (2011) -- it celebrates the beauty found in broken data, pixel sorting, datamoshing, and RGB channel separation. Predecessors include early video feedback experiments and data-bent photography, but the movement crystallized as a distinct genre around 2006-2009, accelerated by social sharing and DIY datamoshing tutorials. In web and UI design, Glitch Art translates to RGB split text effects, scan line overlays, noise grain textures, corrupted grid layouts, distorted imagery, and animations that simulate signal interference. The core philosophy treats the glitch not as failure but as revelation -- exposing the hidden mechanics of digital systems and challenging the assumption that technology should always appear seamless and polished.

---

## Visual Characteristics

### Core Design Traits

- **RGB channel splitting** -- red, green, and blue color channels are offset from each other, producing chromatic aberration that mimics a damaged display or misaligned CRT monitor
- **Scan line overlays** -- thin horizontal lines layered across content to simulate CRT monitors, VHS playback artifacts, or interlaced video rendering
- **Pixel corruption and moshing** -- blocks of pixels are displaced, duplicated, or smeared across the image, replicating the visual artifacts of lossy compression failure or codec errors
- **Digital noise and grain** -- static-like texture applied to backgrounds and images, evoking analog television interference, sensor noise, or degraded signal quality
- **Broken and offset grid layouts** -- content blocks deliberately misaligned, overlapping, or shifted from their expected positions to simulate a page failing to render correctly
- **Text distortion and warping** -- letterforms stretched, fragmented, sliced, or duplicated with offset copies, as though the text buffer has been corrupted mid-render
- **Signal interference patterns** -- horizontal bands of color shift, vertical tearing, or wave distortion applied to sections of the page, suggesting electromagnetic disruption
- **Data artifact textures** -- visual patterns derived from JPEG compression blocks, PNG chunk errors, or hexadecimal data visualized as color, used as decorative or structural elements
- **Flickering and temporal instability** -- elements that rapidly alternate between states (visible/hidden, shifted/aligned, colored/monochrome) to create an unsettled, unstable visual rhythm
- **High-contrast neon on dark backgrounds** -- vivid cyan, magenta, electric green, and hot pink set against deep black or near-black surfaces to maximize the visual impact of corruption effects

### Design Principles

- **Error as aesthetic** -- technological failure is not something to hide but to celebrate; the glitch reveals the hidden substrate of digital media and transforms malfunction into meaning
- **Controlled chaos** -- while the visual language references randomness and corruption, effective glitch design requires precise control over timing, placement, and intensity of distortion effects
- **Tension between order and disruption** -- the most effective glitch layouts maintain an underlying structure that the corruption effects interrupt, creating a push-pull dynamic between legibility and abstraction
- **Temporal instability** -- static designs feel incomplete in Glitch Art; motion, animation, and state changes are essential to communicate the sense of a system in flux
- **Digital materiality** -- the aesthetic foregrounds the physical reality of digital data by making pixels, compression artifacts, and encoding structures visible rather than invisible
- **Layered signal degradation** -- multiple corruption effects stack and interact (noise over scan lines over RGB split), creating depth and complexity that a single effect cannot achieve
- **Readable despite disruption** -- core content must remain accessible even when surrounded by visual chaos; the glitch should enhance, not obliterate, the user's ability to navigate

---

## Color Palette

Glitch Art palettes draw from the RGB color model itself -- the raw channels of digital displays -- combined with neon accents that evoke CRT phosphors, VHS artifacts, and corrupted data streams. Deep black backgrounds maximize the luminosity of channel-split colors.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Void Black** | `#0D0D0D` | Primary background, deepest canvas surface |
| **Screen Dark** | `#1A1A2E` | Secondary background, dark panels with subtle blue cast |
| **Static Gray** | `#2A2A2A` | Tertiary surfaces, noise texture base |
| **Channel Red** | `#FF0040` | RGB red channel, primary split offset color |
| **Channel Green** | `#00FF41` | RGB green channel, terminal/matrix accent |
| **Channel Blue** | `#0080FF` | RGB blue channel, secondary split offset color |
| **Glitch Cyan** | `#00FFFF` | High-energy accent, scan line tint, hyperlinks |
| **Glitch Magenta** | `#FF00FF` | High-energy accent, chromatic aberration highlight |
| **Corrupt Pink** | `#FF2E97` | Hot accent for buttons, alert states, key UI elements |
| **Signal Yellow** | `#F5F500` | Warning accents, data highlight, hover state feedback |
| **Data White** | `#E0E0E0` | Primary text, readable body content |
| **Phosphor White** | `#FFFFFF` | Display headings, maximum-contrast elements |
| **Artifact Purple** | `#7B2FBE` | Decorative gradients, secondary data visualization |
| **Noise Mid** | `#444444` | Muted borders, disabled states, subtle separators |
| **Codec Orange** | `#FF6B2B` | Tertiary accent, compression artifact visualization |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --glitch-void: #0d0d0d;
  --glitch-screen-dark: #1a1a2e;
  --glitch-static-gray: #2a2a2a;

  /* RGB Channels */
  --glitch-red: #ff0040;
  --glitch-green: #00ff41;
  --glitch-blue: #0080ff;

  /* Neon Accents */
  --glitch-cyan: #00ffff;
  --glitch-magenta: #ff00ff;
  --glitch-pink: #ff2e97;
  --glitch-yellow: #f5f500;
  --glitch-purple: #7b2fbe;
  --glitch-orange: #ff6b2b;

  /* Neutrals */
  --glitch-white: #ffffff;
  --glitch-text: #e0e0e0;
  --glitch-muted: #444444;

  /* Functional Tokens */
  --glitch-bg: var(--glitch-void);
  --glitch-surface: var(--glitch-screen-dark);
  --glitch-border: var(--glitch-muted);
  --glitch-accent: var(--glitch-cyan);
  --glitch-accent-alt: var(--glitch-pink);
  --glitch-link: var(--glitch-cyan);
  --glitch-link-hover: var(--glitch-magenta);
}
```

---

## Typography

Glitch Art typography favors monospaced, technical, and geometric typefaces that reference code editors, terminal displays, and early computing. Display text is often treated as a surface for corruption effects -- split, distorted, and layered -- while body text prioritizes legibility against noisy backgrounds.

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| Share Tech Mono | 400 | Body text, data displays, code-like content | [fonts.google.com/specimen/Share+Tech+Mono](https://fonts.google.com/specimen/Share+Tech+Mono) |
| VT323 | 400 | Display text, retro terminal headings, pixel-style accents | [fonts.google.com/specimen/VT323](https://fonts.google.com/specimen/VT323) |
| Space Mono | 400, 700 | Body text, UI labels, technical content | [fonts.google.com/specimen/Space+Mono](https://fonts.google.com/specimen/Space+Mono) |
| Orbitron | 400, 500, 700, 900 | Headlines, display text, futuristic titles | [fonts.google.com/specimen/Orbitron](https://fonts.google.com/specimen/Orbitron) |
| IBM Plex Mono | 400, 500, 700 | Body text, metadata, system-inspired interfaces | [fonts.google.com/specimen/IBM+Plex+Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) |
| Press Start 2P | 400 | Pixel-art accents, retro labels, 8-bit references | [fonts.google.com/specimen/Press+Start+2P](https://fonts.google.com/specimen/Press+Start+2P) |
| Major Mono Display | 400 | Display headlines, abstract title treatments | [fonts.google.com/specimen/Major+Mono+Display](https://fonts.google.com/specimen/Major+Mono+Display) |
| Russo One | 400 | Bold geometric headlines, impactful display text | [fonts.google.com/specimen/Russo+One](https://fonts.google.com/specimen/Russo+One) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Orbitron (700) | Share Tech Mono | Futuristic authority meets clean terminal readability; ideal for tech-forward glitch layouts |
| Russo One | IBM Plex Mono | Bold geometric impact paired with professional monospace; balances chaos with legibility |
| VT323 | Space Mono | Retro pixel nostalgia meets modern monospace precision; perfect for CRT-inspired interfaces |
| Major Mono Display | Share Tech Mono | Abstract, deconstructed headlines with grounded technical body text; maximizes the digital-error feel |
| Orbitron (900) | IBM Plex Mono (400) | Heavy futuristic display with readable IBM technical prose; suitable for data-driven glitch dashboards |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Share+Tech+Mono&family=VT323&display=swap');

/* === Base Typography === */
body {
  font-family: 'Share Tech Mono', 'Courier New', Courier, monospace;
  font-size: 16px;
  line-height: 1.7;
  color: var(--glitch-text);
  background-color: var(--glitch-bg);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Orbitron', 'Arial Black', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  line-height: 1.1;
  color: var(--glitch-white);
  margin: 0 0 0.5em 0;
}

h1 {
  font-size: clamp(2.5rem, 7vw, 6rem);
  font-weight: 900;
}

h2 {
  font-size: clamp(1.8rem, 4vw, 3rem);
  font-weight: 700;
}

h3 {
  font-size: clamp(1.2rem, 2.5vw, 1.8rem);
  font-weight: 700;
}

a {
  color: var(--glitch-link);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: color 0.15s ease, border-color 0.15s ease;
}

a:hover {
  color: var(--glitch-link-hover);
  border-bottom-color: var(--glitch-link-hover);
}

code, pre {
  font-family: 'Share Tech Mono', 'Courier New', monospace;
  background-color: var(--glitch-static-gray);
  border: 1px solid var(--glitch-muted);
  padding: 0.2em 0.5em;
  color: var(--glitch-green);
}

pre {
  padding: 1.25em;
  overflow-x: auto;
  white-space: pre;
  border-left: 3px solid var(--glitch-cyan);
}

::selection {
  background-color: var(--glitch-magenta);
  color: var(--glitch-white);
}
```

---

## Layout Principles

- **Dark-first canvas** -- always design on black or near-black backgrounds; glitch effects depend on high-contrast neon colors that wash out on light surfaces
- **Layered z-index composition** -- scan lines, noise textures, and interference patterns are applied as absolutely-positioned overlay layers on top of content, building visual depth through stacking
- **Broken grid with intent** -- content blocks are deliberately offset, rotated slightly, or overlapping, but always with an underlying invisible grid that prevents total visual chaos
- **Full-bleed sections** -- hero areas, image treatments, and key visual moments span the full viewport width to maximize immersive impact
- **Asymmetric balance** -- avoid perfectly centered, symmetrical layouts; shift elements off-center and use uneven margins to reinforce the sense of disruption
- **Dense information zones** -- cluster data, links, and metadata in tight blocks reminiscent of terminal output or hex editor displays, contrasted against empty dark space
- **Viewport-height sections** -- key content areas use `min-height: 100vh` to create distinct scene-like moments as the user scrolls through the corrupted landscape
- **Animation as layout feature** -- moving, flickering, and shifting elements are part of the spatial composition, not just decoration; account for animated states when planning element placement
- **Mobile degradation** -- on smaller screens, reduce animation intensity and layer count; prioritize content readability over effect complexity, as mobile GPUs may struggle with heavy compositing

---

## CSS / Design Techniques

### Glitch Card Component

A content card with scan line overlay, subtle RGB offset on hover, and a corrupted-data border treatment.

```css
.glitch-card {
  position: relative;
  background-color: var(--glitch-surface);
  border: 1px solid var(--glitch-muted);
  padding: 2rem;
  overflow: hidden;
  transition: transform 0.2s ease, border-color 0.3s ease;
}

/* Scan line overlay */
.glitch-card::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 2px,
    rgba(0, 0, 0, 0.15) 2px,
    rgba(0, 0, 0, 0.15) 4px
  );
  pointer-events: none;
  z-index: 1;
}

.glitch-card:hover {
  border-color: var(--glitch-cyan);
  transform: translate(-2px, -1px);
  box-shadow:
    2px 0 0 var(--glitch-red),
    -2px 0 0 var(--glitch-blue);
}

.glitch-card h3 {
  position: relative;
  z-index: 2;
  font-family: 'Orbitron', sans-serif;
  font-size: 1.1rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--glitch-cyan);
  margin-bottom: 0.75rem;
}

.glitch-card p {
  position: relative;
  z-index: 2;
  font-size: 0.9rem;
  line-height: 1.6;
  color: var(--glitch-text);
}

.glitch-card .tag {
  display: inline-block;
  position: relative;
  z-index: 2;
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  padding: 0.25rem 0.6rem;
  border: 1px solid var(--glitch-muted);
  color: var(--glitch-green);
  margin-right: 0.25rem;
  margin-top: 0.75rem;
}
```

### Glitch Button Component

A button with animated RGB split on hover, using pseudo-elements to create the chromatic aberration effect.

```css
.glitch-btn {
  position: relative;
  display: inline-block;
  font-family: 'Orbitron', sans-serif;
  font-size: 0.85rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  padding: 0.9rem 2rem;
  border: 1px solid var(--glitch-cyan);
  background-color: transparent;
  color: var(--glitch-cyan);
  cursor: pointer;
  text-decoration: none;
  overflow: hidden;
  transition: background-color 0.2s ease, color 0.2s ease;
}

.glitch-btn::before,
.glitch-btn::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0.9rem 2rem;
  opacity: 0;
  pointer-events: none;
}

.glitch-btn::before {
  color: var(--glitch-red);
  z-index: -1;
}

.glitch-btn::after {
  color: var(--glitch-blue);
  z-index: -1;
}

.glitch-btn:hover {
  background-color: var(--glitch-cyan);
  color: var(--glitch-void);
  animation: btn-glitch 0.3s ease forwards;
}

.glitch-btn:hover::before {
  opacity: 0.7;
  animation: rgb-shift-left 0.4s infinite;
}

.glitch-btn:hover::after {
  opacity: 0.7;
  animation: rgb-shift-right 0.4s infinite;
}

@keyframes btn-glitch {
  0% { transform: translate(0); }
  20% { transform: translate(-3px, 2px); }
  40% { transform: translate(2px, -1px); }
  60% { transform: translate(-1px, 1px); }
  80% { transform: translate(1px, -2px); }
  100% { transform: translate(0); }
}

@keyframes rgb-shift-left {
  0%, 100% { transform: translate(-2px, 0); }
  50% { transform: translate(-4px, 1px); }
}

@keyframes rgb-shift-right {
  0%, 100% { transform: translate(2px, 0); }
  50% { transform: translate(4px, -1px); }
}
```

### Glitch Navigation Bar

A top navigation with a subtle interference band and scan line texture, featuring glitch-styled hover states.

```css
.glitch-nav {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
  background-color: var(--glitch-void);
  border-bottom: 1px solid var(--glitch-muted);
  z-index: 100;
}

/* Bottom interference line */
.glitch-nav::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: linear-gradient(
    90deg,
    var(--glitch-cyan) 0%,
    var(--glitch-magenta) 33%,
    var(--glitch-green) 66%,
    var(--glitch-cyan) 100%
  );
  background-size: 200% 100%;
  animation: interference-scan 3s linear infinite;
}

@keyframes interference-scan {
  0% { background-position: 0% 0%; }
  100% { background-position: 200% 0%; }
}

.glitch-nav .logo {
  font-family: 'Orbitron', sans-serif;
  font-size: 1.1rem;
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--glitch-white);
  text-decoration: none;
}

.glitch-nav ul {
  list-style: none;
  display: flex;
  gap: 0;
  margin: 0;
  padding: 0;
}

.glitch-nav a {
  display: block;
  padding: 0.5rem 1.25rem;
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--glitch-text);
  text-decoration: none;
  border: none;
  position: relative;
  transition: color 0.15s ease;
}

.glitch-nav a:hover {
  color: var(--glitch-cyan);
  text-shadow:
    2px 0 var(--glitch-red),
    -2px 0 var(--glitch-blue);
}

.glitch-nav a::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  width: 0;
  height: 1px;
  background-color: var(--glitch-cyan);
  transition: width 0.2s ease, left 0.2s ease;
}

.glitch-nav a:hover::after {
  width: 100%;
  left: 0;
}
```

### Glitch Hero Section

A full-viewport hero with animated RGB-split headline text, scan line overlay, and noise texture background.

```css
.glitch-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 4rem 3rem;
  background-color: var(--glitch-void);
  overflow: hidden;
}

/* Noise texture layer */
.glitch-hero::before {
  content: '';
  position: absolute;
  inset: -50%;
  width: 200%;
  height: 200%;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
  pointer-events: none;
  z-index: 1;
}

/* Scan line overlay */
.glitch-hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 2px,
    rgba(0, 0, 0, 0.12) 2px,
    rgba(0, 0, 0, 0.12) 4px
  );
  pointer-events: none;
  z-index: 2;
}

.glitch-hero__content {
  position: relative;
  z-index: 3;
  max-width: 900px;
}

.glitch-hero__title {
  font-family: 'Orbitron', sans-serif;
  font-size: clamp(3rem, 9vw, 8rem);
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  line-height: 0.95;
  color: var(--glitch-white);
  position: relative;
}

.glitch-hero__subtitle {
  font-family: 'Share Tech Mono', monospace;
  font-size: clamp(0.9rem, 1.5vw, 1.2rem);
  color: var(--glitch-text);
  max-width: 50ch;
  margin-top: 1.5rem;
  line-height: 1.7;
}

.glitch-hero__actions {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  margin-top: 2.5rem;
}
```

### RGB Split Text Effect

An animated chromatic aberration effect on text using pseudo-elements, where red and blue copies of the text are offset and blended to create the signature glitch look.

```css
.rgb-split {
  position: relative;
  display: inline-block;
  color: var(--glitch-white);
  font-family: 'Orbitron', sans-serif;
  font-weight: 900;
  text-transform: uppercase;
}

.rgb-split::before,
.rgb-split::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.rgb-split::before {
  color: var(--glitch-red);
  mix-blend-mode: screen;
  animation: rgb-split-red 3s infinite;
  clip-path: inset(0 0 0 0);
}

.rgb-split::after {
  color: var(--glitch-blue);
  mix-blend-mode: screen;
  animation: rgb-split-blue 3s infinite;
  clip-path: inset(0 0 0 0);
}

@keyframes rgb-split-red {
  0%, 100% { transform: translate(-2px, 0); }
  25% { transform: translate(2px, 1px); clip-path: inset(30% 0 40% 0); }
  50% { transform: translate(-1px, -1px); clip-path: inset(0 0 0 0); }
  75% { transform: translate(3px, 0); clip-path: inset(60% 0 10% 0); }
}

@keyframes rgb-split-blue {
  0%, 100% { transform: translate(2px, 0); }
  25% { transform: translate(-3px, -1px); clip-path: inset(50% 0 20% 0); }
  50% { transform: translate(1px, 1px); clip-path: inset(0 0 0 0); }
  75% { transform: translate(-2px, 0); clip-path: inset(10% 0 70% 0); }
}

/* Reduced motion variant */
@media (prefers-reduced-motion: reduce) {
  .rgb-split::before {
    animation: none;
    transform: translate(-2px, 0);
  }
  .rgb-split::after {
    animation: none;
    transform: translate(2px, 0);
  }
}
```

### Scan Line Overlay

A reusable overlay component that applies CRT-style scan lines to any container, with optional animated flicker.

```css
.scanlines {
  position: relative;
  overflow: hidden;
}

.scanlines::after {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent 0px,
    transparent 2px,
    rgba(0, 0, 0, 0.2) 2px,
    rgba(0, 0, 0, 0.2) 4px
  );
  pointer-events: none;
  z-index: 10;
}

/* Animated variant with vertical scan bar */
.scanlines--animated::before {
  content: '';
  position: absolute;
  top: -100%;
  left: 0;
  width: 100%;
  height: 30%;
  background: linear-gradient(
    180deg,
    transparent 0%,
    rgba(0, 255, 255, 0.03) 50%,
    transparent 100%
  );
  pointer-events: none;
  z-index: 11;
  animation: scan-sweep 4s linear infinite;
}

@keyframes scan-sweep {
  0% { top: -30%; }
  100% { top: 130%; }
}

/* CRT screen curvature (optional enhancement) */
.scanlines--crt {
  border-radius: 12px;
  box-shadow:
    inset 0 0 60px rgba(0, 0, 0, 0.4),
    inset 0 0 10px rgba(0, 0, 0, 0.3);
}

@media (prefers-reduced-motion: reduce) {
  .scanlines--animated::before {
    animation: none;
    display: none;
  }
}
```

### Datamosh / Corrupted Image Treatment

A CSS treatment that simulates datamoshing on images using blend modes, clip-path slicing, and color channel manipulation.

```css
.datamosh {
  position: relative;
  overflow: hidden;
  display: block;
}

.datamosh img {
  display: block;
  width: 100%;
  height: auto;
  filter: contrast(1.1) saturate(1.3);
}

/* Red channel ghost */
.datamosh::before {
  content: '';
  position: absolute;
  inset: 0;
  background: inherit;
  mix-blend-mode: multiply;
  opacity: 0.6;
  background-color: var(--glitch-red);
  clip-path: polygon(0 20%, 100% 15%, 100% 45%, 0 50%);
  transform: translate(8px, 0);
  z-index: 2;
}

/* Blue channel ghost */
.datamosh::after {
  content: '';
  position: absolute;
  inset: 0;
  background: inherit;
  mix-blend-mode: screen;
  opacity: 0.5;
  background-color: var(--glitch-blue);
  clip-path: polygon(0 55%, 100% 60%, 100% 80%, 0 75%);
  transform: translate(-6px, 0);
  z-index: 2;
}

/* Animated variant */
.datamosh--animated::before {
  animation: mosh-slice-a 2.5s steps(1) infinite;
}

.datamosh--animated::after {
  animation: mosh-slice-b 3s steps(1) infinite;
}

@keyframes mosh-slice-a {
  0% { clip-path: polygon(0 20%, 100% 15%, 100% 45%, 0 50%); transform: translate(8px, 0); }
  25% { clip-path: polygon(0 50%, 100% 55%, 100% 70%, 0 65%); transform: translate(-5px, 0); }
  50% { clip-path: polygon(0 10%, 100% 5%, 100% 25%, 0 30%); transform: translate(10px, 0); }
  75% { clip-path: polygon(0 70%, 100% 75%, 100% 90%, 0 85%); transform: translate(-3px, 0); }
}

@keyframes mosh-slice-b {
  0% { clip-path: polygon(0 55%, 100% 60%, 100% 80%, 0 75%); transform: translate(-6px, 0); }
  33% { clip-path: polygon(0 30%, 100% 25%, 100% 50%, 0 55%); transform: translate(7px, 0); }
  66% { clip-path: polygon(0 80%, 100% 85%, 100% 95%, 0 90%); transform: translate(-9px, 0); }
}

@media (prefers-reduced-motion: reduce) {
  .datamosh--animated::before,
  .datamosh--animated::after {
    animation: none;
  }
}
```

### Noise Texture Background

A pure CSS animated noise background using SVG filters, creating a subtle static grain effect across any element.

```css
.noise-bg {
  position: relative;
  isolation: isolate;
}

.noise-bg::before {
  content: '';
  position: absolute;
  inset: 0;
  z-index: -1;
  opacity: 0.06;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 512 512' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)'/%3E%3C/svg%3E");
  background-repeat: repeat;
  pointer-events: none;
}

/* Animated grain variant */
.noise-bg--animated::before {
  animation: noise-shift 0.5s steps(4) infinite;
}

@keyframes noise-shift {
  0% { transform: translate(0, 0); }
  25% { transform: translate(-5%, -5%); }
  50% { transform: translate(5%, 2%); }
  75% { transform: translate(-2%, 5%); }
  100% { transform: translate(0, 0); }
}

@media (prefers-reduced-motion: reduce) {
  .noise-bg--animated::before {
    animation: none;
  }
}
```

---

## Design Do's and Don'ts

### Do's

- **Layer multiple effects** -- combine scan lines, noise textures, and RGB splits for rich, deep visual compositions; a single effect looks thin, but layered effects create immersive environments
- **Use dark backgrounds** -- glitch effects derive their energy from high-contrast neon on dark surfaces; a black or near-black canvas is foundational to the aesthetic
- **Animate with restraint** -- use CSS animations for glitch effects but keep them subtle and intermittent; constant violent flickering becomes fatiguing and can trigger photosensitivity issues
- **Honor `prefers-reduced-motion`** -- always provide a static fallback for every animated effect; users with motion sensitivity must be able to experience the design without discomfort
- **Maintain text legibility** -- apply heavy distortion to display headings and decorative elements but keep body text clean, readable, and well-contrasted against its background
- **Use monospaced fonts** -- monospace typefaces reinforce the digital, code-driven nature of the aesthetic and provide a visual connection to the data layer being exposed
- **Include interactive feedback** -- hover states that trigger glitch effects create a sense of interaction with a volatile system; make the user feel like their input causes disruption
- **Ground chaos in structure** -- even the most corrupted layouts need an underlying grid and clear content hierarchy; the user should still be able to navigate and consume content

### Don'ts

- **Don't use light backgrounds** -- pastel or white backgrounds rob glitch effects of their visual power; the aesthetic depends on the luminosity contrast of neon on dark surfaces
- **Don't apply glitch effects to all text** -- if everything is corrupted, nothing stands out; reserve heavy distortion for display headings, hero text, and accent elements
- **Don't create seizure-inducing flicker** -- rapid full-screen flashing violates WCAG accessibility guidelines and can cause physical harm; keep flicker rates below 3Hz and avoid flashing large areas of the screen
- **Don't ignore performance** -- layered pseudo-elements, blend modes, and clip-path animations are GPU-intensive; test on low-powered devices and set animation budgets
- **Don't use glitch as a substitute for content** -- visual corruption effects should enhance meaningful content, not mask its absence; the aesthetic is a treatment, not a replacement for substance
- **Don't forget mobile** -- complex compositing effects can drain batteries and lag on mobile devices; use `@media` queries to simplify or disable heavy effects on smaller screens
- **Don't mix with soft, organic aesthetics** -- the sharp, digital, pixel-level nature of Glitch Art clashes with rounded, natural, or handcrafted design languages; keep the visual vocabulary consistently digital

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Cyberpunk](Cyberpunk.md) | Shares the neon-on-dark palette and dystopian digital atmosphere; Cyberpunk builds narrative worlds while Glitch Art focuses on the material breakdown of the medium itself |
| [Vaporwave](Vaporwave.md) | Both reference digital artifacts and retro technology, but Vaporwave uses pastels and ironic nostalgia where Glitch Art embraces raw, aggressive corruption |
| [Y2K Futurism](Y2K_Futurism.md) | Both celebrate digital technology as a visual subject; Y2K looks forward with optimism while Glitch Art exposes the fragility behind the polished interface |
| [Terminal CLI Aesthetic](Terminal_CLI_Aesthetic.md) | Shares monospaced typography and the foregrounding of digital infrastructure; Terminal is ordered and systematic while Glitch Art breaks those systems apart |
| [Weirdcore](Weirdcore.md) | Both create unsettling digital imagery through distortion and corruption, but Weirdcore targets surreal emotional discomfort while Glitch Art celebrates technical materiality |
| [Low Poly](Low_Poly.md) | Both foreground the building blocks of digital graphics (polygons vs. pixels); Low Poly is geometric and controlled, Glitch Art is chaotic and deconstructive |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Glitch Art Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Share+Tech+Mono&family=VT323&display=swap" rel="stylesheet">
  <style>
    /* --- Custom Properties --- */
    :root {
      --glitch-void: #0d0d0d;
      --glitch-screen-dark: #1a1a2e;
      --glitch-static-gray: #2a2a2a;
      --glitch-red: #ff0040;
      --glitch-green: #00ff41;
      --glitch-blue: #0080ff;
      --glitch-cyan: #00ffff;
      --glitch-magenta: #ff00ff;
      --glitch-pink: #ff2e97;
      --glitch-yellow: #f5f500;
      --glitch-purple: #7b2fbe;
      --glitch-orange: #ff6b2b;
      --glitch-white: #ffffff;
      --glitch-text: #e0e0e0;
      --glitch-muted: #444444;
    }

    /* --- Reset --- */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Share Tech Mono', 'Courier New', Courier, monospace;
      font-size: 16px;
      line-height: 1.7;
      color: var(--glitch-text);
      background-color: var(--glitch-void);
      -webkit-font-smoothing: antialiased;
      overflow-x: hidden;
    }

    h1, h2, h3, h4 {
      font-family: 'Orbitron', 'Arial Black', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      line-height: 1.1;
      color: var(--glitch-white);
    }

    a {
      color: var(--glitch-cyan);
      text-decoration: none;
      transition: color 0.15s ease;
    }

    a:hover {
      color: var(--glitch-magenta);
    }

    ::selection {
      background-color: var(--glitch-magenta);
      color: var(--glitch-white);
    }

    /* --- Navigation --- */
    .nav {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 2rem;
      background-color: var(--glitch-void);
      border-bottom: 1px solid var(--glitch-muted);
    }

    .nav::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 2px;
      background: linear-gradient(
        90deg,
        var(--glitch-cyan),
        var(--glitch-magenta),
        var(--glitch-green),
        var(--glitch-cyan)
      );
      background-size: 200% 100%;
      animation: interference-line 3s linear infinite;
    }

    @keyframes interference-line {
      0% { background-position: 0% 0%; }
      100% { background-position: 200% 0%; }
    }

    .nav .logo {
      font-family: 'Orbitron', sans-serif;
      font-size: 1rem;
      font-weight: 900;
      text-transform: uppercase;
      letter-spacing: 0.25em;
      color: var(--glitch-white);
    }

    .nav ul {
      list-style: none;
      display: flex;
      gap: 0;
    }

    .nav a {
      display: block;
      padding: 0.5rem 1.2rem;
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      color: var(--glitch-text);
    }

    .nav a:hover {
      color: var(--glitch-cyan);
      text-shadow:
        2px 0 var(--glitch-red),
        -2px 0 var(--glitch-blue);
    }

    /* --- Hero --- */
    .hero {
      position: relative;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 4rem 3rem;
      overflow: hidden;
    }

    /* Scan lines */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        0deg,
        transparent 0px,
        transparent 2px,
        rgba(0, 0, 0, 0.12) 2px,
        rgba(0, 0, 0, 0.12) 4px
      );
      pointer-events: none;
      z-index: 2;
    }

    .hero-content {
      position: relative;
      z-index: 3;
      max-width: 900px;
    }

    /* RGB Split Headline */
    .hero-title {
      font-size: clamp(3rem, 9vw, 8rem);
      font-weight: 900;
      line-height: 0.95;
      position: relative;
      display: inline-block;
    }

    .hero-title::before,
    .hero-title::after {
      content: attr(data-text);
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      overflow: hidden;
    }

    .hero-title::before {
      color: var(--glitch-red);
      mix-blend-mode: screen;
      animation: glitch-r 3s infinite;
    }

    .hero-title::after {
      color: var(--glitch-blue);
      mix-blend-mode: screen;
      animation: glitch-b 3s infinite;
    }

    @keyframes glitch-r {
      0%, 100% { transform: translate(-2px, 0); clip-path: inset(0 0 0 0); }
      20% { transform: translate(3px, 1px); clip-path: inset(25% 0 55% 0); }
      40% { transform: translate(-1px, -1px); clip-path: inset(0 0 0 0); }
      60% { transform: translate(4px, 0); clip-path: inset(60% 0 5% 0); }
      80% { transform: translate(-2px, 1px); clip-path: inset(0 0 0 0); }
    }

    @keyframes glitch-b {
      0%, 100% { transform: translate(2px, 0); clip-path: inset(0 0 0 0); }
      20% { transform: translate(-3px, -1px); clip-path: inset(50% 0 20% 0); }
      40% { transform: translate(1px, 1px); clip-path: inset(0 0 0 0); }
      60% { transform: translate(-4px, 0); clip-path: inset(10% 0 70% 0); }
      80% { transform: translate(2px, -1px); clip-path: inset(0 0 0 0); }
    }

    .hero-sub {
      font-size: clamp(0.9rem, 1.5vw, 1.15rem);
      max-width: 50ch;
      margin-top: 1.5rem;
      color: var(--glitch-text);
      line-height: 1.8;
    }

    .hero-sub span {
      color: var(--glitch-cyan);
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin-top: 2.5rem;
    }

    /* --- Buttons --- */
    .btn {
      position: relative;
      display: inline-block;
      font-family: 'Orbitron', sans-serif;
      font-size: 0.78rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      padding: 0.85rem 2rem;
      border: 1px solid var(--glitch-cyan);
      background-color: transparent;
      color: var(--glitch-cyan);
      cursor: pointer;
      text-decoration: none;
      overflow: hidden;
      transition: background-color 0.2s ease, color 0.2s ease;
    }

    .btn:hover {
      background-color: var(--glitch-cyan);
      color: var(--glitch-void);
      animation: btn-shake 0.3s ease;
    }

    @keyframes btn-shake {
      0% { transform: translate(0); }
      20% { transform: translate(-3px, 2px); }
      40% { transform: translate(2px, -1px); }
      60% { transform: translate(-1px, 1px); }
      80% { transform: translate(1px, -2px); }
      100% { transform: translate(0); }
    }

    .btn--alt {
      border-color: var(--glitch-pink);
      color: var(--glitch-pink);
    }

    .btn--alt:hover {
      background-color: var(--glitch-pink);
      color: var(--glitch-void);
    }

    /* --- Section --- */
    .section {
      position: relative;
      padding: 5rem 3rem;
      border-top: 1px solid var(--glitch-muted);
    }

    .section h2 {
      font-size: clamp(1.8rem, 4vw, 3rem);
      margin-bottom: 1rem;
      color: var(--glitch-cyan);
    }

    .section > p {
      max-width: 65ch;
      margin-bottom: 2rem;
      line-height: 1.8;
    }

    /* Section label */
    .section-label {
      font-family: 'Share Tech Mono', monospace;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.25em;
      color: var(--glitch-muted);
      margin-bottom: 0.5rem;
      display: block;
    }

    /* --- Card Grid --- */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 1px;
      background-color: var(--glitch-muted);
      border: 1px solid var(--glitch-muted);
    }

    .card {
      position: relative;
      background-color: var(--glitch-screen-dark);
      padding: 2rem;
      overflow: hidden;
      transition: transform 0.15s ease;
    }

    /* Scan lines on cards */
    .card::before {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        0deg,
        transparent 0px,
        transparent 2px,
        rgba(0, 0, 0, 0.1) 2px,
        rgba(0, 0, 0, 0.1) 4px
      );
      pointer-events: none;
      z-index: 1;
    }

    .card:hover {
      transform: translate(-2px, -1px);
      box-shadow:
        3px 0 0 var(--glitch-red),
        -3px 0 0 var(--glitch-blue);
    }

    .card h3 {
      position: relative;
      z-index: 2;
      font-size: 1rem;
      letter-spacing: 0.1em;
      color: var(--glitch-cyan);
      margin-bottom: 0.75rem;
    }

    .card p {
      position: relative;
      z-index: 2;
      font-size: 0.88rem;
      line-height: 1.7;
      margin-bottom: 1rem;
    }

    .card .tag {
      display: inline-block;
      position: relative;
      z-index: 2;
      font-size: 0.68rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      padding: 0.2rem 0.5rem;
      border: 1px solid var(--glitch-muted);
      color: var(--glitch-green);
      margin-right: 0.3rem;
      margin-bottom: 0.3rem;
    }

    /* --- Data Table --- */
    .data-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.85rem;
    }

    .data-table th,
    .data-table td {
      border: 1px solid var(--glitch-muted);
      padding: 0.75rem 1rem;
      text-align: left;
    }

    .data-table th {
      background-color: var(--glitch-screen-dark);
      color: var(--glitch-cyan);
      font-family: 'Orbitron', sans-serif;
      font-size: 0.72rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      font-weight: 700;
    }

    .data-table tr:hover td {
      background-color: rgba(0, 255, 255, 0.04);
    }

    .data-table td:first-child {
      color: var(--glitch-white);
    }

    /* --- Corrupted Divider --- */
    .divider {
      position: relative;
      height: 4px;
      background: var(--glitch-muted);
      margin: 0;
      overflow: hidden;
    }

    .divider::before {
      content: '';
      position: absolute;
      inset: 0;
      background: linear-gradient(
        90deg,
        var(--glitch-cyan) 0%,
        var(--glitch-pink) 25%,
        var(--glitch-void) 30%,
        var(--glitch-void) 45%,
        var(--glitch-green) 50%,
        var(--glitch-void) 55%,
        var(--glitch-void) 70%,
        var(--glitch-magenta) 75%,
        var(--glitch-cyan) 100%
      );
      animation: divider-scan 4s linear infinite;
      background-size: 200% 100%;
    }

    @keyframes divider-scan {
      0% { background-position: 0% 0%; }
      100% { background-position: 200% 0%; }
    }

    /* --- Signal Interference Banner --- */
    .interference {
      position: relative;
      padding: 2.5rem 3rem;
      background-color: var(--glitch-screen-dark);
      border-top: 1px solid var(--glitch-muted);
      border-bottom: 1px solid var(--glitch-muted);
      overflow: hidden;
      text-align: center;
    }

    .interference::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 300%;
      height: 100%;
      background: repeating-linear-gradient(
        90deg,
        transparent 0px,
        transparent 3px,
        rgba(0, 255, 255, 0.03) 3px,
        rgba(0, 255, 255, 0.03) 6px
      );
      animation: h-scan 2s linear infinite;
      pointer-events: none;
    }

    @keyframes h-scan {
      0% { transform: translateX(0); }
      100% { transform: translateX(33.33%); }
    }

    .interference .display-text {
      font-family: 'VT323', monospace;
      font-size: clamp(1.5rem, 3vw, 2.5rem);
      color: var(--glitch-green);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      position: relative;
      z-index: 2;
    }

    /* --- Footer --- */
    .footer {
      padding: 2.5rem 3rem;
      border-top: 1px solid var(--glitch-muted);
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 1rem;
    }

    .footer p {
      font-size: 0.78rem;
      color: var(--glitch-muted);
    }

    .footer a {
      color: var(--glitch-text);
      margin-left: 1.5rem;
      font-size: 0.78rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    .footer a:hover {
      color: var(--glitch-cyan);
    }

    /* --- Utilities --- */
    .mt-1 { margin-top: 1rem; }
    .mt-2 { margin-top: 2rem; }
    .text-cyan { color: var(--glitch-cyan); }
    .text-pink { color: var(--glitch-pink); }
    .text-green { color: var(--glitch-green); }

    /* --- Reduced Motion --- */
    @media (prefers-reduced-motion: reduce) {
      .hero-title::before,
      .hero-title::after {
        animation: none;
        transform: translate(0);
        clip-path: inset(0 0 0 0);
      }
      .hero-title::before { transform: translate(-2px, 0); }
      .hero-title::after { transform: translate(2px, 0); }
      .nav::after { animation: none; }
      .divider::before { animation: none; }
      .interference::before { animation: none; }
      .btn:hover { animation: none; }
    }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      .hero {
        min-height: 80vh;
        padding: 3rem 1.5rem;
      }
      .section {
        padding: 3rem 1.5rem;
      }
      .nav {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.75rem;
        padding: 1rem 1.5rem;
      }
      .nav ul {
        flex-wrap: wrap;
      }
      .card-grid {
        grid-template-columns: 1fr;
      }
      .footer {
        flex-direction: column;
        align-items: flex-start;
        padding: 2rem 1.5rem;
      }
      .footer a {
        margin-left: 0;
        margin-right: 1rem;
      }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="nav">
    <span class="logo">GL//TCH</span>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#data">Data</a></li>
      <li><a href="#signal">Signal</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <section class="hero">
    <div class="hero-content">
      <h1 class="hero-title" data-text="Glitch Art">Glitch Art</h1>
      <p class="hero-sub">
        The beauty of <span>broken data</span>. We find aesthetics in
        technological failure -- pixel corruption, signal interference,
        and the hidden structures revealed when digital systems malfunction.
        This is not an error. This is the message.
      </p>
      <div class="hero-actions">
        <a href="#projects" class="btn">Explore Projects</a>
        <a href="#data" class="btn btn--alt">View Data</a>
      </div>
    </div>
  </section>

  <!-- CORRUPTED DIVIDER -->
  <div class="divider"></div>

  <!-- ABOUT -->
  <section class="section" id="about">
    <span class="section-label">// 001 &mdash; About</span>
    <h2>Error as Aesthetic</h2>
    <p>
      Glitch Art transforms technological failure into a creative medium.
      By deliberately inducing or capturing malfunctions in digital systems,
      we expose the hidden mechanics of the tools we use every day.
      Datamoshing, pixel sorting, RGB channel splitting, and data bending
      are not bugs to be fixed -- they are the raw material of a new
      visual language.
    </p>
  </section>

  <!-- PROJECTS -->
  <section class="section" id="projects">
    <span class="section-label">// 002 &mdash; Projects</span>
    <h2>Projects</h2>
    <p>
      Each project explores a different facet of digital disruption.
      Hover to corrupt.
    </p>
    <div class="card-grid mt-2">
      <div class="card">
        <h3>Datamosh Engine</h3>
        <p>A real-time video corruption tool that removes I-frames from compressed video streams, producing the flowing, painterly distortions of datamoshing in the browser.</p>
        <span class="tag">Video</span>
        <span class="tag">WebCodecs</span>
        <span class="tag">Real-time</span>
      </div>
      <div class="card">
        <h3>Hex Painter</h3>
        <p>Open any image file as raw hexadecimal data and paint directly into the byte stream. Watch the image reconstruct with each corrupted edit.</p>
        <span class="tag">Data Bending</span>
        <span class="tag">Canvas</span>
      </div>
      <div class="card">
        <h3>Channel Drift</h3>
        <p>An interactive installation that separates the red, green, and blue channels of a live webcam feed and maps each to independent mouse-controlled offsets.</p>
        <span class="tag">RGB Split</span>
        <span class="tag">WebGL</span>
        <span class="tag">Interactive</span>
      </div>
      <div class="card">
        <h3>Signal Decay</h3>
        <p>Generative compositions that simulate electromagnetic interference, scan line degradation, and VHS tracking errors using pure CSS and SVG filters.</p>
        <span class="tag">Generative</span>
        <span class="tag">CSS</span>
        <span class="tag">SVG</span>
      </div>
      <div class="card">
        <h3>Codec Autopsy</h3>
        <p>A visual explainer that deconstructs JPEG, PNG, and WebP compression in real time, revealing the block artifacts and quantization tables hidden inside every image.</p>
        <span class="tag">Compression</span>
        <span class="tag">Education</span>
      </div>
      <div class="card">
        <h3>Pixel Sort Lab</h3>
        <p>Upload an image and apply pixel sorting algorithms -- by brightness, hue, or saturation -- to create the cascading, waterfall-like distortions of sorted pixel rows.</p>
        <span class="tag">Pixel Sorting</span>
        <span class="tag">WASM</span>
      </div>
    </div>
  </section>

  <!-- SIGNAL INTERFERENCE BANNER -->
  <div class="interference" id="signal">
    <div class="display-text">&#x2588;&#x2588; Signal Acquired &mdash; Corruption Level: 87% &#x2588;&#x2588;</div>
  </div>

  <!-- DATA TABLE -->
  <section class="section" id="data">
    <span class="section-label">// 003 &mdash; Data</span>
    <h2>Corruption Index</h2>
    <p>
      Measured distortion parameters across active signal channels.
    </p>
    <table class="data-table mt-2">
      <thead>
        <tr>
          <th>Channel</th>
          <th>Offset</th>
          <th>Noise Floor</th>
          <th>Artifact Rate</th>
          <th>Status</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>RED</td>
          <td>+3px / -1px</td>
          <td>0.042</td>
          <td>12.7/sec</td>
          <td class="text-pink">CORRUPTED</td>
        </tr>
        <tr>
          <td>GREEN</td>
          <td>+0px / +2px</td>
          <td>0.018</td>
          <td>3.1/sec</td>
          <td class="text-green">NOMINAL</td>
        </tr>
        <tr>
          <td>BLUE</td>
          <td>-2px / +1px</td>
          <td>0.037</td>
          <td>9.4/sec</td>
          <td class="text-cyan">DEGRADED</td>
        </tr>
        <tr>
          <td>ALPHA</td>
          <td>+0px / +0px</td>
          <td>0.003</td>
          <td>0.2/sec</td>
          <td class="text-green">NOMINAL</td>
        </tr>
        <tr>
          <td>SYNC</td>
          <td>+7px / -4px</td>
          <td>0.089</td>
          <td>24.1/sec</td>
          <td class="text-pink">CRITICAL</td>
        </tr>
      </tbody>
    </table>
  </section>

  <!-- CONTACT -->
  <section class="section" id="contact">
    <span class="section-label">// 004 &mdash; Contact</span>
    <h2>Transmit</h2>
    <p>
      Signal endpoint: <a href="mailto:glitch@example.com">glitch@example.com</a>
      &mdash; Source: <a href="#">view repository</a>
      &mdash; License: MIT
    </p>
  </section>

  <!-- FOOTER -->
  <footer class="footer">
    <p>&copy; 2026 GL//TCH &mdash; Error is the message.</p>
    <nav>
      <a href="#">Top</a>
      <a href="#">Source</a>
      <a href="#">RSS</a>
    </nav>
  </footer>

</body>
</html>
```
