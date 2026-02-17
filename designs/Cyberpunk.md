# Cyberpunk Design Reference

Cyberpunk is a neon-soaked dystopian aesthetic rooted in the science fiction subgenre of the same name. It depicts rain-slick megacity streets, holographic advertisements, glitch artifacts, and corporate decay -- a world of high technology and low life. The visual language draws from 1980s sci-fi cinema (Blade Runner, Akira, Ghost in the Shell), combining dense urban layering with electric neon lighting, CRT scan lines, and corrupted digital interfaces. In web and UI design, Cyberpunk translates to dark backgrounds pierced by vivid neon accents, monospaced terminal typography, glitch effects, and a pervasive sense of technological overload.

---

## Visual Characteristics

### Core Design Traits

- **Dark, near-black backgrounds** -- deep navy, charcoal, or pure black simulating nighttime megacity environments
- **Neon accent colors** -- electric cyan, hot magenta, toxic green, and warning amber used sparingly for maximum impact
- **Glitch and distortion effects** -- chromatic aberration, scan lines, pixel displacement, and data corruption artifacts
- **Monospaced and terminal typography** -- code-like fonts that evoke hacker culture and machine interfaces
- **Dense, layered compositions** -- overlapping UI panels, translucent overlays, and information-rich layouts
- **Holographic and translucent elements** -- glass-like panels with backdrop blur and neon-tinted borders
- **Grid lines and wireframes** -- visible structural scaffolding suggesting exposed digital infrastructure
- **CRT and screen effects** -- scan lines, screen flicker, phosphor glow, and vignette darkening at edges
- **Corporate branding motifs** -- fictional mega-corp logos, barcode elements, and Japanese/CJK character accents
- **Rain and atmospheric particles** -- animated rain streaks, floating dust motes, and fog overlays

### Design Principles

- Embrace visual tension between high technology and urban decay
- Use darkness as the dominant canvas -- light is always artificial, always neon
- Layer information densely but maintain readability through luminance contrast
- Treat the interface itself as a narrative element -- it should feel like a diegetic in-world terminal
- Glitch effects should feel intentional, not broken -- controlled chaos
- Color is light: every colored element should appear to emit its own glow
- Reserve warm colors (amber, red) for warnings and danger states
- Cool colors (cyan, blue) serve as primary interactive and informational tones
- Typography should feel utilitarian and machine-generated, never decorative or calligraphic

---

## Color Palette

