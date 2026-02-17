# Dark Aero Design Reference

Dark Aero is a design aesthetic that represents the **middle ground between Frutiger Aero and Skeuomorphism**, combining Frutiger Aero's depth-filled imagery with a distinctly **darker, more restrained color palette**. It is described as more "sleek" and "cleaner" than Frutiger Aero due to its partial omission of varied color palettes, achieving a **less cluttered look** while maintaining a strong sense of **futuristic allure and technological wonder**. The aesthetic is characterized by **black piano gloss finishes**, **aero glass effects**, **neon highlights against dark surfaces**, and visual motifs drawn from electronics, waves, spectrum analyzers, lasers, and electronic pulses.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Black piano gloss / piano finish** -- high-gloss black surfaces with deep reflections, the signature material of Dark Aero
- **Aero glass** -- translucent, frosted-glass UI panels with blur and transparency layered over dark backgrounds
- **Glossy and graphite textures** -- polished dark surfaces ranging from mirror-black to matte graphite
- **Neon highlights** -- vivid colored accents (blue, green, red, yellow) glowing against dark backdrops
- **Auroras** -- flowing, luminous color gradients reminiscent of the Northern Lights, used as background or accent elements
- **Bokeh effects** -- soft, out-of-focus light circles creating depth and atmospheric glow
- **Electronic-inspired visuals** -- waveforms, audio spectrum bars, laser beams, electronic pulses, circuit-like patterns
- **Skeuomorphic elements** -- realistic material textures (glass, metal, carbon fiber) rendered in a dark palette
- **Dark material textures** -- elegant graphite, obsidian, dark cement, brushed dark metal, carbon fiber weave
- **Futuristic design language** -- sleek curves, beveled edges, and contoured forms suggesting advanced technology

### Design Principles

- **Dark-dominant with selective luminance** -- dark backgrounds establish depth; bright elements command attention
- **High contrast compositions** -- neon and gloss highlights against deep blacks create dramatic visual impact
- **Sleek minimalism over clutter** -- fewer colors and cleaner surfaces than Frutiger Aero; every element is intentional
- **Depth through layering** -- aero glass panels, bokeh, and translucent overlays create a sense of Z-axis depth
- **Technological wonder** -- design conveys futurism, precision engineering, and digital sophistication
- **Material authenticity** -- surfaces should feel like real materials (polished glass, brushed metal, glossy plastic)
- **Selective color restraint** -- the palette is mostly achromatic; chromatic accents are used sparingly for maximum impact

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | Black, deep charcoal, obsidian |
| **Surface** | Dark gray, graphite, slate |
| **Neutral** | Chrome, silver-gray, white |
| **Accent** | Neon blue, electric green, signal red, amber yellow |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Piano Black | `#0A0A0A`, `#111111` | Primary backgrounds, hero sections |
| Obsidian | `#1A1A2E`, `#16161A` | Deep backgrounds with slight blue undertone |
| Graphite | `#2D2D30`, `#3A3A3D` | Card surfaces, secondary panels |
| Dark Chrome | `#4A4A4D`, `#555558` | Borders, dividers, tertiary surfaces |
| Silver Chrome | `#B0B0B4`, `#C8C8CC` | Secondary text, metallic accents |
| Gloss White | `#E8E8EC`, `#F0F0F4` | Primary text, bright highlights |
| Neon Blue | `#0088FF`, `#00AAFF` | Primary accent, links, active states |
| Aurora Blue | `#0066CC`, `#3399FF` | Gradients, secondary accent |
| Electric Green | `#00CC66`, `#00FF88` | Success states, secondary accent |
| Signal Red | `#FF3355`, `#FF4466` | Alert states, tertiary accent |
| Amber Yellow | `#FFAA00`, `#FFCC33` | Warning states, highlight accent |
| Bokeh Glow | `rgba(0, 136, 255, 0.15)` | Ambient light effects, background glow |

### Suggested CSS Custom Properties

