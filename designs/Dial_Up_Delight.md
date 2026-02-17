# Dial-Up Delight -- Design Reference

Dial-Up Delight is a web design aesthetic that channels the chaotic, unregulated energy of the late 1990s and early 2000s internet -- GeoCities homepages, AIM profiles, early Myspace pages, and the anarchic visual experiments of a web where everyone was a designer and no one followed rules. But rather than pure nostalgia, this trend remixes that raw digital chaos through a Gen Z lens, fusing **gothic grit with Y2K sparkle**, dial-up modem screech with TikTok polish. The result is a maximalist collision of gothic blackletter fonts, candy-colored gradients, chrome text effects, glitch animations, animated GIF energy, pixel graphics, and visual noise -- all layered on top of each other in deliberate, beautiful disorder. It treats the early web not as an embarrassment to be cleaned up, but as a lost golden age of personal expression to be celebrated and amplified. The aesthetic embraces the handmade, the excessive, the "under construction" -- reclaiming the spirit of a time when the internet felt like a frontier and every homepage was a fever dream.

---

## Visual Characteristics

- **Gothic meets candy** -- blackletter typography and dark grunge textures collide with hot pink gradients and sparkle overlays, creating a tension between dark and saccharine
- **Chrome and metallic text** -- text rendered with reflective silver/chrome gradient fills, evoking early 2000s WordArt and 3D text generators
- **Candy-colored neon gradients** -- backgrounds and panels use vivid pink-to-purple-to-cyan gradients reminiscent of Y2K graphic design
- **Glitch and distortion effects** -- text and images stutter, shift, and fragment through CSS clip-path animations, RGB channel splitting, and scan-line artifacts
- **Layered visual chaos** -- elements stack and overlap with negative margins, rotated frames, and collage-style compositions
- **Star and sparkle decorations** -- small animated or static star/sparkle icons scattered across the page, referencing GeoCities "under construction" aesthetics
- **Pixelated graphics** -- low-resolution pixel art, aliased edges, and chunky bitmap icons used as decorative elements
- **Animated GIF energy** -- even static designs should feel kinetic, as if everything is vibrating, blinking, or spinning
- **Custom cursors** -- novelty cursor icons (stars, crosshairs, trailing sparkles) replacing the default pointer
- **Stacked and overlapping images** -- photos and graphics pile on top of each other at slight angles, taped-to-the-wall collage style
- **Noise and grain textures** -- SVG noise filters and grainy overlays adding grit and analog texture to digital surfaces
- **Chunky 3D text** -- exaggerated text-stroke and layered text-shadows creating bold, dimensional letterforms
- **Bright visuals over gritty textures** -- neon colors and shiny metallics layered atop dark, scratched, or distressed backgrounds
- **Scrolling marquee energy** -- horizontal scrolling text banners and tickers, referencing the `<marquee>` tag era
- **Excessive border decorations** -- dashed, dotted, double, and rainbow borders used liberally and without restraint

---

## Color Palette

The Dial-Up Delight palette is defined by high contrast and maximum saturation -- neon brights punching through dark, gritty backgrounds:

- **Deep dark bases** -- near-black purples and charcoals providing the gothic foundation
- **Hot pink as primary accent** -- the signature color, used for text, borders, gradients, and highlights
- **Electric cyan for contrast** -- cool neon blue-green balancing the warm pinks and purples
- **Chrome silver gradients** -- metallic linear gradients from light silver to medium gray, simulating brushed metal
- **Acid green for shock value** -- fluorescent green used sparingly for maximum visual disruption
- **Neon gradient transitions** -- smooth flows from hot pink through deep purple to electric cyan
- **Deep purple for depth** -- rich, dark violet providing dimensional backgrounds and shadows
- **White used for high-contrast text** -- pure white on dark backgrounds for maximum readability
- **Rainbow sequences** -- full spectrum gradients used for borders, underlines, and decorative strips

### Suggested Implementation Palette

Based on characteristic Dial-Up Delight color selections:

| Role                | Color              | Hex       |
|---------------------|--------------------|-----------|
| Background Dark     | Void Purple        | `#0D0015` |
| Background Mid      | Deep Plum          | `#1A0A2E` |
| Surface             | Gothic Purple      | `#2A0134` |
| Surface Light       | Bruised Violet     | `#3D1A54` |
| Primary Text        | Bright White       | `#F0F0FF` |
| Secondary Text      | Lavender Haze      | `#C8A8E8` |
| Accent Hot Pink     | Hot Pink           | `#FF1493` |
| Accent Cyan         | Electric Cyan      | `#00F5FF` |
| Accent Green        | Acid Green         | `#39FF14` |
| Accent Yellow       | Neon Yellow        | `#FFFF00` |
| Chrome Light        | Silver High        | `#E8E8F0` |
| Chrome Mid          | Chrome Silver      | `#C0C0C0` |
| Chrome Dark         | Steel Gray         | `#808080` |
| Gradient Start      | Magenta            | `#FF00FF` |
| Gradient Mid        | Purple Haze        | `#8B00FF` |
| Gradient End        | Cyan Burst         | `#00F5FF` |

### Neon Gradient Combinations

For signature Dial-Up Delight gradient effects:

