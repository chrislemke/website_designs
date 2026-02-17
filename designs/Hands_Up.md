# Hands Up Design Reference

Hands Up is a visual aesthetic rooted in the **late-2000s Eurodance and Hands Up music scenes**, serving as the high-energy, non-anime counterpart to TechnoNeko2000 for the same musical era. It is defined by **neon light trails on dark backgrounds**, **silhouetted dancers in dynamic poses**, **import tuner car culture**, and **blocky chrome typography**. The aesthetic represents the "club side" of the Eurodance visual language -- loud, kinetic, and maximally saturated. It was the unofficial visual style for Eurodance, Hands Up, and early Nightcore YouTube upload thumbnails from roughly 2005 to 2013. The design philosophy is one of **maximum visual impact through high contrast**: vivid neon accents against deep black voids, with every element either glowing, reflecting, or in motion.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Neon light trails and swirls** -- curved, glowing streaks of color tracing movement paths through dark space; the single most defining visual element
- **Silhouetted dancer figures** -- human forms rendered as solid black or deeply desaturated shapes, posed in dynamic mid-action stances (arms raised, jumping, breaking)
- **Import tuner cars** -- heavily customized Japanese sports cars (Nissan Skyline, Subaru Impreza, Acura Integra) with exaggerated body kits, large spoilers, chrome rims, high-gloss paint, and neon underglow lighting
- **Glowing particle clouds** -- bursts of luminous particles emanating from figures or focal points, suggesting explosive energy
- **Shattering glass effects** -- abstract broken/shattered fragments radiating outward from central subjects, conveying impact and intensity
- **Music iconography** -- glowing speakers, turntables, colorful equalizer bars, mixing desks, and audio production elements
- **Energy bursts and flares** -- lens flares, radial light explosions, and concentrated glow effects at action points
- **Glowing rings and wispy light streaks** -- circular neon halos and thin luminous wisps floating in the composition

### Design Principles

- **Dark-dominant with extreme neon saturation** -- near-black backgrounds exist solely to amplify the intensity of neon-colored light elements
- **High-contrast compositions** -- no mid-tones; everything is either deep shadow or vivid luminance
- **Dynamic asymmetry** -- compositions center on figures but surround them with asymmetrical energy distributions (light trails, particles) to create a sensation of explosive motion
- **Dark negative space as atmosphere** -- large areas of black or near-black are not empty; they represent the darkness of a club environment and give glow effects room to breathe
- **Maximalist energy** -- every surface that can glow, does glow; every figure is in motion; every composition feels like a freeze-frame of an explosion
- **Templated reproducibility** -- the style uses clean, abstract digital forms that can be rapidly applied across album covers, YouTube thumbnails, and event flyers
- **Layered depth through light** -- foreground neon elements, mid-ground figures, and background glow create Z-axis depth without traditional perspective

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | Deep black, near-black, void |
| **Surface** | Dark charcoal, dark gray (rare -- most surfaces are pure black) |
| **Accent Primary** | Electric blue, neon cyan |
| **Accent Secondary** | Hot pink, neon magenta |
| **Accent Tertiary** | Vibrant green, electric lime |
| **Accent Quaternary** | Electric orange, neon amber |
| **Metallic** | Chrome silver, glossy white (for typography effects) |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Void Black | `#050508`, `#000000` | Primary backgrounds, the dominant "canvas" |
| Club Dark | `#0A0A10`, `#0D0D14` | Backgrounds with faint blue-shift suggesting club lighting |
| Charcoal | `#1A1A1F`, `#222228` | Rare secondary panels, card surfaces |
| Electric Blue | `#00AAFF`, `#00CCFF` | Primary neon accent, light trails, glow effects |
| Deep Blue | `#0066FF`, `#0055DD` | Secondary blue, underglow tints |
| Hot Pink | `#FF0080`, `#FF1493` | Primary pink accent, neon trails, text glow |
| Neon Magenta | `#FF00FF`, `#CC00FF` | Intense magenta for particle effects and secondary glow |
| Vibrant Green | `#00FF66`, `#00FF44` | Tertiary accent, equalizer bars, underglow |
| Electric Lime | `#88FF00`, `#AAFF00` | Secondary green, highlight flashes |
| Electric Orange | `#FF6600`, `#FF8800` | Quaternary accent, energy bursts |
| Neon Amber | `#FFAA00`, `#FFCC00` | Warm accent, light flares |
| Chrome Silver | `#C0C0C8`, `#D8D8E0` | Metallic text effects, chrome type |
| Gloss White | `#F0F0FF`, `#FFFFFF` | Pure highlights, light source centers, glossy text peaks |
| Blue Glow | `rgba(0, 170, 255, 0.3)` | Ambient blue glow effects |
| Pink Glow | `rgba(255, 0, 128, 0.3)` | Ambient pink glow effects |
| Green Glow | `rgba(0, 255, 102, 0.25)` | Ambient green glow effects |