```css
:root {
  /* Dark base tones */
  --dark-aero-black: #0a0a0a;
  --dark-aero-obsidian: #1a1a2e;
  --dark-aero-void: #111111;
  --dark-aero-graphite: #2d2d30;
  --dark-aero-slate: #3a3a3d;
  --dark-aero-chrome-dark: #4a4a4d;

  /* Light / chrome tones */
  --dark-aero-chrome: #b0b0b4;
  --dark-aero-chrome-light: #c8c8cc;
  --dark-aero-white: #e8e8ec;
  --dark-aero-bright: #f0f0f4;

  /* Accent -- neon / electric */
  --dark-aero-blue: #0088ff;
  --dark-aero-blue-light: #00aaff;
  --dark-aero-blue-deep: #0066cc;
  --dark-aero-green: #00cc66;
  --dark-aero-green-light: #00ff88;
  --dark-aero-red: #ff3355;
  --dark-aero-yellow: #ffaa00;

  /* Glow / transparency */
  --dark-aero-glow-blue: rgba(0, 136, 255, 0.25);
  --dark-aero-glow-green: rgba(0, 204, 102, 0.2);
  --dark-aero-glow-red: rgba(255, 51, 85, 0.2);
  --dark-aero-glass: rgba(255, 255, 255, 0.06);
  --dark-aero-glass-border: rgba(255, 255, 255, 0.1);

  /* Functional mappings */
  --dark-aero-bg-primary: var(--dark-aero-black);
  --dark-aero-bg-secondary: var(--dark-aero-void);
  --dark-aero-bg-surface: var(--dark-aero-graphite);
  --dark-aero-text-primary: var(--dark-aero-white);
  --dark-aero-text-secondary: var(--dark-aero-chrome);
  --dark-aero-accent: var(--dark-aero-blue);
  --dark-aero-border: var(--dark-aero-chrome-dark);
}
```

### Approaches

- **Primarily achromatic dark palette** -- blacks and grays with chrome metallic neutrals
- **Neon-on-dark contrast model** -- vivid saturated accents against near-black backgrounds
- **Blue as the default chromatic accent** -- other colors (green, red, yellow) used for semantic or secondary purposes
- **Subtle warm/cool undertones in darks** -- obsidian with blue undertone vs. pure neutral black
- **Aurora gradients for decorative backgrounds** -- multi-color gradients at low opacity for atmosphere

---

## Typography

### Typeface Characteristics

Dark Aero typography is clean, futuristic, and highly legible against dark backgrounds:

- **Geometric or humanist sans-serif typefaces** -- modern and technology-forward
- **Light to regular weight for body text** -- thin strokes read well on dark backgrounds without being fragile
- **Semibold to bold for headlines** -- enough weight to anchor attention without feeling heavy
- **Generous letter-spacing on display text** -- creates an airy, futuristic feel
- **No serifs** -- all type is smooth, modern, sans-serif
- **Subtle glow or luminous text effects** -- text can appear to emit light on dark surfaces
- **Small, uppercase labels** -- technical and precise for secondary information

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Exo 2** | Geometric, futuristic sans | Headlines, display text |
| **Rajdhani** | Light, technical, semi-condensed | Subheadings, UI labels |
| **Inter** | Clean, neutral, modern | Body text, paragraphs |
| **Outfit** | Geometric, versatile | Headlines, body text |
| **Space Grotesk** | Proportional, techy | Headlines, feature labels |
| **IBM Plex Sans** | Technical, precise | Body copy, data displays |
| **Orbitron** | Geometric, square, display | Large hero titles, numbers |
| **Chakra Petch** | Tech-angular, modern | Display headlines, UI accents |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Exo 2', 'Outfit', sans-serif;
  font-weight: 600;
  letter-spacing: 0.06em;
  color: var(--dark-aero-white);
}

/* Display / Hero text with glow */
.dark-aero-display {
  font-family: 'Orbitron', 'Chakra Petch', sans-serif;
  font-size: clamp(2.5rem, 6vw, 6rem);
  letter-spacing: 0.12em;
  line-height: 1.1;
  color: var(--dark-aero-bright);
  text-shadow:
    0 0 20px var(--dark-aero-glow-blue),
    0 0 60px rgba(0, 136, 255, 0.1);
}

/* Body text */
body {
  font-family: 'Inter', 'IBM Plex Sans', sans-serif;
  font-weight: 300;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--dark-aero-text-secondary);
}