| Gradient Effect        | Start     | Mid       | End       |
|------------------------|-----------|-----------|-----------|
| Neon sunset            | `#FF1493` | `#8B00FF` | `#00F5FF` |
| Acid trip              | `#39FF14` | `#FFFF00` | `#FF1493` |
| Chrome reflection      | `#E8E8F0` | `#C0C0C0` | `#808080` |
| Gothic flame           | `#FF1493` | `#2A0134` | `#0D0015` |
| Cybervoid              | `#00F5FF` | `#0D0015` | `#39FF14` |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --dialup-bg-dark: #0D0015;
  --dialup-bg-mid: #1A0A2E;
  --dialup-bg-surface: #2A0134;
  --dialup-bg-surface-light: #3D1A54;

  /* Text */
  --dialup-text-primary: #F0F0FF;
  --dialup-text-secondary: #C8A8E8;
  --dialup-text-muted: #8868A8;

  /* Neon Accents */
  --dialup-accent-pink: #FF1493;
  --dialup-accent-cyan: #00F5FF;
  --dialup-accent-green: #39FF14;
  --dialup-accent-yellow: #FFFF00;
  --dialup-accent-magenta: #FF00FF;
  --dialup-accent-purple: #8B00FF;

  /* Chrome / Metallic */
  --dialup-chrome-light: #E8E8F0;
  --dialup-chrome-mid: #C0C0C0;
  --dialup-chrome-dark: #808080;
  --dialup-chrome-gradient: linear-gradient(
    180deg,
    #E8E8F0 0%, #C0C0C0 40%, #808080 60%, #C0C0C0 80%, #E8E8F0 100%
  );

  /* Neon Gradients */
  --dialup-gradient-neon: linear-gradient(
    135deg,
    #FF1493 0%, #8B00FF 50%, #00F5FF 100%
  );
  --dialup-gradient-acid: linear-gradient(
    135deg,
    #39FF14 0%, #FFFF00 50%, #FF1493 100%
  );
  --dialup-gradient-gothic: linear-gradient(
    180deg,
    #FF1493 0%, #2A0134 60%, #0D0015 100%
  );

  /* Shadows and Glow */
  --dialup-shadow: #0D0015;
  --dialup-shadow-soft: rgba(13, 0, 21, 0.7);
  --dialup-glow-pink: 0 0 20px rgba(255, 20, 147, 0.6);
  --dialup-glow-cyan: 0 0 20px rgba(0, 245, 255, 0.6);
  --dialup-glow-green: 0 0 20px rgba(57, 255, 20, 0.6);

  /* Functional mappings */
  --dialup-bg-primary: var(--dialup-bg-dark);
  --dialup-bg-secondary: var(--dialup-bg-mid);
  --dialup-bg-card: var(--dialup-bg-surface);
  --dialup-text-heading: var(--dialup-accent-pink);
  --dialup-text-body: var(--dialup-text-primary);
  --dialup-accent-primary: var(--dialup-accent-pink);
  --dialup-accent-secondary: var(--dialup-accent-cyan);
  --dialup-border: var(--dialup-accent-pink);
}
```

---

## Typography

### Typeface Characteristics

Dial-Up Delight typography is intentionally eclectic, mixing fonts that should never coexist -- gothic blackletter next to pixel bitmap next to chunky display type:

- **Gothic/blackletter headings** -- ornate medieval-style letterforms used for primary headings, creating the "gothic grit" half of the aesthetic
- **Chrome and metallic text fills** -- gradient background-clip techniques making text appear as polished metal or liquid chrome
- **Pixel fonts for UI elements** -- bitmap-style monospace fonts referencing early computer interfaces and chat windows
- **Bold Y2K display fonts** -- chunky, exaggerated letterforms with built-in personality for callouts and labels
- **Exaggerated text-stroke** -- thick outlines around text in contrasting neon colors, creating a sticker/graffiti effect
- **Mixed font sizes within compositions** -- intentional scale contrast with tiny pixel text next to massive display headings
- **Text rotation and skew** -- headings and labels at slight angles, fighting against grid alignment
- **All-caps and mixed-case** used interchangeably for chaotic energy
- **Layered text shadows** -- multiple shadow layers creating depth, glow, or 3D extrusion effects

### Recommended Web Fonts

| Font | Style | Usage |
|------|-------|-------|
| **UnifrakturMaguntia** | Gothic blackletter | Primary headings, dramatic titles -- the "gothic grit" signature |
| **MedievalSharp** | Semi-gothic serif | Secondary headings, subheadings -- readable gothic flavor |
| **Press Start 2P** | Pixel bitmap | UI labels, status text, retro data displays |
| **VT323** | Monospace terminal | Code-style text, timestamps, technical labels |
| **Bungee** | Chunky display | Callout text, bold statements, Y2K display energy |
| **Monoton** | Neon outline display | Hero text, decorative titles with glow effects |
| **Permanent Marker** | Handwritten bold | Annotation-style labels, casual emphasis |
| **Creepster** | Horror display | Accent text, spooky-fun labels for gothic contrast |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&family=MedievalSharp&family=Press+Start+2P&family=VT323&family=Bungee&family=Monoton&family=Permanent+Marker&family=Creepster&display=swap');

/* Primary body text -- clean but with character */
body {
  font-family: 'VT323', 'Courier New', monospace;
  font-size: 18px;
  line-height: 1.7;
  letter-spacing: 0.03em;
  color: var(--dialup-text-primary);
}

/* Gothic headings -- the defining typographic element */
h1, h2, h3 {
  font-family: 'UnifrakturMaguntia', 'MedievalSharp', cursive;
  color: var(--dialup-accent-pink);
  text-shadow:
    0 0 10px rgba(255, 20, 147, 0.5),
    0 0 40px rgba(255, 20, 147, 0.2),
    3px 3px 0px var(--dialup-shadow);
  letter-spacing: 0.04em;
  line-height: 1.3;
}

h1 {
  font-size: clamp(2.5rem, 6vw, 5rem);
  -webkit-text-stroke: 1px rgba(255, 0, 255, 0.3);
}

h2 {
  font-size: clamp(1.5rem, 3.5vw, 2.8rem);
  color: var(--dialup-accent-cyan);
  text-shadow:
    0 0 10px rgba(0, 245, 255, 0.5),
    0 0 40px rgba(0, 245, 255, 0.2),
    2px 2px 0px var(--dialup-shadow);
}

h3 {
  font-family: 'Bungee', 'Impact', sans-serif;
  font-size: clamp(1rem, 2vw, 1.6rem);
  color: var(--dialup-accent-green);
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

/* Chrome/metallic text effect */
.dialup-chrome-text {
  font-family: 'UnifrakturMaguntia', cursive;
  background: linear-gradient(
    180deg,
    #E8E8F0 0%, #C0C0C0 25%, #808080 50%, #C0C0C0 75%, #E8E8F0 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(2px 2px 0px #0D0015);
}

/* Pixel font for UI labels */
.dialup-label {
  font-family: 'Press Start 2P', monospace;
  font-size: 0.65rem;
  color: var(--dialup-accent-cyan);
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

/* Y2K display font for callouts */
.dialup-callout {
  font-family: 'Bungee', sans-serif;
  font-size: 1.2rem;
  color: var(--dialup-accent-yellow);
  -webkit-text-stroke: 1px var(--dialup-accent-pink);
  letter-spacing: 0.05em;
}

/* Neon outline text */
.dialup-neon {
  font-family: 'Monoton', cursive;
  font-size: clamp(2rem, 5vw, 4rem);
  color: var(--dialup-accent-pink);
  text-shadow:
    0 0 7px var(--dialup-accent-pink),
    0 0 10px var(--dialup-accent-pink),
    0 0 21px var(--dialup-accent-pink),
    0 0 42px var(--dialup-accent-magenta),
    0 0 82px var(--dialup-accent-magenta),
    0 0 92px var(--dialup-accent-magenta);
}

/* Monospace data display */
.dialup-mono {
  font-family: 'VT323', monospace;
  font-size: 1rem;
  color: var(--dialup-accent-green);
  text-shadow: 0 0 6px rgba(57, 255, 20, 0.4);
}
```

---

## Key Design Elements and Motifs

### Chrome and Metallic Effects

The defining surface treatment of Dial-Up Delight -- everything that can be chrome, should be chrome:

- **Chrome text gradients** -- linear gradients from white through silver to gray, applied via `background-clip: text`
- **Metallic button bevels** -- raised, shiny button surfaces mimicking early web 3D buttons and WordArt
- **Reflective surface simulation** -- gradient overlays suggesting light bouncing off polished metal
- **Chrome borders** -- metallic gradient borders using `border-image` with silver-to-gray transitions
- **Liquid chrome blobs** -- organic, amoeba-shaped elements with metallic fills referencing Y2K graphic design

### Stars, Sparkles, and Decorative Scatter

The whimsical, handmade layer of Dial-Up Delight:

- **Animated star bursts** -- small 4-point or 6-point stars that scale and fade in CSS animations
- **Sparkle trails** -- elements that leave a trail of small glowing dots, referencing cursor trail scripts
- **Scattered decorative icons** -- tiny pixel hearts, stars, moons, and gems placed randomly across sections
- **Twinkling animations** -- opacity and scale keyframes creating a gentle glittering effect
- **"Under construction" energy** -- spinning warning signs, dancing baby energy, animated dividers

### Glitch and Distortion

The digital breakdown layer that adds grit and movement:

- **RGB channel splitting** -- text or images rendered with offset red, green, and blue copies
- **Clip-path glitch animations** -- rectangular slices of content shifting horizontally at random intervals
- **Scan-line artifacts** -- horizontal line distortion overlays suggesting corrupted video signal
- **Static noise overlay** -- SVG turbulence filters creating TV-static texture
- **Jittery movement** -- subtle random `translate` animations making elements feel unstable

### Layered Collage Composition

The organizational principle (or deliberate lack thereof):

