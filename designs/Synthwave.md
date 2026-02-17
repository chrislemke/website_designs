# Synthwave Design Reference

Synthwave is a retro-futuristic aesthetic rooted in 1980s pop culture, electronic music, and science fiction cinema. It celebrates the neon-drenched optimism of an imagined 1980s future: glowing sunset gradients, chrome lettering, Lamborghini silhouettes, and infinite perspective grids stretching toward electric-purple horizons. Unlike the ironic detachment of Vaporwave, Synthwave is earnest and celebratory -- it genuinely loves the 80s and amplifies its visual language to mythic proportions. In web and UI design, Synthwave translates to bold neon-on-dark palettes, dramatic gradient skies, retro-futuristic typography, chrome effects, and an overwhelming sense of speed, power, and nocturnal glamour.

---

## Visual Characteristics

### Core Design Traits

- **Neon sunset gradients** -- dramatic orange-to-pink-to-purple horizons dominating hero sections and backgrounds
- **Perspective grid floors** -- wireframe grids in neon pink or cyan receding to a vanishing point, evoking Tron and 80s music videos
- **Chrome and metallic lettering** -- reflective, gradient-filled text that appears to be made of polished metal
- **Silhouetted objects** -- sports cars (Lamborghini, DeLorean, Ferrari), palm trees, and cityscapes rendered as dark silhouettes against glowing skies
- **Electric neon outlines** -- thin, glowing neon lines in cyan, magenta, and purple tracing shapes and borders
- **Sun motif** -- a large, horizontally striped setting sun (often with scan-line gaps) is the iconic Synthwave symbol
- **Dark backgrounds** -- deep navy, purple, and black as the dominant canvas, pierced by vibrant neon
- **Retro-futuristic imagery** -- VHS tapes, cassettes, arcade cabinets, motorcycles, aviator sunglasses
- **Starfields and cosmic elements** -- distant stars, nebulae, and galaxies suggesting infinite space
- **1980s geometric patterns** -- chevrons, triangles, parallel lines, and diamond grids

### Design Principles

- Celebrate the 1980s unironically -- Synthwave is sincere nostalgia amplified to the mythic
- Build drama through contrast: dark backgrounds against vivid neon accents
- Use gradient skies as the primary visual motif -- the eternal sunset is the beating heart of Synthwave
- Create depth with perspective grids and vanishing-point compositions
- Chrome and metallic effects should feel polished and premium, never cheap
- Every composition should feel like it could be an album cover or movie poster
- Color transitions should be smooth and cinematic, never harsh
- Motion and speed are implied even in static designs -- diagonal lines, motion blur, perspective
- Keep the palette focused: sunset warm colors (orange, pink, magenta) + cool accents (cyan, purple)

---

## Color Palette

### Neon Sunset Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Horizon Orange** | `#FF6B35` | Sunset lower band, warm accents |
| **Neon Pink** | `#FF2E97` | Primary accent, CTAs, headings |
| **Hot Magenta** | `#FF006E` | Active states, emphasis, hover |
| **Laser Purple** | `#8B00FF` | Gradient midpoint, decorative accents |
| **Deep Violet** | `#4A0080` | Dark gradient end, deep backgrounds |
| **Electric Cyan** | `#00E5FF` | Secondary accent, links, interactive elements |
| **Neon Blue** | `#0066FF` | Tertiary accent, data elements |
| **Chrome Silver** | `#C0C0D0` | Metallic text, borders, dividers |
| **Chrome Highlight** | `#FFFFFF` | Chrome shine points, maximum brightness |
| **Midnight Navy** | `#0D0221` | Primary background, deepest layer |
| **Dark Purple** | `#150030` | Secondary background, elevated surfaces |
| **Twilight** | `#1A0940` | Card backgrounds, panel surfaces |
| **Neon Grid** | `#FF2E97` | Grid lines, structural overlays |
| **Starlight** | `#E0D0FF` | Primary text on dark backgrounds |
| **Muted Lavender** | `#7A6B8E` | Secondary text, captions |

### CSS Custom Properties

