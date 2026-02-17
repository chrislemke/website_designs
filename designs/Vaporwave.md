# Vaporwave Design Reference

Vaporwave is a glitched 90s nostalgia aesthetic born from internet culture in the early 2010s. It appropriates and distorts imagery from late-capitalist consumer culture -- Greek statuary, early Windows operating systems, Japanese text, shopping mall architecture, and corporate clip art -- filtering everything through a pastel pink-and-teal haze. The visual language is deliberately lo-fi, ironic, and surreal, combining VHS tracking errors with marble busts, palm trees, and obsolete technology. In web design, Vaporwave translates to pastel gradient backgrounds, retro UI chrome, grid overlays, glitch distortion, and a tone that hovers between sincere nostalgia and subversive parody.

---

## Visual Characteristics

### Core Design Traits

- **Pastel pink and teal color dominance** -- soft, washed-out gradients that evoke faded VHS tapes and early computer displays
- **Greek and Roman statuary** -- busts, columns, and classical sculptures used ironically as decorative motifs
- **Japanese text accents** -- katakana, hiragana, or kanji characters used decoratively, referencing 90s Japanese consumer culture
- **Windows 95/98 UI elements** -- retro dialog boxes, title bars, scrollbars, and system fonts
- **Checkerboard and perspective grids** -- wireframe floors and tiled patterns suggesting early 3D rendering
- **Palm trees and tropical plants** -- synthetic, oversaturated tropical imagery evoking 80s/90s leisure culture
- **VHS and glitch artifacts** -- tracking errors, chromatic aberration, scan lines, and RGB color separation
- **Marble and faux-luxury textures** -- pink marble, chrome surfaces, and fake opulence
- **Dolphins, sunsets, and water imagery** -- serene, dreamy motifs from stock photography and screensavers
- **Corporate clip art and logos** -- repurposed, distorted commercial imagery from the early internet era

### Design Principles

- Embrace irony and ambiguity -- Vaporwave is simultaneously nostalgic and critical of consumer culture
- Layer disparate cultural elements: classical sculpture + digital glitch + corporate branding + Japanese text
- Use soft, low-contrast pastel palettes rather than harsh neon (distinguish from Cyberpunk)
- Distort and degrade images intentionally -- compression artifacts and color shifts are features, not bugs
- Reference obsolete technology aesthetics: early Macintosh, Windows 95, dial-up internet, CD-ROMs
- Typography can be deliberately "wrong" -- stretched, compressed, or set in inappropriate system fonts
- Negative space and emptiness evoke the lonely, surreal atmosphere of an abandoned digital mall
- The overall mood should feel dreamy, melancholic, and slightly unsettling

---

## Color Palette

### Vaporwave Classic Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Pastel Pink** | `#FF71CE` | Primary accent, headlines, key interactive elements |
| **Soft Rose** | `#FFB3D9` | Light backgrounds, card surfaces, secondary accent |
| **Hot Pink** | `#E50086` | Hover states, active elements, emphasis |
| **Aqua Teal** | `#01CDFE` | Secondary accent, links, interactive elements |
| **Mint Dream** | `#05FFA1` | Success states, tertiary accent |
| **Lavender Haze** | `#B967FF` | Decorative accent, tags, badges |
| **Deep Violet** | `#6B2FA0` | Dark accent, text on light backgrounds |
| **Sunset Orange** | `#FFA86A` | Warm accent, highlights |
| **VHS White** | `#FFFBFC` | Primary text on dark backgrounds, clean surfaces |
| **Faded Cream** | `#F5E6F0` | Light page backgrounds, subtle surfaces |
| **CRT Dark** | `#1A0A2E` | Dark backgrounds, footer, contrast sections |
| **Grid Purple** | `#2D1B4E` | Dark panels, overlay backgrounds |
| **Marble Gray** | `#C4B7C9` | Borders, muted elements, captions |
| **Static** | `#8B7E96` | Secondary text, disabled states |

### CSS Custom Properties