- **Overlapping frames** -- image and content containers stacked with slight rotations and negative margins
- **Mixed media feel** -- combining pixel art, gradient panels, chrome text, and grungy textures in a single view
- **Tape and sticker metaphors** -- decorative elements that look "stuck on" at angles
- **Z-index chaos** -- intentional overlapping where elements compete for visual attention
- **Scrapbook energy** -- the page should feel assembled by hand, not generated by a grid system

### Gothic Grit Elements

The dark, moody counterweight to the neon brightness:

- **Blackletter typography** -- ornate gothic fonts for headings and display text
- **Dark textured backgrounds** -- deep purple and black with grain, scratch, or noise overlays
- **Occult/mystic decorative motifs** -- pentagrams, moons, stars in gothic arrangements (decorative, not literal)
- **Distressed and worn textures** -- backgrounds that feel scratched, aged, or corrupted
- **High contrast pairing** -- dark gothic elements directly adjacent to bright neon candy colors

---

## Layout Principles

- **Controlled chaos** -- the layout should feel chaotic but remain navigable; the disorder is intentional and curated
- **Overlapping elements are expected** -- containers, images, and text blocks should intersect and layer, not sit in clean grid cells
- **Negative margins as a compositional tool** -- pull elements into each other's space to create density and collision
- **Mixed alignment** -- left-aligned, centered, and right-aligned elements within the same section, plus occasional rotation
- **Scroll-heavy single-column base** -- underneath the chaos, the fundamental structure is a long scrolling page (like a GeoCities homepage)
- **Full-width gradient sections** -- wide color bands and gradient backgrounds breaking up the vertical scroll
- **Asymmetric compositions** -- avoid perfect symmetry; one side should be heavier or more chaotic than the other
- **Dense visual filling** -- empty space should be filled with decorative elements (stars, sparkles, dividers, pixel art)
- **Sticky and fixed elements** -- floating decorative panels, persistent cursor effects, and fixed-position sparkle elements
- **Section dividers as decorative opportunities** -- horizontal rules become rainbow gradients, animated marquees, or pixelated divider graphics

### Modern Web Adaptation

- Use **CSS Grid and Flexbox** for the underlying structure, then apply transforms, negative margins, and absolute positioning for the chaotic overlapping layer
- **Custom cursor via CSS** `cursor: url()` for novelty pointer icons (star, crosshair, sparkle)
- **Scroll-triggered animations** via `IntersectionObserver` or CSS `animation-timeline` for elements that glitch into view
- **CSS `mix-blend-mode`** on overlapping layers for color interaction effects
- **Container queries** for responsive chaos -- maintain the overlapping energy at smaller viewports
- **Clamp and fluid typography** to keep gothic headings dramatic at all screen sizes
- **Performance budget** -- despite the visual excess, limit actual DOM complexity; use CSS for decorative effects rather than excessive HTML elements

---

## CSS/Design Techniques

### Glitch Animation

```css
/* Core glitch effect using clip-path slicing */
@keyframes dialup-glitch {
  0% {
    clip-path: inset(40% 0 61% 0);
    transform: translate(-2px, 0);
  }
  10% {
    clip-path: inset(92% 0 1% 0);
    transform: translate(2px, 0);
  }
  20% {
    clip-path: inset(43% 0 1% 0);
    transform: translate(0, 0);
  }
  30% {
    clip-path: inset(25% 0 58% 0);
    transform: translate(3px, 0);
  }
  40% {
    clip-path: inset(54% 0 7% 0);
    transform: translate(-3px, 0);
  }
  50% {
    clip-path: inset(58% 0 43% 0);
    transform: translate(0, 0);
  }
  60% {
    clip-path: inset(2% 0 89% 0);
    transform: translate(4px, 0);
  }
  70% {
    clip-path: inset(76% 0 12% 0);
    transform: translate(-1px, 0);
  }
  80% {
    clip-path: inset(15% 0 65% 0);
    transform: translate(1px, 0);
  }
  90% {
    clip-path: inset(67% 0 8% 0);
    transform: translate(-2px, 0);
  }
  100% {
    clip-path: inset(10% 0 80% 0);
    transform: translate(0, 0);
  }
}

/* Glitching text element */
.dialup-glitch {
  position: relative;
  display: inline-block;
}

.dialup-glitch::before,
.dialup-glitch::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

/* Red channel offset */
.dialup-glitch::before {
  color: var(--dialup-accent-pink);
  animation: dialup-glitch 3s infinite linear alternate-reverse;
  mix-blend-mode: screen;
  z-index: -1;
}

/* Cyan channel offset */
.dialup-glitch::after {
  color: var(--dialup-accent-cyan);
  animation: dialup-glitch 2s infinite linear alternate;
  mix-blend-mode: screen;
  z-index: -2;
}
```

### Chrome / Metallic Gradient Effects

```css
/* Chrome text fill -- the signature Dial-Up Delight text treatment */
.dialup-chrome {
  background: linear-gradient(
    180deg,
    #FFFFFF 0%,
    #E8E8F0 10%,
    #A0A0B0 30%,
    #E8E8F0 45%,
    #808080 55%,
    #C0C0C0 70%,
    #FFFFFF 85%,
    #A0A0B0 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(3px 3px 0px rgba(13, 0, 21, 0.8));
}

/* Animated chrome shimmer */
@keyframes dialup-chrome-shimmer {
  0% { background-position: 0% 0%; }
  100% { background-position: 0% 200%; }
}

.dialup-chrome--animated {
  background-size: 100% 200%;
  animation: dialup-chrome-shimmer 3s ease-in-out infinite;
}

/* Chrome border using border-image */
.dialup-chrome-border {
  border: 3px solid;
  border-image: linear-gradient(
    180deg,
    #E8E8F0, #808080, #C0C0C0, #E8E8F0
  ) 1;
}

/* Chrome button with bevel effect */
.dialup-chrome-button {
  background: linear-gradient(
    180deg,
    #E8E8F0 0%, #C0C0C0 45%, #808080 55%, #A0A0A0 100%
  );
  border: 2px outset #C0C0C0;
  color: var(--dialup-bg-dark);
  font-family: 'Bungee', sans-serif;
  font-weight: bold;
  padding: 0.6rem 2rem;
  text-shadow: 1px 1px 0px rgba(255, 255, 255, 0.5);
  cursor: pointer;
  box-shadow:
    inset 1px 1px 0px rgba(255, 255, 255, 0.6),
    inset -1px -1px 0px rgba(0, 0, 0, 0.3),
    3px 3px 6px rgba(0, 0, 0, 0.5);
}

.dialup-chrome-button:active {
  border-style: inset;
  box-shadow:
    inset 2px 2px 4px rgba(0, 0, 0, 0.4),
    1px 1px 2px rgba(0, 0, 0, 0.3);
  transform: translate(1px, 1px);
}
```

### Star and Sparkle Animations

