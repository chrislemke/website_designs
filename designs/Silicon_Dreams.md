# Silicon Dreams Design Reference

Silicon Dreams, also known as Old CGI or Retro CGI, refers to the surreal and uncanny visuals seen in early CGI animations, art, and video games from the mid-1980s to early 2000s. Characterized by **sparse surrealistic landscapes**, **chrome and reflective surfaces**, **floating geometric shapes**, and **low-resolution textures**, the aesthetic captures the dreamlike quality of primitive 3D rendering -- a world of vast empty horizons, impossible architecture, and smooth synthetic materials that feel simultaneously utopian and deeply alien. The look is heavily associated with Bryce 3D landscape generators, early Pixar shorts, the Mind's Eye video series, and 90s Trapper Keeper art. Silicon Dreams is the visual DNA behind Vaporwave and Seapunk nostalgia.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Surreal, sparse landscapes** -- vast empty terrains with minimal objects, evoking alien planets or dreamscapes; rolling hills, desert plains, and infinite oceans rendered in primitive 3D
- **Reflective water surfaces** -- calm, digitally perfect oceans and lakes with mathematically precise reflections; a signature Bryce 3D element
- **Chrome and metallic spheres** -- highly reflective orbs, tori, and geometric primitives floating in space or sitting on reflective planes
- **Floating geometric shapes** -- spheres, cubes, pyramids, and torus knots suspended in surreal environments with no apparent support
- **Dramatic CG skies** -- banded gradient skies with vivid sunsets, purple-blue atmospheres, and wispy horizontal cloud layers
- **Checkerboard and grid floors** -- reflective checkerboard ground planes extending to the horizon, a hallmark of early ray-tracing demos
- **Glass domes and geodesic structures** -- translucent architectural elements enclosing miniature cities or landscapes on floating islands
- **Neoclassical columns and statues** -- CGI-rendered classical architecture placed incongruously in alien landscapes
- **Low-poly 3D models** -- visible polygon facets, flat or Gouraud shading, and basic texture mapping that reveals the underlying mesh structure
- **Abstract torus knots and interlocking rings** -- mathematically generated sculptural shapes rendered with chrome or glass materials
- **Big planets on the horizon** -- oversized celestial bodies looming in the sky, creating a sci-fi sense of scale
- **Translucent bubbles and glass objects** -- refractive transparent spheres containing other objects or floating through space

### Design Principles

- **Dreamlike surrealism** -- environments feel like half-remembered dreams; familiar objects placed in impossible contexts
- **Vast negative space** -- compositions emphasize emptiness and solitude; single objects in enormous landscapes
- **Perfect synthetic smoothness** -- surfaces are unnaturally smooth, clean, and unblemished, reflecting early CG's inability to render organic imperfection
- **Dramatic lighting** -- strong single-source illumination creating long shadows and vivid specular highlights on reflective surfaces
- **Horizon-line compositions** -- scenes frequently organized around a clear horizon where sky meets water or ground, with the subject centered
- **Uncanny valley of environments** -- spaces that resemble reality but feel fundamentally wrong, too clean, too empty, too perfect
- **Reflections as depth cue** -- water reflections and chrome surface reflections provide depth and visual interest in otherwise minimal scenes
- **Scale distortion** -- objects at impossible scales; tiny buildings under glass domes, enormous spheres on plains
- **Technical limitation as style** -- low polygon counts, basic texture mapping, and simplified lighting are embraced as defining characteristics rather than flaws

---

## Color Palette

The Silicon Dreams palette is defined by two dominant modes: **cool blue-purple atmospheric landscapes** and **warm amber-gold sunset scenes**, both featuring highly reflective chrome and glass materials. Colors are smooth and gradient-heavy, reflecting ray-traced rendering with soft atmospheric haze.

### Primary Palette

| Role | Color | Hex |
|------|-------|-----|
| Deep sky / space | Void black | `#0A0A14` |
| Night sky | Deep indigo | `#1A1040` |
| Atmospheric blue | Bryce blue | `#4466AA` |
| Sky blue | Digital sky | `#6699DD` |
| Bright horizon | Horizon glow | `#AAD4FF` |
| Sunset orange | CGI sunset | `#E88030` |
| Sunset amber | Warm amber | `#D4882C` |
| Sunset magenta | Sky magenta | `#CC4488` |
| Deep purple | Twilight purple | `#5522AA` |
| Crimson glow | Deep crimson | `#AA1133` |