### Neon Megacity Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Void Black** | `#0A0A0F` | Primary background, deepest layer |
| **Dark Steel** | `#12121A` | Card backgrounds, secondary surfaces |
| **Gunmetal** | `#1A1A2E` | Elevated panels, nav backgrounds |
| **Slate Circuit** | `#2A2A3E` | Borders, dividers, subtle backgrounds |
| **Neon Cyan** | `#00F0FF` | Primary accent, links, interactive elements |
| **Electric Blue** | `#0080FF` | Secondary accent, active states |
| **Hot Magenta** | `#FF0080` | Highlight accent, notifications, badges |
| **Toxic Green** | `#00FF41` | Success states, terminal text, confirmations |
| **Warning Amber** | `#FFB800` | Warnings, caution indicators |
| **Danger Red** | `#FF1744` | Error states, critical alerts, destructive actions |
| **Holo Purple** | `#B000FF` | Tertiary accent, decorative elements |
| **Ghost White** | `#E0E0EC` | Primary text on dark backgrounds |
| **Muted Steel** | `#6A6A8A` | Secondary text, captions, disabled states |
| **Dim Grid** | `#2A2A40` | Grid lines, subtle structural elements |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --cyber-bg-void: #0a0a0f;
  --cyber-bg-dark: #12121a;
  --cyber-bg-panel: #1a1a2e;
  --cyber-bg-elevated: #2a2a3e;

  /* Neon accents */
  --cyber-cyan: #00f0ff;
  --cyber-blue: #0080ff;
  --cyber-magenta: #ff0080;
  --cyber-green: #00ff41;
  --cyber-amber: #ffb800;
  --cyber-red: #ff1744;
  --cyber-purple: #b000ff;

  /* Text */
  --cyber-text-primary: #e0e0ec;
  --cyber-text-secondary: #6a6a8a;
  --cyber-text-glow: #00f0ff;

  /* Glows (used for box-shadow and text-shadow) */
  --cyber-glow-cyan: 0 0 10px rgba(0, 240, 255, 0.5), 0 0 40px rgba(0, 240, 255, 0.15);
  --cyber-glow-magenta: 0 0 10px rgba(255, 0, 128, 0.5), 0 0 40px rgba(255, 0, 128, 0.15);
  --cyber-glow-green: 0 0 10px rgba(0, 255, 65, 0.5), 0 0 40px rgba(0, 255, 65, 0.15);

  /* Borders */
  --cyber-border: 1px solid rgba(0, 240, 255, 0.15);
  --cyber-border-bright: 1px solid rgba(0, 240, 255, 0.4);
}
```

---

## Typography

### Typeface Characteristics

Cyberpunk typography is:

- **Monospaced and mechanical** -- evoking terminal readouts and machine interfaces
- **Angular and utilitarian** -- no rounded, friendly shapes; letterforms feel stamped or engineered
- **Variable weight for hierarchy** -- thin weights for ambient data, bold for warnings and headings
- **Uppercase-heavy for display** -- headers and labels often set in all-caps with wide letter-spacing
- **Mixed with CJK characters** -- Japanese katakana or kanji used decoratively to suggest globalized megacity culture

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Share Tech Mono** | Monospaced, techy | Terminal text, code blocks, data readouts |
| **Orbitron** | Geometric, futuristic | Headlines, display text, UI chrome |
| **Rajdhani** | Condensed, semi-rounded | Subheadings, navigation, labels |
| **Exo 2** | Geometric, wide | Headlines, hero text, large display |
| **IBM Plex Mono** | Clean monospace | Body text, readable terminal output |
| **Oxanium** | Rounded tech | Buttons, badges, secondary headings |
| **Audiowide** | Wide, futuristic | Logos, display headings, branding |
| **Electrolize** | Square, digital | Navigation, labels, data dashboards |
| **Fira Code** | Monospace with ligatures | Code blocks, technical content |
| **Space Mono** | Retro-futuristic monospace | Body text, editorial cyberpunk layouts |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Orbitron** (700) | **Share Tech Mono** (400) | Classic cyberpunk terminal, high-tech |
| **Exo 2** (700) | **IBM Plex Mono** (400) | Clean futuristic, readable |
| **Rajdhani** (600) | **Fira Code** (400) | Condensed tech, developer-oriented |
| **Audiowide** (400) | **Space Mono** (400) | Retro-futuristic, editorial |
| **Electrolize** (400) | **Share Tech Mono** (400) | Dashboard, data-heavy interfaces |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;900&family=Share+Tech+Mono&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Orbitron', 'Exo 2', sans-serif;
  font-weight: 700;
  color: var(--cyber-text-primary);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  line-height: 1.2;
}

/* Display / Hero text with neon glow */
.cyber-display {
  font-family: 'Orbitron', sans-serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 900;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--cyber-cyan);
  text-shadow: 0 0 10px rgba(0, 240, 255, 0.6), 0 0 40px rgba(0, 240, 255, 0.2);
}

/* Body / terminal text */
body {
  font-family: 'Share Tech Mono', 'Fira Code', monospace;
  font-size: 0.95rem;
  line-height: 1.7;
  color: var(--cyber-text-primary);
}

/* UI labels */
.cyber-label {
  font-family: 'Orbitron', sans-serif;
  font-weight: 500;
  font-size: 0.75rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--cyber-text-secondary);
}

/* Data readout */
.cyber-data {
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.85rem;
  color: var(--cyber-green);
  line-height: 1.5;
}
```

---

## Layout Principles

### Grid and Structure

- **Dark, full-bleed backgrounds** -- the entire viewport is a dark canvas; there is no white space, only darkness
- **Asymmetric panel layouts** -- HUD-like panels of varying sizes, suggesting a multi-monitor command center
- **Visible grid lines** -- faint grid overlays that suggest the underlying data architecture
- **Dense information layouts** -- more content per viewport than typical web design; Cyberpunk is maximalist within its dark frame
- **Layered depth through translucency** -- panels with `backdrop-filter: blur()` float over background imagery
- **Neon border accents** -- thin glowing borders delineate panels instead of shadows or spacing

