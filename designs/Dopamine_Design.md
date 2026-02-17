# Dopamine Design Reference

Dopamine Design is a maximalist, joy-driven visual aesthetic built around the idea that bold, saturated colors and playful shapes can trigger positive emotional responses. It rejects the restraint of minimalism in favor of exuberant color clashes, chunky geometry, bubbly typography, and unabashed visual delight. Every element is designed to make the viewer smile -- through unexpected color combinations, oversized shapes, and a general sense of creative freedom that prioritizes feeling over convention.

---

## Visual Characteristics

### Core Design Traits

- **Hyper-saturated color palette** -- vivid, fully saturated hues used liberally and simultaneously; no muted tones
- **Playful geometric shapes** -- circles, blobs, squiggles, stars, and rounded polygons scattered as decorative elements
- **Bold color blocking** -- large areas of solid, contrasting color placed side by side for maximum visual impact
- **Chunky, rounded typography** -- fat, bubbly letterforms that feel friendly and approachable
- **Asymmetric, dynamic layouts** -- elements intentionally off-grid, rotated, overlapping, creating energetic compositions
- **Gradient accents** -- rainbow or multi-stop gradients used on backgrounds, shapes, and UI elements
- **Oversized UI elements** -- buttons, icons, and interactive elements are deliberately large and inviting
- **Decorative flourishes** -- confetti, sparkles, squiggly lines, and abstract shapes as pure ornament
- **High visual density** -- pages feel full and alive with color, pattern, and shape
- **No fear of clashing** -- colors that traditional design would never pair are placed together with confidence

### Design Principles

- Maximize visual joy: every design decision should spark a positive emotional response
- Embrace bold color clashes -- harmony comes from confidence, not from conventional palettes
- Use shape and movement to create a sense of playfulness and energy
- Make interactive elements irresistibly clickable through size, color, and animation
- Break the grid intentionally -- asymmetry and overlap create dynamism
- Layer patterns, gradients, and solid colors without restraint
- Typography should have personality: rounded, bold, and expressive
- Accessibility matters even in maximalism: maintain readable contrast ratios in text areas

---

## Color Palette

### Dopamine Core Palette

Colors are chosen for maximum serotonin response: warm, cool, and neon hues in full saturation, designed to be used together without restraint.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Serotonin Pink** | `#FF2D87` | Primary accent, CTAs, hero elements |
| **Dopamine Purple** | `#7B2FFF` | Secondary accent, buttons, badges |
| **Electric Blue** | `#00B4FF` | Links, interactive elements, info states |
| **Sunshine Yellow** | `#FFD000` | Highlights, stars, attention-grabbers |
| **Citrus Orange** | `#FF6B2B` | Warm accent, notifications, badges |
| **Mint Rush** | `#00E5A0` | Success states, positive indicators |
| **Candy Red** | `#FF3B3B` | Alerts, bold statements, emphasis |
| **Lavender Pop** | `#C084FC` | Soft accent, card backgrounds, tags |
| **Lime Fizz** | `#B8FF00` | High-energy accent, highlights on dark backgrounds |
| **Bubblegum** | `#FF8ED4` | Playful accent, decorative elements |
| **Deep Joy** | `#1E0A3C` | Dark text on light, dark card backgrounds |
| **Cloud White** | `#FFFBF5` | Light backgrounds, text on dark |
| **Creamy** | `#FFF3E0` | Warm light background, card surfaces |
| **Soft Violet** | `#F0E6FF` | Light purple background tint |

### CSS Custom Properties