### Chrome and Material Colors

| Role | Color | Hex |
|------|-------|-----|
| Chrome highlight | Peak white | `#F0F0F5` |
| Chrome bright | Silver bright | `#C8C8D0` |
| Chrome mid | Silver mid | `#8888A0` |
| Chrome shadow | Silver dark | `#505068` |
| Gold chrome | Metallic gold | `#C8A832` |
| Bronze chrome | Warm bronze | `#A07830` |
| Glass tint | Ice glass | `#D0E8FF` |
| Glass refraction | Aqua glass | `#80C8E0` |

### Landscape and Water Colors

| Role | Color | Hex |
|------|-------|-----|
| Deep water | Ocean deep | `#182848` |
| Mid water | Ocean mid | `#2848A0` |
| Water surface | Reflective blue | `#4478CC` |
| Water highlight | Foam white | `#B8D8F0` |
| Terrain green | Bryce green | `#6B8830` |
| Terrain sand | Desert tan | `#C0A868` |
| Terrain rock | Stone grey | `#787888` |
| Checkerboard dark | Floor dark | `#2A2A48` |
| Checkerboard light | Floor light | `#6868A8` |

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds -- gradient skies and deep voids */
  --sd-void: #0a0a14;
  --sd-deep-indigo: #1a1040;
  --sd-twilight: #2a1860;
  --sd-night-blue: #182848;
  --sd-surface: #141428;
  --sd-surface-raised: #1e1e3a;

  /* Sky / atmospheric blues */
  --sd-sky-deep: #4466aa;
  --sd-sky-mid: #6699dd;
  --sd-sky-bright: #aad4ff;
  --sd-horizon-glow: #ccddff;

  /* Sunset / warm tones */
  --sd-sunset-orange: #e88030;
  --sd-sunset-amber: #d4882c;
  --sd-sunset-magenta: #cc4488;
  --sd-sunset-red: #aa1133;
  --sd-sunset-gold: #e8b040;

  /* Purple / violet atmospherics */
  --sd-purple-deep: #5522aa;
  --sd-purple-mid: #7744cc;
  --sd-purple-soft: #9966dd;
  --sd-lavender: #b8a0e0;

  /* Chrome / metallic */
  --sd-chrome-peak: #f0f0f5;
  --sd-chrome-bright: #c8c8d0;
  --sd-chrome-mid: #8888a0;
  --sd-chrome-shadow: #505068;
  --sd-gold: #c8a832;
  --sd-bronze: #a07830;

  /* Glass / transparency */
  --sd-glass-tint: #d0e8ff;
  --sd-glass-refract: #80c8e0;
  --sd-glass-overlay: rgba(200, 230, 255, 0.08);

  /* Water */
  --sd-water-deep: #182848;
  --sd-water-mid: #2848a0;
  --sd-water-surface: #4478cc;
  --sd-water-highlight: #b8d8f0;

  /* Checkerboard */
  --sd-check-dark: #2a2a48;
  --sd-check-light: #6868a8;

  /* Functional mappings */
  --sd-bg-primary: var(--sd-void);
  --sd-bg-secondary: var(--sd-deep-indigo);
  --sd-bg-surface: var(--sd-surface);
  --sd-text-primary: var(--sd-chrome-peak);
  --sd-text-secondary: var(--sd-sky-bright);
  --sd-text-muted: var(--sd-chrome-mid);
  --sd-accent-primary: var(--sd-sky-mid);
  --sd-accent-secondary: var(--sd-sunset-amber);
  --sd-border: rgba(100, 150, 220, 0.2);

  /* Glow colors (for box-shadow / text-shadow) */
  --sd-glow-blue: rgba(100, 150, 220, 0.5);
  --sd-glow-purple: rgba(120, 70, 200, 0.5);
  --sd-glow-amber: rgba(230, 140, 50, 0.4);
  --sd-glow-chrome: rgba(200, 200, 220, 0.3);
}
```

### Approaches

- **Gradient-heavy backgrounds** -- skies are never flat; they transition through 3-5 color stops from deep indigo/black at the top through blue to a bright or warm horizon
- **Dual-temperature palette** -- cool blue-purple dominates spatial depth while warm amber-gold provides focal warmth at horizons and light sources
- **Chrome neutrality** -- metallic/reflective elements serve as neutral anchors that pick up surrounding colors through "reflections"
- **Atmospheric perspective** -- distant elements fade toward the horizon color, creating depth through color desaturation
- **Translucency and refraction** -- glass-like materials with subtle tints rather than full transparency
- **Smooth gradient rendering** -- avoid hard color boundaries; everything should feel ray-traced and softly lit

---

## Typography

### Typeface Characteristics

Silicon Dreams typography should evoke the intersection of 90s digital interfaces, early 3D title screens, and new-age spiritualism:

- **Smooth, rounded sans-serifs** -- reflecting the soft, anti-aliased quality of early CG text rendering
- **Geometric sans-serifs** -- clean, mathematical letterforms suited to the technological origins
- **Extended and wide-set display type** -- evoking early 3D movie titles and demo scene intros
- **Metallic/chrome text effects** -- gradient fills simulating reflective metallic surfaces on display type
- **Light body weights** -- thin, airy body text suggesting the ethereal quality of digital spaces
- **Mixed case for body, uppercase for display** -- display headings in caps for geometric regularity, body text in normal case for readability
- **No heavy serifs or handwritten scripts** -- everything should feel digitally generated and smooth

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Rajdhani** | Geometric, semi-condensed | Primary display headlines; its clean geometry evokes 90s tech interfaces |
| **Exo 2** | Geometric, futuristic sans | Section headings, subheadings |
| **Comfortaa** | Rounded geometric | Display text; its rounded terminals echo the smooth surfaces of CG renders |
| **Nunito** | Rounded sans-serif | Alternative display and heading text, warm and approachable |
| **Quicksand** | Rounded geometric | Labels, secondary headings, navigation |
| **Orbitron** | Square geometric, futuristic | Tech-themed display text, data readouts |
| **Jost** | Geometric, Futura-inspired | Clean body text |
| **Inter** | Clean, neutral, modern | Body text, readability |
| **IBM Plex Mono** | Technical monospace | Data displays, code-styled text |
| **Share Tech Mono** | Monospaced, technical | Terminal readouts, coordinates, metadata |

### Typography CSS Example

```css
/* Hero / Display headlines -- smooth, chrome-gradient, wide-tracked */
.sd-display {
  font-family: 'Rajdhani', 'Exo 2', sans-serif;
  font-size: clamp(2.5rem, 7vw, 6rem);
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  line-height: 1.1;
  color: var(--sd-chrome-peak);
  text-shadow:
    0 0 20px var(--sd-glow-blue),
    0 0 60px rgba(100, 150, 220, 0.2);
}