### Section Organization

- **Navigation**: Dark translucent top bar with neon-accented active states and monospaced labels
- **Hero**: Full-viewport dark background with massive glowing headline, atmospheric particles or rain animation
- **Data panels**: Grid of semi-transparent cards with neon borders displaying metrics or features
- **Content blocks**: Two-column layouts with text alongside holographic or wireframe illustrations
- **Terminal section**: Monospaced text block styled as a command-line interface
- **CTA section**: Dark background with single neon-glowing button and stark headline
- **Footer**: Dense, data-rich footer with grid lines and muted secondary text

### Responsive Approach

- Maintain dark backgrounds at all breakpoints -- never introduce light backgrounds on mobile
- Stack panels vertically on mobile; reduce grid complexity from multi-column to single-column
- Preserve neon glow effects but reduce blur radius on lower-powered devices
- Reduce scan line and glitch animation intensity on mobile for performance
- Typography scales down but retains uppercase and letter-spacing characteristics

---

## CSS / Design Techniques

### Cyberpunk Card Component

```css
.cyber-card {
  background: rgba(26, 26, 46, 0.8);
  border: 1px solid rgba(0, 240, 255, 0.15);
  border-radius: 2px;
  padding: 28px;
  position: relative;
  backdrop-filter: blur(10px);
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

.cyber-card:hover {
  border-color: rgba(0, 240, 255, 0.4);
  box-shadow: var(--cyber-glow-cyan);
}

/* Corner accent marks */
.cyber-card::before,
.cyber-card::after {
  content: '';
  position: absolute;
  width: 12px;
  height: 12px;
  border-color: var(--cyber-cyan);
  border-style: solid;
}

.cyber-card::before {
  top: -1px;
  left: -1px;
  border-width: 2px 0 0 2px;
}

.cyber-card::after {
  bottom: -1px;
  right: -1px;
  border-width: 0 2px 2px 0;
}

/* Card grid */
.cyber-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
}
```

### Cyberpunk Button

```css
.cyber-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: transparent;
  color: var(--cyber-cyan);
  border: 1px solid var(--cyber-cyan);
  padding: 12px 32px;
  font-family: 'Orbitron', sans-serif;
  font-weight: 700;
  font-size: 0.85rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  position: relative;
  clip-path: polygon(0 0, calc(100% - 10px) 0, 100% 10px, 100% 100%, 10px 100%, 0 calc(100% - 10px));
  transition: all 0.3s ease;
}

.cyber-button:hover {
  background: var(--cyber-cyan);
  color: var(--cyber-bg-void);
  box-shadow: var(--cyber-glow-cyan);
}

/* Magenta variant */
.cyber-button--magenta {
  color: var(--cyber-magenta);
  border-color: var(--cyber-magenta);
}

.cyber-button--magenta:hover {
  background: var(--cyber-magenta);
  color: var(--cyber-bg-void);
  box-shadow: var(--cyber-glow-magenta);
}

/* Filled variant */
.cyber-button--filled {
  background: var(--cyber-cyan);
  color: var(--cyber-bg-void);
}

.cyber-button--filled:hover {
  box-shadow: var(--cyber-glow-cyan);
  filter: brightness(1.2);
}
```

### Navigation Bar

```css
.cyber-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1400px;
  margin: 0 auto;
  padding: 16px 40px;
  background: rgba(10, 10, 15, 0.85);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(0, 240, 255, 0.1);
}

.cyber-nav__logo {
  font-family: 'Orbitron', sans-serif;
  font-weight: 900;
  font-size: 1.2rem;
  color: var(--cyber-cyan);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  text-shadow: 0 0 8px rgba(0, 240, 255, 0.4);
}

.cyber-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.cyber-nav__links a {
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.85rem;
  color: var(--cyber-text-secondary);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  transition: color 0.2s ease, text-shadow 0.2s ease;
}

.cyber-nav__links a:hover,
.cyber-nav__links a.active {
  color: var(--cyber-cyan);
  text-shadow: 0 0 8px rgba(0, 240, 255, 0.4);
}
```