/* Technical label text */
.dark-aero-label {
  font-family: 'Rajdhani', 'Space Grotesk', sans-serif;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--dark-aero-chrome-dark);
}
```

---

## Layout Principles

### Grid and Structure

- **Dark, expansive backgrounds** -- full-bleed dark sections that establish depth and immersion
- **Centered, focused content** -- content floats on the dark canvas, drawing attention inward
- **Generous negative space** -- dark space is not empty; it provides atmosphere and breathing room
- **Layered glass panels** -- aero glass cards float above the background with translucent surfaces
- **Wide, cinematic proportions** -- sections should feel panoramic, inspired by widescreen displays
- **Subtle depth cues** -- shadows, blur, and transparency create a convincing sense of layered depth

### Section Organization

- Use **thin luminous dividers** between sections (neon accent lines with gradient fade at edges)
- Apply **aero glass containers** for content grouping (semi-transparent with backdrop blur)
- Create **hierarchy through luminance and glow** -- brighter or glowing elements are more important
- Employ **rounded-rectangle containers** -- the ubiquitous shape of late-2000s UI design
- Use **dark-on-darker nesting** -- panels slightly lighter than their parent surface for visual separation
- Add **ambient light effects** -- subtle bokeh circles or aurora gradients in background layers

---

## CSS/Design Techniques

### Piano Black Gloss Surface

```css
/* High-gloss piano black surface with reflection highlight */
.dark-aero-piano {
  background: linear-gradient(
    180deg,
    #1a1a1a 0%,
    #0a0a0a 40%,
    #050505 100%
  );
  position: relative;
  overflow: hidden;
}

.dark-aero-piano::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 45%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.08) 0%,
    rgba(255, 255, 255, 0.02) 60%,
    transparent 100%
  );
  pointer-events: none;
}
```

### Aero Glass Panel

```css
/* Translucent glass panel with blur -- the signature Dark Aero UI element */
.dark-aero-glass {
  background: rgba(255, 255, 255, 0.06);
  backdrop-filter: blur(20px) saturate(1.2);
  -webkit-backdrop-filter: blur(20px) saturate(1.2);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 2rem;
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.4),
    inset 0 1px 0 rgba(255, 255, 255, 0.08);
}

/* Glass panel with subtle inner shine on top edge */
.dark-aero-glass::before {
  content: '';
  position: absolute;
  top: 0;
  left: 5%;
  right: 5%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.3),
    transparent
  );
}
```

### Neon Glow Accents

```css
/* Neon blue glow for interactive elements */
.dark-aero-neon {
  color: var(--dark-aero-blue);
  text-shadow:
    0 0 8px var(--dark-aero-glow-blue),
    0 0 24px rgba(0, 136, 255, 0.15);
}

/* Neon border glow */
.dark-aero-neon-border {
  border: 1px solid var(--dark-aero-blue);
  box-shadow:
    0 0 8px var(--dark-aero-glow-blue),
    0 0 24px rgba(0, 136, 255, 0.1),
    inset 0 0 8px rgba(0, 136, 255, 0.05);
}

/* Accent line divider with neon glow */
.dark-aero-divider {
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--dark-aero-blue) 20%,
    var(--dark-aero-blue) 80%,
    transparent
  );
  box-shadow: 0 0 12px var(--dark-aero-glow-blue);
}
```

### Aurora Background Effect

```css
/* Multi-color aurora gradient for atmospheric backgrounds */
.dark-aero-aurora {
  position: relative;
}

.dark-aero-aurora::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(ellipse 80% 50% at 20% 40%, rgba(0, 136, 255, 0.12) 0%, transparent 60%),
    radial-gradient(ellipse 60% 40% at 70% 60%, rgba(0, 204, 102, 0.08) 0%, transparent 50%),
    radial-gradient(ellipse 50% 60% at 50% 30%, rgba(136, 0, 255, 0.06) 0%, transparent 50%);
  pointer-events: none;
  z-index: 0;
}

/* Animated aurora pulse */
@keyframes aurora-shift {
  0%, 100% {
    opacity: 0.6;
    transform: scale(1) translateY(0);
  }
  50% {
    opacity: 1;
    transform: scale(1.05) translateY(-2%);
  }
}