/* Section headlines */
h1, h2, h3 {
  font-family: 'Exo 2', 'Rajdhani', sans-serif;
  font-weight: 500;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--sd-sky-bright);
}

/* Rounded / softer display variant */
.sd-display-soft {
  font-family: 'Comfortaa', 'Nunito', sans-serif;
  font-size: clamp(1.8rem, 5vw, 4rem);
  font-weight: 300;
  letter-spacing: 0.08em;
  color: var(--sd-lavender);
  text-shadow: 0 0 15px var(--sd-glow-purple);
}

/* Technical / label text */
.sd-label {
  font-family: 'Quicksand', 'Rajdhani', sans-serif;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.25em;
  color: var(--sd-sky-mid);
  text-shadow: 0 0 6px var(--sd-glow-blue);
}

/* Monospaced / terminal text */
.sd-mono {
  font-family: 'Share Tech Mono', 'IBM Plex Mono', monospace;
  font-size: 0.85rem;
  letter-spacing: 0.04em;
  color: var(--sd-sky-mid);
  text-shadow: 0 0 4px var(--sd-glow-blue);
}

/* Body text */
body {
  font-family: 'Inter', 'Jost', sans-serif;
  font-weight: 300;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--sd-text-secondary);
}

/* Chrome metallic text effect */
.sd-chrome-text {
  font-family: 'Rajdhani', 'Exo 2', sans-serif;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  background: linear-gradient(
    180deg,
    #f0f0f5 0%,
    #c8c8d0 20%,
    #606080 48%,
    #a0a0b8 52%,
    #d8d8e0 78%,
    #f0f0f5 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 0 8px rgba(150, 150, 200, 0.3));
}
```

---

## Layout Principles

### Grid and Structure

- **Horizon-anchored compositions** -- layouts organized around a horizontal dividing line (sky/ground), with content floating above or below
- **Centered, symmetrical placement** -- key elements centered in the viewport, reflecting the single-subject-in-vast-space composition of early CG renders
- **Generous negative space** -- large empty areas between elements, evoking the sparse emptiness of primitive 3D landscapes
- **Full-bleed gradient backgrounds** -- the entire viewport is a sky gradient; content floats within the atmosphere
- **Layered depth planes** -- background sky, midground atmosphere/haze, foreground content, creating a parallax sense of depth
- **Minimal content density** -- fewer elements per section, each given breathing room and visual prominence
- **Reflective symmetry** -- mirrored elements or reflected content panels, echoing water reflections in CG landscapes

### Section Organization

- Use **soft gradient dividers** between sections -- horizontal bands that transition through sky colors rather than hard lines
- Apply **atmospheric haze** effects -- sections deeper in the page get slightly more translucent or desaturated, as if receding into the distance
- Create **hierarchy through luminosity** -- brighter, more chrome-like elements are more important; muted elements are secondary
- Employ **translucent glass-panel containers** -- content enclosed in frosted-glass or semi-transparent panels with soft borders
- Use **large display type** as section anchors, with generous spacing above and below
- Overlay **subtle checkerboard or grid patterns** at very low opacity (3-8%) behind content areas
- Maintain **horizontal calm** -- compositions should feel still and serene, reflecting the motionless quality of early renders

### Responsive Considerations

- Display text scales fluidly with `clamp()` for geometric impact at all sizes
- Gradient sky backgrounds work at any viewport dimension
- Glass panels can stack vertically on mobile while maintaining translucency effects
- Chrome text effects degrade gracefully (solid color fallback)
- Reduce glow/shadow layers on mobile for performance
- Checkerboard floor perspective effects can simplify to flat tinted backgrounds on small screens

---

## CSS/Design Techniques

### Gradient Sky Background (Signature Effect)

```css
/* The iconic Bryce 3D sky -- deep space transitioning to bright horizon */
.sd-sky-cool {
  background: linear-gradient(
    180deg,
    #0a0a14 0%,
    #1a1040 15%,
    #2a3078 35%,
    #4466aa 55%,
    #6699dd 75%,
    #aad4ff 90%,
    #ccddff 100%
  );
  min-height: 100vh;
}

/* Warm sunset variant */
.sd-sky-sunset {
  background: linear-gradient(
    180deg,
    #0a0a14 0%,
    #1a1040 10%,
    #5522aa 25%,
    #cc4488 45%,
    #e88030 65%,
    #d4882c 80%,
    #e8b040 95%
  );
  min-height: 100vh;
}

/* Purple twilight variant */
.sd-sky-twilight {
  background: linear-gradient(
    180deg,
    #0a0a14 0%,
    #1a1040 20%,
    #2a1860 40%,
    #5522aa 60%,
    #7744cc 75%,
    #9966dd 90%,
    #b8a0e0 100%
  );
  min-height: 100vh;
}
```

### Reflective Water / Horizon Line

```css
/* Water reflection surface below the horizon */
.sd-water {
  position: relative;
  overflow: hidden;
}

.sd-water::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 40%;
  background: linear-gradient(
    180deg,
    rgba(68, 120, 204, 0.3) 0%,
    rgba(40, 72, 160, 0.5) 40%,
    rgba(24, 40, 72, 0.8) 100%
  );
  mask-image: linear-gradient(
    to bottom,
    transparent 0%,
    rgba(0, 0, 0, 0.3) 5%,
    rgba(0, 0, 0, 0.8) 100%
  );
  -webkit-mask-image: linear-gradient(
    to bottom,
    transparent 0%,
    rgba(0, 0, 0, 0.3) 5%,
    rgba(0, 0, 0, 0.8) 100%
  );
  pointer-events: none;
}

