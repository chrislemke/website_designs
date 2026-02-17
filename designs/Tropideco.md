# Tropideco Design Reference

Tropideco (also known as Tropi-Kitsch, Tiki Liminal, 2000's Tropical, Tropical Nostalgia, or Kitsch Tropical) is a design aesthetic prominent in the **1990s and early 2000s**, characterized by the **commercialized simulation of tropical environments**. It captures the look and feel of shopping malls, water parks, themed restaurants (like Rainforest Cafe), resort hotels, and indoor leisure complexes that recreated a synthetic version of "paradise." Unlike traditional Tiki or Polynesian pop-culture styling, Tropideco emphasizes **artificiality and exaggeration** -- fiberglass palm trees over real ones, neon-lit tiki bars over authentic craftsmanship, hyper-saturated colors over natural tones. The aesthetic evokes a nostalgic, slightly surreal atmosphere where the boundary between genuine tropical warmth and plastic commercial recreation is deliberately blurred.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Tiki masks and Moai statues** -- carved, cartoonish Polynesian-style faces and Easter Island heads used as decorative focal points
- **Artificial tropical foliage** -- fiberglass and plastic palm trees, ferns, monstera leaves, and tropical flowers; lush but unmistakably synthetic
- **Neon lighting** -- colored neon tubing in tropical hues (magenta, teal, electric blue, hot pink) used as signage, accent lighting, and atmospheric glow
- **Aquariums and fish tanks** -- built-in wall aquariums, cylindrical fish tanks, and contained tropical wildlife displays as architectural features
- **Cartoonish marine life** -- stylized, oversized depictions of tropical fish, seahorses, starfish, dolphins, and sea turtles in bright saturated colors
- **Water features** -- artificial waterfalls, rock grottos, splash pads, water slides, and indoor pools with tropical theming
- **Faux wood and bamboo** -- plastic and fiberglass surfaces molded to imitate bamboo, driftwood, and tropical hardwoods; smooth and polished rather than rough
- **Resort architecture** -- thatched roof structures (made of synthetic materials), poolside cabanas, A-frame huts, and open-air dining pavilions
- **Beach and pool accessories** -- inflatable toys, tiki torches, cocktail umbrellas, lei garlands, surfboards as wall decor
- **Stereotypical Hawaiian motifs** -- hibiscus flowers, plumeria, pineapples, hula dancers, steel guitars, Hawaiian shirt patterns
- **Terrazzo and polished stone floors** -- the smooth, commercial-grade flooring of malls and resort lobbies
- **Themed signage** -- bamboo-framed menu boards, carved wooden signs with tropical typography, backlit acrylic panels

### Design Principles

- **Synthetic over authentic** -- every element should feel like a commercial recreation, not the real thing; smooth plastic over rough natural texture
- **Hyper-saturation** -- colors are pushed beyond natural levels; greens are electric, blues are neon, reds are punchy
- **Enclosed tropical simulation** -- the environment is self-contained; an indoor world with no real sky, creating a liminal, timeless quality
- **Cartoonish exaggeration** -- motifs are oversized, simplified, and playful rather than detailed or realistic
- **Layered theming** -- multiple tropical elements stacked together: foliage + water + neon + tiki + marine life all in one space
- **Commercial warmth** -- the atmosphere is inviting and entertaining, designed to sell the fantasy of a tropical vacation
- **Nostalgic artificiality** -- the fakeness is part of the charm; it triggers memories of childhood visits to themed restaurants and water parks

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base / Dark** | Deep teal, dark jungle green, rich navy |
| **Primary accents** | Neon magenta, electric teal, hot coral |
| **Warm tones** | Sunset orange, golden yellow, warm tan |
| **Foliage** | Electric green, lime, deep emerald |
| **Water** | Bright cyan, turquoise, aqua blue |
| **Accent / Glow** | Neon pink, purple, electric blue |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Deep Teal | `#004D4D`, `#006666` | Primary dark backgrounds, section bases |
| Jungle Green | `#1A3C2A`, `#0D2818` | Dark background panels, footer areas |
| Rich Navy | `#0A1628`, `#0F1E3D` | Deep background, night-sky sections |
| Neon Magenta | `#FF2D8A`, `#FF1493` | Primary neon accent, signage glow, highlights |
| Electric Teal | `#00E5CC`, `#00D4AA` | Secondary neon accent, water references, glow effects |
| Hot Coral | `#FF6B4A`, `#FF5733` | Warm accent, call-to-action, tropical flowers |
| Sunset Orange | `#FF8C42`, `#FFA447` | Warm accent, sunset gradients, decorative elements |
| Golden Yellow | `#FFD700`, `#FFC300` | Sand tones, sunlight accents, tiki torch glow |
| Warm Tan | `#D4A574`, `#C4956A` | Bamboo and wood surfaces, neutral warmth |
| Faux Bamboo | `#B8945A`, `#A07D4A` | Faux-wood borders, frame elements |
| Electric Green | `#39FF14`, `#32CD32` | Neon foliage highlights, glow accents |
| Lime | `#A8E06C`, `#8BC34A` | Tropical leaf accents, fresh plant tones |
| Deep Emerald | `#006B3F`, `#004D2C` | Dense foliage backgrounds, leaf shapes |
| Bright Cyan | `#00E5FF`, `#00BCD4` | Pool water, aquarium glow, water features |
| Turquoise | `#40E0D0`, `#48D1CC` | Tropical ocean, light water sections |
| Aqua Blue | `#7FDBFF`, `#87CEEB` | Light water tones, sky references, gentle accents |
| Dark Purple | `#4A0E4E`, `#5C1A66` | Atmospheric depth, neon glow undertones |
| Neon Purple | `#BF40FF`, `#9B30FF` | Secondary neon accent, evening atmosphere |
| Fiberglass White | `#F5F0E6`, `#EDE8D8` | Smooth artificial surfaces, card backgrounds |
| Pool Tile White | `#E8F4F8`, `#D4EEF2` | Light panels, content surfaces with cool tint |

### Suggested CSS Custom Properties

```css
:root {
  /* Dark bases */
  --tropi-teal-deep: #004d4d;
  --tropi-jungle: #1a3c2a;
  --tropi-navy: #0a1628;
  --tropi-dark: #0d2818;

  /* Neon accents */
  --tropi-magenta: #ff2d8a;
  --tropi-cyan: #00e5ff;
  --tropi-teal-neon: #00e5cc;
  --tropi-green-neon: #39ff14;
  --tropi-purple-neon: #bf40ff;

  /* Warm tones */
  --tropi-coral: #ff6b4a;
  --tropi-orange: #ff8c42;
  --tropi-gold: #ffd700;
  --tropi-tan: #d4a574;
  --tropi-bamboo: #b8945a;

  /* Foliage */
  --tropi-emerald: #006b3f;
  --tropi-lime: #a8e06c;
  --tropi-green: #32cd32;

  /* Water */
  --tropi-turquoise: #40e0d0;
  --tropi-aqua: #7fdbff;
  --tropi-pool: #00bcd4;

  /* Purples */
  --tropi-purple-deep: #4a0e4e;
  --tropi-purple: #5c1a66;

  /* Neutrals */
  --tropi-white: #f5f0e6;
  --tropi-tile: #e8f4f8;
  --tropi-sand: #ede8d8;

  /* Neon glows (for box-shadow / text-shadow) */
  --tropi-glow-magenta: rgba(255, 45, 138, 0.45);
  --tropi-glow-cyan: rgba(0, 229, 255, 0.4);
  --tropi-glow-teal: rgba(0, 229, 204, 0.4);
  --tropi-glow-green: rgba(57, 255, 20, 0.35);
  --tropi-glow-purple: rgba(191, 64, 255, 0.35);
  --tropi-glow-magenta-strong: rgba(255, 45, 138, 0.65);
  --tropi-glow-cyan-strong: rgba(0, 229, 255, 0.6);

  /* Functional mappings */
  --tropi-bg-primary: var(--tropi-teal-deep);
  --tropi-bg-secondary: var(--tropi-jungle);
  --tropi-bg-surface: var(--tropi-dark);
  --tropi-text-primary: var(--tropi-white);
  --tropi-text-secondary: var(--tropi-sand);
  --tropi-accent: var(--tropi-magenta);
  --tropi-accent-secondary: var(--tropi-cyan);
  --tropi-border: rgba(0, 229, 204, 0.25);
}
```

### Approaches

- **Dark tropical base** -- deep teals, jungle greens, and navy blues form the primary backgrounds, simulating an indoor tropical environment at night or under dim themed lighting
- **Neon as the signature element** -- magenta, cyan, and electric green neon glow effects punctuate the dark base, replicating the neon signage and accent lighting of 90s themed venues
- **Hyper-saturated accent colors** -- every accent color is pushed beyond natural levels; nothing is muted or subtle
- **Warm-cool contrast** -- hot corals, oranges, and golds contrast against cool teals, cyans, and aquas, creating the collision of sunset warmth and tropical water
- **Water tones for depth** -- turquoise, aqua, and pool-blue tones reference the ever-present water features, aquariums, and pools
- **Faux-natural neutrals** -- tan, bamboo, and warm off-white tones reference the fake wood and fiberglass surfaces

---

## Typography

### Typeface Characteristics

Tropideco typography reflects **themed restaurant signage, water park branding, and 90s resort-style commercial lettering**:

- **Rounded, bold display fonts** -- chunky, friendly letterforms evoking theme park and water park branding
- **Tiki/bamboo-inspired display faces** -- decorative fonts with a carved, organic, or tropical character for headlines
- **Wide, heavy sans-serifs** -- bold, expanded typefaces for maximum legibility from a distance (like mall signage)
- **Playful, cartoonish weights** -- exaggerated thick strokes and rounded terminals that feel fun and approachable
- **Uppercase for impact** -- display text in all caps with generous letter-spacing for a commercial, branded feel
- **Clean sans-serif for body** -- modern readable type for content areas, contrasting with the decorative headlines
- **Occasional retro-tropical scripts** -- flowing cursive for decorative accents, evoking hand-painted beach-bar signs

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Bungee** | Bold, chunky display | Headlines, hero text -- captures the bold commercial signage energy |
| **Bungee Shade** | Layered, dimensional display | Feature titles, special headings -- adds depth and 90s flair |
| **Lilita One** | Heavy, rounded sans-serif | Headlines, section titles -- friendly and bold |
| **Luckiest Guy** | Playful, cartoonish display | Accent headings, decorative text -- theme park energy |
| **Fredoka One** | Rounded, bubbly | Subheadings, callouts -- approachable tropical warmth |
| **Pacifico** | Retro tropical script | Decorative accents, taglines -- beachy hand-painted vibe |
| **Righteous** | Retro condensed display | Secondary headlines, labels -- 90s commercial feel |
| **Nunito** | Rounded geometric sans | Body text, UI elements -- friendly readability |
| **Quicksand** | Rounded geometric sans | Body text, captions -- soft and warm |
| **Montserrat** | Clean geometric sans | Navigation, labels, metadata -- structured and legible |

### Typography CSS Example

```css
/* Headlines -- bold themed signage */
h1, h2, h3 {
  font-family: 'Lilita One', 'Bungee', 'Luckiest Guy', sans-serif;
  font-weight: 400;
  letter-spacing: 0.04em;
  color: var(--tropi-gold);
  text-shadow:
    0 0 10px var(--tropi-glow-cyan),
    0 2px 4px rgba(0, 0, 0, 0.4);
}

/* Display / Hero text -- neon tiki sign */
.tropi-display {
  font-family: 'Bungee Shade', 'Bungee', sans-serif;
  font-size: clamp(2.5rem, 7vw, 6rem);
  font-weight: 400;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  line-height: 1.1;
  color: var(--tropi-magenta);
  text-shadow:
    0 0 10px var(--tropi-glow-magenta),
    0 0 40px var(--tropi-glow-magenta),
    0 0 80px var(--tropi-glow-magenta-strong),
    0 3px 6px rgba(0, 0, 0, 0.5);
}

/* Body text */
body {
  font-family: 'Nunito', 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1.05rem;
  letter-spacing: 0.01em;
  line-height: 1.7;
  color: var(--tropi-sand);
  -webkit-font-smoothing: antialiased;
}

/* Tropical script accent -- beach bar signage */
.tropi-script {
  font-family: 'Pacifico', cursive;
  font-size: 1.5em;
  font-weight: 400;
  color: var(--tropi-coral);
  text-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
}

/* Navigation / wayfinding */
nav a {
  font-family: 'Montserrat', 'Righteous', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--tropi-teal-neon);
}

/* Playful callout text */
.tropi-callout {
  font-family: 'Fredoka One', 'Luckiest Guy', sans-serif;
  font-size: 1.3rem;
  color: var(--tropi-cyan);
  text-shadow: 0 0 6px var(--tropi-glow-cyan);
}
```

---

## Layout Principles

### Grid and Structure

- **Dark, immersive full-bleed sections** -- backgrounds that wrap the user in a themed environment, like walking through a themed restaurant or water park
- **Centered content corridors** -- content flows down a central axis, like moving through a resort lobby or mall concourse
- **Layered depth** -- overlapping elements at different z-depths (foliage in foreground, content in middle, atmospheric glow in background) to simulate the dense, layered theming of real Tropideco spaces
- **Full-width hero sections** -- dramatic, atmospheric headers that establish the tropical-commercial mood immediately
- **Card-based content groups** -- rounded-corner cards with neon accents, like themed information boards or resort directory panels
- **Generous padding** -- spacious layouts reflecting the open architecture of resort lobbies and themed dining areas

### Section Organization

- Use **gradient transitions** between sections, fading from one tropical tone to another (deep teal to jungle green, navy to purple)
- Apply **neon-accented section headers** -- text with glow effects that feel like themed signage
- Create **bamboo/wood-framed containers** -- border effects that simulate the faux-bamboo frames used in real Tropideco environments
- Employ **foliage overlays** -- decorative leaf shapes at section edges and corners, partially overlapping content
- Add **water-inspired dividers** -- wavy lines, gradient washes in aqua/turquoise tones between content blocks
- Incorporate **atmospheric background textures** -- subtle gradients, gentle noise, and color washes suggesting colored ambient lighting

---

## CSS/Design Techniques

### Tropical Night Background

```css
/* Dark, neon-lit tropical environment */
.tropi-night-bg {
  background: linear-gradient(
    180deg,
    #0a1628 0%,
    #004d4d 30%,
    #0d2818 60%,
    #1a3c2a 100%
  );
  min-height: 100vh;
}

/* Resort lobby -- warmer, with ambient glow */
.tropi-lobby-bg {
  background:
    radial-gradient(
      ellipse 80% 50% at 50% 20%,
      rgba(255, 45, 138, 0.08) 0%,
      transparent 60%
    ),
    radial-gradient(
      ellipse 60% 40% at 70% 80%,
      rgba(0, 229, 255, 0.06) 0%,
      transparent 50%
    ),
    linear-gradient(
      180deg,
      #004d4d 0%,
      #0d2818 50%,
      #0a1628 100%
    );
}

/* Pool-side gradient */
.tropi-pool-bg {
  background: linear-gradient(
    180deg,
    #006666 0%,
    #00bcd4 40%,
    #40e0d0 70%,
    #7fdbff 100%
  );
}
```

### Neon Tiki Sign Text Effect

```css
/* Glowing neon text -- the signature Tropideco signage */
.tropi-neon {
  color: var(--tropi-magenta);
  text-shadow:
    0 0 7px var(--tropi-glow-magenta),
    0 0 20px var(--tropi-glow-magenta),
    0 0 42px var(--tropi-glow-magenta-strong),
    0 0 82px var(--tropi-glow-magenta-strong);
}

/* Cyan neon variant -- aquarium / pool glow */
.tropi-neon--cyan {
  color: var(--tropi-cyan);
  text-shadow:
    0 0 7px var(--tropi-glow-cyan),
    0 0 20px var(--tropi-glow-cyan),
    0 0 42px var(--tropi-glow-cyan-strong),
    0 0 82px var(--tropi-glow-cyan-strong);
}

/* Green neon variant -- jungle foliage glow */
.tropi-neon--green {
  color: var(--tropi-green-neon);
  text-shadow:
    0 0 7px var(--tropi-glow-green),
    0 0 20px var(--tropi-glow-green),
    0 0 42px rgba(57, 255, 20, 0.5),
    0 0 82px rgba(57, 255, 20, 0.5);
}

/* Flickering neon -- aging tiki bar sign */
@keyframes tropi-neon-flicker {
  0%, 18%, 22%, 25%, 53%, 57%, 100% {
    text-shadow:
      0 0 7px var(--tropi-glow-magenta),
      0 0 20px var(--tropi-glow-magenta),
      0 0 42px var(--tropi-glow-magenta-strong);
    opacity: 1;
  }
  20%, 24%, 55% {
    text-shadow: none;
    opacity: 0.5;
  }
}

.tropi-neon--flicker {
  animation: tropi-neon-flicker 4s infinite;
}
```

### Bamboo Frame / Border

```css
/* Faux-bamboo frame for content panels */
.tropi-bamboo-frame {
  border: 4px solid var(--tropi-bamboo);
  border-radius: 8px;
  padding: 2rem;
  position: relative;
  background: rgba(13, 40, 24, 0.85);
  box-shadow:
    inset 0 0 20px rgba(0, 0, 0, 0.3),
    0 4px 20px rgba(0, 0, 0, 0.4);
}

/* Bamboo joint accents at corners */
.tropi-bamboo-frame::before,
.tropi-bamboo-frame::after {
  content: '';
  position: absolute;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: var(--tropi-tan);
  border: 2px solid var(--tropi-bamboo);
}

.tropi-bamboo-frame::before {
  top: -6px;
  left: -6px;
}

.tropi-bamboo-frame::after {
  bottom: -6px;
  right: -6px;
}

/* Double-bamboo border variant */
.tropi-bamboo-double {
  border: 3px solid var(--tropi-bamboo);
  outline: 3px solid var(--tropi-bamboo);
  outline-offset: 5px;
  border-radius: 6px;
  padding: 2.5rem;
}
```

### Aquarium / Fish Tank Panel

```css
/* Content panel styled like a built-in aquarium */
.tropi-aquarium {
  background: linear-gradient(
    180deg,
    rgba(0, 107, 63, 0.15) 0%,
    rgba(0, 188, 212, 0.2) 50%,
    rgba(0, 77, 77, 0.25) 100%
  );
  border: 2px solid rgba(0, 229, 255, 0.2);
  border-radius: 12px;
  padding: 2.5rem;
  position: relative;
  overflow: hidden;
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  box-shadow:
    0 0 30px rgba(0, 229, 255, 0.08),
    inset 0 0 40px rgba(0, 188, 212, 0.05);
}

/* Subtle light caustics / water ripple overlay */
.tropi-aquarium::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(ellipse 30% 20% at 25% 30%, rgba(0, 229, 255, 0.06) 0%, transparent 70%),
    radial-gradient(ellipse 25% 15% at 65% 55%, rgba(64, 224, 208, 0.05) 0%, transparent 70%),
    radial-gradient(ellipse 20% 25% at 80% 20%, rgba(0, 229, 255, 0.04) 0%, transparent 70%);
  pointer-events: none;
  animation: tropi-caustics 8s ease-in-out infinite alternate;
}

@keyframes tropi-caustics {
  0% { opacity: 0.6; transform: translateX(0) translateY(0); }
  100% { opacity: 1; transform: translateX(10px) translateY(-5px); }
}
```

### Tropical Foliage Overlay

```css
/* Decorative leaf shapes at section edges */
.tropi-foliage-left::before {
  content: '';
  position: absolute;
  top: 0;
  left: -20px;
  width: 200px;
  height: 300px;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 300'%3E%3Cpath d='M10 300 Q50 200 30 150 Q10 100 50 50 Q70 20 100 10 Q80 60 90 100 Q100 150 80 200 Q60 250 50 300Z' fill='%23006b3f' opacity='0.3'/%3E%3Cpath d='M0 280 Q30 220 20 170 Q10 130 40 80 Q55 50 80 30 Q65 80 70 120 Q80 170 60 220 Q40 260 35 280Z' fill='%2332cd32' opacity='0.15'/%3E%3C/svg%3E") no-repeat;
  background-size: contain;
  pointer-events: none;
  z-index: 2;
}

.tropi-foliage-right::after {
  content: '';
  position: absolute;
  top: 10%;
  right: -20px;
  width: 180px;
  height: 280px;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 180 280'%3E%3Cpath d='M170 280 Q130 200 150 140 Q170 90 130 40 Q110 15 80 5 Q100 50 90 100 Q80 150 100 200 Q120 250 130 280Z' fill='%23006b3f' opacity='0.25'/%3E%3Cpath d='M180 260 Q150 200 160 150 Q170 110 140 60 Q120 30 100 20 Q115 65 110 110 Q100 160 120 210 Q140 250 145 260Z' fill='%23a8e06c' opacity='0.12'/%3E%3C/svg%3E") no-repeat;
  background-size: contain;
  pointer-events: none;
  z-index: 2;
}
```

### Resort Card / Content Panel

```css
/* Content card styled like a themed resort information board */
.tropi-card {
  background: linear-gradient(
    180deg,
    rgba(0, 77, 77, 0.7) 0%,
    rgba(13, 40, 24, 0.85) 100%
  );
  border: 1px solid rgba(0, 229, 204, 0.2);
  border-radius: 14px;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 4px 24px rgba(0, 0, 0, 0.3),
    0 0 40px rgba(0, 229, 204, 0.05);
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

/* Neon accent strip at top */
.tropi-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: linear-gradient(
    90deg,
    var(--tropi-magenta) 0%,
    var(--tropi-cyan) 50%,
    var(--tropi-green-neon) 100%
  );
  box-shadow: 0 0 10px var(--tropi-glow-cyan);
}

.tropi-card:hover {
  transform: translateY(-3px);
  box-shadow:
    0 8px 30px rgba(0, 0, 0, 0.4),
    0 0 30px rgba(0, 229, 204, 0.1),
    0 0 60px var(--tropi-glow-magenta);
}
```

### Water Wave Divider

```css
/* Wavy divider between sections -- pool/ocean reference */
.tropi-wave-divider {
  width: 100%;
  height: 60px;
  position: relative;
  overflow: hidden;
}

.tropi-wave-divider svg {
  display: block;
  width: 100%;
  height: 100%;
}

/* CSS-only wave alternative */
.tropi-wave-line {
  width: 80%;
  margin: 2rem auto;
  height: 3px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--tropi-cyan) 15%,
    var(--tropi-turquoise) 35%,
    var(--tropi-teal-neon) 50%,
    var(--tropi-turquoise) 65%,
    var(--tropi-cyan) 85%,
    transparent
  );
  border-radius: 2px;
  box-shadow:
    0 0 8px var(--tropi-glow-cyan),
    0 0 20px var(--tropi-glow-teal);
  position: relative;
}
```

```html
<!-- SVG wave divider for organic water shape -->
<svg class="tropi-wave-svg" viewBox="0 0 1440 60" preserveAspectRatio="none">
  <path d="M0,30 C240,55 480,5 720,30 C960,55 1200,5 1440,30 L1440,60 L0,60 Z"
        fill="#004d4d" />
</svg>
```

### Tiki Torch / Neon Border Glow

```css
/* Neon-glowing border for containers -- tiki bar neon tubing */
.tropi-neon-border {
  border: 2px solid var(--tropi-magenta);
  border-radius: 12px;
  box-shadow:
    0 0 8px var(--tropi-glow-magenta),
    0 0 20px var(--tropi-glow-magenta),
    inset 0 0 8px var(--tropi-glow-magenta);
}

.tropi-neon-border--cyan {
  border-color: var(--tropi-cyan);
  box-shadow:
    0 0 8px var(--tropi-glow-cyan),
    0 0 20px var(--tropi-glow-cyan),
    inset 0 0 8px var(--tropi-glow-cyan);
}

/* Tiki torch warm glow */
.tropi-torch-glow {
  background: radial-gradient(
    circle at 50% 30%,
    rgba(255, 140, 66, 0.15) 0%,
    rgba(255, 107, 74, 0.08) 40%,
    transparent 70%
  );
}
```

### Button Styles

```css
/* Primary -- neon tropical button */
.tropi-btn-primary {
  background: var(--tropi-magenta);
  color: #fff;
  border: none;
  padding: 0.85rem 2.2rem;
  border-radius: 8px;
  font-family: 'Lilita One', 'Bungee', sans-serif;
  font-size: 0.95rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  cursor: pointer;
  box-shadow: 0 4px 16px var(--tropi-glow-magenta);
  transition: all 0.3s ease;
}

.tropi-btn-primary:hover {
  background: #ff1493;
  box-shadow:
    0 4px 20px var(--tropi-glow-magenta-strong),
    0 0 40px var(--tropi-glow-magenta);
  transform: translateY(-2px);
}

/* Secondary -- outlined neon */
.tropi-btn-secondary {
  background: transparent;
  color: var(--tropi-cyan);
  border: 2px solid var(--tropi-cyan);
  padding: 0.75rem 2rem;
  border-radius: 8px;
  font-family: 'Montserrat', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
}

.tropi-btn-secondary:hover {
  background: var(--tropi-cyan);
  color: var(--tropi-dark);
  box-shadow:
    0 0 12px var(--tropi-glow-cyan),
    0 0 30px var(--tropi-glow-cyan);
}

/* Warm CTA -- sunset coral */
.tropi-btn-cta {
  background: linear-gradient(135deg, var(--tropi-coral), var(--tropi-orange));
  color: #fff;
  border: none;
  padding: 0.9rem 2.4rem;
  border-radius: 24px;
  font-family: 'Lilita One', sans-serif;
  font-size: 1rem;
  letter-spacing: 0.04em;
  cursor: pointer;
  box-shadow: 0 4px 16px rgba(255, 107, 74, 0.3);
  transition: all 0.3s ease;
}

.tropi-btn-cta:hover {
  box-shadow:
    0 6px 24px rgba(255, 107, 74, 0.45),
    0 0 30px rgba(255, 140, 66, 0.2);
  transform: translateY(-2px);
}
```

### Faux-Wood / Polished Surface Texture

```css
/* Smooth polished surface -- fiberglass/plastic tropical material */
.tropi-polished {
  background: linear-gradient(
    135deg,
    rgba(212, 165, 116, 0.12) 0%,
    rgba(184, 148, 90, 0.08) 50%,
    rgba(212, 165, 116, 0.12) 100%
  );
  position: relative;
}

/* Faux wood grain overlay at very low opacity */
.tropi-polished::after {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    175deg,
    rgba(184, 148, 90, 0.04) 0px,
    transparent 2px,
    transparent 8px,
    rgba(184, 148, 90, 0.03) 10px
  );
  pointer-events: none;
}

/* Terrazzo / polished stone floor texture */
.tropi-terrazzo {
  background-color: var(--tropi-tile);
  background-image:
    radial-gradient(circle 3px at 12% 20%, rgba(0, 229, 204, 0.15) 1.5px, transparent 2px),
    radial-gradient(circle 2px at 40% 55%, rgba(255, 45, 138, 0.1) 1px, transparent 1.5px),
    radial-gradient(circle 4px at 65% 25%, rgba(168, 224, 108, 0.12) 2px, transparent 3px),
    radial-gradient(circle 2.5px at 25% 75%, rgba(0, 188, 212, 0.1) 1.2px, transparent 2px),
    radial-gradient(circle 3px at 80% 50%, rgba(255, 215, 0, 0.08) 1.5px, transparent 2px),
    radial-gradient(circle 2px at 50% 85%, rgba(191, 64, 255, 0.08) 1px, transparent 1.5px);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Tropideco materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Fiberglass palm trees / foliage | SVG leaf shapes as decorative overlays at section edges, in saturated greens at low-medium opacity |
| Faux bamboo | Warm tan/brown border effects with rounded joint accents at corners; `border` + pseudo-element circles |
| Polished plastic surfaces | Smooth dark gradient backgrounds with subtle sheen; `linear-gradient` with soft highlight bands |
| Neon tube lighting | Multi-layered `text-shadow` and `box-shadow` glow effects in magenta, cyan, and green |
| Aquarium glass | Semi-transparent panels with `backdrop-filter: blur()` and cool blue-green tints |
| Pool / water feature | Turquoise-to-cyan gradients, animated caustic light patterns using radial gradients |
| Terrazzo floor | Speckled `radial-gradient` chips in tropical colors on light stone-toned backgrounds |
| Tiki wood carving | Dark, warm-toned panels with inset shadows and carved-border effects |
| Thatched roof | Repeating diagonal line pattern in warm tan/straw tones at low opacity |
| Smooth resort tile | Clean, slightly cool-tinted white backgrounds with faint blue undertone |
| Rock grotto / waterfall | Dark textured backgrounds with layered depth gradients and mist-like `radial-gradient` overlays |
| Sunset sky | Warm gradient backgrounds transitioning from orange through coral to deep purple |

---

## Sub-styles and Variations

### Golden-Era Tropideco (Peak 90s)

- Bright, bustling, maximally themed environment
- Every surface covered in tropical decoration; dense and immersive
- Neon signage glowing at full brightness, aquariums bubbling, waterfalls running
- Optimistic, commercial, family-entertainment energy
- Web approach: vibrant saturated colors, multiple neon glow effects, layered foliage overlays, dense visual richness

### Dead Tropideco (Liminal Variant)

- The abandoned water park, the shuttered themed restaurant, the decaying resort lobby
- Shared sensibility with Liminal Space and Dreamcore aesthetics
- Faded, desaturated colors; neon signs half-lit or flickering; empty pools, dry fountains
- Eerie, nostalgic, melancholic atmosphere
- Web approach: muted/desaturated palette, flickering neon animations, reduced opacity on decorative elements, darker backgrounds, subtle grain overlay

### Water Park Tropideco

- Focused specifically on the indoor water park experience
- Dominated by bright aquas, cyans, and turquoises with splash-zone energy
- Slide structures, wave pools, lazy rivers as visual motifs
- More active and kinetic than the general variant
- Web approach: bright water-tone palette, dynamic wave dividers, bold rounded typography, energetic and playful layout

### Resort Lobby Tropideco

- The quieter, more refined side of the aesthetic
- Polished stone floors, large potted palms, soft ambient lighting
- Tiki bar elements mixed with commercial hospitality design
- More subdued neon, more warm wood tones, upscale-casual atmosphere
- Web approach: warmer palette with more tan/bamboo, subtler neon, elegant rounded typography, spacious layouts with premium feel

---

## Related Aesthetics

| Aesthetic | Relationship to Tropideco |
|-----------|---------------------------|
| **Tropical** | Broader parent category; Tropideco is specifically the commercialized, artificial simulation of tropical environments |
| **Tiki** | Close sibling; shares Polynesian motifs but Tiki is more rooted in mid-century pop-culture authenticity while Tropideco is 90s synthetic |
| **Mallsoft** | Shared commercial-indoor-space DNA; Mallsoft is the mall itself, Tropideco is the themed tropical zone within it |
| **Liminal Space** | Shared in the "dead" variant; empty themed spaces are powerfully liminal |
| **Dreamcore** | Shared surreal, half-remembered quality; Tropideco environments often appear in Dreamcore imagery |
| **Frutiger Aero** | Both feature glossy, nature-referencing commercial design from the 2000s; Frutiger Aero is digital/tech, Tropideco is physical/architectural |
| **Poolcore** | Subset focused on pool and water aesthetics; overlaps with Tropideco's water park dimension |
| **Nautical** | Shares marine elements but Nautical is traditional and preppy while Tropideco is synthetic and kitschy |
| **Beach Day** | Shares beach motifs but Beach Day is outdoors and natural while Tropideco is indoors and artificial |
| **Nostalgia** | Tropideco is inherently nostalgic, evoking specific 90s-2000s childhood commercial experiences |

---

## Quick-Start: Minimal Tropideco Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tropideco Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Lilita+One&family=Nunito:wght@400;600;700&family=Pacifico&family=Montserrat:wght@500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --tropi-teal-deep: #004d4d;
      --tropi-jungle: #1a3c2a;
      --tropi-navy: #0a1628;
      --tropi-dark: #0d2818;
      --tropi-magenta: #ff2d8a;
      --tropi-cyan: #00e5ff;
      --tropi-teal-neon: #00e5cc;
      --tropi-coral: #ff6b4a;
      --tropi-orange: #ff8c42;
      --tropi-gold: #ffd700;
      --tropi-tan: #d4a574;
      --tropi-bamboo: #b8945a;
      --tropi-emerald: #006b3f;
      --tropi-lime: #a8e06c;
      --tropi-turquoise: #40e0d0;
      --tropi-aqua: #7fdbff;
      --tropi-white: #f5f0e6;
      --tropi-sand: #ede8d8;
      --tropi-glow-magenta: rgba(255, 45, 138, 0.45);
      --tropi-glow-cyan: rgba(0, 229, 255, 0.4);
      --tropi-glow-teal: rgba(0, 229, 204, 0.4);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: linear-gradient(
        180deg,
        #0a1628 0%,
        #004d4d 30%,
        #0d2818 60%,
        #1a3c2a 100%
      );
      color: var(--tropi-sand);
      font-family: 'Nunito', sans-serif;
      font-weight: 400;
      font-size: 1.05rem;
      line-height: 1.7;
      letter-spacing: 0.01em;
      min-height: 100vh;
      overflow-x: hidden;
      -webkit-font-smoothing: antialiased;
    }

    h1, h2, h3 {
      font-family: 'Lilita One', sans-serif;
      font-weight: 400;
      letter-spacing: 0.04em;
      color: var(--tropi-gold);
      text-shadow:
        0 0 10px var(--tropi-glow-cyan),
        0 2px 4px rgba(0, 0, 0, 0.4);
    }

    /* Hero -- themed resort entrance */
    .hero {
      text-align: center;
      padding: 8rem 2rem 5rem;
      position: relative;
      overflow: hidden;
    }

    /* Ambient neon glow behind hero */
    .hero::before {
      content: '';
      position: absolute;
      top: -10%;
      left: 20%;
      width: 60%;
      height: 70%;
      background: radial-gradient(
        ellipse at center,
        rgba(255, 45, 138, 0.1) 0%,
        rgba(0, 229, 255, 0.05) 40%,
        transparent 70%
      );
      pointer-events: none;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 7vw, 5.5rem);
      text-transform: uppercase;
      color: var(--tropi-magenta);
      text-shadow:
        0 0 10px var(--tropi-glow-magenta),
        0 0 40px var(--tropi-glow-magenta),
        0 0 80px rgba(255, 45, 138, 0.65),
        0 3px 6px rgba(0, 0, 0, 0.5);
      position: relative;
      z-index: 1;
    }

    .hero .tagline {
      font-family: 'Pacifico', cursive;
      font-size: 1.4rem;
      color: var(--tropi-coral);
      margin-top: 1rem;
      text-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
      position: relative;
      z-index: 1;
    }

    /* Neon wave divider */
    .neon-wave {
      width: 60%;
      margin: 2rem auto;
      height: 3px;
      background: linear-gradient(
        90deg,
        transparent,
        var(--tropi-cyan) 15%,
        var(--tropi-turquoise) 50%,
        var(--tropi-cyan) 85%,
        transparent
      );
      border-radius: 2px;
      box-shadow:
        0 0 8px var(--tropi-glow-cyan),
        0 0 20px var(--tropi-glow-teal);
      position: relative;
      z-index: 1;
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    /* Resort info card */
    .tropi-card {
      background: linear-gradient(
        180deg,
        rgba(0, 77, 77, 0.7) 0%,
        rgba(13, 40, 24, 0.85) 100%
      );
      border: 1px solid rgba(0, 229, 204, 0.2);
      border-radius: 14px;
      padding: 2.5rem;
      position: relative;
      overflow: hidden;
      box-shadow:
        0 4px 24px rgba(0, 0, 0, 0.3),
        0 0 40px rgba(0, 229, 204, 0.05);
      transition: box-shadow 0.3s ease, transform 0.3s ease;
    }

    .tropi-card::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0;
      height: 3px;
      background: linear-gradient(
        90deg,
        var(--tropi-magenta),
        var(--tropi-cyan),
        var(--tropi-lime)
      );
      box-shadow: 0 0 10px var(--tropi-glow-cyan);
    }

    .tropi-card:hover {
      transform: translateY(-3px);
      box-shadow:
        0 8px 30px rgba(0, 0, 0, 0.4),
        0 0 30px rgba(0, 229, 204, 0.1);
    }

    .tropi-card h2 {
      font-size: 1.6rem;
      margin-bottom: 1rem;
    }

    /* Neon tropical button */
    .tropi-btn {
      display: inline-block;
      padding: 0.85rem 2.2rem;
      margin-top: 1.5rem;
      border-radius: 8px;
      border: 2px solid var(--tropi-magenta);
      background: transparent;
      color: var(--tropi-magenta);
      font-family: 'Montserrat', sans-serif;
      font-size: 0.85rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .tropi-btn:hover {
      background: var(--tropi-magenta);
      color: #fff;
      box-shadow:
        0 0 12px var(--tropi-glow-magenta),
        0 0 30px var(--tropi-glow-magenta);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <hr class="neon-wave">
    <p class="tagline">Where the palms are plastic and the neon never fades</p>
  </div>

  <section>
    <div class="tropi-card">
      <h2>Section Heading</h2>
      <p>Content displayed on a dark tropical panel with neon accent lighting, capturing the synthetic paradise of 90s-era themed restaurants, water parks, and resort lobbies -- fiberglass foliage, glowing aquariums, and the warm hum of commercial tropicana.</p>
      <a href="#" class="tropi-btn">Explore</a>
    </div>
  </section>
</body>
</html>
```