.dark-aero-aurora::before {
  animation: aurora-shift 8s ease-in-out infinite;
}
```

### Bokeh Background Effect

```css
/* Soft, blurred light circles for depth and atmosphere */
.dark-aero-bokeh {
  position: absolute;
  border-radius: 50%;
  filter: blur(40px);
  opacity: 0.15;
  pointer-events: none;
}

/* Usage: create several positioned bokeh elements */
.dark-aero-bokeh--blue {
  background: var(--dark-aero-blue);
  width: 300px;
  height: 300px;
}

.dark-aero-bokeh--green {
  background: var(--dark-aero-green);
  width: 200px;
  height: 200px;
}

/* Animated floating bokeh */
@keyframes bokeh-float {
  0%, 100% { transform: translate(0, 0) scale(1); }
  33% { transform: translate(20px, -30px) scale(1.1); }
  66% { transform: translate(-15px, 15px) scale(0.95); }
}

.dark-aero-bokeh--animated {
  animation: bokeh-float 12s ease-in-out infinite;
}
```

### Graphite / Dark Texture Surfaces

```css
/* Graphite brushed texture */
.dark-aero-graphite {
  background:
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 1px,
      rgba(255, 255, 255, 0.015) 1px,
      rgba(255, 255, 255, 0.015) 2px
    ),
    linear-gradient(
      180deg,
      #2d2d30 0%,
      #222225 50%,
      #2a2a2d 100%
    );
}

/* Dark cement / concrete texture */
.dark-aero-cement {
  background:
    radial-gradient(circle at 30% 40%, rgba(255, 255, 255, 0.02) 0%, transparent 50%),
    radial-gradient(circle at 70% 60%, rgba(255, 255, 255, 0.015) 0%, transparent 40%),
    linear-gradient(180deg, #1e1e20 0%, #1a1a1c 100%);
}

/* Obsidian / volcanic glass */
.dark-aero-obsidian {
  background: linear-gradient(
    135deg,
    #1a1a2e 0%,
    #12121e 30%,
    #0e0e18 60%,
    #1a1a2e 100%
  );
}
```

### Electronic Waveform / Spectrum Visualization

```css
/* Animated spectrum bar container */
.dark-aero-spectrum {
  display: flex;
  align-items: flex-end;
  gap: 3px;
  height: 60px;
}

.dark-aero-spectrum-bar {
  width: 4px;
  background: linear-gradient(
    0deg,
    var(--dark-aero-blue) 0%,
    var(--dark-aero-blue-light) 100%
  );
  border-radius: 2px 2px 0 0;
  box-shadow: 0 0 6px var(--dark-aero-glow-blue);
  animation: spectrum-bounce 0.8s ease-in-out infinite alternate;
}

@keyframes spectrum-bounce {
  0% { height: 20%; }
  100% { height: 100%; }
}

/* Stagger animation for each bar */
.dark-aero-spectrum-bar:nth-child(2n) { animation-delay: 0.1s; }
.dark-aero-spectrum-bar:nth-child(3n) { animation-delay: 0.2s; }
.dark-aero-spectrum-bar:nth-child(4n) { animation-delay: 0.15s; }
```

### Dark Aero Card / Panel

```css
.dark-aero-card {
  background: linear-gradient(
    160deg,
    rgba(45, 45, 48, 0.8) 0%,
    rgba(26, 26, 30, 0.9) 100%
  );
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid var(--dark-aero-glass-border);
  border-radius: 14px;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 8px 24px rgba(0, 0, 0, 0.5),
    inset 0 1px 0 rgba(255, 255, 255, 0.06);
  transition: box-shadow 0.3s ease, border-color 0.3s ease;
}

.dark-aero-card:hover {
  border-color: rgba(0, 136, 255, 0.3);
  box-shadow:
    0 8px 24px rgba(0, 0, 0, 0.5),
    0 0 16px rgba(0, 136, 255, 0.1),
    inset 0 1px 0 rgba(255, 255, 255, 0.08);
}

/* Top-edge gloss highlight */
.dark-aero-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.25),
    transparent
  );
}
```

### Dark Aero Button

```css
.dark-aero-button {
  display: inline-block;
  padding: 0.7rem 2.2rem;
  border-radius: 10px;
  border: 1px solid rgba(0, 136, 255, 0.4);
  background: linear-gradient(
    180deg,
    rgba(0, 136, 255, 0.15) 0%,
    rgba(0, 136, 255, 0.05) 100%
  );
  color: var(--dark-aero-blue-light);
  font-family: 'Rajdhani', 'Exo 2', sans-serif;
  font-size: 0.85rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  cursor: pointer;
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  box-shadow:
    0 0 12px rgba(0, 136, 255, 0.15),
    inset 0 1px 0 rgba(255, 255, 255, 0.06);
  transition: all 0.25s ease;
}