/* Horizon glow line */
.sd-horizon {
  width: 100%;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent 5%,
    rgba(170, 212, 255, 0.6) 30%,
    rgba(200, 220, 255, 0.9) 50%,
    rgba(170, 212, 255, 0.6) 70%,
    transparent 95%
  );
  box-shadow:
    0 0 20px rgba(170, 212, 255, 0.4),
    0 0 60px rgba(100, 150, 220, 0.2);
}
```

### Checkerboard Floor

```css
/* Classic ray-tracing demo checkerboard floor with perspective */
.sd-checkerboard {
  position: relative;
  overflow: hidden;
}

.sd-checkerboard::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: -50%;
  right: -50%;
  height: 45%;
  background:
    repeating-conic-gradient(
      var(--sd-check-dark) 0% 25%,
      var(--sd-check-light) 0% 50%
    );
  background-size: 60px 60px;
  transform: perspective(600px) rotateX(70deg);
  transform-origin: bottom center;
  mask-image: linear-gradient(to top, rgba(0, 0, 0, 0.7), transparent 80%);
  -webkit-mask-image: linear-gradient(to top, rgba(0, 0, 0, 0.7), transparent 80%);
  opacity: 0.5;
  pointer-events: none;
}
```

### Glass / Translucent Panel

```css
/* Frosted glass content panel -- the dome/glass material translated to UI */
.sd-glass-panel {
  background: rgba(20, 30, 60, 0.4);
  border: 1px solid rgba(170, 212, 255, 0.15);
  border-radius: 12px;
  padding: 2.5rem;
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.3),
    inset 0 1px 0 rgba(200, 220, 255, 0.1);
}

