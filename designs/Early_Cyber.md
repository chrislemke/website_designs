# Early Cyber

An aesthetic born from the first wave of desktop publishing and image manipulation software,
spanning the mid-1980s to mid-1990s. Early Cyber captures the raw, experimental energy of
newly accessible digital tools -- pixelization, thermographic imagery, fractals, and warped
fonts -- before mainstream polish arrived. It reflects a moment when artists, musicians, and
TV producers were discovering what computers could do to visuals and embracing the alien,
often garish results as a legitimate style rather than a technical limitation.

---

## Visual Characteristics

- **Harsh pixelated imagery** -- low-resolution bitmap graphics with visible pixel structure, not smoothed or anti-aliased
- **Thermographic color mapping** -- false-color heat-map rendering applied to photographs and video, turning subjects into vivid rainbow gradients
- **Warped and distorted typography** -- letterforms stretched, squeezed, fisheye-warped, and liquified using early digital transformation tools
- **Dot matrix patterns** -- visible halftone-style dot grids from early printing and display technologies
- **Posterization and solarization** -- reduced color depth creating flat, banded areas of tone with inverted highlight regions
- **Early greenscreen compositing** -- crude chroma-key effects with visible edge artifacts and color spill
- **Kaleidoscope effects** -- mirrored and rotationally tiled imagery creating symmetrical mandala-like patterns
- **Head-up display (HUD) overlays** -- wireframe targeting reticles, data readouts, and scan-line graphics layered over imagery
- **Squash, stretch, and fisheye distortion** -- exaggerated perspective warps applied to faces, objects, and text
- **Fractals** -- Mandelbrot and Julia set renders, often in rainbow colormaps, used as backgrounds and decorative elements
- **Water-drop / ripple tools** -- circular displacement distortions simulating liquid surface effects
- **Glow effects** -- soft luminous halos around text, lines, and shapes, often in neon colors against dark backgrounds
- **Abstract CGI** -- early 3D renders with visible polygon edges, flat shading, and primitive ray-tracing; less polished than later Silicon Dreams imagery

---

## Color Palette

The palette is fundamentally **rainbow-spectrum** -- thermographic false color applied with maximum saturation. Colors shift abruptly rather than blending smoothly, creating banded, posterized regions.

### Primary Palette

| Role                  | Color              | Hex       |
|-----------------------|--------------------|-----------|
| Deep background       | Black              | `#000000` |
| Alt background        | Dark navy          | `#0A0A2E` |
| Thermographic red     | Hot red            | `#FF1A1A` |
| Thermographic orange  | Blaze orange       | `#FF6600` |
| Thermographic yellow  | Bright yellow      | `#FFD700` |
| Thermographic green   | Neon green         | `#00FF41` |
| Thermographic cyan    | Electric cyan      | `#00FFFF` |
| Thermographic blue    | Deep blue          | `#0044FF` |
| Thermographic magenta | Hot magenta        | `#FF00FF` |
| Thermographic violet  | Deep violet        | `#8800FF` |

### Greenscreen Palette

| Role         | Color           | Hex       |
|--------------|-----------------|-----------|
| Terminal bg  | Near-black      | `#001100` |
| Dim green    | Phosphor dark   | `#004400` |
| Mid green    | Phosphor mid    | `#00AA00` |
| Bright green | Phosphor bright | `#00FF41` |
| Peak green   | Phosphor bloom  | `#66FF99` |

### Fractal Accent Colors

| Role          | Color        | Hex       |
|---------------|--------------|-----------|
| Fractal blue  | Cobalt       | `#0055FF` |
| Fractal teal  | Electric     | `#00CED1` |
| Fractal gold  | Amber        | `#FFBF00` |
| Fractal rose  | Neon pink    | `#FF3399` |
| Fractal white | Bloom white  | `#EEFFFF` |

### Usage Notes

- Backgrounds are predominantly **black or very dark** to let neon and thermographic colors glow
- Color transitions should be **abrupt and banded**, not smooth gradients -- use hard color stops
- Rainbow gradients should feel **synthetic and computational**, not natural
- Green-on-black monochrome is equally authentic for terminal/HUD overlays
- Avoid pastels, earth tones, or muted palettes entirely

---

## Typography

- **Warped and distorted display fonts** -- the defining typographic trait; letterforms are never "clean"
- **Fisheye and bulge distortion** applied to headlines
- **Pixelated bitmap fonts** for body text and HUD readouts
- **Monospaced terminal fonts** for data overlays and technical text
- **No conventional serif or sans-serif body text** -- everything should feel digitally processed