### Suggested CSS Custom Properties

```css
:root {
  /* Dark base tones */
  --hands-up-void: #050508;
  --hands-up-black: #0a0a10;
  --hands-up-club-dark: #0d0d14;
  --hands-up-charcoal: #1a1a1f;
  --hands-up-dark-gray: #222228;

  /* Neon accent -- blue */
  --hands-up-blue: #00aaff;
  --hands-up-blue-bright: #00ccff;
  --hands-up-blue-deep: #0066ff;

  /* Neon accent -- pink */
  --hands-up-pink: #ff0080;
  --hands-up-pink-hot: #ff1493;
  --hands-up-magenta: #ff00ff;

  /* Neon accent -- green */
  --hands-up-green: #00ff66;
  --hands-up-lime: #88ff00;

  /* Neon accent -- orange/amber */
  --hands-up-orange: #ff6600;
  --hands-up-amber: #ffaa00;

  /* Metallic / chrome */
  --hands-up-chrome: #c0c0c8;
  --hands-up-chrome-light: #d8d8e0;
  --hands-up-white: #f0f0ff;

  /* Glow / transparency */
  --hands-up-glow-blue: rgba(0, 170, 255, 0.3);
  --hands-up-glow-pink: rgba(255, 0, 128, 0.3);
  --hands-up-glow-green: rgba(0, 255, 102, 0.25);
  --hands-up-glow-orange: rgba(255, 102, 0, 0.25);
  --hands-up-glow-magenta: rgba(255, 0, 255, 0.2);

  /* Functional mappings */
  --hands-up-bg-primary: var(--hands-up-void);
  --hands-up-bg-secondary: var(--hands-up-black);
  --hands-up-bg-surface: var(--hands-up-charcoal);
  --hands-up-text-primary: var(--hands-up-white);
  --hands-up-text-secondary: var(--hands-up-chrome);
  --hands-up-accent: var(--hands-up-blue);
  --hands-up-accent-alt: var(--hands-up-pink);
}
```

### Approaches

- **Pure black backgrounds** -- not dark gray, not charcoal, but true near-black to maximize neon contrast
- **Multi-color neon on black** -- unlike Dark Aero's single-accent model, Hands Up uses 3-4 vivid neon colors simultaneously
- **No subtle undertones** -- backgrounds are flat black; all color lives in the neon elements
- **Gradients within neon elements** -- light trails often shift between two neon hues (blue-to-pink, green-to-blue)
- **White-core glow model** -- the center of a glow effect is near-white, radiating outward through the saturated color to transparency

---

## Typography

### Typeface Characteristics

Hands Up typography is aggressive, futuristic, and treated as a visual effect rather than pure text:

- **Blocky, futuristic sans-serif typefaces** -- heavy geometric forms with squared-off terminals
- **Glossy, metallic, or chrome finish** -- text surfaces should appear reflective, as if cast in polished metal
- **Heavy drop shadows** -- deep, often colored shadows that ground the text against the dark background
- **Neon outline treatment** -- text rendered as hollow outlines that glow in neon colors
- **Large display scale** -- text is used at hero/poster scale, not for extended reading
- **Uppercase dominance** -- virtually all display text is set in all-caps for maximum visual punch
- **Digital / reflective surface quality** -- text should suggest technological advancement and synthetic materials

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Orbitron** | Geometric, squared, futuristic display | Hero titles, primary headings -- the closest match to the canonical Hands Up type style |
| **Audiowide** | Wide, techy, single-weight display | Hero titles, event-style headlines |
| **Black Ops One** | Heavy, military-futuristic display | Impact headings, high-energy callouts |
| **Bungee** | Chunky, blocky, display | Bold section titles, poster-style type |
| **Chakra Petch** | Angular, tech-forward, multiple weights | Subheadings, UI elements |
| **Exo 2** | Geometric futuristic, versatile | Headings and body at various weights |
| **Rajdhani** | Technical, semi-condensed | Labels, secondary text, data readouts |
| **Play** | Clean, wide, geometric | Body text at larger sizes |
| **Electrolize** | Monoline, digital readout style | Stats, counters, technical labels |
| **Share Tech** | Technical, monospaced feel | Labels, metadata, small text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Audiowide&family=Chakra+Petch:wght@400;600;700&family=Exo+2:wght@300;400;600;700&family=Rajdhani:wght@400;500;600&family=Electrolize&display=swap');

/* Hero / display text -- chrome effect */
.hands-up-hero-text {
  font-family: 'Orbitron', 'Audiowide', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  font-weight: 900;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  line-height: 1.0;
  color: var(--hands-up-white);
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #e0e0e8 30%,
    #a0a0b0 60%,
    #c0c0d0 80%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 0 20px var(--hands-up-glow-blue))
          drop-shadow(0 4px 8px rgba(0, 0, 0, 0.8));
}