### Hero Section

```css
.cyber-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 40px;
  background: var(--cyber-bg-void);
  overflow: hidden;
}

/* Scan line overlay */
.cyber-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 2px,
    rgba(0, 240, 255, 0.02) 2px,
    rgba(0, 240, 255, 0.02) 4px
  );
  pointer-events: none;
  z-index: 2;
}

/* Grid floor effect */
.cyber-hero::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 40%;
  background:
    linear-gradient(to bottom, transparent, rgba(0, 240, 255, 0.03)),
    repeating-linear-gradient(90deg, transparent, transparent 79px, rgba(0, 240, 255, 0.06) 79px, rgba(0, 240, 255, 0.06) 80px),
    repeating-linear-gradient(0deg, transparent, transparent 79px, rgba(0, 240, 255, 0.06) 79px, rgba(0, 240, 255, 0.06) 80px);
  transform: perspective(500px) rotateX(45deg);
  transform-origin: bottom;
  pointer-events: none;
  z-index: 1;
}

.cyber-hero__content {
  position: relative;
  z-index: 3;
  max-width: 800px;
}

.cyber-hero__content h1 {
  font-size: clamp(2.5rem, 6vw, 5rem);
  color: var(--cyber-cyan);
  text-shadow: 0 0 20px rgba(0, 240, 255, 0.5), 0 0 60px rgba(0, 240, 255, 0.15);
  margin-bottom: 1.5rem;
}

.cyber-hero__content p {
  font-size: 1.1rem;
  color: var(--cyber-text-secondary);
  max-width: 600px;
  margin: 0 auto 2.5rem;
  line-height: 1.8;
}

@media (max-width: 768px) {
  .cyber-hero {
    min-height: auto;
    padding: 60px 20px;
  }
}
```

### Glitch Text Effect

```css
@keyframes cyber-glitch {
  0%, 100% { clip-path: inset(0 0 0 0); transform: translate(0); }
  20% { clip-path: inset(20% 0 60% 0); transform: translate(-3px, 2px); }
  40% { clip-path: inset(60% 0 10% 0); transform: translate(3px, -1px); }
  60% { clip-path: inset(40% 0 30% 0); transform: translate(-2px, 1px); }
  80% { clip-path: inset(10% 0 70% 0); transform: translate(2px, -2px); }
}

.cyber-glitch {
  position: relative;
}

.cyber-glitch::before,
.cyber-glitch::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.cyber-glitch::before {
  color: var(--cyber-magenta);
  animation: cyber-glitch 3s infinite linear alternate;
  z-index: -1;
}

.cyber-glitch::after {
  color: var(--cyber-cyan);
  animation: cyber-glitch 2s infinite linear alternate-reverse;
  z-index: -1;
}
```

### Scan Line Overlay

```css
.cyber-scanlines {
  position: relative;
}

.cyber-scanlines::after {
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
}
```

### Data Table

```css
.cyber-table {
  width: 100%;
  border-collapse: collapse;
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.85rem;
}

.cyber-table th {
  font-family: 'Orbitron', sans-serif;
  font-weight: 500;
  font-size: 0.7rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--cyber-cyan);
  text-align: left;
  padding: 12px 16px;
  border-bottom: 1px solid rgba(0, 240, 255, 0.2);
}

.cyber-table td {
  padding: 10px 16px;
  color: var(--cyber-text-primary);
  border-bottom: 1px solid rgba(0, 240, 255, 0.06);
}

.cyber-table tr:hover td {
  background: rgba(0, 240, 255, 0.04);
}
```

---

## Design Do's and Don'ts

### Do

- Use very dark backgrounds (near-black) as the primary canvas
- Apply neon glow effects to key interactive elements and headings via `text-shadow` and `box-shadow`
- Use monospaced fonts for body text and data to maintain the terminal aesthetic
- Add subtle scan line overlays and grid patterns to create atmosphere
- Use `clip-path` for angular, cut-corner shapes on buttons and panels
- Apply `backdrop-filter: blur()` to create holographic translucent panels
- Reserve bright neon colors for interactive and high-priority elements only
- Include small atmospheric details: corner brackets, data labels, progress bars