```css
:root {
  /* Primary palette */
  --vapor-pink: #ff71ce;
  --vapor-soft-rose: #ffb3d9;
  --vapor-hot-pink: #e50086;
  --vapor-teal: #01cdfe;
  --vapor-mint: #05ffa1;
  --vapor-lavender: #b967ff;
  --vapor-violet: #6b2fa0;
  --vapor-orange: #ffa86a;

  /* Backgrounds */
  --vapor-bg-light: #f5e6f0;
  --vapor-bg-cream: #fffbfc;
  --vapor-bg-dark: #1a0a2e;
  --vapor-bg-panel: #2d1b4e;

  /* Text */
  --vapor-text-dark: #2d1b4e;
  --vapor-text-light: #fffbfc;
  --vapor-text-muted: #8b7e96;

  /* Gradients */
  --vapor-gradient-sky: linear-gradient(135deg, #ff71ce 0%, #01cdfe 50%, #b967ff 100%);
  --vapor-gradient-sunset: linear-gradient(180deg, #ff71ce 0%, #ffa86a 50%, #b967ff 100%);
  --vapor-gradient-soft: linear-gradient(135deg, #f5e6f0 0%, #e8d5f5 50%, #d5e8f5 100%);
}
```

---

## Typography

### Typeface Characteristics

Vaporwave typography is:

- **Deliberately eclectic** -- mixing system fonts, pixel fonts, and wide geometric faces in unexpected ways
- **Often stretched or compressed** -- horizontal scaling distorts letterforms for surreal effect
- **Full-width or spaced-out** -- extreme letter-spacing creates a dreamy, disconnected feeling
- **Japanese text mixed with Latin** -- decorative use of CJK characters alongside English
- **Retro system font references** -- Chicago, MS Sans Serif, Arial aesthetic recalling 90s operating systems
- **All-caps for display text** -- uppercase headlines with maximum letter-spacing

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **VT323** | Pixel/CRT monospace | Retro UI elements, terminal text, system dialogs |
| **Press Start 2P** | Pixel art, 8-bit | Decorative headlines, game-style elements |
| **Libre Barcode 39** | Barcode font | Decorative barcode accents |
| **Zen Maru Gothic** | Japanese rounded gothic | Japanese text accents, CJK elements |
| **Noto Sans JP** | Japanese sans-serif | Japanese text body, labels |
| **Monoton** | Retro outline display | Large display headlines, hero text |
| **Bungee** | Chromatic display | Bold headlines, sign-style text |
| **DM Sans** | Clean geometric sans | Body text, readable content sections |
| **Space Grotesk** | Geometric, wide | Subheadings, navigation, modern contrast |
| **Silkscreen** | Pixel bitmap | Small labels, pixel-art UI chrome |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Monoton** (400) | **DM Sans** (400) | Classic vaporwave, retro display + clean body |
| **Bungee** (400) | **Space Grotesk** (400) | Bold chromatic headers, geometric body |
| **VT323** (400) | **DM Sans** (400) | CRT terminal heading, clean body contrast |
| **Press Start 2P** (400) | **VT323** (400) | Full retro pixel aesthetic |
| **Space Grotesk** (700) | **Noto Sans JP** (400) | Modern + Japanese text integration |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Monoton&family=DM+Sans:wght@400;500;700&family=VT323&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  color: var(--vapor-text-dark);
  line-height: 1.2;
}

/* Display / Hero text */
.vapor-display {
  font-family: 'Monoton', cursive;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 400;
  letter-spacing: 0.06em;
  color: var(--vapor-pink);
  text-shadow: 3px 3px 0 var(--vapor-teal), -1px -1px 0 var(--vapor-lavender);
}

/* Spaced-out subtitle */
.vapor-subtitle {
  font-family: 'DM Sans', sans-serif;
  font-weight: 500;
  font-size: 1rem;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  color: var(--vapor-text-muted);
}

/* Body text */
body {
  font-family: 'DM Sans', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--vapor-text-dark);
}

/* CRT / retro text */
.vapor-crt {
  font-family: 'VT323', monospace;
  font-size: 1.1rem;
  color: var(--vapor-mint);
  text-shadow: 0 0 5px rgba(5, 255, 161, 0.5);
}