/* Glass panel hover -- slight brightening */
.sd-glass-panel:hover {
  background: rgba(25, 40, 80, 0.45);
  border-color: rgba(170, 212, 255, 0.25);
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.3),
    0 0 20px rgba(100, 150, 220, 0.08),
    inset 0 1px 0 rgba(200, 220, 255, 0.15);
  transition: all 0.5s ease;
}

/* Stronger glass variant (more visible panel) */
.sd-glass-panel--strong {
  background: rgba(30, 50, 100, 0.35);
  border: 1px solid rgba(170, 212, 255, 0.25);
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.4),
    inset 0 0 40px rgba(100, 150, 220, 0.05),
    inset 0 1px 0 rgba(200, 220, 255, 0.15);
}
```

### Chrome Sphere / Metallic Gradient

```css
/* Decorative chrome sphere element */
.sd-chrome-sphere {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  background: radial-gradient(
    circle at 35% 30%,
    #f0f0f5 0%,
    #c8c8d0 15%,
    #8888a0 35%,
    #505068 55%,
    #2a2a48 75%,
    #181830 100%
  );
  box-shadow:
    0 4px 20px rgba(0, 0, 0, 0.5),
    inset 0 -2px 6px rgba(0, 0, 0, 0.3);
}

/* Chrome surface for decorative elements */
.sd-chrome-surface {
  background: linear-gradient(
    135deg,
    #505068 0%,
    #c8c8d0 20%,
    #f0f0f5 30%,
    #8888a0 50%,
    #c8c8d0 70%,
    #f0f0f5 80%,
    #505068 100%
  );
}

/* Gold chrome variant */
.sd-gold-surface {
  background: linear-gradient(
    135deg,
    #604820 0%,
    #c8a832 25%,
    #e8d060 40%,
    #a07830 55%,
    #c8a832 70%,
    #e8d060 85%,
    #604820 100%
  );
}
```

### Atmospheric Glow Effects

```css
/* Soft atmospheric glow behind key elements */
.sd-atmo-glow {
  position: absolute;
  width: 400px;
  height: 200px;
  border-radius: 50%;
  background: radial-gradient(
    ellipse,
    rgba(100, 150, 220, 0.2) 0%,
    rgba(85, 34, 170, 0.1) 40%,
    transparent 70%
  );
  filter: blur(40px);
  pointer-events: none;
  z-index: 0;
}

/* Sunset/warm glow variant */
.sd-atmo-glow--warm {
  background: radial-gradient(
    ellipse,
    rgba(232, 128, 48, 0.25) 0%,
    rgba(212, 136, 44, 0.1) 35%,
    rgba(204, 68, 136, 0.05) 60%,
    transparent 80%
  );
}