### Don't

- Use white or light backgrounds -- they break the immersion completely
- Overuse glitch animations -- they should be accents, not constant distractions
- Apply neon glow to everything -- when everything glows, nothing stands out
- Use rounded, friendly typefaces -- they conflict with the angular, mechanical mood
- Mix more than 2-3 neon accent colors on a single page; maintain a focused palette
- Forget readability -- neon on dark must still meet contrast requirements for body text
- Use organic, natural textures -- everything should feel synthetic and manufactured
- Add cute or whimsical illustrations -- the tone is serious, gritty, and urban

---

## Related Aesthetics

| Aesthetic | Relationship to Cyberpunk |
|-----------|--------------------------|
| **Synthwave** | Shares the neon-on-dark palette and 1980s roots, but Synthwave is nostalgic and celebratory while Cyberpunk is dystopian and critical |
| **Vaporwave** | Both reference technology culture, but Vaporwave is ironic and pastel while Cyberpunk is earnest and high-contrast |
| **Y2K Futurism** | Late-90s techno-optimism with chrome and glass; Cyberpunk is the darker, more cynical cousin |
| **Silicon Dreams** | Shares digital themes but with a cleaner, more corporate-utopian presentation |
| **RGB Gamer** | Overlaps in neon-on-dark color schemes but lacks the narrative dystopian context |
| **Glassmorphism** | The translucent panel technique is shared; Cyberpunk uses it within a darker, grittier frame |
| **8-Bit** | Both reference digital culture; 8-Bit is retro and playful, Cyberpunk is forward-looking and tense |
| **Steampunk** | Both are "-punk" aesthetics that critique technology and society, but from different eras (Victorian vs. near-future) |

---