.dark-aero-button:hover {
  background: linear-gradient(
    180deg,
    rgba(0, 136, 255, 0.25) 0%,
    rgba(0, 136, 255, 0.1) 100%
  );
  border-color: rgba(0, 170, 255, 0.6);
  box-shadow:
    0 0 20px rgba(0, 136, 255, 0.3),
    0 0 40px rgba(0, 136, 255, 0.1),
    inset 0 1px 0 rgba(255, 255, 255, 0.1);
  color: var(--dark-aero-bright);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Dark Aero materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Piano black gloss | Near-black background with `::before` gloss overlay (white gradient, top-half, low opacity) |
| Aero glass | Semi-transparent background + `backdrop-filter: blur(20px)` + subtle white border |
| Graphite / brushed dark metal | Dark gray base gradient + fine `repeating-linear-gradient` texture overlay |
| Obsidian | Very dark gradient with slight blue-purple undertone |
| Dark cement / concrete | Dark gray with scattered faint `radial-gradient` spots for texture |
| Neon light tubes | Bright saturated color + `text-shadow` / `box-shadow` glow in matching hue |
| Bokeh light circles | Large `border-radius: 50%` divs with `filter: blur()` and low opacity |
| Aurora / northern lights | Multiple overlapping `radial-gradient` layers with different hues, animated |
| Chrome trim | Thin lines or borders using silver-to-white linear gradients |
| Electronic spectrum display | Flex-row of narrow bars with gradient fills and staggered CSS animations |

---

## Associated Brands and Interfaces

The following products and interfaces exemplify the Dark Aero aesthetic:

- **Microsoft Windows 7** -- Aero Glass theme with dark wallpapers and translucent taskbar
- **Microsoft Windows Longhorn** (concept) -- early dark glass UI experiments
- **Sony PlayStation 3** -- XMB interface with glossy black chrome and flowing aurora backgrounds
- **Sony PSP** -- dark UI with glass-panel menus and wave animations
- **Apple iPhone 3G / 3GS** -- iOS 6 dark-mode contexts with glossy skeuomorphic icons
- **BlackBerry OS 5.0-7.1, BlackBerry 10** -- dark, professional UI with glass panels
- **Nintendo 3DS, Wii U** -- dark system UI themes with gloss and glow
- **5 Gum packaging** -- dark matte with neon accent colors and electronic motifs
- **Alienware hardware** -- aggressive dark surfaces with neon accent lighting
- **Pontiac (automotive)** -- dark instrument clusters with glowing gauge elements
- **Windows 10 default wallpaper** -- dark blue light beam on black, hero-style

---

## Related Aesthetics

| Aesthetic | Relationship to Dark Aero |
|-----------|--------------------------|
| **Frutiger Aero** | Parent aesthetic; Dark Aero is Frutiger Aero's dark-palette variant, retaining glass and depth but dropping the colorful, nature-inspired motifs |
| **Skeuomorphism** | Shares realistic material rendering; Dark Aero borrows skeuomorphism's darker, more serious tonal approach |
| **Metalheart** | Related; shares dark metallic surfaces and technological heaviness |
| **Hexatron** | Related; shares geometric precision and dark technological futurism |
| **Y2K Futurism** | Broader umbrella; Dark Aero is a later, more refined expression of Y2K tech optimism |
| **Abstract Tech** | Related; shares electronic/digital visual motifs and dark backgrounds |
| **Vectordelia** | Related; shares flowing curves and digital abstraction |
| **Recession Pop** | Contemporary; represents the economic-era counterpoint, sharing some dark/restrained qualities |
| **Flat Design** | Successor; the minimalist movement that eventually replaced Dark Aero's rich textures and depth |

---

## Quick-Start: Minimal Dark Aero Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dark Aero Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Exo+2:wght@300;400;600&family=Orbitron:wght@400;700&family=Inter:wght@300;400&family=Rajdhani:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --dark-aero-black: #0a0a0a;
      --dark-aero-void: #111111;
      --dark-aero-graphite: #2d2d30;
      --dark-aero-chrome: #b0b0b4;
      --dark-aero-white: #e8e8ec;
      --dark-aero-bright: #f0f0f4;
      --dark-aero-blue: #0088ff;
      --dark-aero-blue-light: #00aaff;
      --dark-aero-glow-blue: rgba(0, 136, 255, 0.25);
      --dark-aero-glass: rgba(255, 255, 255, 0.06);
      --dark-aero-glass-border: rgba(255, 255, 255, 0.1);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--dark-aero-black);
      color: var(--dark-aero-chrome);
      font-family: 'Inter', sans-serif;
      font-weight: 300;
      letter-spacing: 0.02em;
      line-height: 1.7;
      min-height: 100vh;
      overflow-x: hidden;
    }

    h1, h2, h3 {
      font-family: 'Exo 2', sans-serif;
      font-weight: 600;
      letter-spacing: 0.06em;
      color: var(--dark-aero-white);
    }

    /* Hero with aurora background */
    .hero {
      text-align: center;
      padding: 8rem 2rem 6rem;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse 80% 50% at 30% 40%, rgba(0, 136, 255, 0.1) 0%, transparent 60%),
        radial-gradient(ellipse 60% 40% at 70% 60%, rgba(0, 204, 102, 0.06) 0%, transparent 50%);
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: clamp(2.5rem, 6vw, 5rem);
      letter-spacing: 0.12em;
      color: var(--dark-aero-bright);
      text-shadow:
        0 0 20px var(--dark-aero-glow-blue),
        0 0 60px rgba(0, 136, 255, 0.1);
      position: relative;
      z-index: 1;
    }

    .hero p {
      margin-top: 1.5rem;
      font-size: 1.1rem;
      color: var(--dark-aero-chrome);
      position: relative;
      z-index: 1;
    }

    /* Neon divider */
    .neon-divider {
      width: 40%;
      margin: 2rem auto;
      border: none;
      height: 2px;
      background: linear-gradient(
        90deg,
        transparent,
        var(--dark-aero-blue) 20%,
        var(--dark-aero-blue) 80%,
        transparent
      );
      box-shadow: 0 0 12px var(--dark-aero-glow-blue);
      position: relative;
      z-index: 1;
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
    }

    /* Aero glass card */
    .glass-card {
      background: var(--dark-aero-glass);
      backdrop-filter: blur(20px) saturate(1.2);
      -webkit-backdrop-filter: blur(20px) saturate(1.2);
      border: 1px solid var(--dark-aero-glass-border);
      border-radius: 16px;
      padding: 2.5rem;
      position: relative;
      box-shadow:
        0 8px 32px rgba(0, 0, 0, 0.4),
        inset 0 1px 0 rgba(255, 255, 255, 0.08);
    }

    .glass-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 10%;
      right: 10%;
      height: 1px;
      background: linear-gradient(
        90deg,
        transparent,
        rgba(255, 255, 255, 0.25),
        transparent
      );
    }

    /* Bokeh decorative elements */
    .bokeh {
      position: fixed;
      border-radius: 50%;
      filter: blur(60px);
      opacity: 0.1;
      pointer-events: none;
      z-index: 0;
    }

    .bokeh--1 {
      width: 400px;
      height: 400px;
      background: var(--dark-aero-blue);
      top: 10%;
      left: -5%;
    }

    .bokeh--2 {
      width: 250px;
      height: 250px;
      background: #00cc66;
      bottom: 20%;
      right: -3%;
    }
  </style>
</head>
<body>
  <!-- Ambient bokeh lights -->
  <div class="bokeh bokeh--1"></div>
  <div class="bokeh bokeh--2"></div>

  <div class="hero">
    <h1>Title Here</h1>
    <hr class="neon-divider">
    <p>Subtitle styled with Dark Aero glass and glow</p>
  </div>

  <section>
    <div class="glass-card">
      <h2>Section Heading</h2>
      <p style="margin-top: 1rem;">Content rendered on a translucent aero glass panel with ambient bokeh lighting.</p>
    </div>
  </section>
</body>
</html>
```