```css
:root {
  /* Warm neons */
  --synth-orange: #ff6b35;
  --synth-pink: #ff2e97;
  --synth-magenta: #ff006e;
  --synth-purple: #8b00ff;
  --synth-violet: #4a0080;

  /* Cool neons */
  --synth-cyan: #00e5ff;
  --synth-blue: #0066ff;

  /* Chrome */
  --synth-chrome: #c0c0d0;
  --synth-chrome-bright: #ffffff;

  /* Backgrounds */
  --synth-bg-midnight: #0d0221;
  --synth-bg-dark: #150030;
  --synth-bg-panel: #1a0940;

  /* Text */
  --synth-text-primary: #e0d0ff;
  --synth-text-secondary: #7a6b8e;

  /* Gradients */
  --synth-gradient-sunset: linear-gradient(180deg, #ff6b35 0%, #ff2e97 30%, #8b00ff 60%, #0d0221 100%);
  --synth-gradient-sky: linear-gradient(180deg, #4a0080 0%, #8b00ff 40%, #ff2e97 70%, #ff6b35 100%);
  --synth-gradient-chrome: linear-gradient(180deg, #ffffff 0%, #c0c0d0 40%, #606080 60%, #c0c0d0 80%, #ffffff 100%);

  /* Glows */
  --synth-glow-pink: 0 0 10px rgba(255, 46, 151, 0.5), 0 0 40px rgba(255, 46, 151, 0.2);
  --synth-glow-cyan: 0 0 10px rgba(0, 229, 255, 0.5), 0 0 40px rgba(0, 229, 255, 0.2);
}
```

---

## Typography

### Typeface Characteristics

Synthwave typography is:

- **Bold and dramatic** -- large-scale display text that dominates the composition like a movie title
- **Chrome and metallic styled** -- gradient fills that simulate polished metal or neon tube lighting
- **Uppercase and wide** -- all-caps with generous letter-spacing for cinematic impact
- **Retro-futuristic faces** -- geometric, wide, and slightly rounded, referencing 80s movie posters and album art
- **Italic for speed** -- slanted text implying motion and dynamism
- **Clean sans-serifs for body** -- readable body text that stays out of the way of dramatic headlines

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Orbitron** | Geometric, futuristic | Headlines, hero text, display |
| **Audiowide** | Wide, retro-futuristic | Logos, titles, branding text |
| **Righteous** | Rounded retro | Headlines, subheadings, 80s feel |
| **Bungee Shade** | 3D shadow display | Large display text, decorative headers |
| **Russo One** | Bold, wide, mechanical | Headlines, navigation, strong statements |
| **Exo 2** | Geometric, clean | Subheadings, body text, versatile |
| **Rajdhani** | Condensed, tech | Navigation, labels, data displays |
| **Outfit** | Modern geometric sans | Body text, readable content |
| **Quicksand** | Rounded geometric | Friendly body text, soft contrast |
| **Space Grotesk** | Geometric, contemporary | Body text, modern synthwave layouts |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Audiowide** (400) | **Outfit** (400) | Classic synthwave, album-cover drama |
| **Orbitron** (700) | **Exo 2** (400) | Futuristic, tech-forward |
| **Righteous** (400) | **Quicksand** (400) | Warm retro, approachable 80s |
| **Russo One** (400) | **Space Grotesk** (400) | Bold mechanical, clean body |
| **Bungee Shade** (400) | **Rajdhani** (400) | Maximum drama, condensed body |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Audiowide&family=Outfit:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Audiowide', cursive;
  font-weight: 400;
  color: var(--synth-text-primary);
  text-transform: uppercase;
  letter-spacing: 0.06em;
  line-height: 1.15;
}

/* Display / Hero text with chrome gradient */
.synth-display {
  font-family: 'Audiowide', cursive;
  font-size: clamp(3rem, 7vw, 6rem);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  background: var(--synth-gradient-chrome);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 0 20px rgba(255, 46, 151, 0.4));
}

/* Neon glow heading */
.synth-neon {
  font-family: 'Audiowide', cursive;
  color: var(--synth-pink);
  text-shadow:
    0 0 7px rgba(255, 46, 151, 0.8),
    0 0 20px rgba(255, 46, 151, 0.4),
    0 0 40px rgba(255, 46, 151, 0.2);
}

/* Body text */
body {
  font-family: 'Outfit', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--synth-text-primary);
}