/* Japanese accent text */
.vapor-jp {
  font-family: 'Noto Sans JP', sans-serif;
  font-size: 0.85rem;
  color: var(--vapor-text-muted);
  letter-spacing: 0.2em;
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, medium-width containers** -- 900-1100px max-width; generous padding for a spacious, empty feeling
- **Perspective grid backgrounds** -- wireframe grids receding to a vanishing point, referencing early 3D software
- **Retro window/dialog layouts** -- content wrapped in faux Windows 95 title bars and borders
- **Asymmetric, collage-style arrangements** -- elements placed somewhat randomly, like a surreal digital collage
- **Gradient backgrounds** -- full-bleed pastel gradients (pink-to-teal, pink-to-purple) behind content
- **Wide letter-spacing in headers** -- text expands across the width, filling horizontal space dreamily
- **Floating decorative elements** -- statues, palm trees, and geometric shapes positioned as background accents

### Section Organization

- **Navigation**: Retro-styled top bar mimicking Windows 95 title bar, or minimal text links with extreme spacing
- **Hero**: Large gradient background with Monoton/display headline, floating decorative imagery
- **Content cards**: Rounded or retro-framed cards on soft gradient or marble-textured backgrounds
- **Gallery**: Collage grid of distorted images with VHS tracking overlays
- **Quote/Text blocks**: Wide letter-spaced text centered on pastel backgrounds
- **CTA section**: Gradient background with retro button styling
- **Footer**: Dark purple/navy, Japanese text accents, pixel font

### Responsive Approach

- Maintain pastel gradient backgrounds across all breakpoints
- Reduce floating decorative elements on mobile to avoid clutter
- Stack collage-style layouts into single columns on small screens
- Preserve letter-spacing on headlines but reduce font size
- Retro dialog-box UI elements remain but shrink to fit mobile widths

---

## CSS / Design Techniques

### Vaporwave Card Component

```css
.vapor-card {
  background: rgba(255, 255, 255, 0.7);
  border: 2px solid var(--vapor-pink);
  border-radius: 0;
  padding: 28px;
  position: relative;
  backdrop-filter: blur(8px);
}

/* Retro title bar */
.vapor-card__titlebar {
  display: flex;
  align-items: center;
  gap: 6px;
  background: linear-gradient(90deg, var(--vapor-pink), var(--vapor-lavender));
  margin: -28px -28px 20px -28px;
  padding: 6px 10px;
  font-family: 'VT323', monospace;
  font-size: 0.9rem;
  color: white;
}

.vapor-card__titlebar-dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  border: 1px solid rgba(255, 255, 255, 0.6);
}

/* Card grid */
.vapor-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
}
```

### Vaporwave Button

```css
.vapor-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--vapor-gradient-sky);
  color: #ffffff;
  border: none;
  border-radius: 0;
  padding: 14px 36px;
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  font-size: 0.9rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  cursor: pointer;
  transition: transform 0.2s, box-shadow 0.2s;
  box-shadow: 4px 4px 0 var(--vapor-violet);
}

.vapor-button:hover {
  transform: translate(-2px, -2px);
  box-shadow: 6px 6px 0 var(--vapor-violet);
}

.vapor-button:active {
  transform: translate(2px, 2px);
  box-shadow: 2px 2px 0 var(--vapor-violet);
}

/* Retro outline variant */
.vapor-button--retro {
  background: transparent;
  color: var(--vapor-pink);
  border: 2px solid var(--vapor-pink);
  box-shadow: 3px 3px 0 var(--vapor-teal);
  font-family: 'VT323', monospace;
  font-size: 1.1rem;
  letter-spacing: 0.06em;
}

.vapor-button--retro:hover {
  background: var(--vapor-pink);
  color: white;
}
```

### Navigation Bar

```css
.vapor-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1100px;
  margin: 0 auto;
  padding: 20px 40px;
}

.vapor-nav__logo {
  font-family: 'Monoton', cursive;
  font-size: 1.5rem;
  color: var(--vapor-pink);
  text-decoration: none;
  text-shadow: 2px 2px 0 var(--vapor-teal);
}

.vapor-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.vapor-nav__links a {
  font-family: 'DM Sans', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--vapor-text-muted);
  text-decoration: none;
  transition: color 0.2s;
}

.vapor-nav__links a:hover {
  color: var(--vapor-pink);
}
```

### Hero Section

```css
.vapor-hero {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  min-height: 80vh;
  padding: 80px 40px;
  background: var(--vapor-gradient-sunset);
  position: relative;
  overflow: hidden;
}

/* Perspective grid floor */
.vapor-hero::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: -20%;
  right: -20%;
  height: 45%;
  background:
    repeating-linear-gradient(90deg, transparent, transparent 59px, rgba(255, 113, 206, 0.25) 59px, rgba(255, 113, 206, 0.25) 60px),
    repeating-linear-gradient(0deg, transparent, transparent 59px, rgba(255, 113, 206, 0.25) 59px, rgba(255, 113, 206, 0.25) 60px);
  transform: perspective(400px) rotateX(55deg);
  transform-origin: bottom;
  pointer-events: none;
}

.vapor-hero__content {
  position: relative;
  z-index: 2;
  max-width: 700px;
}

.vapor-hero__content h1 {
  font-family: 'Monoton', cursive;
  font-size: clamp(2.5rem, 6vw, 5rem);
  color: #ffffff;
  text-shadow: 3px 3px 0 var(--vapor-teal), 6px 6px 0 rgba(107, 47, 160, 0.3);
  margin-bottom: 1.5rem;
}

.vapor-hero__content p {
  font-family: 'DM Sans', sans-serif;
  font-size: 1.1rem;
  color: rgba(255, 255, 255, 0.85);
  letter-spacing: 0.15em;
  margin-bottom: 2.5rem;
}

@media (max-width: 768px) {
  .vapor-hero { min-height: auto; padding: 60px 20px; }
}
```

### VHS Glitch Overlay

```css
@keyframes vapor-tracking {
  0% { transform: translateX(0); opacity: 0; }
  10% { transform: translateX(-5px); opacity: 1; }
  12% { transform: translateX(3px); opacity: 1; }
  14% { transform: translateX(0); opacity: 0; }
  100% { transform: translateX(0); opacity: 0; }
}

.vapor-vhs {
  position: relative;
  overflow: hidden;
}

.vapor-vhs::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 3px,
    rgba(255, 113, 206, 0.03) 3px,
    rgba(255, 113, 206, 0.03) 6px
  );
  pointer-events: none;
}

.vapor-vhs::after {
  content: '';
  position: absolute;
  left: 0;
  right: 0;
  height: 4px;
  background: rgba(255, 113, 206, 0.3);
  animation: vapor-tracking 8s infinite;
  pointer-events: none;
}
```

### Retro Window Component

```css
.vapor-window {
  border: 2px solid var(--vapor-violet);
  background: var(--vapor-bg-cream);
  max-width: 500px;
}

.vapor-window__titlebar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: linear-gradient(90deg, var(--vapor-violet), var(--vapor-pink));
  padding: 4px 8px;
  font-family: 'VT323', monospace;
  font-size: 0.85rem;
  color: white;
}

.vapor-window__controls {
  display: flex;
  gap: 4px;
}

.vapor-window__controls span {
  display: inline-block;
  width: 12px;
  height: 12px;
  border: 1px solid rgba(255, 255, 255, 0.5);
  font-size: 8px;
  text-align: center;
  line-height: 10px;
}

.vapor-window__body {
  padding: 20px;
}
```

---

## Design Do's and Don'ts

### Do

- Use pastel pink-to-teal gradients as the foundational color story
- Reference 90s digital culture: Windows 95 UI, early web graphics, clip art
- Include Japanese text as decorative accents (with cultural awareness)
- Apply VHS tracking lines, scan lines, and chromatic aberration effects subtly
- Use extremely wide letter-spacing on display text for a dreamy, spaced-out feeling
- Mix classical imagery (Greek busts, columns) with digital glitch for surreal contrast
- Incorporate retro UI elements: dialog boxes, pixel scroll bars, system fonts
- Maintain a tone that balances nostalgia with irony

### Don't

- Use dark, high-contrast neon-on-black palettes (that is Cyberpunk, not Vaporwave)
- Make the aesthetic too clean or polished -- some visual "degradation" is essential
- Use modern, minimalist UI patterns -- the whole point is referencing outdated interfaces
- Overload with too many competing elements -- Vaporwave has a sense of emptiness and loneliness
- Use aggressive, angular shapes -- favor soft gradients, curves, and gentle geometry
- Forget the ironic distance -- Vaporwave is not sincere celebration of 90s consumerism
- Use serif or script typefaces -- stick to system fonts, pixel fonts, and geometric sans-serifs
- Apply the aesthetic randomly -- the clash of elements should feel curated, not chaotic

---

## Related Aesthetics

| Aesthetic | Relationship to Vaporwave |
|-----------|--------------------------|
| **Synthwave** | Shares 80s nostalgia and neon colors, but Synthwave is more earnest, action-oriented, and music-driven; Vaporwave is ironic and melancholic |
| **Cyberpunk** | Both reference technology culture, but Cyberpunk is dark and dystopian while Vaporwave is pastel and surreal |
| **Y2K Futurism** | Overlaps in late-90s digital aesthetics (chrome, translucency), but Y2K is optimistic while Vaporwave is nostalgic |
| **8-Bit** | Both use pixel art and retro technology references; 8-Bit is more game-focused and playful |
| **Liminal Space** | Shares the eerie, empty, nostalgic quality of abandoned digital and physical spaces |
| **Poolcore** | Shares the still-water, tiled-surface, liminal-space imagery and the pastel-blue palette |
| **Frutiger Aero** | The sincere, corporate version of the same late-90s/early-2000s digital aesthetic that Vaporwave deconstructs |
| **Seapunk** | Direct sibling aesthetic; shares the teal/aqua palette and aquatic imagery, more ocean-focused |
| **Webcore** | Both celebrate early internet aesthetics; Webcore is broader, Vaporwave is more specific in its cultural critique |

---

## Quick-Start: Minimal Vaporwave Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vaporwave Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Monoton&family=DM+Sans:wght@400;500;700&family=VT323&display=swap" rel="stylesheet">
  <style>
    :root {
      --vapor-pink: #ff71ce;
      --vapor-soft-rose: #ffb3d9;
      --vapor-hot-pink: #e50086;
      --vapor-teal: #01cdfe;
      --vapor-mint: #05ffa1;
      --vapor-lavender: #b967ff;
      --vapor-violet: #6b2fa0;
      --vapor-orange: #ffa86a;
      --vapor-bg-light: #f5e6f0;
      --vapor-bg-dark: #1a0a2e;
      --vapor-text-dark: #2d1b4e;
      --vapor-text-muted: #8b7e96;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--vapor-bg-light);
      color: var(--vapor-text-dark);
      font-family: 'DM Sans', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'DM Sans', sans-serif;
      font-weight: 700;
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1100px;
      margin: 0 auto;
      padding: 20px 40px;
    }

    nav a.logo {
      font-family: 'Monoton', cursive;
      font-size: 1.4rem;
      color: var(--vapor-pink);
      text-decoration: none;
      text-shadow: 2px 2px 0 var(--vapor-teal);
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'DM Sans', sans-serif;
      font-weight: 500;
      font-size: 0.85rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--vapor-text-muted);
      text-decoration: none;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--vapor-pink); }

    /* Hero */
    .hero {
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 75vh;
      padding: 80px 40px;
      background: linear-gradient(180deg, #ff71ce 0%, #ffa86a 40%, #b967ff 100%);
      position: relative;
      overflow: hidden;
    }

    /* Grid floor */
    .hero::after {
      content: '';
      position: absolute;
      bottom: 0; left: -20%; right: -20%; height: 45%;
      background:
        repeating-linear-gradient(90deg, transparent, transparent 59px, rgba(255,255,255,0.2) 59px, rgba(255,255,255,0.2) 60px),
        repeating-linear-gradient(0deg, transparent, transparent 59px, rgba(255,255,255,0.2) 59px, rgba(255,255,255,0.2) 60px);
      transform: perspective(400px) rotateX(55deg);
      transform-origin: bottom;
      pointer-events: none;
    }

    .hero-content { position: relative; z-index: 2; max-width: 700px; }

    .hero h1 {
      font-family: 'Monoton', cursive;
      font-size: clamp(2.5rem, 6vw, 5rem);
      font-weight: 400;
      color: #fff;
      text-shadow: 3px 3px 0 var(--vapor-teal), 6px 6px 0 rgba(107, 47, 160, 0.3);
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1rem;
      color: rgba(255, 255, 255, 0.85);
      letter-spacing: 0.15em;
      margin-bottom: 2.5rem;
    }

    .btn {
      display: inline-block;
      background: linear-gradient(135deg, var(--vapor-pink), var(--vapor-teal), var(--vapor-lavender));
      color: #fff;
      border: none;
      padding: 14px 36px;
      font-family: 'DM Sans', sans-serif;
      font-weight: 700;
      font-size: 0.9rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 4px 4px 0 var(--vapor-violet);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .btn:hover {
      transform: translate(-2px, -2px);
      box-shadow: 6px 6px 0 var(--vapor-violet);
    }

    /* Features */
    .features {
      padding: 80px 0;
      background: var(--vapor-bg-light);
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--vapor-violet);
      margin-bottom: 8px;
    }

    .features .subtitle {
      text-align: center;
      font-size: 0.85rem;
      letter-spacing: 0.3em;
      text-transform: uppercase;
      color: var(--vapor-text-muted);
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: rgba(255, 255, 255, 0.7);
      border: 2px solid var(--vapor-pink);
      padding: 0;
      backdrop-filter: blur(6px);
    }

    .feature-titlebar {
      background: linear-gradient(90deg, var(--vapor-pink), var(--vapor-lavender));
      padding: 5px 10px;
      font-family: 'VT323', monospace;
      font-size: 0.85rem;
      color: white;
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .feature-titlebar .dot {
      width: 8px; height: 8px;
      border-radius: 50%;
      border: 1px solid rgba(255,255,255,0.6);
    }

    .feature-body { padding: 24px; }
    .feature h3 { font-size: 1.1rem; margin-bottom: 0.5rem; color: var(--vapor-violet); }
    .feature p { color: var(--vapor-text-muted); font-size: 0.95rem; }

    /* CTA */
    .cta {
      background: var(--vapor-bg-dark);
      text-align: center;
      padding: 80px 40px;
    }

    .cta h2 {
      font-family: 'Monoton', cursive;
      font-weight: 400;
      font-size: 2.2rem;
      color: var(--vapor-pink);
      text-shadow: 2px 2px 0 var(--vapor-teal);
      margin-bottom: 1rem;
    }

    .cta p {
      color: rgba(255, 255, 255, 0.6);
      letter-spacing: 0.15em;
      margin-bottom: 2rem;
    }

    /* Footer */
    footer {
      background: var(--vapor-bg-dark);
      border-top: 1px solid rgba(255, 113, 206, 0.2);
      text-align: center;
      padding: 30px 40px;
      font-family: 'VT323', monospace;
      font-size: 0.95rem;
      color: var(--vapor-text-muted);
    }

    @media (max-width: 768px) {
      .hero { min-height: auto; padding: 60px 20px; }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">PLAZA</a>
    <ul>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">Dreams</a></li>
      <li><a href="#">Archive</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Digital Plaza</h1>
      <p>Welcome to the abandoned shopping mall of the internet. Everything is on sale. Nothing is real.</p>
      <a href="#" class="btn">Enter</a>
    </div>
  </section>

  <section class="features">
    <h2>Explore the Archive</h2>
    <p class="subtitle">A collection of forgotten futures</p>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-titlebar">
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          marble_dreams.exe
        </div>
        <div class="feature-body">
          <h3>Marble Dreams</h3>
          <p>Classical sculpture meets digital decay. Greek busts rendered in pink marble, floating in an infinite void.</p>
        </div>
      </div>
      <div class="feature">
        <div class="feature-titlebar">
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          sunset_protocol.exe
        </div>
        <div class="feature-body">
          <h3>Sunset Protocol</h3>
          <p>Eternal sunset gradients cascading over wireframe horizons. The sun never sets in the digital plaza.</p>
        </div>
      </div>
      <div class="feature">
        <div class="feature-titlebar">
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          palm_memory.exe
        </div>
        <div class="feature-body">
          <h3>Palm Memory</h3>
          <p>Tropical stock photography refracted through VHS tracking errors. Paradise as remembered by a corrupted hard drive.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Remember</h2>
    <p>The future was supposed to be different. It was supposed to be beautiful.</p>
    <a href="#" class="btn">Rewind</a>
  </section>

  <footer>
    <p>[ DIGITAL PLAZA ] // est. 1995 // all rights imagined</p>
  </footer>
</body>
</html>
```