```css
:root {
  /* Primary palette */
  --dopa-pink: #ff2d87;
  --dopa-purple: #7b2fff;
  --dopa-blue: #00b4ff;
  --dopa-yellow: #ffd000;
  --dopa-orange: #ff6b2b;
  --dopa-green: #00e5a0;
  --dopa-red: #ff3b3b;
  --dopa-lavender: #c084fc;
  --dopa-lime: #b8ff00;
  --dopa-bubblegum: #ff8ed4;

  /* Backgrounds */
  --dopa-bg-dark: #1e0a3c;
  --dopa-bg-light: #fffbf5;
  --dopa-bg-cream: #fff3e0;
  --dopa-bg-violet: #f0e6ff;

  /* Text */
  --dopa-text-dark: #1e0a3c;
  --dopa-text-light: #fffbf5;
  --dopa-text-muted: #7a6b8a;

  /* Gradients */
  --dopa-gradient-rainbow: linear-gradient(135deg, #ff2d87, #ff6b2b, #ffd000, #00e5a0, #00b4ff, #7b2fff);
  --dopa-gradient-sunset: linear-gradient(135deg, #ff2d87, #ff6b2b, #ffd000);
  --dopa-gradient-ocean: linear-gradient(135deg, #00b4ff, #7b2fff, #c084fc);
}
```

---

## Typography

### Typeface Characteristics

Dopamine Design typography is:

- **Rounded, chunky, and bubbly** -- letterforms that feel like they could bounce
- **Extra-bold weights preferred** -- 700-900 weights for headings to maximize visual punch
- **Playful and expressive** -- personality-driven typefaces that reject corporate neutrality
- **Variable sizing** -- extreme contrasts between massive headlines and compact body text
- **Occasionally decorative** -- display fonts with character used for hero text and accents

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Baloo 2** | Rounded, chunky, friendly | Headlines, hero text -- pure dopamine energy |
| **Fredoka** | Rounded, bold, bubbly | Display text, buttons, playful headings |
| **Quicksand** | Geometric, rounded, clean | Body text, balanced playfulness and legibility |
| **Comfortaa** | Rounded, geometric, modern | Headlines, navigation, brand text |
| **Nunito** | Rounded terminals, versatile | Body text, all-purpose friendly font |
| **Rubik** | Slightly rounded, geometric | Body text, UI elements, compact spaces |
| **Lilita One** | Ultra-bold, display | Hero headlines, maximum impact |
| **Bubblegum Sans** | Casual, handwritten feel | Decorative accents, playful labels |
| **Outfit** | Modern geometric, clean | Body text, metrics, balanced readability |
| **Poppins** | Geometric, versatile | Fallback body font, clean readability |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Fredoka** (700) | **Quicksand** (400) | Maximum playfulness, bubbly and warm |
| **Baloo 2** (700) | **Nunito** (400) | Chunky energy meets clean readability |
| **Lilita One** (400) | **Rubik** (400) | Bold impact with grounded body text |
| **Comfortaa** (700) | **Outfit** (400) | Modern rounded with efficient body text |
| **Fredoka** (600) | **Poppins** (400) | Playful heads, professional body balance |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Quicksand:wght@400;500;600;700&display=swap');

h1, h2, h3, h4, h5, h6 {
  font-family: 'Fredoka', cursive;
  font-weight: 700;
  color: var(--dopa-text-dark);
  line-height: 1.15;
  letter-spacing: -0.01em;
}

.dopa-display {
  font-family: 'Fredoka', cursive;
  font-size: clamp(3rem, 6vw, 5.5rem);
  font-weight: 700;
  letter-spacing: -0.02em;
  line-height: 1.05;
}

body {
  font-family: 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--dopa-text-dark);
}

.dopa-label {
  font-family: 'Fredoka', cursive;
  font-weight: 600;
  font-size: 0.85rem;
  letter-spacing: 0.03em;
  text-transform: uppercase;
}