/* Neon outline text variant */
.hands-up-neon-text {
  font-family: 'Orbitron', 'Audiowide', sans-serif;
  font-size: clamp(2rem, 5vw, 5rem);
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: transparent;
  -webkit-text-stroke: 2px var(--hands-up-blue);
  text-shadow:
    0 0 10px var(--hands-up-glow-blue),
    0 0 30px var(--hands-up-glow-blue),
    0 0 60px rgba(0, 170, 255, 0.15);
}

/* Headings */
h1, h2, h3 {
  font-family: 'Chakra Petch', 'Exo 2', sans-serif;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--hands-up-white);
  text-shadow: 0 0 12px var(--hands-up-glow-blue);
}

/* Body text */
body {
  font-family: 'Exo 2', 'Rajdhani', sans-serif;
  font-weight: 300;
  letter-spacing: 0.02em;
  line-height: 1.6;
  color: var(--hands-up-chrome);
}

/* Technical labels */
.hands-up-label {
  font-family: 'Electrolize', 'Rajdhani', monospace;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--hands-up-blue);
  text-shadow: 0 0 6px var(--hands-up-glow-blue);
}
```

---

## Layout Principles

### Grid and Structure

- **Full-bleed dark backgrounds** -- the entire viewport is near-black; there are no light sections
- **Centered focal compositions** -- primary content (figures, titles) occupy the center; neon effects radiate outward
- **Asymmetric energy distribution** -- light trails and particles are not symmetrical; they create directional motion (usually upward and outward)
- **Generous negative space** -- large expanses of black between elements; the darkness is the "stage" for the neon performance
- **Cinematic, poster-like proportions** -- sections feel like individual posters or album covers stacked vertically
- **No traditional grid rigidity** -- elements float, overlap, and bleed; the layout follows energy flow rather than columns

### Section Organization

- Use **neon light dividers** between sections (glowing horizontal lines with fade-out at edges)
- Apply **dark card panels** sparingly -- most content floats directly on the black void
- Create **hierarchy through glow intensity** -- the most important elements glow the brightest
- Use **full-width hero sections** with silhouetted figures as background elements
- Employ **overlapping layers** -- neon trails can cross over UI elements for immersive depth
- Add **equalizer / spectrum visualizer strips** as decorative section dividers
- Use **radial energy compositions** -- content arranged in a burst pattern emanating from a central point

---

## CSS/Design Techniques

### Neon Light Trail Effect

```css
/* SVG-based neon light trail using CSS glow */
.hands-up-light-trail {
  position: absolute;
  pointer-events: none;
}

.hands-up-light-trail path {
  fill: none;
  stroke: var(--hands-up-blue);
  stroke-width: 3;
  stroke-linecap: round;
  filter:
    drop-shadow(0 0 4px var(--hands-up-blue))
    drop-shadow(0 0 12px var(--hands-up-glow-blue))
    drop-shadow(0 0 30px rgba(0, 170, 255, 0.2));
}

/* Animated trail drawing effect */
.hands-up-light-trail path {
  stroke-dasharray: 1000;
  stroke-dashoffset: 1000;
  animation: trail-draw 2s ease-out forwards;
}

@keyframes trail-draw {
  to {
    stroke-dashoffset: 0;
  }
}

/* Multi-color trail variant */
.hands-up-light-trail--pink path {
  stroke: var(--hands-up-pink);
  filter:
    drop-shadow(0 0 4px var(--hands-up-pink))
    drop-shadow(0 0 12px var(--hands-up-glow-pink))
    drop-shadow(0 0 30px rgba(255, 0, 128, 0.2));
}
```

### Neon Glow Text and Elements

```css
/* Multi-layered neon glow for any element */
.hands-up-neon-glow {
  color: var(--hands-up-blue-bright);
  text-shadow:
    0 0 4px var(--hands-up-blue-bright),
    0 0 10px var(--hands-up-blue),
    0 0 20px var(--hands-up-glow-blue),
    0 0 40px rgba(0, 170, 255, 0.15),
    0 0 80px rgba(0, 170, 255, 0.08);
}

/* Neon glow box -- for borders and containers */
.hands-up-neon-box {
  border: 2px solid var(--hands-up-blue);
  box-shadow:
    0 0 6px var(--hands-up-blue),
    0 0 15px var(--hands-up-glow-blue),
    0 0 30px rgba(0, 170, 255, 0.12),
    inset 0 0 10px rgba(0, 170, 255, 0.08);
  border-radius: 4px;
}

/* Pink neon variant */
.hands-up-neon-glow--pink {
  color: var(--hands-up-pink);
  text-shadow:
    0 0 4px var(--hands-up-pink),
    0 0 10px var(--hands-up-pink),
    0 0 20px var(--hands-up-glow-pink),
    0 0 40px rgba(255, 0, 128, 0.15),
    0 0 80px rgba(255, 0, 128, 0.08);
}