```css
/* Twinkling star animation */
@keyframes dialup-twinkle {
  0%, 100% {
    opacity: 0;
    transform: scale(0) rotate(0deg);
  }
  50% {
    opacity: 1;
    transform: scale(1) rotate(180deg);
  }
}

/* Star shape using clip-path */
.dialup-star {
  position: absolute;
  width: 12px;
  height: 12px;
  background: var(--dialup-accent-yellow);
  clip-path: polygon(
    50% 0%, 61% 35%, 98% 35%, 68% 57%,
    79% 91%, 50% 70%, 21% 91%, 32% 57%,
    2% 35%, 39% 35%
  );
  animation: dialup-twinkle 2s ease-in-out infinite;
  pointer-events: none;
}

/* Stagger sparkle timing for scattered effect */
.dialup-star:nth-child(2n)   { animation-delay: 0.3s; animation-duration: 2.5s; }
.dialup-star:nth-child(3n)   { animation-delay: 0.7s; animation-duration: 1.8s; }
.dialup-star:nth-child(4n)   { animation-delay: 1.1s; animation-duration: 3s; }
.dialup-star:nth-child(5n)   { animation-delay: 0.5s; animation-duration: 2.2s; }
.dialup-star:nth-child(6n)   { animation-delay: 1.5s; animation-duration: 1.6s; }

/* Sparkle burst on hover */
@keyframes dialup-sparkle-burst {
  0% {
    box-shadow:
      0 0 0 0 rgba(255, 20, 147, 0.6),
      0 0 0 0 rgba(0, 245, 255, 0.6);
  }
  50% {
    box-shadow:
      0 0 20px 10px rgba(255, 20, 147, 0.3),
      0 0 40px 20px rgba(0, 245, 255, 0.15);
  }
  100% {
    box-shadow:
      0 0 0 0 rgba(255, 20, 147, 0),
      0 0 0 0 rgba(0, 245, 255, 0);
  }
}

.dialup-sparkle-hover:hover {
  animation: dialup-sparkle-burst 0.6s ease-out;
}

/* Floating sparkle container */
.dialup-sparkle-field {
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 9998;
  overflow: hidden;
}
```

### Noise Texture Overlay (SVG Filter)

```css
/* SVG noise filter -- creates analog grain/static texture */
.dialup-noise {
  position: relative;
}

.dialup-noise::after {
  content: '';
  position: absolute;
  inset: 0;
  opacity: 0.06;
  pointer-events: none;
  z-index: 50;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
  background-repeat: repeat;
  background-size: 256px 256px;
}

/* Animated static noise -- subtle jitter */
@keyframes dialup-static {
  0%  { transform: translate(0, 0); }
  10% { transform: translate(-1px, 1px); }
  20% { transform: translate(1px, -1px); }
  30% { transform: translate(-1px, 0); }
  40% { transform: translate(0, 1px); }
  50% { transform: translate(1px, 0); }
  60% { transform: translate(0, -1px); }
  70% { transform: translate(-1px, 1px); }
  80% { transform: translate(1px, -1px); }
  90% { transform: translate(0, 1px); }
  100% { transform: translate(0, 0); }
}

.dialup-noise--animated::after {
  animation: dialup-static 0.5s steps(10) infinite;
}
```

### Neon Gradient Backgrounds

```css
/* Full-page neon gradient -- the signature Dial-Up Delight backdrop */
.dialup-gradient-bg {
  background: linear-gradient(
    135deg,
    var(--dialup-bg-dark) 0%,
    var(--dialup-bg-mid) 20%,
    #2A0134 40%,
    #1A0A3E 60%,
    var(--dialup-bg-mid) 80%,
    var(--dialup-bg-dark) 100%
  );
}

/* Neon accent gradient strip */
.dialup-gradient-strip {
  height: 4px;
  background: var(--dialup-gradient-neon);
  box-shadow:
    0 0 10px rgba(255, 20, 147, 0.5),
    0 0 30px rgba(139, 0, 255, 0.3);
}

/* Animated gradient border using pseudo-element */
@keyframes dialup-gradient-rotate {
  0%   { background-position: 0% 50%; }
  50%  { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.dialup-rainbow-border {
  position: relative;
  padding: 3px;
  background: linear-gradient(
    90deg,
    #FF1493, #FF00FF, #8B00FF, #00F5FF, #39FF14, #FFFF00, #FF1493
  );
  background-size: 300% 100%;
  animation: dialup-gradient-rotate 4s ease infinite;
}

.dialup-rainbow-border > * {
  background: var(--dialup-bg-dark);
}

/* Radial glow accent -- placed behind key elements */
.dialup-glow-accent {
  position: absolute;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  background: radial-gradient(
    circle,
    rgba(255, 20, 147, 0.2) 0%,
    rgba(139, 0, 255, 0.1) 40%,
    transparent 70%
  );
  pointer-events: none;
  filter: blur(40px);
  z-index: 0;
}
```

### Overlapping Collage Layout

```css
/* Collage container -- allows overlapping children */
.dialup-collage {
  position: relative;
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 0;
  padding: 2rem 0;
}

/* Collage items overlap and rotate */
.dialup-collage-item {
  position: relative;
  z-index: 1;
  transition: transform 0.3s ease, z-index 0s;
}

.dialup-collage-item:nth-child(1) {
  grid-column: 1 / 7;
  grid-row: 1;
  transform: rotate(-3deg);
  margin-right: -2rem;
}

.dialup-collage-item:nth-child(2) {
  grid-column: 5 / 11;
  grid-row: 1;
  transform: rotate(2deg);
  margin-top: 3rem;
  margin-left: -2rem;
  z-index: 2;
}

.dialup-collage-item:nth-child(3) {
  grid-column: 3 / 9;
  grid-row: 1;
  transform: rotate(-1deg);
  margin-top: 6rem;
  z-index: 3;
}

.dialup-collage-item:hover {
  z-index: 10;
  transform: rotate(0deg) scale(1.05);
}

/* Polaroid-style frame for collage images */
.dialup-polaroid {
  background: white;
  padding: 8px 8px 30px 8px;
  box-shadow: 4px 4px 12px rgba(0, 0, 0, 0.5);
}

.dialup-polaroid img {
  width: 100%;
  display: block;
  image-rendering: pixelated;
}
```

### Custom Cursor and Interaction Effects

```css
/* Custom cursor -- star shape */
.dialup-cursor-star {
  cursor: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath fill='%23FF1493' d='M12 0l3 9h9l-7.5 5.5L19.5 24 12 18l-7.5 6 3-9.5L0 9h9z'/%3E%3C/svg%3E") 12 12, auto;
}

/* Crosshair cursor for interactive elements */
.dialup-cursor-crosshair {
  cursor: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24'%3E%3Cline x1='12' y1='0' x2='12' y2='24' stroke='%2300F5FF' stroke-width='2'/%3E%3Cline x1='0' y1='12' x2='24' y2='12' stroke='%2300F5FF' stroke-width='2'/%3E%3Ccircle cx='12' cy='12' r='4' fill='none' stroke='%2300F5FF' stroke-width='1'/%3E%3C/svg%3E") 12 12, crosshair;
}

/* Hover glow effect for interactive elements */
.dialup-interact {
  transition: all 0.2s ease;
}

.dialup-interact:hover {
  filter: brightness(1.2) drop-shadow(0 0 8px rgba(255, 20, 147, 0.6));
  transform: scale(1.02);
}
```

### Marquee / Scrolling Text

```css
/* CSS-only marquee effect -- replacing the deprecated <marquee> tag */
@keyframes dialup-marquee {
  0%   { transform: translateX(100%); }
  100% { transform: translateX(-100%); }
}

.dialup-marquee {
  overflow: hidden;
  white-space: nowrap;
  background: var(--dialup-bg-dark);
  border-top: 2px solid var(--dialup-accent-pink);
  border-bottom: 2px solid var(--dialup-accent-cyan);
  padding: 0.5rem 0;
}

.dialup-marquee span {
  display: inline-block;
  animation: dialup-marquee 15s linear infinite;
  font-family: 'Press Start 2P', monospace;
  font-size: 0.7rem;
  color: var(--dialup-accent-yellow);
  text-shadow: 0 0 6px rgba(255, 255, 0, 0.4);
}

/* Stacked marquee banners going opposite directions */
.dialup-marquee--reverse span {
  animation-direction: reverse;
  color: var(--dialup-accent-green);
  text-shadow: 0 0 6px rgba(57, 255, 20, 0.4);
}
```

### Card / Content Panel