### Recommended Google Fonts

| Font                  | Use Case                               | Style                                    |
|-----------------------|----------------------------------------|------------------------------------------|
| **VT323**             | Terminal text, HUD readouts            | Monospace CRT-style pixel font           |
| **Press Start 2P**    | Headings, pixel-heavy sections         | Blocky pixel font                        |
| **Share Tech Mono**   | Data overlays, technical readouts      | Clean monospace with digital feel        |
| **Orbitron**          | Futuristic headings                    | Geometric, digital display typeface      |
| **Silkscreen**        | Small UI text, labels                  | Minimal pixel font                       |
| **Major Mono Display**| Decorative headlines                   | Monospace with quirky digital character   |

### CSS Implementation

```css
@import url('https://fonts.googleapis.com/css2?family=VT323&family=Orbitron:wght@400;700;900&family=Share+Tech+Mono&display=swap');

/* Primary body text -- terminal style */
body {
  font-family: 'VT323', monospace;
  font-size: 20px;
  line-height: 1.6;
  color: #00FF41;
  background: #000000;
  letter-spacing: 0.04em;
}

/* Headlines -- digital display with distortion potential */
h1, h2, h3 {
  font-family: 'Orbitron', sans-serif;
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

/* Data readout text */
.hud-text {
  font-family: 'Share Tech Mono', monospace;
  font-size: 14px;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}
```

### Warped Text Effect

```css
/* Fisheye / bulge distortion on headlines */
.warped-title {
  font-family: 'Orbitron', sans-serif;
  font-size: 4rem;
  font-weight: 900;
  color: #00FFFF;
  text-shadow:
    0 0 10px #00FFFF,
    0 0 30px #0088FF,
    0 0 60px #0044FF;
  filter: url('#fisheye-distort');  /* SVG filter reference */
  animation: text-warp 4s ease-in-out infinite alternate;
}

@keyframes text-warp {
  0% { transform: scaleX(1) scaleY(1); letter-spacing: 0.1em; }
  50% { transform: scaleX(1.15) scaleY(0.85); letter-spacing: 0.2em; }
  100% { transform: scaleX(0.9) scaleY(1.1); letter-spacing: 0.05em; }
}
```

---

## Key Design Elements and Motifs

### Thermographic Imagery
- Photographs and video stills processed through false-color thermal mapping
- Bodies and objects rendered as rainbow heat signatures
- Abrupt color bands rather than smooth gradients

### Fractals
- Mandelbrot set and Julia set renders as backgrounds or decorative panels
- Typically rendered in rainbow or electric color ramps
- Deep zoom imagery with spiraling, self-similar structures

### Wireframe 3D
- Simple geometric solids (spheres, cubes, toruses) in wireframe rendering
- Green or cyan lines on black background
- Visible polygon edges, no texture mapping or smooth shading

### HUD Overlays
- Targeting reticles and crosshairs
- Numeric data readouts with rapidly changing values
- Scan-line sweeps and radar-style circular displays
- Grid coordinates and measurement callouts

### Kaleidoscope Patterns
- Rotationally symmetric mirrored imagery
- Often derived from processed video or photographic source material
- Creates mandala-like decorative frames and backgrounds

### Dot Matrix and Halftone
- Visible dot patterns from early digital printing
- Oversized halftone dots used as texture overlays
- Grid-aligned circular elements creating tonal variation

---

## Composition and Layout Principles

- **Screen-as-monitor metaphor** -- the viewport represents a CRT monitor or early digital display; frame content within a "screen" boundary
- **Dark field composition** -- imagery floats on black or very dark backgrounds, as if displayed in a darkened room
- **Centered focal point** -- key imagery or text placed centrally, often with radial symmetry
- **Layered data overlays** -- HUD elements, readouts, and grid lines layered over primary content
- **Scan-line horizontal bias** -- composition follows horizontal bands and sweep lines
- **Generous negative space** -- isolated glowing elements against darkness create dramatic contrast
- **Frame-within-frame** -- content enclosed in monitor bezels, wireframe boxes, or HUD targeting brackets
- **No conventional grid layouts** -- arrangement feels like a display terminal, not a magazine page

### Layout CSS

```css
/* Monitor-frame container */
.cyber-viewport {
  max-width: 1024px;
  margin: 0 auto;
  background: #000000;
  border: 2px solid #00FF41;
  border-radius: 16px;
  box-shadow:
    0 0 30px rgba(0, 255, 65, 0.15),
    inset 0 0 80px rgba(0, 0, 0, 0.8);
  padding: 40px;
  position: relative;
  overflow: hidden;
}

/* HUD overlay grid */
.hud-overlay {
  position: absolute;
  inset: 0;
  pointer-events: none;
  background-image:
    linear-gradient(rgba(0, 255, 65, 0.03) 1px, transparent 1px),
    linear-gradient(90deg, rgba(0, 255, 65, 0.03) 1px, transparent 1px);
  background-size: 32px 32px;
  z-index: 10;
}
```