/* Labels */
.synth-label {
  font-family: 'Audiowide', cursive;
  font-size: 0.7rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--synth-text-secondary);
}
```

---

## Layout Principles

### Grid and Structure

- **Full-bleed gradient backgrounds** -- sunset gradients span the entire viewport; no white borders or margins
- **Centered, medium-width containers** -- content at 1000-1200px max-width, letting the gradient sky show on sides
- **Perspective grid floors** -- the iconic receding grid dominates lower portions of hero sections
- **Vertical dramatic compositions** -- tall hero sections (80-100vh) with content centered in the upper third
- **Symmetrical layouts** -- centered headlines, centered CTAs, balanced grid columns
- **Layered depth** -- silhouetted foreground objects, midground content, background gradient sky
- **Strong horizontal bands** -- sections divided by gradient shifts rather than borders

### Section Organization

- **Navigation**: Transparent or semi-transparent bar with neon-accented links, glowing logo
- **Hero**: Full-viewport sunset gradient with chrome headline, perspective grid floor, silhouetted imagery
- **Features**: Dark background with neon-bordered cards or glowing icon grids
- **Content rows**: Dark panels with neon accent borders, text + visual side by side
- **Stats/Metrics**: Large chrome-styled numbers with glowing accents
- **CTA section**: Gradient band with centered neon text and glowing button
- **Footer**: Deepest dark background with muted text and subtle neon divider

### Responsive Approach

- Maintain gradient backgrounds at all breakpoints -- they are essential to the aesthetic
- Reduce perspective grid complexity on mobile but keep the visual suggestion
- Scale chrome/display text aggressively with `clamp()` for mobile
- Stack feature cards vertically; maintain neon border styling
- Simplify glow effects on mobile to preserve performance

---

## CSS / Design Techniques

### Synthwave Card Component

```css
.synth-card {
  background: rgba(26, 9, 64, 0.7);
  border: 1px solid rgba(255, 46, 151, 0.2);
  border-radius: 4px;
  padding: 32px;
  position: relative;
  transition: border-color 0.3s, box-shadow 0.3s;
}

.synth-card:hover {
  border-color: rgba(255, 46, 151, 0.5);
  box-shadow: var(--synth-glow-pink);
}

/* Top accent line */
.synth-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: linear-gradient(90deg, var(--synth-cyan), var(--synth-pink), var(--synth-purple));
}

/* Card grid */
.synth-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
}
```

### Synthwave Button

```css
.synth-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: transparent;
  color: var(--synth-pink);
  border: 2px solid var(--synth-pink);
  border-radius: 4px;
  padding: 14px 40px;
  font-family: 'Audiowide', cursive;
  font-size: 0.85rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
}

.synth-button:hover {
  background: var(--synth-pink);
  color: var(--synth-bg-midnight);
  box-shadow: var(--synth-glow-pink);
}

/* Cyan variant */
.synth-button--cyan {
  color: var(--synth-cyan);
  border-color: var(--synth-cyan);
}

.synth-button--cyan:hover {
  background: var(--synth-cyan);
  color: var(--synth-bg-midnight);
  box-shadow: var(--synth-glow-cyan);
}

/* Filled gradient variant */
.synth-button--filled {
  background: linear-gradient(135deg, var(--synth-pink), var(--synth-purple));
  color: #ffffff;
  border: none;
}

.synth-button--filled:hover {
  box-shadow: var(--synth-glow-pink);
  filter: brightness(1.15);
}
```

### Navigation Bar

```css
.synth-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  position: relative;
  z-index: 10;
}

.synth-nav__logo {
  font-family: 'Audiowide', cursive;
  font-size: 1.3rem;
  color: var(--synth-pink);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  text-shadow: 0 0 10px rgba(255, 46, 151, 0.5);
}

.synth-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.synth-nav__links a {
  font-family: 'Outfit', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--synth-text-secondary);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  transition: color 0.2s, text-shadow 0.2s;
}

.synth-nav__links a:hover {
  color: var(--synth-cyan);
  text-shadow: 0 0 8px rgba(0, 229, 255, 0.4);
}
```

### Hero Section with Sunset and Grid

```css
.synth-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 40px;
  background: var(--synth-gradient-sunset);
  overflow: hidden;
}

