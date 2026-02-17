# Aurora Gradient Reference

Aurora Gradient is a dreamy, ethereal design aesthetic inspired by the Northern Lights (Aurora Borealis). It employs smooth, flowing color transitions across purple, pink, blue, green, and teal -- mimicking the undulating luminescence of polar skies. The style creates interfaces that feel cosmic and serene, using multi-stop gradients, soft blur effects, and translucent layers to evoke a sense of wonder. Every surface seems to glow from within, as if illuminated by distant celestial light.

---

## Visual Characteristics

### Core Design Traits

- **Multi-stop flowing gradients** -- smooth transitions through 3-5 colors (purple, pink, blue, green, teal) that mimic aurora curtains
- **Soft, diffused color washes** -- backgrounds feel painted with light rather than filled with flat color
- **Translucent glass layers** -- frosted-glass cards and surfaces that reveal gradient backgrounds beneath
- **Ethereal glow effects** -- soft radial glows and gradient overlays that simulate luminescence
- **Cool-to-warm color flow** -- palettes transition from deep blues and purples through pinks to greens and teals
- **Generous blur and feathering** -- backdrop-filter blur and soft-edged shapes create atmospheric depth
- **Dark or deep-toned bases** -- aurora gradients pop most against midnight-blue or deep purple backgrounds
- **Smooth, organic shapes** -- blob-like forms and rounded containers complement the flowing color transitions
- **Subtle animation** -- slow, gentle color shifts and gradient movement that mimic the aurora's natural dance
- **Light, airy typography** -- thin-to-medium weight fonts that don't compete with the gradient spectacle

### Design Principles

- Let the gradient be the hero: design everything else to support and not compete with it
- Use translucency to create depth while keeping the aurora visible through layers
- Dark backgrounds make gradients glow; avoid pure white bases that flatten the effect
- Color transitions should feel natural and smooth -- never harsh or banded
- Blur effects create atmosphere; use them on overlays, cards, and decorative elements
- Keep UI elements minimal so the celestial backdrop remains the focal point
- Animation should be slow and meditative, never jarring -- think time-lapse, not strobe
- Text on gradients needs careful contrast management: use solid-background chips or text shadows

---

## Color Palette

### Aurora Gradient Core Palette

Colors drawn from the actual Aurora Borealis: ionized oxygen (green, red), ionized nitrogen (blue, purple), with artistic additions of pink and teal for digital expression.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Midnight Sky** | `#0B0D1A` | Deepest background, page base |
| **Deep Space** | `#111827` | Primary surface, card base before glass effect |
| **Cosmic Blue** | `#1E1B4B` | Elevated surfaces, section backgrounds |
| **Aurora Purple** | `#7C3AED` | Primary purple gradient stop, accent elements |
| **Aurora Violet** | `#A855F7` | Mid-tone purple, badges, tags |
| **Aurora Pink** | `#EC4899` | Warm gradient stop, CTAs, highlights |
| **Aurora Rose** | `#F472B6` | Soft pink, secondary accents |
| **Aurora Blue** | `#3B82F6` | Cool gradient stop, links, info states |
| **Aurora Cyan** | `#06B6D4` | Teal gradient stop, secondary interactive |
| **Aurora Green** | `#10B981` | Green gradient stop, success states |
| **Aurora Mint** | `#34D399` | Light green, positive indicators |
| **Stardust** | `#E0E7FF` | Primary text on dark backgrounds |
| **Nebula** | `#A5B4FC` | Secondary text, descriptions |
| **Cosmic Dust** | `#6366F1` | Muted accent, tertiary text on dark |
| **Starlight** | `#F8FAFC` | Bright text, maximum contrast |

### CSS Custom Properties