---

## Textures and Surface Effects

### Scanline Overlay

```css
.scanlines {
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 9999;
  background: repeating-linear-gradient(
    to bottom,
    transparent 0px,
    transparent 2px,
    rgba(0, 0, 0, 0.2) 2px,
    rgba(0, 0, 0, 0.2) 4px
  );
}
```

### CRT Screen Curvature and Glow

```css
.crt-screen {
  border-radius: 18px;
  box-shadow:
    inset 0 0 100px rgba(0, 0, 0, 0.5),
    0 0 40px rgba(0, 255, 65, 0.1),
    0 0 80px rgba(0, 255, 65, 0.05);
}
```

### Thermographic Gradient

```css
.thermographic {
  background: linear-gradient(
    180deg,
    #FF1A1A 0%,
    #FF6600 15%,
    #FFD700 30%,
    #00FF41 45%,
    #00FFFF 60%,
    #0044FF 75%,
    #8800FF 90%,
    #FF00FF 100%
  );
}

/* Apply thermographic color to text */
.thermo-text {
  background: linear-gradient(
    90deg,
    #FF1A1A, #FF6600, #FFD700,
    #00FF41, #00FFFF, #0044FF,
    #8800FF, #FF00FF
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

### Pixelation Effect

```css
/* Apply to images for deliberately pixelated look */
.pixelated {
  image-rendering: pixelated;
  image-rendering: crisp-edges;
}

/* CSS-only pixelation via downscale/upscale trick */
.pixel-filter {
  filter: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg'><filter id='p'><feConvolveMatrix order='3' kernelMatrix='0 0 0 0 1 0 0 0 0'/></filter></svg>#p");
}
```

### Glow / Bloom Effect

```css
.neon-glow {
  color: #00FFFF;
  text-shadow:
    0 0 4px #00FFFF,
    0 0 11px #00FFFF,
    0 0 19px #00FFFF,
    0 0 40px #0088FF,
    0 0 80px #0088FF;
}

.element-glow {
  box-shadow:
    0 0 5px #00FFFF,
    0 0 15px #00FFFF,
    0 0 30px #0088FF,
    0 0 60px #0044FF;
  border: 1px solid #00FFFF;
}
```

---

## SVG Filters for Distortion Effects

### Fisheye / Bulge Distortion

```html
<svg xmlns="http://www.w3.org/2000/svg" style="position:absolute;width:0;height:0;">
  <filter id="fisheye-distort">
    <feTurbulence type="turbulence" baseFrequency="0.01" numOctaves="2" result="turbulence"/>
    <feDisplacementMap in="SourceGraphic" in2="turbulence" scale="15" xChannelSelector="R" yChannelSelector="G"/>
  </filter>
</svg>
```

### Posterization

```html
<svg xmlns="http://www.w3.org/2000/svg" style="position:absolute;width:0;height:0;">
  <filter id="posterize">
    <feComponentTransfer>
      <feFuncR type="discrete" tableValues="0 0.25 0.5 0.75 1"/>
      <feFuncG type="discrete" tableValues="0 0.25 0.5 0.75 1"/>
      <feFuncB type="discrete" tableValues="0 0.25 0.5 0.75 1"/>
    </feComponentTransfer>
  </filter>
</svg>
```

### Solarization

```css
.solarized {
  filter: saturate(2) contrast(1.5) invert(0.15) hue-rotate(30deg);
}
```

---

## Animation and Motion

### Scan-Line Sweep

```css
@keyframes scan-sweep {
  0% { transform: translateY(-100%); }
  100% { transform: translateY(100vh); }
}

.scan-line {
  position: fixed;
  width: 100%;
  height: 4px;
  background: linear-gradient(
    to bottom,
    transparent,
    rgba(0, 255, 65, 0.3),
    transparent
  );
  animation: scan-sweep 6s linear infinite;
  pointer-events: none;
  z-index: 9998;
}
```

### Data Readout Flicker

```css
@keyframes data-flicker {
  0%, 92%, 100% { opacity: 1; }
  93% { opacity: 0.7; }
  94% { opacity: 1; }
  96% { opacity: 0.4; }
  97% { opacity: 1; }
}