/* Striped sun */
.synth-hero__sun {
  position: absolute;
  bottom: 30%;
  left: 50%;
  transform: translateX(-50%);
  width: 300px;
  height: 300px;
  border-radius: 50%;
  background: linear-gradient(180deg, #ff6b35 0%, #ff2e97 50%, #8b00ff 100%);
  mask-image: repeating-linear-gradient(
    0deg,
    #000 0px,
    #000 8px,
    transparent 8px,
    transparent 12px
  );
  -webkit-mask-image: repeating-linear-gradient(
    0deg,
    #000 0px,
    #000 8px,
    transparent 8px,
    transparent 12px
  );
  z-index: 1;
}

/* Perspective grid */
.synth-hero__grid {
  position: absolute;
  bottom: 0;
  left: -20%;
  right: -20%;
  height: 40%;
  background:
    repeating-linear-gradient(90deg, transparent, transparent 79px, rgba(255, 46, 151, 0.3) 79px, rgba(255, 46, 151, 0.3) 80px),
    repeating-linear-gradient(0deg, transparent, transparent 79px, rgba(255, 46, 151, 0.3) 79px, rgba(255, 46, 151, 0.3) 80px);
  transform: perspective(500px) rotateX(50deg);
  transform-origin: bottom;
  z-index: 1;
}

.synth-hero__content {
  position: relative;
  z-index: 5;
  max-width: 800px;
}

.synth-hero__content h1 {
  font-size: clamp(3rem, 7vw, 6rem);
  margin-bottom: 1.5rem;
  background: var(--synth-gradient-chrome);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 0 20px rgba(255, 46, 151, 0.3));
}

.synth-hero__content p {
  font-size: 1.15rem;
  color: rgba(224, 208, 255, 0.8);
  margin-bottom: 2.5rem;
}

