# Dark Mode Neon Reference

Dark Mode Neon is a high-contrast digital aesthetic that pairs deep, near-black backgrounds with vivid neon accent colors to create interfaces that feel electric and alive. Inspired by neon signage, cyberpunk cityscapes, and late-night coding sessions, the style uses glowing effects, sharp color contrasts, and strategic luminance to guide the eye through dark environments. It transforms the utility of dark mode into a visual statement -- functional darkness punctuated by bursts of radiant, eye-catching color.

---

## Visual Characteristics

### Core Design Traits

- **Near-black backgrounds** -- base surfaces in deep charcoal, navy, or pure dark tones (not pure black, to reduce eye strain)
- **Vivid neon accents** -- electric cyan, hot magenta, neon green, and violet used sparingly but intensely
- **Glowing UI elements** -- box-shadow and text-shadow with neon colors create the illusion of light emission
- **High luminance contrast** -- bright elements on dark surfaces for maximum visual pop
- **Layered dark surfaces** -- multiple dark shades (dark-1, dark-2, dark-3) create depth without light colors
- **Neon line work and borders** -- thin glowing borders on cards, buttons, and inputs
- **Subtle gradient overlays** -- dark-to-darker gradients on backgrounds for depth without brightness
- **Monospace or tech-forward typography** -- fonts that evoke terminals, code editors, and sci-fi interfaces
- **Minimal use of white** -- replaced by light grays and neon colors for text and accents
- **Strategic color glow** -- blur and spread on shadows create a neon-tube luminescence effect

### Design Principles

- Dark backgrounds are the canvas; neon accents are the paint -- use color with intention
- Create hierarchy through luminance: the brightest element gets the most attention
- Layer dark shades to create depth without introducing light colors
- Glow effects should feel like actual light emission, not flat color
- Limit neon to 2-3 accent colors per page to avoid visual noise
- Ensure text remains highly readable against dark backgrounds (minimum WCAG AA contrast)
- Use transitions and subtle animations to reinforce the sense of energy and electricity
- Reserve the most vivid neon for interactive and primary action elements

---

## Color Palette

### Dark Mode Neon Core Palette

Deep foundations with electric accents. The palette is designed to create maximum contrast while maintaining visual comfort on dark backgrounds.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Void** | `#0A0A0F` | Deepest background, page base |
| **Carbon** | `#111118` | Primary surface, card backgrounds |
| **Graphite** | `#1A1A24` | Elevated surfaces, modals, dropdowns |
| **Slate** | `#252532` | Borders, dividers, tertiary surfaces |
| **Smoke** | `#3A3A4A` | Disabled states, subtle borders |
| **Ash** | `#6B6B80` | Muted text, placeholders, captions |
| **Silver** | `#9CA3AF` | Secondary text, descriptions |
| **Ghost** | `#E0E0E8` | Primary text on dark backgrounds |
| **Cyber Cyan** | `#00F0FF` | Primary accent, links, interactive focus |
| **Hot Magenta** | `#FF0080` | Secondary accent, CTAs, alerts |
| **Neon Green** | `#39FF14` | Success states, positive indicators, terminals |
| **Electric Violet** | `#8B5CF6` | Tertiary accent, badges, tags |
| **Plasma Orange** | `#FF6B00` | Warning states, warm highlights |
| **Ion Blue** | `#3B82F6` | Info states, secondary links |

### CSS Custom Properties

```css
:root {
  /* Dark surfaces (lightest to darkest) */
  --neon-void: #0a0a0f;
  --neon-carbon: #111118;
  --neon-graphite: #1a1a24;
  --neon-slate: #252532;
  --neon-smoke: #3a3a4a;

  /* Text */
  --neon-text-primary: #e0e0e8;
  --neon-text-secondary: #9ca3af;
  --neon-text-muted: #6b6b80;

  /* Neon accents */
  --neon-cyan: #00f0ff;
  --neon-magenta: #ff0080;
  --neon-green: #39ff14;
  --neon-violet: #8b5cf6;
  --neon-orange: #ff6b00;
  --neon-blue: #3b82f6;

  /* Glow shadows */
  --glow-cyan: 0 0 20px rgba(0, 240, 255, 0.3), 0 0 40px rgba(0, 240, 255, 0.1);
  --glow-magenta: 0 0 20px rgba(255, 0, 128, 0.3), 0 0 40px rgba(255, 0, 128, 0.1);
  --glow-green: 0 0 20px rgba(57, 255, 20, 0.3), 0 0 40px rgba(57, 255, 20, 0.1);
  --glow-violet: 0 0 20px rgba(139, 92, 246, 0.3), 0 0 40px rgba(139, 92, 246, 0.1);
}
```