.dopa-caption {
  font-family: 'Quicksand', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--dopa-text-muted);
}
```

---

## Layout Principles

### Grid and Structure

- **Deliberately broken grids** -- elements overlap, rotate, and escape their containers for dynamic energy
- **Large, chunky sections** -- generous section heights with oversized padding (80-120px)
- **Color-blocked sections** -- each section uses a different bold background color for maximum contrast
- **Scattered decorative elements** -- blobs, circles, and squiggles positioned absolutely to break rigidity
- **Rounded containers everywhere** -- border-radius of 20-40px on cards, sections, and images
- **Oversized hero areas** -- the hero section dominates with massive type and bold color

### Section Organization

- **Navigation**: Pill-shaped nav with colorful active states; logo can be playful/illustrated
- **Hero**: Massive headline in bold colors, decorative shapes floating in background, oversized CTA button
- **Features**: Colorful cards with icons, arranged in a loose grid with varied background colors
- **Showcase**: Full-bleed color section with large imagery or illustrations
- **Testimonials**: Rounded cards with colored borders or backgrounds, oversized quotation marks
- **CTA section**: Gradient background with large, inviting button
- **Footer**: Dark background with colorful accent links and shapes

### Responsive Approach

- Stack sections vertically on mobile while maintaining bold color blocks
- Reduce decorative elements on small screens to prevent clutter
- Typography scales dramatically: hero text can be 3x larger on desktop vs mobile
- Buttons remain oversized and finger-friendly at all breakpoints
- Maintain rounded corners and playful shapes even at compact sizes

---

## CSS / Design Techniques

### Dopamine Card Component

```css
.dopa-card {
  background: var(--dopa-bg-light);
  border-radius: 24px;
  padding: 32px;
  position: relative;
  overflow: hidden;
  transition: transform 0.3s ease;
}

.dopa-card:hover {
  transform: translateY(-4px) rotate(1deg);
}