```css
:root {
  /* Dark bases */
  --aurora-midnight: #0b0d1a;
  --aurora-deep-space: #111827;
  --aurora-cosmic: #1e1b4b;

  /* Aurora spectrum */
  --aurora-purple: #7c3aed;
  --aurora-violet: #a855f7;
  --aurora-pink: #ec4899;
  --aurora-rose: #f472b6;
  --aurora-blue: #3b82f6;
  --aurora-cyan: #06b6d4;
  --aurora-green: #10b981;
  --aurora-mint: #34d399;

  /* Text */
  --aurora-text-primary: #e0e7ff;
  --aurora-text-secondary: #a5b4fc;
  --aurora-text-muted: #6366f1;
  --aurora-text-bright: #f8fafc;

  /* Signature gradients */
  --aurora-gradient-full: linear-gradient(135deg, #7c3aed, #ec4899, #3b82f6, #06b6d4, #10b981);
  --aurora-gradient-warm: linear-gradient(135deg, #7c3aed, #a855f7, #ec4899, #f472b6);
  --aurora-gradient-cool: linear-gradient(135deg, #3b82f6, #06b6d4, #10b981, #34d399);
  --aurora-gradient-subtle: linear-gradient(135deg, rgba(124,58,237,0.15), rgba(236,72,153,0.1), rgba(6,182,212,0.15));

  /* Glass */
  --aurora-glass-bg: rgba(255, 255, 255, 0.05);
  --aurora-glass-border: rgba(255, 255, 255, 0.1);
  --aurora-glass-blur: 16px;
}
```

---

## Typography

### Typeface Characteristics

Aurora Gradient typography is:

- **Light to medium weight** -- thin, elegant fonts that let the gradient backgrounds shine through
- **Modern and geometric** -- clean letterforms that complement the smooth gradient curves
- **High legibility on dark backgrounds** -- tall x-height and open counters for readability against complex gradients
- **Subtly luminous** -- text can pick up gradient colors through subtle text-shadow or color inheritance
- **Airy with generous spacing** -- relaxed letter-spacing and line-height to match the ethereal mood

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Sora** | Geometric, modern, variable weight | Headlines, hero text -- perfect aurora companion |
| **Inter** | Screen-optimized, versatile | Body text, labels, UI elements |
| **Outfit** | Geometric, contemporary | Headlines, metrics, clean modern feel |
| **Albert Sans** | Geometric, clean | Body text, all-purpose on dark backgrounds |
| **Figtree** | Geometric, friendly, open | Body text, approachable aurora interfaces |
| **Urbanist** | Geometric, tall, modern | Headlines, navigation, elegant headers |
| **Lexend** | Designed for reading ease | Body text, accessibility-focused aurora pages |
| **Plus Jakarta Sans** | Geometric, slightly rounded | Headlines, warm yet modern feel |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Sora** (600) | **Inter** (400) | Clean, modern, cosmic elegance |
| **Urbanist** (600) | **Figtree** (400) | Tall and elegant meets friendly body |
| **Outfit** (600) | **Albert Sans** (400) | Contemporary, balanced, geometric |
| **Plus Jakarta Sans** (700) | **Inter** (400) | Warm headers, crisp body |
| **Sora** (700) | **Lexend** (400) | Bold display, accessible reading |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700&family=Inter:wght@400;500;600&display=swap');

h1, h2, h3, h4, h5, h6 {
  font-family: 'Sora', sans-serif;
  font-weight: 600;
  color: var(--aurora-text-primary);
  line-height: 1.2;
  letter-spacing: -0.02em;
}

.aurora-display {
  font-family: 'Sora', sans-serif;
  font-size: clamp(2.5rem, 5vw, 5rem);
  font-weight: 700;
  letter-spacing: -0.03em;
  line-height: 1.1;
  background: var(--aurora-gradient-full);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--aurora-text-secondary);
}

.aurora-label {
  font-family: 'Sora', sans-serif;
  font-weight: 500;
  font-size: 0.8rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--aurora-text-muted);
}