/* Horizon glow -- the bright band at the horizon line */
.sd-horizon-glow {
  position: absolute;
  left: 0;
  right: 0;
  height: 120px;
  background: linear-gradient(
    180deg,
    transparent 0%,
    rgba(170, 212, 255, 0.15) 40%,
    rgba(200, 220, 255, 0.25) 50%,
    rgba(170, 212, 255, 0.15) 60%,
    transparent 100%
  );
  filter: blur(10px);
  pointer-events: none;
}
```

### Floating Element Animation

```css
/* Slow, dreamy floating motion for decorative elements */
@keyframes sd-float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-12px); }
}

.sd-floating {
  animation: sd-float 6s ease-in-out infinite;
}

/* Slower variant for background elements */
.sd-floating--slow {
  animation: sd-float 10s ease-in-out infinite;
}

/* Gentle rotation for spheres/shapes */
@keyframes sd-rotate {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}

.sd-rotating {
  animation: sd-rotate 30s linear infinite;
}
```

### Section Divider

```css
/* Atmospheric gradient divider between sections */
.sd-divider {
  width: 60%;
  margin: 3rem auto;
  border: none;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--sd-sky-mid) 30%,
    var(--sd-sky-bright) 50%,
    var(--sd-sky-mid) 70%,
    transparent
  );
  box-shadow:
    0 0 8px var(--sd-glow-blue),
    0 0 20px rgba(100, 150, 220, 0.15);
}

/* Warm divider variant */
.sd-divider--warm {
  background: linear-gradient(
    90deg,
    transparent,
    var(--sd-sunset-amber) 30%,
    var(--sd-sunset-orange) 50%,
    var(--sd-sunset-amber) 70%,
    transparent
  );
  box-shadow:
    0 0 8px var(--sd-glow-amber),
    0 0 20px rgba(230, 140, 50, 0.15);
}
```

### Dreamy Button

```css
.sd-button {
  display: inline-block;
  padding: 0.75rem 2.5rem;
  border: 1px solid rgba(170, 212, 255, 0.3);
  border-radius: 8px;
  background: rgba(30, 50, 100, 0.3);
  color: var(--sd-sky-bright);
  font-family: 'Exo 2', 'Rajdhani', sans-serif;
  font-size: 0.8rem;
  font-weight: 500;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.4s ease;
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  box-shadow:
    0 4px 15px rgba(0, 0, 0, 0.2),
    0 0 8px rgba(100, 150, 220, 0.1);
}

.sd-button:hover {
  background: rgba(50, 80, 140, 0.4);
  border-color: rgba(170, 212, 255, 0.5);
  box-shadow:
    0 4px 15px rgba(0, 0, 0, 0.2),
    0 0 20px rgba(100, 150, 220, 0.2),
    0 0 40px rgba(100, 150, 220, 0.08);
}

/* Warm/sunset button variant */
.sd-button--warm {
  border-color: rgba(232, 176, 64, 0.3);
  background: rgba(100, 60, 20, 0.3);
  color: var(--sd-sunset-gold);
  box-shadow:
    0 4px 15px rgba(0, 0, 0, 0.2),
    0 0 8px rgba(230, 140, 50, 0.1);
}