.dopa-card--pink { background: #ffe0ee; }
.dopa-card--blue { background: #dff2ff; }
.dopa-card--yellow { background: #fff6d6; }
.dopa-card--green { background: #d6fff0; }
.dopa-card--violet { background: var(--dopa-bg-violet); }

/* Decorative blob */
.dopa-card::after {
  content: '';
  position: absolute;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  background: var(--dopa-pink);
  opacity: 0.1;
  top: -30px;
  right: -30px;
}
```

### Dopamine Button

```css
.dopa-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: var(--dopa-pink);
  color: #ffffff;
  border: none;
  border-radius: 50px;
  padding: 16px 40px;
  font-family: 'Fredoka', cursive;
  font-weight: 600;
  font-size: 1.1rem;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  text-decoration: none;
  box-shadow: 0 4px 20px rgba(255, 45, 135, 0.3);
}

.dopa-button:hover {
  transform: translateY(-3px) scale(1.02);
  box-shadow: 0 8px 30px rgba(255, 45, 135, 0.4);
}

.dopa-button--purple {
  background: var(--dopa-purple);
  box-shadow: 0 4px 20px rgba(123, 47, 255, 0.3);
}

.dopa-button--yellow {
  background: var(--dopa-yellow);
  color: var(--dopa-text-dark);
  box-shadow: 0 4px 20px rgba(255, 208, 0, 0.3);
}

.dopa-button--gradient {
  background: var(--dopa-gradient-sunset);
  box-shadow: 0 4px 20px rgba(255, 107, 43, 0.3);
}
```

### Navigation Bar

```css
.dopa-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
}

.dopa-nav__logo {
  font-family: 'Fredoka', cursive;
  font-weight: 700;
  font-size: 1.5rem;
  color: var(--dopa-pink);
  text-decoration: none;
}

.dopa-nav__links {
  display: flex;
  gap: 8px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.dopa-nav__links a {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: var(--dopa-text-dark);
  text-decoration: none;
  padding: 8px 20px;
  border-radius: 50px;
  transition: background 0.2s ease, color 0.2s ease;
}

.dopa-nav__links a:hover {
  background: var(--dopa-bg-violet);
  color: var(--dopa-purple);
}

.dopa-nav__links a.active {
  background: var(--dopa-purple);
  color: #ffffff;
}
```

### Hero Section

```css
.dopa-hero {
  position: relative;
  text-align: center;
  padding: 100px 40px;
  overflow: hidden;
  background: var(--dopa-bg-cream);
}

.dopa-hero h1 {
  font-size: clamp(3rem, 7vw, 5.5rem);
  font-weight: 700;
  margin-bottom: 1rem;
  line-height: 1.05;
  background: var(--dopa-gradient-sunset);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.dopa-hero p {
  font-size: 1.25rem;
  color: var(--dopa-text-muted);
  margin-bottom: 2.5rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

/* Decorative floating shapes */
.dopa-hero__blob {
  position: absolute;
  border-radius: 50%;
  opacity: 0.6;
  animation: float 6s ease-in-out infinite;
}

@keyframes float {
  0%, 100% { transform: translateY(0) rotate(0deg); }
  50% { transform: translateY(-20px) rotate(5deg); }
}
```

### Feature Grid

```css
.dopa-features {
  padding: 80px 40px;
}

.dopa-features__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  max-width: 1200px;
  margin: 0 auto;
}

.dopa-feature {
  border-radius: 24px;
  padding: 32px;
  text-align: left;
}

.dopa-feature__icon {
  width: 60px;
  height: 60px;
  border-radius: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.75rem;
  margin-bottom: 20px;
}

.dopa-feature h3 {
  font-size: 1.3rem;
  margin-bottom: 0.5rem;
}

.dopa-feature p {
  font-size: 0.95rem;
  color: var(--dopa-text-muted);
  line-height: 1.6;
}
```

### Decorative Shapes

```css
.dopa-shape {
  position: absolute;
  pointer-events: none;
}

.dopa-shape--circle {
  border-radius: 50%;
}

.dopa-shape--squiggle {
  width: 120px;
  height: 30px;
  background: repeating-linear-gradient(
    90deg,
    var(--dopa-yellow) 0px,
    var(--dopa-yellow) 15px,
    transparent 15px,
    transparent 30px
  );
  border-radius: 15px;
  transform: rotate(-15deg);
}

.dopa-shape--star {
  clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
}
```

---

## Design Do's and Don'ts

### Do

- Use at least 4-5 bold, saturated colors on a single page
- Make buttons oversized, rounded, and irresistibly clickable
- Add decorative shapes (blobs, squiggles, stars) as background flourishes
- Use color-blocked sections for strong visual rhythm
- Apply gradients generously on backgrounds, text, and shapes
- Let elements overlap, rotate, and break out of rigid grids
- Use chunky, rounded typography for headings
- Create hover animations that feel bouncy and playful

### Don't

- Use muted, desaturated, or earthy color palettes
- Keep layouts rigidly aligned and symmetrical -- embrace controlled chaos
- Use thin, elegant serif fonts -- they conflict with the bubbly energy
- Leave too much white space -- fill the page with color and life
- Use only one or two colors -- dopamine comes from abundance
- Skip accessibility: even maximalist design needs readable text contrast
- Make decorative elements so large they obscure content
- Forget mobile users -- playful design must still be functional

---

## Related Aesthetics

| Aesthetic | Relationship to Dopamine Design |
|-----------|-------------------------------|
| **Memphis Design** | Spiritual ancestor; 1980s movement with bold color, geometric shapes, and anti-minimalist attitude |
| **Gen Z Maximalism** | Contemporary sibling; shares the more-is-more philosophy with internet-native visual language |
| **Colorful Pop** | Directly related; both celebrate saturated color and graphic boldness |
| **Maximalism** | Parent philosophy; Dopamine Design applies maximalist principles specifically to digital interface design |
| **Flat Design** | Opposite philosophy; shares bold color use but rejects the decorative exuberance Dopamine Design embraces |
| **Cutecore** | Shares playful, joyful energy with a focus on kawaii-influenced rounded shapes and pastel-to-neon palette |
| **Bright Tertiaries** | Related color approach; both use vivid, unconventional color combinations for emotional impact |
| **Corporate Memphis** | Simplified cousin; uses flat illustration and color but with corporate restraint Dopamine Design rejects |
| **Acid Design** | Shares neon intensity and rule-breaking attitude but pushes toward unsettling rather than joyful |
| **Avant Basic** | Shares the bold, trend-driven approach but channels it through a fashion and lifestyle lens |

---

## Quick-Start: Minimal Dopamine Design Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dopamine Design Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --dopa-pink: #ff2d87;
      --dopa-purple: #7b2fff;
      --dopa-blue: #00b4ff;
      --dopa-yellow: #ffd000;
      --dopa-orange: #ff6b2b;
      --dopa-green: #00e5a0;
      --dopa-lavender: #c084fc;
      --dopa-lime: #b8ff00;
      --dopa-bg-dark: #1e0a3c;
      --dopa-bg-light: #fffbf5;
      --dopa-bg-cream: #fff3e0;
      --dopa-bg-violet: #f0e6ff;
      --dopa-text-dark: #1e0a3c;
      --dopa-text-muted: #7a6b8a;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--dopa-bg-light);
      color: var(--dopa-text-dark);
      font-family: 'Quicksand', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Fredoka', cursive;
      font-weight: 700;
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
    }

    nav a.logo {
      font-family: 'Fredoka', cursive;
      font-weight: 700;
      font-size: 1.5rem;
      color: var(--dopa-pink);
      text-decoration: none;
    }

    nav ul { display: flex; gap: 8px; list-style: none; }

    nav ul a {
      color: var(--dopa-text-dark);
      text-decoration: none;
      font-weight: 600;
      font-size: 0.95rem;
      padding: 8px 20px;
      border-radius: 50px;
      transition: background 0.2s, color 0.2s;
    }

    nav ul a:hover { background: var(--dopa-bg-violet); color: var(--dopa-purple); }

    /* Hero */
    .hero {
      position: relative;
      text-align: center;
      padding: 100px 40px 80px;
      overflow: hidden;
      background: var(--dopa-bg-cream);
      border-radius: 0 0 48px 48px;
    }

    .hero h1 {
      font-size: clamp(3rem, 7vw, 5rem);
      margin-bottom: 1rem;
      background: linear-gradient(135deg, var(--dopa-pink), var(--dopa-orange), var(--dopa-yellow));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero p {
      font-size: 1.2rem;
      color: var(--dopa-text-muted);
      margin-bottom: 2.5rem;
      max-width: 550px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: var(--dopa-pink);
      color: #fff;
      border: none;
      border-radius: 50px;
      padding: 16px 40px;
      font-family: 'Fredoka', cursive;
      font-weight: 600;
      font-size: 1.1rem;
      cursor: pointer;
      text-decoration: none;
      box-shadow: 0 4px 20px rgba(255, 45, 135, 0.3);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .btn:hover { transform: translateY(-3px) scale(1.02); box-shadow: 0 8px 30px rgba(255, 45, 135, 0.4); }

    /* Floating shapes */
    .blob {
      position: absolute;
      border-radius: 50%;
      animation: float 6s ease-in-out infinite;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-20px); }
    }

    /* Features */
    .features {
      padding: 80px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .features h2 { text-align: center; font-size: 2.5rem; margin-bottom: 48px; }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
    }

    .feature {
      border-radius: 24px;
      padding: 32px;
      transition: transform 0.3s;
    }

    .feature:hover { transform: translateY(-4px) rotate(1deg); }

    .feature:nth-child(1) { background: #ffe0ee; }
    .feature:nth-child(2) { background: #dff2ff; }
    .feature:nth-child(3) { background: #fff6d6; }

    .feature-icon {
      width: 56px;
      height: 56px;
      border-radius: 16px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 20px;
    }

    .feature h3 { font-size: 1.25rem; margin-bottom: 0.5rem; }
    .feature p { font-size: 0.95rem; color: var(--dopa-text-muted); }

    /* CTA */
    .cta {
      background: linear-gradient(135deg, var(--dopa-purple), var(--dopa-pink));
      color: #fff;
      text-align: center;
      padding: 80px 40px;
      border-radius: 48px;
      max-width: 1200px;
      margin: 0 auto 40px;
    }

    .cta h2 { font-size: 2.5rem; margin-bottom: 1rem; color: #fff; }
    .cta p { font-size: 1.1rem; opacity: 0.9; margin-bottom: 2rem; }
    .cta .btn { background: var(--dopa-yellow); color: var(--dopa-text-dark); box-shadow: 0 4px 20px rgba(255, 208, 0, 0.3); }

    /* Footer */
    footer {
      background: var(--dopa-bg-dark);
      color: var(--dopa-lavender);
      text-align: center;
      padding: 40px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .hero { padding: 60px 20px 50px; border-radius: 0 0 32px 32px; }
      nav { padding: 16px 20px; }
      nav ul { gap: 4px; }
      nav ul a { padding: 6px 14px; font-size: 0.85rem; }
      .cta { border-radius: 32px; margin: 0 16px 24px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Joyful</a>
    <ul>
      <li><a href="#">Create</a></li>
      <li><a href="#">Explore</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <!-- Decorative blobs -->
    <div class="blob" style="width:120px;height:120px;background:#ff2d87;opacity:0.15;top:10%;left:5%;"></div>
    <div class="blob" style="width:80px;height:80px;background:#7b2fff;opacity:0.15;top:20%;right:8%;animation-delay:-2s;"></div>
    <div class="blob" style="width:60px;height:60px;background:#ffd000;opacity:0.2;bottom:15%;left:12%;animation-delay:-4s;"></div>
    <div class="blob" style="width:100px;height:100px;background:#00e5a0;opacity:0.12;bottom:10%;right:15%;animation-delay:-1s;"></div>

    <h1>Design that makes you smile</h1>
    <p>Bold colors, playful shapes, and unabashed visual joy. Because life is too short for boring design.</p>
    <a href="#" class="btn">Start Creating</a>
  </section>

  <section class="features">
    <h2>Pure creative energy</h2>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon" style="background:var(--dopa-pink);">
          <svg width="28" height="28" viewBox="0 0 28 28"><circle cx="14" cy="14" r="10" fill="#fff"/><path d="M10 17 C10 17 12 13 14 13 C16 13 18 17 18 17" stroke="#ff2d87" stroke-width="2" fill="none" stroke-linecap="round"/><circle cx="10" cy="11" r="1.5" fill="#ff2d87"/><circle cx="18" cy="11" r="1.5" fill="#ff2d87"/></svg>
        </div>
        <h3>Instant Joy</h3>
        <p>Colors and shapes that trigger genuine positive emotions. Design that feels like a celebration.</p>
      </div>
      <div class="feature">
        <div class="feature-icon" style="background:var(--dopa-blue);">
          <svg width="28" height="28" viewBox="0 0 28 28"><rect x="4" y="4" width="20" height="20" rx="6" fill="#fff"/><circle cx="14" cy="14" r="5" fill="#00b4ff"/></svg>
        </div>
        <h3>Bold Expression</h3>
        <p>Break free from muted palettes and rigid grids. Express yourself with maximum visual impact.</p>
      </div>
      <div class="feature">
        <div class="feature-icon" style="background:var(--dopa-yellow);">
          <svg width="28" height="28" viewBox="0 0 28 28"><polygon points="14,2 17.5,10 26,10 19.5,15.5 22,24 14,19 6,24 8.5,15.5 2,10 10.5,10" fill="#fff"/></svg>
        </div>
        <h3>Stand Out</h3>
        <p>In a sea of minimalism, dopamine design demands attention and leaves a lasting impression.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Ready to inject some joy?</h2>
    <p>Join thousands of creators who believe design should make people happy.</p>
    <a href="#" class="btn">Get Started Free</a>
  </section>

  <footer>
    <p>Built with Dopamine Design principles. Bold, playful, joyful.</p>
  </footer>
</body>
</html>
```