```css
/* Dial-Up Delight styled content card */
.dialup-card {
  background: var(--dialup-bg-surface);
  border: 2px solid var(--dialup-accent-pink);
  padding: 2rem;
  position: relative;
  box-shadow:
    0 0 15px rgba(255, 20, 147, 0.15),
    inset 0 0 30px rgba(13, 0, 21, 0.5),
    5px 5px 0px var(--dialup-shadow);
  overflow: hidden;
}

/* Neon border glow on hover */
.dialup-card:hover {
  border-color: var(--dialup-accent-cyan);
  box-shadow:
    0 0 20px rgba(0, 245, 255, 0.3),
    0 0 40px rgba(0, 245, 255, 0.1),
    inset 0 0 30px rgba(13, 0, 21, 0.5),
    5px 5px 0px var(--dialup-shadow);
  transition: all 0.3s ease;
}

/* Diagonal stripe corner accent */
.dialup-card::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 60px;
  height: 60px;
  background: repeating-linear-gradient(
    45deg,
    var(--dialup-accent-pink) 0px,
    var(--dialup-accent-pink) 3px,
    transparent 3px,
    transparent 6px
  );
  clip-path: polygon(100% 0, 0 0, 100% 100%);
  opacity: 0.6;
}

/* Card with rainbow animated border */
.dialup-card--rainbow {
  border: none;
  padding: 0;
  background: linear-gradient(
    90deg,
    #FF1493, #FF00FF, #8B00FF, #00F5FF, #39FF14, #FFFF00, #FF1493
  );
  background-size: 300% 100%;
  animation: dialup-gradient-rotate 4s ease infinite;
}

.dialup-card--rainbow > .dialup-card-inner {
  background: var(--dialup-bg-surface);
  margin: 3px;
  padding: 2rem;
}
```

### Button