.aurora-caption {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--aurora-text-secondary);
}
```

---

## Layout Principles

### Grid and Structure

- **Full-viewport gradient backgrounds** -- the aurora gradient often spans the entire page or large sections
- **Glassmorphic card layers** -- translucent cards float above the gradient, creating depth
- **Centered, constrained content** -- max-width 1100px keeps content readable against flowing backgrounds
- **Vertical rhythm through gradient shifts** -- sections transition through different gradient phases
- **Organic, flowing section breaks** -- wavy SVG dividers or gradient fades between sections
- **Generous vertical spacing** -- 100-140px between sections to let the gradient breathe

### Section Organization

- **Navigation**: Transparent or glass-effect nav bar that reveals the gradient beneath
- **Hero**: Full-height gradient background with large display text (often gradient-clipped), centered
- **Features**: Glass cards floating on the gradient background in a clean grid
- **Showcase**: Large section where the gradient itself is the visual feature
- **Metrics**: Gradient-text numbers on dark translucent cards
- **CTA section**: Concentrated gradient area with glass button
- **Footer**: Fade to deepest dark with muted text

### Responsive Approach

- Gradients scale naturally across all screen sizes
- Glass cards stack vertically on mobile while maintaining translucency
- Background gradient can simplify (fewer stops) on mobile for performance
- Text on gradient requires extra contrast attention on small screens
- Blur effects may be reduced on mobile devices for performance

---

## CSS / Design Techniques

### Aurora Background

```css
.aurora-bg {
  background: var(--aurora-midnight);
  position: relative;
  overflow: hidden;
}

.aurora-bg::before {
  content: '';
  position: absolute;
  width: 150%;
  height: 150%;
  top: -25%;
  left: -25%;
  background:
    radial-gradient(ellipse at 20% 50%, rgba(124, 58, 237, 0.3) 0%, transparent 50%),
    radial-gradient(ellipse at 80% 20%, rgba(236, 72, 153, 0.2) 0%, transparent 50%),
    radial-gradient(ellipse at 60% 80%, rgba(6, 182, 212, 0.25) 0%, transparent 50%),
    radial-gradient(ellipse at 30% 20%, rgba(16, 185, 129, 0.15) 0%, transparent 50%);
  animation: auroraShift 20s ease-in-out infinite alternate;
  pointer-events: none;
}

@keyframes auroraShift {
  0% { transform: translate(0, 0) rotate(0deg); }
  50% { transform: translate(-5%, 3%) rotate(1deg); }
  100% { transform: translate(3%, -2%) rotate(-1deg); }
}
```

### Glass Card

```css
.aurora-glass {
  background: var(--aurora-glass-bg);
  backdrop-filter: blur(var(--aurora-glass-blur));
  -webkit-backdrop-filter: blur(var(--aurora-glass-blur));
  border: 1px solid var(--aurora-glass-border);
  border-radius: 16px;
  padding: 32px;
  transition: background 0.3s ease, border-color 0.3s ease;
}

.aurora-glass:hover {
  background: rgba(255, 255, 255, 0.08);
  border-color: rgba(255, 255, 255, 0.15);
}

.aurora-glass--strong {
  background: rgba(255, 255, 255, 0.08);
  backdrop-filter: blur(24px);
  -webkit-backdrop-filter: blur(24px);
}
```

### Aurora Button

```css
.aurora-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: var(--aurora-gradient-warm);
  color: #ffffff;
  border: none;
  border-radius: 12px;
  padding: 14px 36px;
  font-family: 'Sora', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  text-decoration: none;
  background-size: 200% 200%;
  animation: gradientShift 4s ease infinite;
}

@keyframes gradientShift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.aurora-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(124, 58, 237, 0.3);
}

.aurora-button--glass {
  background: var(--aurora-glass-bg);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid var(--aurora-glass-border);
  color: var(--aurora-text-primary);
}