/* Animated neon pulse */
@keyframes neon-pulse {
  0%, 100% {
    text-shadow:
      0 0 4px var(--hands-up-blue-bright),
      0 0 10px var(--hands-up-blue),
      0 0 20px var(--hands-up-glow-blue),
      0 0 40px rgba(0, 170, 255, 0.15);
  }
  50% {
    text-shadow:
      0 0 6px var(--hands-up-blue-bright),
      0 0 15px var(--hands-up-blue),
      0 0 30px var(--hands-up-glow-blue),
      0 0 60px rgba(0, 170, 255, 0.25),
      0 0 100px rgba(0, 170, 255, 0.1);
  }
}

.hands-up-neon-pulse {
  animation: neon-pulse 2s ease-in-out infinite;
}
```

### Chrome / Metallic Text Effect

```css
/* Glossy chrome text -- the signature Hands Up typography treatment */
.hands-up-chrome-text {
  font-family: 'Orbitron', sans-serif;
  font-weight: 900;
  text-transform: uppercase;
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #f0f0f4 15%,
    #808090 35%,
    #b0b0c0 50%,
    #606070 65%,
    #a0a0b0 80%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.8))
          drop-shadow(0 0 15px var(--hands-up-glow-blue));
  position: relative;
}

/* Chrome text with colored reflection */
.hands-up-chrome-text--blue {
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #c0d8ff 20%,
    #4080c0 40%,
    #80b0e0 55%,
    #3060a0 70%,
    #90c0ff 85%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

### Particle Explosion Effect

```css
/* CSS-only particle burst using radial gradients */
.hands-up-particles {
  position: absolute;
  width: 100%;
  height: 100%;
  pointer-events: none;
  background:
    radial-gradient(circle 2px at 20% 30%, var(--hands-up-blue-bright) 0%, transparent 100%),
    radial-gradient(circle 1px at 45% 15%, var(--hands-up-pink) 0%, transparent 100%),
    radial-gradient(circle 3px at 70% 25%, var(--hands-up-green) 0%, transparent 100%),
    radial-gradient(circle 1px at 15% 60%, var(--hands-up-blue-bright) 0%, transparent 100%),
    radial-gradient(circle 2px at 80% 50%, var(--hands-up-pink) 0%, transparent 100%),
    radial-gradient(circle 1px at 55% 70%, var(--hands-up-amber) 0%, transparent 100%),
    radial-gradient(circle 2px at 35% 80%, var(--hands-up-blue) 0%, transparent 100%),
    radial-gradient(circle 1px at 90% 75%, var(--hands-up-green) 0%, transparent 100%),
    radial-gradient(circle 2px at 10% 85%, var(--hands-up-magenta) 0%, transparent 100%);
  filter: blur(0.5px);
  opacity: 0.8;
}

/* Animated particle float */
@keyframes particle-drift {
  0% { transform: translateY(0) scale(1); opacity: 0.8; }
  50% { transform: translateY(-15px) scale(1.2); opacity: 1; }
  100% { transform: translateY(-30px) scale(0.8); opacity: 0; }
}

.hands-up-particle {
  position: absolute;
  width: 4px;
  height: 4px;
  border-radius: 50%;
  background: var(--hands-up-blue-bright);
  box-shadow: 0 0 6px var(--hands-up-blue), 0 0 12px var(--hands-up-glow-blue);
  animation: particle-drift 2s ease-out infinite;
}
```

### Shatter / Glass Fragment Effect

```css
/* Shattering glass fragments emanating outward */
.hands-up-shatter {
  position: absolute;
  inset: 0;
  pointer-events: none;
  overflow: hidden;
}

.hands-up-shard {
  position: absolute;
  width: 20px;
  height: 30px;
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.3) 0%,
    rgba(255, 255, 255, 0.05) 50%,
    rgba(0, 170, 255, 0.2) 100%
  );
  clip-path: polygon(10% 0%, 100% 20%, 80% 100%, 0% 70%);
  animation: shard-fly 1.5s ease-out forwards;
  opacity: 0;
}

@keyframes shard-fly {
  0% {
    transform: translate(0, 0) rotate(0deg) scale(0.5);
    opacity: 0.9;
  }
  100% {
    transform: translate(var(--shard-x, 100px), var(--shard-y, -80px)) rotate(var(--shard-rot, 45deg)) scale(0.3);
    opacity: 0;
  }
}

/* Position individual shards with custom properties */
.hands-up-shard:nth-child(1) { --shard-x: 120px; --shard-y: -90px; --shard-rot: 35deg; animation-delay: 0s; }
.hands-up-shard:nth-child(2) { --shard-x: -80px; --shard-y: -120px; --shard-rot: -60deg; animation-delay: 0.05s; }
.hands-up-shard:nth-child(3) { --shard-x: 60px; --shard-y: 80px; --shard-rot: 110deg; animation-delay: 0.1s; }
.hands-up-shard:nth-child(4) { --shard-x: -140px; --shard-y: -40px; --shard-rot: -25deg; animation-delay: 0.08s; }
.hands-up-shard:nth-child(5) { --shard-x: 100px; --shard-y: 60px; --shard-rot: 70deg; animation-delay: 0.12s; }
```

### Equalizer / Spectrum Visualizer

```css
/* Colorful equalizer bar strip -- a signature Hands Up decorative motif */
.hands-up-equalizer {
  display: flex;
  align-items: flex-end;
  justify-content: center;
  gap: 4px;
  height: 80px;
  padding: 0 1rem;
}

.hands-up-eq-bar {
  width: 6px;
  border-radius: 3px 3px 0 0;
  animation: eq-bounce 0.6s ease-in-out infinite alternate;
}

.hands-up-eq-bar--blue {
  background: linear-gradient(0deg, var(--hands-up-blue-deep), var(--hands-up-blue-bright));
  box-shadow: 0 0 8px var(--hands-up-glow-blue);
}

.hands-up-eq-bar--pink {
  background: linear-gradient(0deg, #cc0066, var(--hands-up-pink));
  box-shadow: 0 0 8px var(--hands-up-glow-pink);
}

.hands-up-eq-bar--green {
  background: linear-gradient(0deg, #009944, var(--hands-up-green));
  box-shadow: 0 0 8px var(--hands-up-glow-green);
}

.hands-up-eq-bar--orange {
  background: linear-gradient(0deg, #cc4400, var(--hands-up-orange));
  box-shadow: 0 0 8px var(--hands-up-glow-orange);
}

@keyframes eq-bounce {
  0% { height: 15%; }
  100% { height: 100%; }
}

/* Stagger bars for organic feel */
.hands-up-eq-bar:nth-child(1) { animation-delay: 0s; animation-duration: 0.5s; }
.hands-up-eq-bar:nth-child(2) { animation-delay: 0.08s; animation-duration: 0.65s; }
.hands-up-eq-bar:nth-child(3) { animation-delay: 0.03s; animation-duration: 0.55s; }
.hands-up-eq-bar:nth-child(4) { animation-delay: 0.12s; animation-duration: 0.7s; }
.hands-up-eq-bar:nth-child(5) { animation-delay: 0.05s; animation-duration: 0.45s; }
.hands-up-eq-bar:nth-child(6) { animation-delay: 0.15s; animation-duration: 0.6s; }
.hands-up-eq-bar:nth-child(7) { animation-delay: 0.02s; animation-duration: 0.75s; }
.hands-up-eq-bar:nth-child(8) { animation-delay: 0.1s; animation-duration: 0.5s; }
```

### Silhouette Figure with Energy Aura

```css
/* Dark silhouette figure with neon energy radiating outward */
.hands-up-silhouette {
  position: relative;
  display: inline-block;
}

/* The figure itself -- darkened/silhouetted via filter */
.hands-up-silhouette img {
  filter: brightness(0) saturate(0);
  position: relative;
  z-index: 2;
}

/* Multi-color energy aura behind the silhouette */
.hands-up-silhouette::before {
  content: '';
  position: absolute;
  top: -20%;
  left: -30%;
  right: -30%;
  bottom: -10%;
  background:
    radial-gradient(ellipse 50% 60% at 50% 50%, var(--hands-up-glow-blue) 0%, transparent 60%),
    radial-gradient(ellipse 40% 50% at 30% 40%, var(--hands-up-glow-pink) 0%, transparent 50%),
    radial-gradient(ellipse 35% 45% at 70% 55%, var(--hands-up-glow-green) 0%, transparent 50%);
  filter: blur(20px);
  z-index: 1;
  animation: aura-pulse 3s ease-in-out infinite;
}

@keyframes aura-pulse {
  0%, 100% { opacity: 0.7; transform: scale(1); }
  50% { opacity: 1; transform: scale(1.08); }
}
```

### Neon Underglow (for car imagery or bottom-lit elements)

```css
/* Neon underglow effect -- mimics import tuner car lighting */
.hands-up-underglow {
  position: relative;
}

.hands-up-underglow::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 5%;
  right: 5%;
  height: 20px;
  background: var(--hands-up-blue);
  filter: blur(15px);
  opacity: 0.6;
  border-radius: 50%;
  z-index: -1;
}

/* Pink underglow variant */
.hands-up-underglow--pink::after {
  background: var(--hands-up-pink);
}

/* Green underglow variant */
.hands-up-underglow--green::after {
  background: var(--hands-up-green);
}

/* Animated color-shifting underglow */
@keyframes underglow-shift {
  0%, 100% { background: var(--hands-up-blue); }
  33% { background: var(--hands-up-pink); }
  66% { background: var(--hands-up-green); }
}

.hands-up-underglow--animated::after {
  animation: underglow-shift 4s ease-in-out infinite;
}
```

### Neon Divider Line

```css
/* Glowing neon section divider */
.hands-up-divider {
  border: none;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    var(--hands-up-blue) 15%,
    var(--hands-up-pink) 50%,
    var(--hands-up-blue) 85%,
    transparent 100%
  );
  box-shadow:
    0 0 8px var(--hands-up-glow-blue),
    0 0 20px var(--hands-up-glow-pink);
  margin: 3rem 0;
}

/* Single-color variant */
.hands-up-divider--blue {
  background: linear-gradient(
    90deg,
    transparent,
    var(--hands-up-blue) 20%,
    var(--hands-up-blue) 80%,
    transparent
  );
  box-shadow: 0 0 12px var(--hands-up-glow-blue);
}
```

### Hands Up Card / Panel

```css
/* Dark card with neon border accent */
.hands-up-card {
  background: rgba(10, 10, 16, 0.9);
  border: 1px solid rgba(0, 170, 255, 0.2);
  border-radius: 8px;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 0 15px rgba(0, 170, 255, 0.08),
    0 8px 24px rgba(0, 0, 0, 0.6);
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

.hands-up-card:hover {
  border-color: rgba(0, 170, 255, 0.5);
  box-shadow:
    0 0 20px rgba(0, 170, 255, 0.15),
    0 0 40px rgba(0, 170, 255, 0.06),
    0 8px 24px rgba(0, 0, 0, 0.6);
}

/* Top-edge neon accent line */
.hands-up-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: linear-gradient(
    90deg,
    var(--hands-up-blue),
    var(--hands-up-pink),
    var(--hands-up-blue)
  );
  box-shadow: 0 0 10px var(--hands-up-glow-blue);
}
```

### Hands Up Button

```css
/* High-energy neon button */
.hands-up-button {
  display: inline-block;
  padding: 0.8rem 2.5rem;
  border-radius: 6px;
  border: 2px solid var(--hands-up-blue);
  background: transparent;
  color: var(--hands-up-blue-bright);
  font-family: 'Orbitron', 'Chakra Petch', sans-serif;
  font-size: 0.85rem;
  font-weight: 700;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 0 10px var(--hands-up-glow-blue),
    inset 0 0 10px rgba(0, 170, 255, 0.05);
  transition: all 0.3s ease;
}

.hands-up-button:hover {
  background: rgba(0, 170, 255, 0.15);
  border-color: var(--hands-up-blue-bright);
  color: var(--hands-up-white);
  box-shadow:
    0 0 20px var(--hands-up-glow-blue),
    0 0 40px rgba(0, 170, 255, 0.15),
    inset 0 0 20px rgba(0, 170, 255, 0.1);
  text-shadow: 0 0 8px var(--hands-up-glow-blue);
}

/* Sweep animation on hover */
.hands-up-button::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(0, 170, 255, 0.2),
    transparent
  );
  transition: left 0.5s ease;
}

.hands-up-button:hover::before {
  left: 100%;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical/visual Hands Up materials and their web equivalents:

| Visual Element | Web Equivalent |
|----------------|----------------|
| Neon light tubes/trails | SVG paths with bright stroke color + multi-layer `filter: drop-shadow()` glow; animated with `stroke-dashoffset` |
| Chrome/metallic text | `linear-gradient` on text with `background-clip: text` + light/dark bands simulating reflection |
| Silhouetted dancer | Image with `filter: brightness(0)` + positioned `radial-gradient` glow behind |
| Particle cloud/explosion | Scattered small `radial-gradient` dots or animated `border-radius: 50%` elements with glow |
| Shattering glass | `clip-path: polygon()` fragments animated outward with `transform` |
| Equalizer bars | Flex-row of narrow `div`s with gradient fills, staggered bounce `animation` |
| Neon underglow | `::after` pseudo-element with bright color, heavy `filter: blur()`, positioned below subject |
| Glowing speaker | Circular element with concentric `box-shadow` rings in neon colors |
| Club darkness | `background: #050508` -- pure, deep, flat black with no texture |
| Light flare/burst | `radial-gradient` with white-to-neon-to-transparent, placed at focal points |
| Import tuner car paint | High-gloss solid color surface with `linear-gradient` highlight band suggesting reflection |

---

## Cultural Context and Visual References

The Hands Up aesthetic draws from and is informed by:

- **Clubland compilation album covers** -- the canonical visual format; silhouetted dancers, neon trails, chrome text on black
- **Ekwador nightclub branding** -- the Polish club whose visual identity became synonymous with the style
- **YouTube unofficial music visualizers (2005-2013)** -- fan-made thumbnails and video backgrounds for Eurodance/Hands Up uploads
- **Import tuner car culture** -- Need for Speed Underground, The Fast and the Furious (2001), midnight car meets with underglow
- **Early-2000s club flyer design** -- event promotion posters with photoshopped neon effects
- **DJ Manga / Cascada / Basshunter era** -- album art and single covers from peak Hands Up artists
- **Breaking/B-boy culture** -- dancer silhouette poses drawn from hip-hop dance freezes and power moves

---

## Related Aesthetics

| Aesthetic | Relationship to Hands Up |
|-----------|--------------------------|
| **TechnoNeko2000** | Sibling aesthetic; the anime-side counterpart to Hands Up for the same Eurodance musical era |
| **Y2K Futurism** | Broader umbrella; Hands Up is a late expression of Y2K tech-optimist visual culture |
| **Frutiger Aero** | Contemporary parallel; shares glossy, digitally-rendered qualities but diverges in color palette and subject matter |
| **Dark Aero** | Shares the dark-background-with-neon-accents principle, but Dark Aero is more restrained and UI-focused |
| **Vectordelia** | Shares flowing curves and abstract digital forms; Vectordelia is more organic, Hands Up more kinetic |
| **Rave** | Parent culture; Hands Up inherits rave's neon-on-black visual language and club environment |
| **Brostep** | Contemporary; shares aggressive neon-on-dark energy and maximalist approach, with heavier/darker tone |
| **Tecktonik** | Closely related; the French electro-dance scene with nearly identical neon-silhouette visual language |
| **Vectorheart** | Related; shares the glossy digital aesthetic with more romantic/emotive direction |
| **Nightcore** | Overlapping; early Nightcore YouTube uploads frequently used Hands Up visual templates |

---

## Quick-Start: Minimal Hands Up Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hands Up Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Chakra+Petch:wght@400;600;700&family=Exo+2:wght@300;400;600&family=Electrolize&display=swap" rel="stylesheet">
  <style>
    :root {
      --hands-up-void: #050508;
      --hands-up-black: #0a0a10;
      --hands-up-charcoal: #1a1a1f;
      --hands-up-blue: #00aaff;
      --hands-up-blue-bright: #00ccff;
      --hands-up-pink: #ff0080;
      --hands-up-green: #00ff66;
      --hands-up-chrome: #c0c0c8;
      --hands-up-white: #f0f0ff;
      --hands-up-glow-blue: rgba(0, 170, 255, 0.3);
      --hands-up-glow-pink: rgba(255, 0, 128, 0.3);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--hands-up-void);
      color: var(--hands-up-chrome);
      font-family: 'Exo 2', sans-serif;
      font-weight: 300;
      letter-spacing: 0.02em;
      line-height: 1.6;
      min-height: 100vh;
      overflow-x: hidden;
    }

    h1, h2, h3 {
      font-family: 'Chakra Petch', sans-serif;
      font-weight: 700;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      color: var(--hands-up-white);
    }

    /* Hero with neon energy */
    .hero {
      text-align: center;
      padding: 10rem 2rem 8rem;
      position: relative;
      overflow: hidden;
    }

    /* Multi-color glow background */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse 40% 50% at 30% 50%, rgba(0, 170, 255, 0.15) 0%, transparent 60%),
        radial-gradient(ellipse 35% 45% at 70% 45%, rgba(255, 0, 128, 0.1) 0%, transparent 55%),
        radial-gradient(ellipse 30% 40% at 50% 70%, rgba(0, 255, 102, 0.06) 0%, transparent 50%);
      pointer-events: none;
      animation: glow-shift 6s ease-in-out infinite;
    }

    @keyframes glow-shift {
      0%, 100% { opacity: 0.7; transform: scale(1); }
      50% { opacity: 1; transform: scale(1.05); }
    }

    /* Chrome hero text */
    .hero h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: clamp(3rem, 8vw, 6rem);
      font-weight: 900;
      letter-spacing: 0.08em;
      background: linear-gradient(
        180deg,
        #ffffff 0%,
        #e0e0e8 30%,
        #808090 55%,
        #c0c0d0 75%,
        #ffffff 100%
      );
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      filter: drop-shadow(0 0 20px var(--hands-up-glow-blue))
              drop-shadow(0 4px 8px rgba(0, 0, 0, 0.9));
      position: relative;
      z-index: 1;
    }

    .hero p {
      margin-top: 1.5rem;
      font-size: 1.15rem;
      color: var(--hands-up-chrome);
      text-shadow: 0 0 8px var(--hands-up-glow-blue);
      position: relative;
      z-index: 1;
    }

    /* Neon divider */
    .neon-divider {
      width: 50%;
      margin: 2.5rem auto;
      border: none;
      height: 2px;
      background: linear-gradient(
        90deg,
        transparent,
        var(--hands-up-blue) 15%,
        var(--hands-up-pink) 50%,
        var(--hands-up-blue) 85%,
        transparent
      );
      box-shadow:
        0 0 8px var(--hands-up-glow-blue),
        0 0 20px var(--hands-up-glow-pink);
      position: relative;
      z-index: 1;
    }

    /* Equalizer decoration */
    .equalizer {
      display: flex;
      align-items: flex-end;
      justify-content: center;
      gap: 4px;
      height: 50px;
      margin: 2rem auto;
      position: relative;
      z-index: 1;
    }

    .eq-bar {
      width: 5px;
      border-radius: 3px 3px 0 0;
      animation: eq-bounce 0.6s ease-in-out infinite alternate;
    }

    .eq-bar.blue {
      background: linear-gradient(0deg, #0055dd, var(--hands-up-blue-bright));
      box-shadow: 0 0 6px var(--hands-up-glow-blue);
    }

    .eq-bar.pink {
      background: linear-gradient(0deg, #cc0066, var(--hands-up-pink));
      box-shadow: 0 0 6px var(--hands-up-glow-pink);
    }

    .eq-bar.green {
      background: linear-gradient(0deg, #009944, var(--hands-up-green));
      box-shadow: 0 0 6px rgba(0, 255, 102, 0.3);
    }

    @keyframes eq-bounce {
      0% { height: 15%; }
      100% { height: 100%; }
    }

    .eq-bar:nth-child(1) { animation-delay: 0s; animation-duration: 0.5s; }
    .eq-bar:nth-child(2) { animation-delay: 0.08s; animation-duration: 0.65s; }
    .eq-bar:nth-child(3) { animation-delay: 0.03s; animation-duration: 0.55s; }
    .eq-bar:nth-child(4) { animation-delay: 0.12s; animation-duration: 0.7s; }
    .eq-bar:nth-child(5) { animation-delay: 0.05s; animation-duration: 0.45s; }
    .eq-bar:nth-child(6) { animation-delay: 0.15s; animation-duration: 0.6s; }
    .eq-bar:nth-child(7) { animation-delay: 0.02s; animation-duration: 0.75s; }
    .eq-bar:nth-child(8) { animation-delay: 0.1s; animation-duration: 0.5s; }
    .eq-bar:nth-child(9) { animation-delay: 0.07s; animation-duration: 0.55s; }
    .eq-bar:nth-child(10) { animation-delay: 0.13s; animation-duration: 0.65s; }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
    }

    /* Neon-bordered card */
    .neon-card {
      background: rgba(10, 10, 16, 0.9);
      border: 1px solid rgba(0, 170, 255, 0.2);
      border-radius: 8px;
      padding: 2.5rem;
      position: relative;
      overflow: hidden;
      box-shadow:
        0 0 15px rgba(0, 170, 255, 0.08),
        0 8px 24px rgba(0, 0, 0, 0.6);
      transition: border-color 0.3s ease, box-shadow 0.3s ease;
    }

    .neon-card:hover {
      border-color: rgba(0, 170, 255, 0.5);
      box-shadow:
        0 0 20px rgba(0, 170, 255, 0.15),
        0 8px 24px rgba(0, 0, 0, 0.6);
    }

    /* Top neon accent line on card */
    .neon-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 2px;
      background: linear-gradient(
        90deg,
        var(--hands-up-blue),
        var(--hands-up-pink),
        var(--hands-up-blue)
      );
      box-shadow: 0 0 10px var(--hands-up-glow-blue);
    }

    .neon-card h2 {
      text-shadow: 0 0 12px var(--hands-up-glow-blue);
    }

    .neon-card p {
      margin-top: 1rem;
    }

    /* Neon button */
    .neon-button {
      display: inline-block;
      margin-top: 2rem;
      padding: 0.8rem 2.5rem;
      border-radius: 6px;
      border: 2px solid var(--hands-up-blue);
      background: transparent;
      color: var(--hands-up-blue-bright);
      font-family: 'Orbitron', sans-serif;
      font-size: 0.8rem;
      font-weight: 700;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 0 0 10px var(--hands-up-glow-blue);
      transition: all 0.3s ease;
    }

    .neon-button:hover {
      background: rgba(0, 170, 255, 0.15);
      color: var(--hands-up-white);
      box-shadow:
        0 0 20px var(--hands-up-glow-blue),
        0 0 40px rgba(0, 170, 255, 0.15);
      text-shadow: 0 0 8px var(--hands-up-glow-blue);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <hr class="neon-divider">
    <p>Subtitle with Hands Up neon energy</p>
    <div class="equalizer">
      <div class="eq-bar blue"></div>
      <div class="eq-bar pink"></div>
      <div class="eq-bar green"></div>
      <div class="eq-bar blue"></div>
      <div class="eq-bar pink"></div>
      <div class="eq-bar green"></div>
      <div class="eq-bar blue"></div>
      <div class="eq-bar pink"></div>
      <div class="eq-bar green"></div>
      <div class="eq-bar blue"></div>
    </div>
  </div>

  <section>
    <div class="neon-card">
      <h2>Section Heading</h2>
      <p>Content rendered on a dark panel with neon accent borders and chrome-styled headings.</p>
      <a href="#" class="neon-button">Take Action</a>
    </div>
  </section>
</body>
</html>
```