---

## Typography

### Typeface Characteristics

Dark Mode Neon typography is:

- **Monospace or geometric sans-serif** -- evoking terminals, code editors, and futuristic interfaces
- **Clean and sharp at all sizes** -- crisp rendering against dark backgrounds is critical
- **Light to medium weight for body** -- avoiding heavy weights that can bleed on dark backgrounds
- **All-caps for labels and UI elements** -- geometric uppercase letters reinforce the technical feel
- **Generous letter-spacing** -- especially in uppercase text for readability and futuristic style

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **JetBrains Mono** | Monospace, programming font | Code blocks, terminal displays, tech labels |
| **Space Mono** | Monospace, geometric | Headlines, nav, retro-tech feel |
| **Inter** | Screen-optimized sans | Body text, UI labels, maximum readability |
| **Space Grotesk** | Monospace-inspired proportional | Headlines, metrics, tech-forward body |
| **Outfit** | Modern geometric | Body text, balanced technical feel |
| **Chakra Petch** | Tech-inspired, angular | Headlines, sci-fi displays, cyberpunk feel |
| **Orbitron** | Geometric, futuristic display | Hero headlines, display numbers |
| **Exo 2** | Geometric, semi-futuristic | Headlines, navigation, clean tech look |
| **IBM Plex Mono** | Professional monospace | Code, data, technical displays |
| **Fira Code** | Monospace with ligatures | Code blocks, terminal aesthetic |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Space Grotesk** (600) | **Inter** (400) | Modern tech, clean and readable |
| **Chakra Petch** (600) | **Inter** (400) | Cyberpunk edge, functional body |
| **Orbitron** (600) | **Space Grotesk** (400) | Futuristic display, tech body |
| **Exo 2** (600) | **Outfit** (400) | Balanced sci-fi, approachable body |
| **Space Mono** (700) | **JetBrains Mono** (400) | Full monospace, terminal aesthetic |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap');

h1, h2, h3, h4, h5, h6 {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 600;
  color: var(--neon-text-primary);
  line-height: 1.2;
  letter-spacing: -0.01em;
}

.neon-display {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 700;
  letter-spacing: -0.02em;
  line-height: 1.1;
  color: var(--neon-cyan);
  text-shadow: 0 0 30px rgba(0, 240, 255, 0.3);
}

body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--neon-text-secondary);
}

.neon-label {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--neon-text-muted);
}

.neon-code {
  font-family: 'JetBrains Mono', monospace;
  font-weight: 400;
  font-size: 0.9rem;
  color: var(--neon-green);
}
```

---

## Layout Principles

### Grid and Structure

- **Dark layered surfaces** -- use 3-4 shades of dark to create depth: page bg, card bg, elevated bg, border
- **Centered, constrained containers** -- max-width 1200px with generous side padding
- **Card-based layouts with subtle borders** -- cards defined by 1px neon-tinted borders or slight background elevation
- **Strategic glow placement** -- glow effects on primary actions and focal points, not everywhere
- **Full-width dark sections** -- sections separated by shade differences, not whitespace alone
- **Grid-based metric displays** -- data-heavy layouts suit the technical aesthetic well

### Section Organization

- **Navigation**: Dark bar with neon-accented logo and link hover states; subtle bottom border glow
- **Hero**: Large headline with neon text-shadow, dark background, optional gradient overlay
- **Features**: Cards on dark backgrounds with neon icon accents and glowing hover borders
- **Metrics**: Large neon-colored numbers with muted labels on dark cards
- **Code/Terminal block**: Monospace text on near-black background with syntax-colored accents
- **CTA section**: Gradient border or glow effect surrounding the action area
- **Footer**: Darkest shade background with muted text and neon link highlights

### Responsive Approach

- Dark backgrounds work well on all screen sizes and in ambient light conditions
- Reduce glow intensity on mobile to prevent visual overload on smaller screens
- Typography remains crisp on dark backgrounds at all sizes when using screen-optimized fonts
- Single-column stack on mobile with maintained dark surface layering
- Neon accents become even more impactful on smaller, closer-viewed screens

---

## CSS / Design Techniques

### Neon Card Component

```css
.neon-card {
  background: var(--neon-carbon);
  border: 1px solid var(--neon-slate);
  border-radius: 12px;
  padding: 32px;
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

.neon-card:hover {
  border-color: var(--neon-cyan);
  box-shadow: var(--glow-cyan);
}

.neon-card--elevated {
  background: var(--neon-graphite);
}

.neon-card--magenta:hover {
  border-color: var(--neon-magenta);
  box-shadow: var(--glow-magenta);
}

.neon-card--green:hover {
  border-color: var(--neon-green);
  box-shadow: var(--glow-green);
}
```

### Neon Button

```css
.neon-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: transparent;
  color: var(--neon-cyan);
  border: 2px solid var(--neon-cyan);
  border-radius: 8px;
  padding: 12px 32px;
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  letter-spacing: 0.03em;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
  text-transform: uppercase;
}