## Quick-Start: Minimal Cyberpunk Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cyberpunk Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;900&family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
    :root {
      --cyber-bg-void: #0a0a0f;
      --cyber-bg-panel: #1a1a2e;
      --cyber-bg-elevated: #2a2a3e;
      --cyber-cyan: #00f0ff;
      --cyber-magenta: #ff0080;
      --cyber-green: #00ff41;
      --cyber-amber: #ffb800;
      --cyber-red: #ff1744;
      --cyber-text-primary: #e0e0ec;
      --cyber-text-secondary: #6a6a8a;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--cyber-bg-void);
      color: var(--cyber-text-primary);
      font-family: 'Share Tech Mono', monospace;
      font-size: 0.95rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1400px;
      margin: 0 auto;
      padding: 16px 40px;
      border-bottom: 1px solid rgba(0, 240, 255, 0.1);
    }

    nav a.logo {
      font-family: 'Orbitron', sans-serif;
      font-weight: 900;
      font-size: 1.1rem;
      color: var(--cyber-cyan);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      text-shadow: 0 0 8px rgba(0, 240, 255, 0.4);
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'Share Tech Mono', monospace;
      color: var(--cyber-text-secondary);
      text-decoration: none;
      text-transform: uppercase;
      font-size: 0.85rem;
      letter-spacing: 0.08em;
      transition: color 0.2s, text-shadow 0.2s;
    }

    nav ul a:hover {
      color: var(--cyber-cyan);
      text-shadow: 0 0 8px rgba(0, 240, 255, 0.4);
    }

    /* Hero */
    .hero {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 80vh;
      padding: 80px 40px;
      overflow: hidden;
    }

    /* Scan lines */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(0deg, transparent, transparent 2px, rgba(0, 240, 255, 0.02) 2px, rgba(0, 240, 255, 0.02) 4px);
      pointer-events: none;
    }

    .hero-content { position: relative; z-index: 2; max-width: 700px; }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      color: var(--cyber-cyan);
      text-shadow: 0 0 20px rgba(0, 240, 255, 0.5), 0 0 60px rgba(0, 240, 255, 0.15);
      margin-bottom: 1.5rem;
    }

    .hero p {
      color: var(--cyber-text-secondary);
      font-size: 1rem;
      margin-bottom: 2.5rem;
    }

    .btn {
      display: inline-block;
      background: transparent;
      color: var(--cyber-cyan);
      border: 1px solid var(--cyber-cyan);
      padding: 14px 36px;
      font-family: 'Orbitron', sans-serif;
      font-weight: 700;
      font-size: 0.85rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      clip-path: polygon(0 0, calc(100% - 10px) 0, 100% 10px, 100% 100%, 10px 100%, 0 calc(100% - 10px));
      transition: all 0.3s;
    }

    .btn:hover {
      background: var(--cyber-cyan);
      color: var(--cyber-bg-void);
      box-shadow: 0 0 10px rgba(0, 240, 255, 0.5), 0 0 40px rgba(0, 240, 255, 0.15);
    }

    /* Features */
    .features {
      padding: 80px 0;
      border-top: 1px solid rgba(0, 240, 255, 0.08);
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--cyber-text-primary);
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 20px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: rgba(26, 26, 46, 0.6);
      border: 1px solid rgba(0, 240, 255, 0.12);
      padding: 28px;
      position: relative;
      transition: border-color 0.3s, box-shadow 0.3s;
    }

    .feature:hover {
      border-color: rgba(0, 240, 255, 0.35);
      box-shadow: 0 0 10px rgba(0, 240, 255, 0.1);
    }

    .feature-label {
      font-family: 'Orbitron', sans-serif;
      font-size: 0.65rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--cyber-cyan);
      margin-bottom: 12px;
    }

    .feature h3 { font-size: 1.1rem; margin-bottom: 0.75rem; }
    .feature p { color: var(--cyber-text-secondary); font-size: 0.9rem; }

    /* CTA */
    .cta {
      text-align: center;
      padding: 80px 40px;
      border-top: 1px solid rgba(0, 240, 255, 0.08);
    }

    .cta h2 {
      font-size: 2rem;
      color: var(--cyber-magenta);
      text-shadow: 0 0 15px rgba(255, 0, 128, 0.4);
      margin-bottom: 1rem;
    }

    .cta p {
      color: var(--cyber-text-secondary);
      margin-bottom: 2rem;
    }

    .cta .btn {
      color: var(--cyber-magenta);
      border-color: var(--cyber-magenta);
    }

    .cta .btn:hover {
      background: var(--cyber-magenta);
      color: var(--cyber-bg-void);
      box-shadow: 0 0 10px rgba(255, 0, 128, 0.5), 0 0 40px rgba(255, 0, 128, 0.15);
    }

    /* Footer */
    footer {
      border-top: 1px solid rgba(0, 240, 255, 0.08);
      text-align: center;
      padding: 30px 40px;
      color: var(--cyber-text-secondary);
      font-size: 0.8rem;
    }

    @media (max-width: 768px) {
      .hero { min-height: auto; padding: 60px 20px; }
      nav { padding: 12px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">NeoKorp</a>
    <ul>
      <li><a href="#">Systems</a></li>
      <li><a href="#">Network</a></li>
      <li><a href="#">Decrypt</a></li>
      <li><a href="#">Access</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Jack into the grid</h1>
      <p>Next-generation neural interface systems for the connected megacity. Bypass the corporate firewalls. Reclaim your data sovereignty.</p>
      <a href="#" class="btn">Initialize</a>
    </div>
  </section>

  <section class="features">
    <h2>System Modules</h2>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-label">// module.01</div>
        <h3>Neural Uplink</h3>
        <p>Direct cortical interface with sub-millisecond latency. Full-spectrum data transfer through encrypted channels.</p>
      </div>
      <div class="feature">
        <div class="feature-label">// module.02</div>
        <h3>Ghost Protocol</h3>
        <p>Zero-trace network traversal. Your digital footprint dissolves the moment you disconnect from the node.</p>
      </div>
      <div class="feature">
        <div class="feature-label">// module.03</div>
        <h3>Ice Breaker</h3>
        <p>Advanced intrusion countermeasures. Adaptive algorithms that evolve faster than corporate defense systems.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Ready to disconnect?</h2>
    <p>The megacorps control the network. We offer an alternative.</p>
    <a href="#" class="btn">Go dark</a>
  </section>

  <footer>
    <p>[ NEOKORP SYSTEMS ] // Built in the neon glow of a dying world</p>
  </footer>
</body>
</html>
```