.sd-button--warm:hover {
  background: rgba(120, 80, 30, 0.4);
  border-color: rgba(232, 176, 64, 0.5);
  box-shadow:
    0 4px 15px rgba(0, 0, 0, 0.2),
    0 0 20px rgba(230, 140, 50, 0.2);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical Reference | Web Equivalent |
|-------------------|----------------|
| Bryce 3D sky gradient | Multi-stop `linear-gradient` background from deep indigo through blue to bright horizon |
| Reflective water surface | Semi-transparent overlay with soft `linear-gradient` and `mask-image` fade |
| Chrome sphere | `radial-gradient` with sharp highlight placement and dark edges on circular element |
| Checkerboard floor | `repeating-conic-gradient` with `perspective` and `rotateX` transform |
| Glass dome / translucent panel | `backdrop-filter: blur()` with semi-transparent tinted `background` and subtle `border` |
| Low-poly surface | Subtle faceted look via `clip-path` on decorative elements or angular `border-radius` |
| Atmospheric haze | Blurred `radial-gradient` elements with `filter: blur()`, low opacity |
| Sunset horizon glow | Horizontal `linear-gradient` band with warm colors and soft `box-shadow` |
| Gold/bronze metallic | Multi-stop `linear-gradient` with alternating gold tones |
| Floating geometric shape | `border-radius: 50%` elements with chrome `radial-gradient` and `animation: float` |

---

## Imagery and Photography Guidelines

When sourcing or creating imagery for a Silicon Dreams styled site:

- **Embrace surreal CG landscapes** -- Bryce 3D-style renders with vast skies, still water, and sparse terrain
- **Feature chrome and reflective objects** -- metallic spheres, torus knots, and geometric primitives on reflective surfaces
- **Use dramatic gradient skies** -- vivid multi-color sunsets and deep blue-purple twilight atmospheres
- **Include floating or impossible objects** -- elements suspended in space, islands floating over oceans, oversized celestial bodies
- **Show low-poly 3D aesthetic** -- visible polygon facets, basic shading, the "imperfect perfection" of early rendering
- **Feature water reflections** -- still, glassy water surfaces creating perfect mirror reflections of sky and objects
- **Favor emptiness and solitude** -- single subjects in vast, uninhabited environments; avoid crowded compositions
- **Apply a dreamlike, new-age quality** -- scenes should feel meditative, cosmic, and slightly otherworldly
- **Incorporate glass and transparency** -- domes, bubbles, and translucent structures enclosing smaller worlds
- **Avoid photorealism** -- the charm is in the synthetic, obviously-computer-generated quality; embrace smooth surfaces and simplified forms

---

## Related Aesthetics

| Aesthetic | Relationship to Silicon Dreams |
|-----------|-------------------------------|
| **Vaporwave** | 2010s revival aesthetic; recontextualizes Silicon Dreams imagery with ironic/nostalgic undertones, pink-purple shift |
| **Seapunk** | Heavily inspired by Silicon Dreams; shares chrome, water, and CG aesthetics with an aquatic/ocean theme |
| **Y2K Futurism** | Shares the chrome-and-glass material obsession and optimistic technological utopianism |
| **Low Poly** | Focuses on the polygon-count limitations that define Silicon Dreams' 3D models |
| **Laser Grid** | Shares early CG origins and chrome surfaces, but favors wireframe and neon-on-black rather than rendered landscapes |
| **Early Cyber** | Overlapping era; shares raw digital experimentation but focuses on 2D manipulation rather than 3D rendering |
| **Frutiger Aero** | Spiritual successor; represents what happened when CGI matured past Silicon Dreams' primitive charm |
| **Dreamcore** | Shares the surreal, uncanny, dream-like quality of environments |
| **Weirdcore** | Related through surreal and unsettling digital imagery, though more intentionally disturbing |
| **Memphis Design** | Contemporary influence on CG color choices; the playful geometric forms overlap |
| **Synthwave** | Shares retro-tech nostalgia and chrome surfaces, though more neon-focused and music-driven |
| **Metalheart** | Shares the chrome and metallic surface obsession |

---

## Quick-Start: Minimal Silicon Dreams Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Silicon Dreams Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@300;500;600;700&family=Exo+2:wght@300;500&family=Share+Tech+Mono&family=Inter:wght@300;400&display=swap" rel="stylesheet">
  <style>
    :root {
      --sd-void: #0a0a14;
      --sd-deep-indigo: #1a1040;
      --sd-sky-deep: #4466aa;
      --sd-sky-mid: #6699dd;
      --sd-sky-bright: #aad4ff;
      --sd-sunset-amber: #d4882c;
      --sd-chrome-peak: #f0f0f5;
      --sd-chrome-bright: #c8c8d0;
      --sd-chrome-mid: #8888a0;
      --sd-chrome-shadow: #505068;
      --sd-lavender: #b8a0e0;
      --sd-glow-blue: rgba(100, 150, 220, 0.5);
      --sd-check-dark: #2a2a48;
      --sd-check-light: #6868a8;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: linear-gradient(
        180deg,
        #0a0a14 0%,
        #1a1040 15%,
        #2a3078 35%,
        #4466aa 55%,
        #6699dd 75%,
        #aad4ff 92%,
        #ccddff 100%
      );
      color: var(--sd-sky-bright);
      font-family: 'Inter', sans-serif;
      font-weight: 300;
      letter-spacing: 0.02em;
      line-height: 1.7;
      min-height: 100vh;
      overflow-x: hidden;
    }

    /* Hero with dreamy atmosphere */
    .hero {
      text-align: center;
      padding: 12rem 2rem 8rem;
      position: relative;
      min-height: 80vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }

    /* Atmospheric glow behind title */
    .hero::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 500px;
      height: 250px;
      border-radius: 50%;
      background: radial-gradient(
        ellipse,
        rgba(100, 150, 220, 0.2) 0%,
        rgba(85, 34, 170, 0.08) 50%,
        transparent 75%
      );
      filter: blur(40px);
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Rajdhani', sans-serif;
      font-size: clamp(2.5rem, 7vw, 5.5rem);
      font-weight: 600;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      background: linear-gradient(
        180deg,
        #f0f0f5 0%,
        #c8c8d0 25%,
        #8888a0 50%,
        #c8c8d0 75%,
        #f0f0f5 100%
      );
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      filter: drop-shadow(0 0 15px rgba(100, 150, 220, 0.3));
      position: relative;
      z-index: 1;
    }

    .hero .subtitle {
      font-family: 'Exo 2', sans-serif;
      font-size: clamp(0.8rem, 2vw, 1.1rem);
      font-weight: 300;
      letter-spacing: 0.25em;
      text-transform: uppercase;
      color: var(--sd-lavender);
      margin-top: 1.5rem;
      text-shadow: 0 0 12px rgba(184, 160, 224, 0.3);
      position: relative;
      z-index: 1;
    }

    /* Horizon glow line */
    .sd-horizon {
      width: 80%;
      margin: 0 auto;
      height: 2px;
      background: linear-gradient(
        90deg,
        transparent 5%,
        rgba(170, 212, 255, 0.5) 30%,
        rgba(200, 220, 255, 0.8) 50%,
        rgba(170, 212, 255, 0.5) 70%,
        transparent 95%
      );
      box-shadow:
        0 0 15px rgba(170, 212, 255, 0.3),
        0 0 40px rgba(100, 150, 220, 0.15);
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
      position: relative;
      z-index: 1;
    }

    section h2 {
      font-family: 'Exo 2', sans-serif;
      font-size: 1.4rem;
      font-weight: 500;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--sd-sky-bright);
      text-shadow: 0 0 10px var(--sd-glow-blue);
      margin-bottom: 1.5rem;
    }

    .sd-glass-panel {
      background: rgba(20, 30, 60, 0.4);
      border: 1px solid rgba(170, 212, 255, 0.15);
      border-radius: 12px;
      padding: 2.5rem;
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      box-shadow:
        0 8px 32px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(200, 220, 255, 0.1);
    }

    .sd-button {
      display: inline-block;
      margin-top: 2rem;
      padding: 0.75rem 2.5rem;
      border: 1px solid rgba(170, 212, 255, 0.3);
      border-radius: 8px;
      background: rgba(30, 50, 100, 0.3);
      color: var(--sd-sky-bright);
      font-family: 'Exo 2', sans-serif;
      font-size: 0.8rem;
      font-weight: 500;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.4s ease;
      backdrop-filter: blur(8px);
      -webkit-backdrop-filter: blur(8px);
      box-shadow:
        0 4px 15px rgba(0, 0, 0, 0.2),
        0 0 8px rgba(100, 150, 220, 0.1);
    }

    .sd-button:hover {
      background: rgba(50, 80, 140, 0.4);
      border-color: rgba(170, 212, 255, 0.5);
      box-shadow:
        0 4px 15px rgba(0, 0, 0, 0.2),
        0 0 20px rgba(100, 150, 220, 0.2);
    }

    .mono {
      font-family: 'Share Tech Mono', monospace;
      font-size: 0.85rem;
      color: var(--sd-chrome-mid);
      text-shadow: 0 0 4px rgba(100, 150, 220, 0.2);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p class="subtitle">A digital dreamscape rendered in light</p>
  </div>
  <div class="sd-horizon"></div>
  <section>
    <div class="sd-glass-panel">
      <h2>Section Heading</h2>
      <p>Content styled with the Silicon Dreams aesthetic -- surreal CG landscapes, chrome surfaces, glass panels, and the dreamy atmosphere of early 3D rendering.</p>
      <p class="mono" style="margin-top: 1rem;">BRYCE 3D // RENDER COMPLETE // 640x480</p>
      <a href="#" class="sd-button">Explore</a>
    </div>
  </section>
</body>
</html>
```