.neon-button:hover {
  background: rgba(0, 240, 255, 0.1);
  box-shadow: var(--glow-cyan);
  text-shadow: 0 0 10px rgba(0, 240, 255, 0.5);
}

.neon-button--filled {
  background: var(--neon-cyan);
  color: var(--neon-void);
  border-color: var(--neon-cyan);
}

.neon-button--filled:hover {
  background: #33f3ff;
  box-shadow: var(--glow-cyan);
}

.neon-button--magenta {
  color: var(--neon-magenta);
  border-color: var(--neon-magenta);
}

.neon-button--magenta:hover {
  background: rgba(255, 0, 128, 0.1);
  box-shadow: var(--glow-magenta);
}
```

### Navigation Bar

```css
.neon-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  border-bottom: 1px solid var(--neon-slate);
}

.neon-nav__logo {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  font-size: 1.3rem;
  color: var(--neon-cyan);
  text-decoration: none;
  text-shadow: 0 0 20px rgba(0, 240, 255, 0.3);
}

.neon-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.neon-nav__links a {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--neon-text-muted);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  transition: color 0.2s ease, text-shadow 0.2s ease;
}

.neon-nav__links a:hover {
  color: var(--neon-cyan);
  text-shadow: 0 0 10px rgba(0, 240, 255, 0.3);
}
```

### Hero Section

```css
.neon-hero {
  text-align: center;
  padding: 120px 40px 100px;
  position: relative;
  overflow: hidden;
  background: radial-gradient(ellipse at 50% 0%, rgba(0, 240, 255, 0.05) 0%, transparent 60%);
}

.neon-hero h1 {
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  margin-bottom: 1.5rem;
  color: var(--neon-text-primary);
}

.neon-hero h1 span {
  color: var(--neon-cyan);
  text-shadow: 0 0 30px rgba(0, 240, 255, 0.4);
}

.neon-hero p {
  font-size: 1.15rem;
  color: var(--neon-text-secondary);
  margin-bottom: 2.5rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}
```

### Glowing Border Effect

```css
.neon-glow-border {
  position: relative;
  border-radius: 12px;
  padding: 32px;
  background: var(--neon-carbon);
}

.neon-glow-border::before {
  content: '';
  position: absolute;
  inset: -1px;
  border-radius: 13px;
  background: linear-gradient(135deg, var(--neon-cyan), var(--neon-magenta), var(--neon-violet));
  z-index: -1;
  opacity: 0.5;
  transition: opacity 0.3s ease;
}

.neon-glow-border:hover::before {
  opacity: 1;
}
```

### Terminal / Code Block

```css
.neon-terminal {
  background: var(--neon-void);
  border: 1px solid var(--neon-slate);
  border-radius: 8px;
  padding: 24px;
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.9rem;
  line-height: 1.8;
  color: var(--neon-green);
  overflow-x: auto;
}

.neon-terminal__prompt {
  color: var(--neon-cyan);
}

.neon-terminal__comment {
  color: var(--neon-text-muted);
}