```css
/* Dial-Up Delight styled button */
.dialup-button {
  display: inline-block;
  padding: 0.7rem 2rem;
  background: var(--dialup-bg-surface);
  border: 2px solid var(--dialup-accent-pink);
  color: var(--dialup-accent-pink);
  font-family: 'Press Start 2P', monospace;
  font-size: 0.65rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  text-decoration: none;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: all 0.2s ease;
  box-shadow:
    0 0 10px rgba(255, 20, 147, 0.2),
    3px 3px 0px var(--dialup-shadow);
}

.dialup-button:hover {
  background: var(--dialup-accent-pink);
  color: var(--dialup-bg-dark);
  box-shadow:
    0 0 20px rgba(255, 20, 147, 0.5),
    0 0 40px rgba(255, 20, 147, 0.2),
    3px 3px 0px var(--dialup-shadow);
  transform: translate(-1px, -1px);
}

.dialup-button:active {
  transform: translate(2px, 2px);
  box-shadow:
    0 0 5px rgba(255, 20, 147, 0.3),
    1px 1px 0px var(--dialup-shadow);
}

/* Scan-line sweep on hover */
.dialup-button::after {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.15),
    transparent
  );
  transition: left 0.4s ease;
}

.dialup-button:hover::after {
  left: 100%;
}

/* Chrome bevel button variant */
.dialup-button--chrome {
  background: linear-gradient(
    180deg,
    #E8E8F0 0%, #C0C0C0 45%, #808080 55%, #A0A0A0 100%
  );
  border: 2px outset #C0C0C0;
  color: var(--dialup-bg-dark);
  font-family: 'Bungee', sans-serif;
  font-size: 0.8rem;
  text-shadow: 1px 1px 0px rgba(255, 255, 255, 0.4);
  box-shadow:
    inset 1px 1px 0px rgba(255, 255, 255, 0.5),
    inset -1px -1px 0px rgba(0, 0, 0, 0.3),
    3px 3px 6px rgba(0, 0, 0, 0.4);
}

.dialup-button--chrome:hover {
  background: linear-gradient(
    180deg,
    #FFFFFF 0%, #D0D0D0 45%, #909090 55%, #B0B0B0 100%
  );
  color: var(--dialup-bg-dark);
}

.dialup-button--chrome:active {
  border-style: inset;
  box-shadow:
    inset 2px 2px 4px rgba(0, 0, 0, 0.4);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical / Cultural Reference | Web Equivalent |
|-------------------------------|----------------|
| Brushed chrome and polished metal surfaces | CSS linear gradients (white-silver-gray-silver-white) applied via `background-clip: text` or as element backgrounds |
| GeoCities tiled backgrounds | `background-repeat: repeat` with small tileable pattern images or SVG patterns |
| CRT monitor scanlines and static | `repeating-linear-gradient` overlays (2px transparent/dark bands) and SVG `feTurbulence` noise filters |
| Sticker-covered laptop lids and skateboard decks | Overlapping absolutely-positioned elements with rotation transforms and `box-shadow` for "stuck on" depth |
| Dial-up modem noise / corrupted data | CSS `clip-path` glitch animations with horizontal slice distortion and RGB channel offset |
| Animated GIF cursor trails | CSS `@keyframes` scale/opacity animations on scattered star/sparkle pseudo-elements |
| WordArt 3D text from Microsoft Word | Layered `text-shadow` stacks (5+ layers) creating depth, combined with `text-stroke` and gradient text fills |
| Hot Topic store signage and merchandise | High contrast neon-on-black color schemes with gothic blackletter fonts and bright accent borders |
| AIM buddy profile / Myspace page customization | Dense, maximalist layouts with mixed fonts, embedded media, rainbow gradients, and blinking text |
| Pixelated low-resolution web graphics | `image-rendering: pixelated` on small images scaled up, pixel-font text, aliased edges |
| Holographic and iridescent stickers | Multi-stop gradient backgrounds with `background-size` animation creating a shifting shimmer effect |
| Grunge photocopied flyers | `filter: contrast(1.5) grayscale(0.3)` on images plus noise overlay for distressed texture |

---

## Imagery and Visual Content Guidelines

When creating or sourcing imagery for a Dial-Up Delight styled site:

- **Embrace low resolution** -- scale small images up with `image-rendering: pixelated` for intentional chunkiness; avoid crisp high-res photography
- **Collage and layer images** -- stack photos at angles with borders, tape marks, and overlapping frames rather than single hero images
- **Apply glitch effects to photos** -- RGB channel splitting, horizontal line corruption, and scan-line overlays on imagery
- **Mix pixel art with photography** -- combine hand-drawn pixel graphics alongside processed photographs
- **Use neon color overlays** -- apply `mix-blend-mode: screen` or `multiply` with hot pink, cyan, and purple overlays on images
- **Animated GIF energy** -- even static images should feel kinetic; use subtle CSS transforms and opacity animations
- **Gothic and occult iconography** -- moons, stars, pentagrams, roses, thorns used decoratively alongside bright neon elements
- **Y2K graphic design references** -- chrome 3D renders, blob shapes, translucent orbs, and metallic textures from early 2000s design
- **GeoCities-era web graphics** -- "under construction" signs, spinning icons, blinking dividers, counter badges
- **Dark, moody base tones** -- imagery should lean dark with bright accents rather than bright with dark accents
- **Avoid clean, corporate stock photography** -- everything should feel personal, handmade, chaotic, and expressive
- **Custom cursors and interaction hints** -- use decorative cursor states and hover effects to make interaction feel playful
- **Star and sparkle scatter** -- layer small twinkling stars and sparkle graphics over and around images

---

## Related Aesthetics

| Aesthetic | Relationship to Dial-Up Delight |
|-----------|--------------------------------|
| **[Y2K Futurism](Y2K_Futurism.md)** | Shares the chrome textures, metallic gradients, and early 2000s techno-optimism; Dial-Up Delight is Y2K Futurism's messy, gothic, Gen Z-remixed cousin |
| **[FantasY2K](FantasY2K.md)** | Overlapping medieval-meets-Y2K fusion; FantasY2K focuses on medieval fantasy imagery while Dial-Up Delight focuses on early web culture, but both share gothic fonts and chrome |
| **[Cyberpunk](Cyberpunk.md)** | Shares neon-on-dark palettes and glitch aesthetics, but Cyberpunk is dystopian-serious while Dial-Up Delight is nostalgic-playful |
| **[Dark Mode Neon](Dark_Mode_Neon.md)** | Similar color approach (bright neons on dark backgrounds), but Dark Mode Neon is cleaner and more minimal; Dial-Up Delight adds chaos and texture |
| **[Early Cyber](Early_Cyber.md)** | Shares roots in early internet culture and digital aesthetics, but Early Cyber is more austere and techy; Dial-Up Delight is more colorful and emotional |
| **[Gen Z Maximalism](Gen_Z_Maximalism.md)** | Same generational impulse toward visual excess and rule-breaking; Dial-Up Delight channels that energy specifically through '90s/'00s internet nostalgia |
| **[Acid Design](Acid_Design.md)** | Shares distorted typography, neon colors, and anti-design principles; Acid Design is more contemporary-experimental while Dial-Up Delight is retro-nostalgic |
| **[Chromecore](Chromecore.md)** | Shares the metallic/chrome surface obsession; Chromecore is purely about reflective metal while Dial-Up Delight mixes chrome with gothic, pixel, and neon elements |
| **[Dopamine Design](Dopamine_Design.md)** | Both seek maximum visual stimulation through bright colors and dense compositions; Dial-Up Delight adds the specific early-web and gothic layers |
| **[Glitch Art / Corporate Grunge](Corporate_Grunge.md)** | Shares distortion and digital decay motifs; Corporate Grunge applies these to corporate/clean contexts while Dial-Up Delight applies them to retro-web chaos |

---

## Implementation Notes

- The Dial-Up Delight aesthetic is **chaotic but intentional** -- every overlapping element, misaligned frame, and clashing font should be a deliberate design choice, not an accident. The chaos is curated. A page that is truly broken is not Dial-Up Delight; a page that looks beautifully broken is.
- **Performance matters despite the visual excess** -- glitch animations, noise filters, and sparkle elements can be GPU-intensive. Use `will-change` sparingly, prefer `transform` and `opacity` for animations, and set reasonable `animation-iteration-count` values rather than infinite loops on heavy effects.
- **The gothic-neon tension is essential** -- without the blackletter fonts and dark grungy textures, the result is just generic neon design. Without the bright neons and sparkles, it is just gothic. The magic is in the collision of the two.
- **Chrome text is the signature visual** -- a single gothic heading rendered in chrome gradient is enough to establish the aesthetic. Prioritize this technique if implementing only one element.
- **Accessibility requires extra care** -- the chaotic overlapping and low-contrast decorative elements can harm readability. Ensure body text maintains WCAG AA contrast (at minimum) against its actual background, and provide sufficient font sizes for pixel fonts (they become illegible below 12px).
- **Custom cursors degrade gracefully** -- always include a fallback cursor keyword after the `url()` value (`cursor: url(...) 12 12, auto`). Some browsers restrict custom cursor sizes.
- **Noise and grain overlays must be subtle** -- SVG turbulence filters at high opacity will obscure content. Keep noise overlay opacity between 0.03 and 0.08 for texture without obstruction.
- **Test marquee and glitch animations for motion sensitivity** -- wrap continuous animations in a `@media (prefers-reduced-motion: no-preference)` check, and provide a static fallback.
- **The GeoCities spirit is about personal expression** -- when in doubt, add another sparkle, another layer, another clashing font. Restraint is the opposite of this aesthetic. But make sure the underlying content remains accessible and navigable beneath the visual spectacle.

---

## Quick-Start: Minimal Dial-Up Delight Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dial-Up Delight Page</title>
  <link href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&family=MedievalSharp&family=Press+Start+2P&family=VT323&family=Bungee&family=Monoton&display=swap" rel="stylesheet">
  <style>
    :root {
      --dialup-bg-dark: #0D0015;
      --dialup-bg-mid: #1A0A2E;
      --dialup-bg-surface: #2A0134;
      --dialup-bg-surface-light: #3D1A54;
      --dialup-text-primary: #F0F0FF;
      --dialup-text-secondary: #C8A8E8;
      --dialup-accent-pink: #FF1493;
      --dialup-accent-cyan: #00F5FF;
      --dialup-accent-green: #39FF14;
      --dialup-accent-yellow: #FFFF00;
      --dialup-accent-magenta: #FF00FF;
      --dialup-accent-purple: #8B00FF;
      --dialup-chrome-light: #E8E8F0;
      --dialup-chrome-mid: #C0C0C0;
      --dialup-chrome-dark: #808080;
      --dialup-shadow: #0D0015;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--dialup-bg-dark);
      color: var(--dialup-text-primary);
      font-family: 'VT323', 'Courier New', monospace;
      font-size: 18px;
      line-height: 1.7;
      min-height: 100vh;
      overflow-x: hidden;
      cursor: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' viewBox='0 0 20 20'%3E%3Cpath fill='%23FF1493' d='M10 0l2.5 7.5h7.5l-6 4.5 2.5 8L10 15l-6.5 5 2.5-8-6-4.5h7.5z'/%3E%3C/svg%3E") 10 10, auto;
    }

    /* Noise texture overlay */
    body::after {
      content: '';
      position: fixed;
      inset: 0;
      opacity: 0.05;
      pointer-events: none;
      z-index: 9999;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
      background-repeat: repeat;
      background-size: 256px 256px;
    }

    /* Neon gradient background glow */
    .dialup-page {
      max-width: 1000px;
      margin: 0 auto;
      padding: 2rem;
      position: relative;
    }

    .dialup-page::before {
      content: '';
      position: fixed;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(
        ellipse at 30% 20%,
        rgba(255, 20, 147, 0.08) 0%,
        transparent 50%
      ),
      radial-gradient(
        ellipse at 70% 80%,
        rgba(0, 245, 255, 0.06) 0%,
        transparent 50%
      ),
      radial-gradient(
        ellipse at 50% 50%,
        rgba(139, 0, 255, 0.04) 0%,
        transparent 60%
      );
      pointer-events: none;
      z-index: 0;
    }

    .dialup-page > * {
      position: relative;
      z-index: 1;
    }

    /* Scrolling marquee banner */
    .dialup-marquee {
      overflow: hidden;
      white-space: nowrap;
      border-top: 2px solid var(--dialup-accent-pink);
      border-bottom: 2px solid var(--dialup-accent-cyan);
      padding: 0.4rem 0;
      margin-bottom: 2rem;
      background: rgba(13, 0, 21, 0.8);
    }

    @keyframes marquee-scroll {
      0%   { transform: translateX(100%); }
      100% { transform: translateX(-100%); }
    }

    .dialup-marquee span {
      display: inline-block;
      animation: marquee-scroll 18s linear infinite;
      font-family: 'Press Start 2P', monospace;
      font-size: 0.6rem;
      color: var(--dialup-accent-yellow);
      text-shadow: 0 0 8px rgba(255, 255, 0, 0.5);
      letter-spacing: 0.05em;
    }

    /* Chrome gothic heading */
    .dialup-hero {
      text-align: center;
      margin: 3rem 0;
      position: relative;
    }

    .dialup-hero h1 {
      font-family: 'UnifrakturMaguntia', cursive;
      font-size: clamp(3rem, 8vw, 6rem);
      line-height: 1.2;
      background: linear-gradient(
        180deg,
        #FFFFFF 0%, #E8E8F0 15%, #A0A0B0 35%,
        #E8E8F0 50%, #808080 65%, #C0C0C0 80%, #FFFFFF 100%
      );
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      filter: drop-shadow(3px 3px 0px rgba(13, 0, 21, 0.9))
              drop-shadow(0 0 20px rgba(255, 20, 147, 0.3));
      position: relative;
    }

    /* Glitch copies of the heading */
    .dialup-hero .glitch-layer {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      font-family: 'UnifrakturMaguntia', cursive;
      font-size: clamp(3rem, 8vw, 6rem);
      line-height: 1.2;
      pointer-events: none;
    }

    @keyframes glitch-1 {
      0%, 90%, 100% { clip-path: inset(0 0 100% 0); transform: translate(0); }
      92% { clip-path: inset(20% 0 60% 0); transform: translate(-4px, 0); }
      94% { clip-path: inset(70% 0 10% 0); transform: translate(4px, 0); }
      96% { clip-path: inset(40% 0 30% 0); transform: translate(-2px, 0); }
      98% { clip-path: inset(5% 0 80% 0); transform: translate(3px, 0); }
    }

    @keyframes glitch-2 {
      0%, 88%, 100% { clip-path: inset(0 0 100% 0); transform: translate(0); }
      90% { clip-path: inset(60% 0 10% 0); transform: translate(3px, 0); }
      93% { clip-path: inset(10% 0 70% 0); transform: translate(-3px, 0); }
      96% { clip-path: inset(80% 0 5% 0); transform: translate(2px, 0); }
    }

    .dialup-hero .glitch-layer:nth-child(2) {
      color: var(--dialup-accent-pink);
      animation: glitch-1 4s infinite;
      -webkit-text-fill-color: var(--dialup-accent-pink);
      background: none;
      opacity: 0.7;
    }

    .dialup-hero .glitch-layer:nth-child(3) {
      color: var(--dialup-accent-cyan);
      animation: glitch-2 4s infinite;
      -webkit-text-fill-color: var(--dialup-accent-cyan);
      background: none;
      opacity: 0.7;
    }

    /* Subtitle with neon glow */
    .dialup-hero p {
      font-family: 'Press Start 2P', monospace;
      font-size: clamp(0.5rem, 1.2vw, 0.75rem);
      color: var(--dialup-accent-pink);
      text-shadow:
        0 0 7px var(--dialup-accent-pink),
        0 0 20px rgba(255, 20, 147, 0.4);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      margin-top: 1rem;
    }

    /* Neon gradient divider */
    .dialup-divider {
      height: 3px;
      background: linear-gradient(
        90deg,
        var(--dialup-accent-pink),
        var(--dialup-accent-magenta),
        var(--dialup-accent-purple),
        var(--dialup-accent-cyan)
      );
      margin: 2.5rem 0;
      box-shadow: 0 0 10px rgba(255, 20, 147, 0.4), 0 0 20px rgba(139, 0, 255, 0.2);
    }

    /* Overlapping collage section */
    .dialup-collage {
      position: relative;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1rem;
      margin: 2rem 0;
      min-height: 300px;
    }

    .dialup-collage-item {
      border: 2px solid var(--dialup-accent-pink);
      padding: 1.5rem;
      background: var(--dialup-bg-surface);
      position: relative;
      transition: all 0.3s ease;
    }

    .dialup-collage-item:nth-child(1) {
      transform: rotate(-2deg);
      z-index: 1;
      border-color: var(--dialup-accent-pink);
      margin-right: -1.5rem;
      box-shadow: 0 0 15px rgba(255, 20, 147, 0.2), 4px 4px 0px var(--dialup-shadow);
    }

    .dialup-collage-item:nth-child(2) {
      transform: rotate(1.5deg);
      z-index: 2;
      border-color: var(--dialup-accent-cyan);
      margin-left: -1.5rem;
      margin-top: 2rem;
      box-shadow: 0 0 15px rgba(0, 245, 255, 0.2), 4px 4px 0px var(--dialup-shadow);
    }

    .dialup-collage-item:hover {
      z-index: 10;
      transform: rotate(0deg) scale(1.03);
    }

    .dialup-collage-item h2 {
      font-family: 'MedievalSharp', cursive;
      font-size: clamp(1.2rem, 2.5vw, 1.8rem);
      margin-bottom: 0.8rem;
    }

    .dialup-collage-item:nth-child(1) h2 {
      color: var(--dialup-accent-pink);
      text-shadow: 0 0 10px rgba(255, 20, 147, 0.4), 2px 2px 0px var(--dialup-shadow);
    }

    .dialup-collage-item:nth-child(2) h2 {
      color: var(--dialup-accent-cyan);
      text-shadow: 0 0 10px rgba(0, 245, 255, 0.4), 2px 2px 0px var(--dialup-shadow);
    }

    .dialup-collage-item p {
      color: var(--dialup-text-secondary);
      font-size: 1rem;
    }

    /* Stripe accent in corner */
    .dialup-collage-item::before {
      content: '';
      position: absolute;
      top: 0;
      right: 0;
      width: 40px;
      height: 40px;
      background: repeating-linear-gradient(
        45deg,
        var(--dialup-accent-pink) 0px, var(--dialup-accent-pink) 3px,
        transparent 3px, transparent 6px
      );
      clip-path: polygon(100% 0, 0 0, 100% 100%);
      opacity: 0.5;
    }

    .dialup-collage-item:nth-child(2)::before {
      background: repeating-linear-gradient(
        45deg,
        var(--dialup-accent-cyan) 0px, var(--dialup-accent-cyan) 3px,
        transparent 3px, transparent 6px
      );
    }

    /* Card with rainbow animated border */
    .dialup-card-rainbow {
      margin: 2rem 0;
      padding: 3px;
      background: linear-gradient(
        90deg,
        #FF1493, #FF00FF, #8B00FF, #00F5FF, #39FF14, #FFFF00, #FF1493
      );
      background-size: 300% 100%;
      animation: rainbow-shift 4s ease infinite;
      box-shadow: 0 0 15px rgba(255, 20, 147, 0.2);
    }

    @keyframes rainbow-shift {
      0%   { background-position: 0% 50%; }
      50%  { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .dialup-card-rainbow-inner {
      background: var(--dialup-bg-surface);
      padding: 2rem;
    }

    .dialup-card-rainbow-inner h2 {
      font-family: 'Bungee', sans-serif;
      font-size: clamp(1rem, 2vw, 1.4rem);
      color: var(--dialup-accent-green);
      text-transform: uppercase;
      letter-spacing: 0.1em;
      text-shadow: 0 0 10px rgba(57, 255, 20, 0.4);
      margin-bottom: 1rem;
    }

    /* Pixel status label */
    .dialup-status {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      font-family: 'Press Start 2P', monospace;
      font-size: 0.55rem;
      color: var(--dialup-accent-green);
      background: rgba(0, 0, 0, 0.6);
      border: 1px solid var(--dialup-accent-green);
      padding: 0.4rem 0.8rem;
      text-shadow: 0 0 6px rgba(57, 255, 20, 0.5);
      letter-spacing: 0.05em;
    }

    .dialup-status::before {
      content: '';
      display: inline-block;
      width: 6px;
      height: 6px;
      background: var(--dialup-accent-green);
      border-radius: 50%;
      box-shadow: 0 0 6px var(--dialup-accent-green);
      animation: blink 1.5s ease-in-out infinite;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.3; }
    }

    /* Chrome button */
    .dialup-btn-chrome {
      display: inline-block;
      padding: 0.6rem 2rem;
      background: linear-gradient(
        180deg,
        #E8E8F0 0%, #C0C0C0 40%, #808080 55%, #A0A0A0 100%
      );
      border: 2px outset #C0C0C0;
      color: var(--dialup-bg-dark);
      font-family: 'Bungee', sans-serif;
      font-size: 0.8rem;
      text-decoration: none;
      cursor: pointer;
      text-shadow: 1px 1px 0px rgba(255, 255, 255, 0.4);
      box-shadow:
        inset 1px 1px 0px rgba(255, 255, 255, 0.5),
        inset -1px -1px 0px rgba(0, 0, 0, 0.3),
        3px 3px 8px rgba(0, 0, 0, 0.5);
      transition: all 0.15s ease;
      letter-spacing: 0.05em;
    }

    .dialup-btn-chrome:hover {
      background: linear-gradient(
        180deg,
        #FFFFFF 0%, #D0D0D0 40%, #909090 55%, #B0B0B0 100%
      );
    }

    .dialup-btn-chrome:active {
      border-style: inset;
      transform: translate(1px, 1px);
      box-shadow: inset 2px 2px 4px rgba(0, 0, 0, 0.4);
    }

    /* Neon outline button */
    .dialup-btn-neon {
      display: inline-block;
      padding: 0.6rem 2rem;
      background: transparent;
      border: 2px solid var(--dialup-accent-pink);
      color: var(--dialup-accent-pink);
      font-family: 'Press Start 2P', monospace;
      font-size: 0.55rem;
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      cursor: pointer;
      transition: all 0.2s ease;
      box-shadow: 0 0 10px rgba(255, 20, 147, 0.2);
    }

    .dialup-btn-neon:hover {
      background: var(--dialup-accent-pink);
      color: var(--dialup-bg-dark);
      box-shadow: 0 0 20px rgba(255, 20, 147, 0.5), 0 0 40px rgba(255, 20, 147, 0.2);
    }

    /* Sparkle decorations */
    .dialup-sparkles {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 9998;
      overflow: hidden;
    }

    @keyframes twinkle {
      0%, 100% { opacity: 0; transform: scale(0) rotate(0deg); }
      50% { opacity: 1; transform: scale(1) rotate(180deg); }
    }

    .dialup-sparkles .star {
      position: absolute;
      width: 10px;
      height: 10px;
      background: var(--dialup-accent-yellow);
      clip-path: polygon(
        50% 0%, 61% 35%, 98% 35%, 68% 57%,
        79% 91%, 50% 70%, 21% 91%, 32% 57%,
        2% 35%, 39% 35%
      );
      animation: twinkle 2.5s ease-in-out infinite;
    }

    .dialup-sparkles .star:nth-child(1)  { top: 8%; left: 5%; animation-delay: 0s; }
    .dialup-sparkles .star:nth-child(2)  { top: 15%; left: 85%; animation-delay: 0.4s; width: 8px; height: 8px; }
    .dialup-sparkles .star:nth-child(3)  { top: 30%; left: 92%; animation-delay: 1.1s; }
    .dialup-sparkles .star:nth-child(4)  { top: 45%; left: 3%; animation-delay: 0.7s; width: 6px; height: 6px; }
    .dialup-sparkles .star:nth-child(5)  { top: 55%; left: 88%; animation-delay: 1.5s; }
    .dialup-sparkles .star:nth-child(6)  { top: 70%; left: 10%; animation-delay: 0.2s; width: 12px; height: 12px; background: var(--dialup-accent-pink); }
    .dialup-sparkles .star:nth-child(7)  { top: 82%; left: 78%; animation-delay: 1.8s; width: 7px; height: 7px; background: var(--dialup-accent-cyan); }
    .dialup-sparkles .star:nth-child(8)  { top: 25%; left: 45%; animation-delay: 2.2s; width: 5px; height: 5px; }
    .dialup-sparkles .star:nth-child(9)  { top: 65%; left: 55%; animation-delay: 0.9s; background: var(--dialup-accent-pink); }
    .dialup-sparkles .star:nth-child(10) { top: 90%; left: 40%; animation-delay: 1.3s; width: 8px; height: 8px; background: var(--dialup-accent-cyan); }

    /* Footer */
    .dialup-footer {
      text-align: center;
      padding: 2rem 0;
      margin-top: 3rem;
      border-top: 2px solid var(--dialup-bg-surface-light);
    }

    .dialup-footer p {
      font-family: 'Press Start 2P', monospace;
      font-size: 0.5rem;
      color: var(--dialup-text-secondary);
      letter-spacing: 0.05em;
      line-height: 2.5;
    }

    .dialup-footer a {
      color: var(--dialup-accent-pink);
      text-decoration: none;
    }

    .dialup-footer a:hover {
      text-shadow: 0 0 8px rgba(255, 20, 147, 0.6);
    }

    /* Reduced motion preference */
    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
      }
    }
  </style>
</head>
<body>
  <!-- Sparkle decorations -->
  <div class="dialup-sparkles">
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
  </div>

  <div class="dialup-page">
    <!-- Marquee banner -->
    <div class="dialup-marquee">
      <span>*** WELCOME TO MY PAGE *** YOU ARE VISITOR #000042 *** BEST VIEWED AT 1024x768 *** SIGN MY GUESTBOOK *** UNDER CONSTRUCTION *** </span>
    </div>

    <!-- Chrome gothic hero heading with glitch layers -->
    <div class="dialup-hero">
      <h1>
        Dial-Up Delight
        <span class="glitch-layer" aria-hidden="true">Dial-Up Delight</span>
        <span class="glitch-layer" aria-hidden="true">Dial-Up Delight</span>
      </h1>
      <p>gothic grit meets y2k sparkle</p>
    </div>

    <div class="dialup-divider"></div>

    <!-- Overlapping collage cards -->
    <div class="dialup-collage">
      <div class="dialup-collage-item">
        <h2>Gothic Grit</h2>
        <p>Blackletter fonts rise from dark, distressed backgrounds. The modem screams its handshake into the void. Every pixel placed with the reckless confidence of someone who just discovered FrontPage.</p>
        <br>
        <span class="dialup-status">ONLINE</span>
      </div>
      <div class="dialup-collage-item">
        <h2>Y2K Sparkle</h2>
        <p>Chrome text catches the light of a thousand animated GIFs. Candy gradients flow like liquid metal through layouts that defy every grid system ever invented. This is the internet we deserved.</p>
        <br>
        <span class="dialup-btn-neon">ENTER</span>
      </div>
    </div>

    <div class="dialup-divider"></div>

    <!-- Rainbow border card -->
    <div class="dialup-card-rainbow">
      <div class="dialup-card-rainbow-inner">
        <h2>// SYSTEM STATUS</h2>
        <p>The Dial-Up Delight aesthetic remixes the chaotic energy of late '90s and early 2000s internet culture through a modern lens. Gothic blackletter meets chrome metallic meets neon candy -- every design rule broken on purpose, every clashing font a deliberate choice.</p>
        <br>
        <div style="display: flex; gap: 1rem; flex-wrap: wrap;">
          <span class="dialup-btn-chrome">CHROME BUTTON</span>
          <span class="dialup-btn-neon">NEON BUTTON</span>
        </div>
      </div>
    </div>

    <!-- Footer -->
    <div class="dialup-footer">
      <p>
        MADE WITH NOTEPAD.EXE AND A DREAM<br>
        <a href="#">GUESTBOOK</a> | <a href="#">LINKS</a> | <a href="#">WEBRINGS</a><br>
        &copy; 2002 FOREVER
      </p>
    </div>
  </div>
</body>
</html>
```