@media (max-width: 768px) {
  .synth-hero { min-height: auto; padding: 60px 20px; }
  .synth-hero__sun { width: 180px; height: 180px; }
}
```

### Chrome Text Effect

```css
.synth-chrome {
  font-family: 'Audiowide', cursive;
  text-transform: uppercase;
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #d0d0e0 20%,
    #808098 40%,
    #d0d0e0 50%,
    #ffffff 60%,
    #a0a0b8 80%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

### Neon Line Divider

```css
.synth-divider {
  border: none;
  height: 2px;
  background: linear-gradient(90deg,
    transparent 0%,
    var(--synth-cyan) 20%,
    var(--synth-pink) 50%,
    var(--synth-purple) 80%,
    transparent 100%
  );
  margin: 60px 0;
  box-shadow: 0 0 8px rgba(255, 46, 151, 0.3);
}
```

### Stat / Metric Display

```css
.synth-stat {
  text-align: center;
  padding: 24px;
}

.synth-stat__number {
  font-family: 'Audiowide', cursive;
  font-size: 3rem;
  background: var(--synth-gradient-chrome);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  line-height: 1.1;
  margin-bottom: 8px;
}

.synth-stat__label {
  font-family: 'Outfit', sans-serif;
  font-size: 0.85rem;
  color: var(--synth-text-secondary);
  text-transform: uppercase;
  letter-spacing: 0.12em;
}
```

---

## Design Do's and Don'ts

### Do

- Use dramatic sunset gradients (orange-to-pink-to-purple-to-dark) as hero backgrounds
- Apply chrome/metallic gradient effects to headlines using `background-clip: text`
- Include the iconic striped sun motif in hero sections
- Add perspective grid floors that recede toward the horizon
- Use neon glow effects (`text-shadow`, `box-shadow`) on interactive elements
- Maintain a dark canvas (navy, deep purple) for non-gradient sections
- Keep typography bold, wide, uppercase, and cinematic
- Reference 80s visual culture: sports cars, palm trees, geometric patterns, starfields

### Don't

- Use pastel, washed-out colors -- Synthwave is vivid and high-contrast (distinguish from Vaporwave)
- Apply ironic or deconstructive treatments -- Synthwave celebrates the 80s sincerely
- Use light/white backgrounds -- the aesthetic requires darkness for neon to shine
- Mix too many neon colors in one area -- maintain the sunset warm-to-cool gradient logic
- Use serif or handwritten typefaces -- stick to geometric sans-serifs and display faces
- Over-complicate layouts -- Synthwave compositions are bold and simple, like movie posters
- Forget the sense of depth and perspective -- flat layouts miss the cinematic quality
- Add VHS degradation or glitch effects -- those belong to Vaporwave, not Synthwave

---

## Related Aesthetics

| Aesthetic | Relationship to Synthwave |
|-----------|--------------------------|
| **Vaporwave** | Both reference 80s/90s nostalgia, but Synthwave is sincere and cinematic while Vaporwave is ironic and deconstructive |
| **Cyberpunk** | Shares the neon-on-dark palette; Cyberpunk is dystopian and gritty, Synthwave is glamorous and aspirational |
| **Outrun** | A direct visual sub-genre of Synthwave; specifically focused on driving, speed, and sports car imagery |
| **Retrowave** | Often used interchangeably with Synthwave; may emphasize the music scene more than the visual aesthetic |
| **RGB Gamer** | Shares neon LED lighting; RGB Gamer is more about hardware and performance culture |
| **Silicon Dreams** | Shares retro-futuristic digital themes but with a more corporate, utopian tone |
| **Space Age** | Both imagine futuristic visions; Space Age references 1960s NASA optimism, Synthwave references 1980s pop culture |
| **Chromecore** | Shares the metallic/chrome visual treatment; Chromecore is broader and not era-specific |
| **8-Bit** | Both reference retro technology; 8-Bit focuses on pixel art and gaming, Synthwave on cinematic glamour |

---

## Quick-Start: Minimal Synthwave Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Synthwave Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Audiowide&family=Outfit:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --synth-orange: #ff6b35;
      --synth-pink: #ff2e97;
      --synth-magenta: #ff006e;
      --synth-purple: #8b00ff;
      --synth-violet: #4a0080;
      --synth-cyan: #00e5ff;
      --synth-bg-midnight: #0d0221;
      --synth-bg-panel: #1a0940;
      --synth-text-primary: #e0d0ff;
      --synth-text-secondary: #7a6b8e;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--synth-bg-midnight);
      color: var(--synth-text-primary);
      font-family: 'Outfit', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Audiowide', cursive;
      font-weight: 400;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      line-height: 1.15;
    }

    /* Navigation */
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
      font-family: 'Audiowide', cursive;
      font-size: 1.2rem;
      color: var(--synth-pink);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      text-shadow: 0 0 10px rgba(255, 46, 151, 0.5);
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'Outfit', sans-serif;
      font-weight: 500;
      font-size: 0.9rem;
      color: var(--synth-text-secondary);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      transition: color 0.2s, text-shadow 0.2s;
    }

    nav ul a:hover {
      color: var(--synth-cyan);
      text-shadow: 0 0 8px rgba(0, 229, 255, 0.4);
    }

    /* Hero */
    .hero {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 90vh;
      padding: 80px 40px;
      background: linear-gradient(180deg, #ff6b35 0%, #ff2e97 25%, #8b00ff 50%, #150030 75%, #0d0221 100%);
      overflow: hidden;
    }

    /* Striped sun */
    .sun {
      position: absolute;
      bottom: 32%;
      left: 50%;
      transform: translateX(-50%);
      width: 280px;
      height: 280px;
      border-radius: 50%;
      background: linear-gradient(180deg, #ff6b35, #ff2e97, #8b00ff);
      -webkit-mask-image: repeating-linear-gradient(0deg, #000 0px, #000 8px, transparent 8px, transparent 13px);
      mask-image: repeating-linear-gradient(0deg, #000 0px, #000 8px, transparent 8px, transparent 13px);
      z-index: 1;
    }

    /* Grid floor */
    .grid-floor {
      position: absolute;
      bottom: 0; left: -20%; right: -20%; height: 38%;
      background:
        repeating-linear-gradient(90deg, transparent, transparent 79px, rgba(255, 46, 151, 0.3) 79px, rgba(255, 46, 151, 0.3) 80px),
        repeating-linear-gradient(0deg, transparent, transparent 79px, rgba(255, 46, 151, 0.3) 79px, rgba(255, 46, 151, 0.3) 80px);
      transform: perspective(500px) rotateX(50deg);
      transform-origin: bottom;
      z-index: 1;
    }

    .hero-content { position: relative; z-index: 5; max-width: 800px; }

    .hero h1 {
      font-size: clamp(2.5rem, 7vw, 5.5rem);
      margin-bottom: 1.5rem;
      background: linear-gradient(180deg, #fff 0%, #c0c0d0 40%, #808098 55%, #c0c0d0 70%, #fff 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      filter: drop-shadow(0 0 20px rgba(255, 46, 151, 0.3));
    }

    .hero p {
      font-size: 1.1rem;
      color: rgba(224, 208, 255, 0.75);
      margin-bottom: 2.5rem;
    }

    .btn {
      display: inline-block;
      background: transparent;
      color: var(--synth-pink);
      border: 2px solid var(--synth-pink);
      border-radius: 4px;
      padding: 14px 40px;
      font-family: 'Audiowide', cursive;
      font-size: 0.85rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.3s;
    }

    .btn:hover {
      background: var(--synth-pink);
      color: var(--synth-bg-midnight);
      box-shadow: 0 0 10px rgba(255, 46, 151, 0.5), 0 0 40px rgba(255, 46, 151, 0.2);
    }

    /* Features */
    .features {
      padding: 80px 0;
      background: var(--synth-bg-midnight);
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--synth-cyan);
      text-shadow: 0 0 10px rgba(0, 229, 255, 0.3);
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: rgba(26, 9, 64, 0.6);
      border: 1px solid rgba(255, 46, 151, 0.15);
      border-radius: 4px;
      padding: 32px;
      position: relative;
      transition: border-color 0.3s, box-shadow 0.3s;
    }

    .feature::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 2px;
      background: linear-gradient(90deg, var(--synth-cyan), var(--synth-pink), var(--synth-purple));
    }

    .feature:hover {
      border-color: rgba(255, 46, 151, 0.4);
      box-shadow: 0 0 10px rgba(255, 46, 151, 0.15);
    }

    .feature h3 { font-size: 1rem; margin-bottom: 0.75rem; }
    .feature p { color: var(--synth-text-secondary); font-size: 0.95rem; }

    /* CTA */
    .cta {
      text-align: center;
      padding: 80px 40px;
      background: linear-gradient(180deg, var(--synth-bg-midnight), #1a0940);
    }

    .cta h2 {
      font-size: 2rem;
      color: var(--synth-pink);
      text-shadow: 0 0 15px rgba(255, 46, 151, 0.4);
      margin-bottom: 1rem;
    }

    .cta p {
      color: var(--synth-text-secondary);
      margin-bottom: 2rem;
    }

    /* Neon divider */
    .divider {
      border: none; height: 2px;
      background: linear-gradient(90deg, transparent 0%, var(--synth-cyan) 20%, var(--synth-pink) 50%, var(--synth-purple) 80%, transparent 100%);
      max-width: 1200px;
      margin: 0 auto;
      box-shadow: 0 0 8px rgba(255, 46, 151, 0.3);
    }

    /* Footer */
    footer {
      background: #080015;
      text-align: center;
      padding: 30px 40px;
      color: var(--synth-text-secondary);
      font-size: 0.85rem;
    }

    @media (max-width: 768px) {
      .hero { min-height: auto; padding: 60px 20px; }
      .sun { width: 160px; height: 160px; }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Turbo</a>
    <ul>
      <li><a href="#">Drive</a></li>
      <li><a href="#">Tracks</a></li>
      <li><a href="#">Neon</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="sun"></div>
    <div class="grid-floor"></div>
    <div class="hero-content">
      <h1>Midnight Drive</h1>
      <p>Accelerate through the neon-lit corridors of a city that never sleeps. The horizon calls.</p>
      <a href="#" class="btn">Ignite</a>
    </div>
  </section>

  <hr class="divider">

  <section class="features">
    <h2>Specifications</h2>
    <div class="features-grid">
      <div class="feature">
        <h3>Turbo Core</h3>
        <p>Twin-turbocharged processing with neon-cooled heatsinks. Maximum velocity is not optional, it is the baseline.</p>
      </div>
      <div class="feature">
        <h3>Chrome Armor</h3>
        <p>Polished metallic defense layers that reflect every threat. Style and substance forged in the same crucible.</p>
      </div>
      <div class="feature">
        <h3>Night Vision</h3>
        <p>Enhanced optics for navigating the grid after dark. See the data streams that others miss entirely.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Chase the horizon</h2>
    <p>The sunset never ends. The grid stretches forever. The only question is how fast you want to go.</p>
    <a href="#" class="btn">Launch</a>
  </section>

  <footer>
    <p>TURBO SYSTEMS // Forged in the neon glow of an endless 1985</p>
  </footer>
</body>
</html>
```