.flicker {
  animation: data-flicker 3s ease-in-out infinite;
}
```

### Fractal Zoom (Background Animation)

```css
@keyframes fractal-zoom {
  0% { background-size: 100% 100%; filter: hue-rotate(0deg); }
  50% { background-size: 200% 200%; filter: hue-rotate(180deg); }
  100% { background-size: 100% 100%; filter: hue-rotate(360deg); }
}

.fractal-bg {
  background-image: url('fractal.png');
  background-position: center;
  animation: fractal-zoom 20s ease-in-out infinite;
}
```

### Glitch Displacement

```css
@keyframes cyber-glitch {
  0%, 95%, 100% { transform: translate(0, 0); filter: none; }
  96% { transform: translate(-3px, 1px); filter: hue-rotate(90deg); }
  97% { transform: translate(2px, -1px); filter: hue-rotate(180deg); }
  98% { transform: translate(-1px, 2px); filter: hue-rotate(270deg); }
  99% { transform: translate(3px, -2px); filter: hue-rotate(45deg); }
}

.glitch {
  animation: cyber-glitch 4s step-end infinite;
}
```

---

## CSS Techniques Summary

| Technique                   | CSS Property / Approach                                                        |
|-----------------------------|--------------------------------------------------------------------------------|
| Thermographic color         | `linear-gradient` with rainbow hard stops on text or backgrounds               |
| Neon glow                   | Multiple `text-shadow` or `box-shadow` with same-hue colors at increasing blur |
| CRT scanlines               | `repeating-linear-gradient` with 2px transparent/dark alternation              |
| Screen curvature            | `border-radius` + deep `inset box-shadow`                                      |
| Pixelation                  | `image-rendering: pixelated` on images and canvases                            |
| Fisheye distortion          | SVG `feTurbulence` + `feDisplacementMap` filters                               |
| Posterization               | SVG `feComponentTransfer` with `discrete` table values                         |
| Solarization                | Combined `saturate()`, `contrast()`, `invert()`, `hue-rotate()` filters        |
| HUD grid overlay            | Two-axis `linear-gradient` background-image at fixed intervals                 |
| Wireframe borders           | Thin solid borders (`1px solid`) in neon green or cyan on black                |
| Data flicker                | `@keyframes` with rapid opacity steps                                          |
| Monitor frame               | `border-radius` + `border` + `box-shadow` to simulate CRT housing             |
| Rainbow text                | `background-clip: text` with multi-stop linear gradient                        |
| Greenscreen monochrome      | Single hue (green) at varying lightness values for all UI elements             |

---

## Cultural Context and Media References

### Television
- *Doctor Who* title sequences (1982-1986) -- pioneering use of early CGI
- ITV *The Chart Show* (1986-1998) -- computer-generated graphics for music programming
- *GamesMaster* intro (1992-1998) -- CG head, wireframe environments, thermographic visuals
- *Red Dwarf* (1988-1999) -- lo-fi spaceship computer interfaces
- *ReBoot* (1994) -- first fully CGI-animated television series

### Film
- *The Lawnmower Man* (1992) -- virtual reality sequences with primitive CGI
- *Hackers* (1995) -- stylized representations of cyberspace
- *Johnny Mnemonic* (1995) -- data visualization and VR environments
- *Batman Forever* (1995) -- neon-soaked Gotham computer interfaces

### Music
- Tangerine Dream -- album artwork with fractal imagery and electronic landscapes
- Billy Idol, *Cyberpunk* (1993) -- thermographic and distorted digital imagery
- Cabaret Voltaire -- pioneering electronic music with early digital video art

---

## Related Aesthetics

- **Cyberdelia** -- psychedelic digital culture of the early-to-mid 1990s; overlaps heavily
- **Cyberpunk** -- broader dystopian tech aesthetic; Early Cyber is the visual artifact of its era
- **Silicon Dreams** -- more polished CGI renders; Early Cyber is the rawer precursor
- **Cassette Futurism** -- analog-era retro-tech; shares the pre-digital-polish sensibility
- **Synthwave** -- modern revival drawing on similar neon-on-dark visual language
- **Vaporwave** -- nostalgic recontextualization of early digital culture
- **Y2K Futurism** -- the polished successor aesthetic that Early Cyber evolved into by the late 1990s
- **Metalheart** -- another late-1990s evolution with chrome and metallic polish
- **Pixel UI** -- pixel-art-based interface design sharing the low-resolution heritage
- **Acid Design** -- 1990s rave culture visuals with similar distortion and neon sensibilities
- **90s Cool** -- broader 1990s visual culture context