.aurora-button--glass:hover {
  background: rgba(255, 255, 255, 0.1);
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
}
```

### Navigation Bar

```css
.aurora-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  position: relative;
  z-index: 10;
}

.aurora-nav__logo {
  font-family: 'Sora', sans-serif;
  font-weight: 700;
  font-size: 1.3rem;
  background: var(--aurora-gradient-warm);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  text-decoration: none;
}

.aurora-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.aurora-nav__links a {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--aurora-text-secondary);
  text-decoration: none;
  transition: color 0.2s ease;
}

.aurora-nav__links a:hover {
  color: var(--aurora-text-bright);
}
```

### Hero Section

```css
.aurora-hero {
  min-height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 40px;
  position: relative;
  z-index: 1;
}

.aurora-hero h1 {
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  margin-bottom: 1.5rem;
  background: var(--aurora-gradient-full);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.aurora-hero p {
  font-size: 1.2rem;
  color: var(--aurora-text-secondary);
  margin-bottom: 2.5rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.8;
}
```

### Gradient Text

```css
.aurora-gradient-text {
  background: var(--aurora-gradient-full);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  background-size: 200% auto;
  animation: textShimmer 6s ease-in-out infinite alternate;
}

@keyframes textShimmer {
  0% { background-position: 0% center; }
  100% { background-position: 200% center; }
}
```

### Wavy Section Divider

```css
.aurora-wave {
  position: relative;
  height: 80px;
}

.aurora-wave svg {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 80px;
}

.aurora-wave path {
  fill: var(--aurora-deep-space);
}
```

---

## Design Do's and Don'ts

### Do

- Use multi-stop gradients with smooth transitions through the aurora spectrum
- Pair gradients with dark backgrounds for maximum luminous impact
- Layer translucent glass elements to create depth and atmosphere
- Animate gradients slowly and subtly to mimic the aurora's natural movement
- Use gradient-clipped text for display headings as a focal point
- Apply backdrop-filter blur on overlaying elements for the glass effect
- Maintain sufficient text contrast on gradient backgrounds using text shadows or solid chips
- Let the gradient be the star; keep UI elements simple and understated

### Don't

- Use gradients on light/white backgrounds -- they lose their luminous quality
- Create harsh, banded color transitions -- all shifts should be smooth and diffused
- Animate gradients quickly or erratically -- the aurora effect requires slow, meditative motion
- Layer too many glass elements -- performance suffers and the effect becomes muddy
- Use more than one gradient system per page -- pick one aurora flow and commit
- Pair with sharp, angular, geometric patterns -- organic, flowing shapes complement better
- Ignore text readability: gradient backgrounds make contrast unpredictable
- Apply the aurora effect to small elements like buttons or badges -- it works best at large scale

---

## Related Aesthetics

| Aesthetic | Relationship to Aurora Gradient |
|-----------|-------------------------------|
| **Glassmorphism** | Core technique; frosted glass cards layered on aurora gradients create the signature effect |
| **Dark Aero** | Shares dark-base translucency; aurora adds flowing color where Dark Aero stays monochrome |
| **Frutiger Aero** | Predecessor; glossy, nature-inspired UI that aurora aesthetics update with cosmic gradients |
| **Laser Grid** | Shares vivid neon-on-dark approach but with rigid geometric grids instead of organic flows |
| **Acid Design** | Both use vivid gradients but Acid pushes toward chaos while Aurora maintains serenity |
| **Flat Design** | Opposite approach; solid, flat colors without any gradients, blur, or depth effects |
| **Neumorphism** | Contrasting approach; monochromatic soft shadows vs. polychromatic luminous gradients |
| **Cosmic** | Shares celestial inspiration; aurora focuses on light phenomena while Cosmic includes stars and space |
| **Cyberminimalism** | Both can coexist; minimal UI structure with aurora gradients as the decorative layer |
| **Dopamine Design** | Shares bold color but channels it into structured, energetic compositions rather than flowing serenity |

---

## Quick-Start: Minimal Aurora Gradient Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aurora Gradient Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --aurora-midnight: #0b0d1a;
      --aurora-deep-space: #111827;
      --aurora-cosmic: #1e1b4b;
      --aurora-purple: #7c3aed;
      --aurora-violet: #a855f7;
      --aurora-pink: #ec4899;
      --aurora-rose: #f472b6;
      --aurora-blue: #3b82f6;
      --aurora-cyan: #06b6d4;
      --aurora-green: #10b981;
      --aurora-mint: #34d399;
      --aurora-text-primary: #e0e7ff;
      --aurora-text-secondary: #a5b4fc;
      --aurora-text-muted: #6366f1;
      --aurora-text-bright: #f8fafc;
      --aurora-glass-bg: rgba(255, 255, 255, 0.05);
      --aurora-glass-border: rgba(255, 255, 255, 0.1);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--aurora-midnight);
      color: var(--aurora-text-secondary);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      line-height: 1.7;
      overflow-x: hidden;
    }

    h1, h2, h3 {
      font-family: 'Sora', sans-serif;
      font-weight: 600;
      color: var(--aurora-text-primary);
      line-height: 1.2;
      letter-spacing: -0.02em;
    }

    /* Aurora background effect */
    .aurora-bg {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 0;
      pointer-events: none;
    }

    .aurora-bg::before {
      content: '';
      position: absolute;
      width: 150%;
      height: 150%;
      top: -25%;
      left: -25%;
      background:
        radial-gradient(ellipse at 20% 50%, rgba(124,58,237,0.3) 0%, transparent 50%),
        radial-gradient(ellipse at 80% 20%, rgba(236,72,153,0.2) 0%, transparent 50%),
        radial-gradient(ellipse at 60% 80%, rgba(6,182,212,0.25) 0%, transparent 50%),
        radial-gradient(ellipse at 30% 20%, rgba(16,185,129,0.15) 0%, transparent 50%);
      animation: auroraShift 20s ease-in-out infinite alternate;
    }

    @keyframes auroraShift {
      0% { transform: translate(0, 0) rotate(0deg); }
      50% { transform: translate(-5%, 3%) rotate(1deg); }
      100% { transform: translate(3%, -2%) rotate(-1deg); }
    }

    /* All content above aurora bg */
    .content { position: relative; z-index: 1; }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
    }

    nav a.logo {
      font-family: 'Sora', sans-serif;
      font-weight: 700;
      font-size: 1.3rem;
      background: linear-gradient(135deg, var(--aurora-purple), var(--aurora-pink));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-decoration: none;
    }

    nav ul { display: flex; gap: 32px; list-style: none; }

    nav ul a {
      color: var(--aurora-text-secondary);
      text-decoration: none;
      font-weight: 500;
      font-size: 0.9rem;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--aurora-text-bright); }

    /* Hero */
    .hero {
      min-height: 80vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 80px 40px;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      font-weight: 700;
      margin-bottom: 1.5rem;
      letter-spacing: -0.03em;
      background: linear-gradient(135deg, #7c3aed, #ec4899, #3b82f6, #06b6d4, #10b981);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 2.5rem;
      max-width: 580px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: linear-gradient(135deg, var(--aurora-purple), var(--aurora-pink));
      color: #fff;
      border: none;
      border-radius: 12px;
      padding: 14px 36px;
      font-family: 'Sora', sans-serif;
      font-weight: 600;
      font-size: 0.95rem;
      cursor: pointer;
      text-decoration: none;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(124, 58, 237, 0.3);
    }

    .btn--glass {
      background: var(--aurora-glass-bg);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border: 1px solid var(--aurora-glass-border);
      color: var(--aurora-text-primary);
    }

    /* Features */
    .features {
      padding: 80px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .features h2 { text-align: center; font-size: 2rem; margin-bottom: 48px; }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
    }

    .glass-card {
      background: var(--aurora-glass-bg);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid var(--aurora-glass-border);
      border-radius: 16px;
      padding: 32px;
      transition: background 0.3s, border-color 0.3s;
    }

    .glass-card:hover {
      background: rgba(255, 255, 255, 0.08);
      border-color: rgba(255, 255, 255, 0.15);
    }

    .card-icon {
      width: 48px;
      height: 48px;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 20px;
    }

    .glass-card h3 { font-size: 1.15rem; margin-bottom: 0.75rem; }
    .glass-card p { font-size: 0.95rem; line-height: 1.6; }

    /* CTA */
    .cta {
      text-align: center;
      padding: 100px 40px;
    }

    .cta-inner {
      background: var(--aurora-glass-bg);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      border: 1px solid var(--aurora-glass-border);
      border-radius: 24px;
      padding: 60px 40px;
      max-width: 800px;
      margin: 0 auto;
    }

    .cta h2 { font-size: 2rem; margin-bottom: 1rem; }
    .cta p { margin-bottom: 2rem; }

    /* Footer */
    footer {
      text-align: center;
      padding: 40px;
      font-size: 0.85rem;
      color: var(--aurora-text-muted);
    }

    @media (max-width: 768px) {
      .hero { min-height: 60vh; padding: 60px 20px; }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
      .cta-inner { padding: 40px 24px; }
    }
  </style>
</head>
<body>
  <div class="aurora-bg"></div>

  <div class="content">
    <nav>
      <a href="#" class="logo">Aurora</a>
      <ul>
        <li><a href="#">Product</a></li>
        <li><a href="#">Features</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">About</a></li>
      </ul>
    </nav>

    <section class="hero">
      <div>
        <h1>Design that glows from within</h1>
        <p>Experience interfaces inspired by the Northern Lights. Flowing gradients, translucent layers, and cosmic serenity.</p>
        <a href="#" class="btn">Explore Aurora</a>
      </div>
    </section>

    <section class="features">
      <h2>Celestial features</h2>
      <div class="features-grid">
        <div class="glass-card">
          <div class="card-icon" style="background:rgba(124,58,237,0.2);">
            <svg width="24" height="24" viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" fill="none" stroke="#a855f7" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
          </div>
          <h3>Layered Depth</h3>
          <p>Translucent glass surfaces create natural hierarchy. Content floats above cosmic gradients with effortless elegance.</p>
        </div>
        <div class="glass-card">
          <div class="card-icon" style="background:rgba(236,72,153,0.2);">
            <svg width="24" height="24" viewBox="0 0 24 24"><circle cx="12" cy="12" r="5" fill="none" stroke="#ec4899" stroke-width="2"/><path d="M12 1v2M12 21v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M1 12h2M21 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42" stroke="#ec4899" stroke-width="2" stroke-linecap="round"/></svg>
          </div>
          <h3>Living Color</h3>
          <p>Gradients shift and flow like the aurora itself. Slow, meditative animations create a sense of wonder and serenity.</p>
        </div>
        <div class="glass-card">
          <div class="card-icon" style="background:rgba(6,182,212,0.2);">
            <svg width="24" height="24" viewBox="0 0 24 24"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z" fill="none" stroke="#06b6d4" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
          </div>
          <h3>Cosmic Calm</h3>
          <p>Dark foundations and soft light create interfaces that reduce eye strain while maintaining visual richness.</p>
        </div>
      </div>
    </section>

    <section class="cta">
      <div class="cta-inner">
        <h2>Ready to see the lights?</h2>
        <p>Join creators who design with the beauty of the aurora borealis.</p>
        <a href="#" class="btn--glass btn">Get Started Free</a>
      </div>
    </section>

    <footer>
      <p>Built with Aurora Gradient aesthetics. Dreamy, luminous, serene.</p>
    </footer>
  </div>
</body>
</html>
```