.neon-terminal__string {
  color: var(--neon-magenta);
}
```

---

## Design Do's and Don'ts

### Do

- Use 3-4 dark shades to create depth and layered surfaces
- Apply glow effects strategically to primary actions and focal points
- Maintain high contrast between text and dark backgrounds (WCAG AA minimum)
- Use neon color sparingly: 2-3 accent colors maximum per page
- Create the illusion of light emission with multi-layered box-shadows
- Use monospace or geometric sans-serif fonts for the tech aesthetic
- Test on both OLED and LCD screens -- glow effects render differently
- Let the dark background breathe; negative space is powerful in dark themes

### Don't

- Use pure black (#000000) as the base -- it causes halation with bright text
- Apply glow effects to every element -- it becomes visual noise
- Use light or pastel colors for large surfaces -- they break the dark mode illusion
- Pair multiple neon colors in equal amounts -- one should dominate
- Skip contrast checking because "it looks cool" -- readability is paramount
- Use warm-toned backgrounds (brown, dark red) -- stick to cool, neutral darks
- Overuse animations on glowing elements -- subtle pulse is fine, constant flashing is not
- Forget that dark mode is functional first: reduce eye strain, then add style

---

## Related Aesthetics

| Aesthetic | Relationship to Dark Mode Neon |
|-----------|-------------------------------|
| **Laser Grid** | Shares neon-on-dark palette with a specific retrowave/synthwave grid visual language |
| **Cyberminimalism** | Shares dark, tech-forward approach but strips away the glow and maximalist neon energy |
| **RGB Gamer** | Cousin aesthetic; uses RGB lighting and neon but with a gaming hardware focus |
| **Early Cyber** | Historical precursor; 90s hacker/cyber culture with green-on-black terminal aesthetics |
| **Dark Aero** | Shares dark UI approach with glossy, translucent elements rather than neon glow |
| **Neon Ooze** | Maximalist neon sibling; pushes neon saturation and organic forms to the extreme |
| **Acid Design** | Shares electric color intensity but embraces chaos and distortion over the clean glow |
| **Metalheart** | Shares dark backgrounds with metallic and chrome accents rather than neon |
| **Glassmorphism** | Can be combined: frosted glass cards on dark backgrounds with neon glow borders |
| **Flat Design** | Opposite approach; bright backgrounds, solid colors, no shadows or glow effects |
| **PC-98** | Retro precursor; limited-palette pixel art on dark backgrounds from Japanese PCs |
| **Neumorphism** | Contrasting approach; soft shadows on light/same-tone backgrounds vs. sharp glow on dark |

---

## Quick-Start: Minimal Dark Mode Neon Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dark Mode Neon Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --neon-void: #0a0a0f;
      --neon-carbon: #111118;
      --neon-graphite: #1a1a24;
      --neon-slate: #252532;
      --neon-smoke: #3a3a4a;
      --neon-text-primary: #e0e0e8;
      --neon-text-secondary: #9ca3af;
      --neon-text-muted: #6b6b80;
      --neon-cyan: #00f0ff;
      --neon-magenta: #ff0080;
      --neon-green: #39ff14;
      --neon-violet: #8b5cf6;
      --glow-cyan: 0 0 20px rgba(0,240,255,0.3), 0 0 40px rgba(0,240,255,0.1);
      --glow-magenta: 0 0 20px rgba(255,0,128,0.3), 0 0 40px rgba(255,0,128,0.1);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--neon-void);
      color: var(--neon-text-secondary);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 600;
      color: var(--neon-text-primary);
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
      border-bottom: 1px solid var(--neon-slate);
    }

    nav a.logo {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      font-size: 1.3rem;
      color: var(--neon-cyan);
      text-decoration: none;
      text-shadow: 0 0 20px rgba(0, 240, 255, 0.3);
    }

    nav ul { display: flex; gap: 32px; list-style: none; }

    nav ul a {
      color: var(--neon-text-muted);
      text-decoration: none;
      font-weight: 500;
      font-size: 0.9rem;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      transition: color 0.2s, text-shadow 0.2s;
    }

    nav ul a:hover {
      color: var(--neon-cyan);
      text-shadow: 0 0 10px rgba(0, 240, 255, 0.3);
    }

    /* Hero */
    .hero {
      text-align: center;
      padding: 120px 40px 100px;
      background: radial-gradient(ellipse at 50% 0%, rgba(0, 240, 255, 0.05) 0%, transparent 60%);
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      font-weight: 700;
      margin-bottom: 1.5rem;
    }

    .hero h1 .glow {
      color: var(--neon-cyan);
      text-shadow: 0 0 30px rgba(0, 240, 255, 0.4);
    }

    .hero p {
      font-size: 1.15rem;
      margin-bottom: 2.5rem;
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: transparent;
      color: var(--neon-cyan);
      border: 2px solid var(--neon-cyan);
      border-radius: 8px;
      padding: 14px 36px;
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 600;
      font-size: 0.95rem;
      letter-spacing: 0.03em;
      text-transform: uppercase;
      cursor: pointer;
      text-decoration: none;
      transition: all 0.3s;
    }

    .btn:hover {
      background: rgba(0, 240, 255, 0.1);
      box-shadow: var(--glow-cyan);
    }

    .btn--filled {
      background: var(--neon-cyan);
      color: var(--neon-void);
    }

    .btn--filled:hover {
      background: #33f3ff;
      box-shadow: var(--glow-cyan);
    }

    /* Features */
    .features {
      padding: 80px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .features h2 {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
    }

    .feature-card {
      background: var(--neon-carbon);
      border: 1px solid var(--neon-slate);
      border-radius: 12px;
      padding: 32px;
      transition: border-color 0.3s, box-shadow 0.3s;
    }

    .feature-card:nth-child(1):hover { border-color: var(--neon-cyan); box-shadow: var(--glow-cyan); }
    .feature-card:nth-child(2):hover { border-color: var(--neon-magenta); box-shadow: var(--glow-magenta); }
    .feature-card:nth-child(3):hover { border-color: var(--neon-green); box-shadow: 0 0 20px rgba(57,255,20,0.3), 0 0 40px rgba(57,255,20,0.1); }

    .feature-icon {
      width: 48px;
      height: 48px;
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 20px;
      border: 1px solid var(--neon-slate);
    }

    .feature-card h3 { font-size: 1.15rem; margin-bottom: 0.75rem; }
    .feature-card p { font-size: 0.95rem; line-height: 1.6; }

    /* Terminal section */
    .terminal-section {
      padding: 60px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .terminal {
      background: var(--neon-void);
      border: 1px solid var(--neon-slate);
      border-radius: 8px;
      padding: 24px;
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.9rem;
      line-height: 1.8;
      color: var(--neon-green);
      overflow-x: auto;
    }

    .terminal .prompt { color: var(--neon-cyan); }
    .terminal .comment { color: var(--neon-text-muted); }

    /* CTA */
    .cta {
      text-align: center;
      padding: 80px 40px;
      position: relative;
    }

    .cta-inner {
      background: var(--neon-carbon);
      border: 1px solid var(--neon-cyan);
      border-radius: 16px;
      padding: 60px 40px;
      max-width: 800px;
      margin: 0 auto;
      box-shadow: var(--glow-cyan);
    }

    .cta h2 { font-size: 2rem; margin-bottom: 1rem; }
    .cta p { margin-bottom: 2rem; }

    /* Footer */
    footer {
      border-top: 1px solid var(--neon-slate);
      text-align: center;
      padding: 40px;
      font-size: 0.85rem;
      color: var(--neon-text-muted);
    }

    @media (max-width: 768px) {
      .hero { padding: 80px 20px 60px; }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
      .cta-inner { padding: 40px 24px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">NEON//UI</a>
    <ul>
      <li><a href="#">Platform</a></li>
      <li><a href="#">Docs</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">Blog</a></li>
    </ul>
  </nav>

  <section class="hero">
    <h1>Build at the <span class="glow">speed of light</span></h1>
    <p>A developer platform that cuts through the noise. Dark by default, powered by precision.</p>
    <a href="#" class="btn btn--filled">Get Started</a>
  </section>

  <section class="features">
    <h2>Engineered for developers</h2>
    <div class="features-grid">
      <div class="feature-card">
        <div class="feature-icon">
          <svg width="24" height="24" viewBox="0 0 24 24"><path d="M13 10V3L4 14h7v7l9-11h-7z" fill="#00f0ff"/></svg>
        </div>
        <h3>Instant Deployments</h3>
        <p>Push to production in seconds. Our edge network delivers your code globally with zero-config scaling.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">
          <svg width="24" height="24" viewBox="0 0 24 24"><path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4z" fill="#ff0080"/></svg>
        </div>
        <h3>Built-in Security</h3>
        <p>End-to-end encryption, automated vulnerability scanning, and SOC 2 compliance from day one.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">
          <svg width="24" height="24" viewBox="0 0 24 24"><path d="M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z" fill="#39ff14"/></svg>
        </div>
        <h3>Developer First</h3>
        <p>CLI tools, Git integration, and APIs designed by developers for developers. No abstractions in the way.</p>
      </div>
    </div>
  </section>

  <section class="terminal-section">
    <div class="terminal">
      <span class="comment"># Deploy your app in one command</span><br>
      <span class="prompt">$</span> neon deploy --production<br>
      <span style="color:var(--neon-text-secondary);">Uploading build artifacts...</span><br>
      <span style="color:var(--neon-cyan);">Deployed to 42 edge nodes in 2.3s</span><br>
      <span class="prompt">$</span> <span style="opacity:0.5;">_</span>
    </div>
  </section>

  <section class="cta">
    <div class="cta-inner">
      <h2>Ready to build something electric?</h2>
      <p>Join 50,000+ developers shipping faster with NEON//UI.</p>
      <a href="#" class="btn">Start Free Trial</a>
    </div>
  </section>

  <footer>
    <p>Built with Dark Mode Neon aesthetics. High contrast, vivid accents, pure focus.</p>
  </footer>
</body>
</html>
```
