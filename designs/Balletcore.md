# Balletcore Design Reference

## Overview

Balletcore is a soft, graceful aesthetic inspired by the world of classical and contemporary ballet. Rooted in the visual language of dance studios, rehearsals, and stage performances, it celebrates femininity, discipline, and ethereal beauty through delicate materials like tulle, satin, chiffon, and lace. The aesthetic emerged on TikTok in the early 2020s, gaining mainstream momentum after Miu Miu's Fall/Winter 2022 collection reintroduced ballet flats and dancewear silhouettes to high fashion, while designers like Simone Rocha reinforced the trend through consistent use of tulle and pearls. In web and UI design, Balletcore translates into airy, light-filled interfaces with blush and nude palettes, elongated serif typography that echoes the long lines of a dancer's body, generous white space reminiscent of a bright studio, and fluid motion through subtle CSS animations. The result is a digital experience that feels poised, intimate, and weightlessly elegant — as if the interface itself is en pointe.

---

## Visual Characteristics

### Core Design Traits

- **Satin and silk textures**: Smooth, luminous surface treatments with subtle sheen gradients that evoke the look of satin pointe shoes and ribbons
- **Tulle and chiffon layering**: Semi-transparent overlays, frosted panels, and layered translucent elements that mimic the gauzy layers of a ballet tutu
- **Ribbon and bow motifs**: Thin, elegant ribbon shapes used as decorative accents, dividers, and navigation highlights — more refined and restrained than Coquette's ornamental bows
- **Barre and mirror references**: Clean horizontal lines, reflective surfaces, and mirrored gradients that recall the ballet studio environment
- **Soft pink and nude palette**: A tonal range anchored in ballet pink, blush, champagne, and warm ivory — the colors of pointe shoes, leotards, and stage lighting
- **Elongated proportions**: Tall, narrow containers, stretched vertical layouts, and generous line-height that echo the extended lines of a dancer's posture
- **Fluid motion and transitions**: Gentle CSS animations, smooth hover states, and ease-in-out curves that replicate the controlled grace of ballet movement
- **Pointe shoe and slipper imagery**: Iconic ballet footwear shapes referenced in rounded-bottom cards, lace-up decorative details, and ribbon-tie visual elements
- **Warm stage lighting effects**: Soft radial gradients and warm glows that simulate the amber and rose-tinted wash of theatrical spotlights
- **Disciplined minimalism**: Despite its decorative nature, Balletcore maintains a sense of control and restraint — every element is placed with intention, like choreography

### Design Principles

- Embrace the tension between softness and discipline: every visual element should feel both delicate and deliberate
- Use vertical space generously to create the sense of height and elongation central to ballet's visual language
- Layer translucent elements to build depth without weight, like tulle over skin
- Maintain a tonal palette rather than high-contrast color pairings; let values shift gently
- Animate sparingly but gracefully — transitions should feel like movements, not jumps
- Treat negative space as the visual equivalent of silence between musical phrases
- Let typography carry the elegance: favor refined serifs and fluid italics over heavy decorative scripts

---

## Color Palette

| Swatch | Hex | Role / Usage |
|--------|-----|-------------|
| Ballet Pink | `#F2D1CB` | Primary brand color, hero backgrounds, key accent |
| Pointe Satin | `#FDEEF4` | Card surfaces, soft panel fills |
| Blush Tulle | `#F8E0E6` | Secondary backgrounds, hover states |
| Warm Ivory | `#FFF8F3` | Page background, primary canvas |
| Studio White | `#FFFBF8` | Bright white space, clean sections |
| Champagne Silk | `#F7E7CE` | Warm neutral accent, secondary cards |
| Dusty Rose | `#D4A5A5` | Muted text accents, secondary headings |
| Stage Mauve | `#C9929D` | Interactive element accents, borders |
| Ribbon Pink | `#E8A0B5` | Buttons, call-to-action elements |
| Chiffon Lavender | `#E6D5E8` | Tertiary decorative accent, tags |
| Leotard Nude | `#EDBBA8` | Warm accent, illustration fills |
| Barre Charcoal | `#5C4A4F` | Primary text, headings on light backgrounds |
| Spotlight Gold | `#D4B896` | Metallic accents, premium highlights |
| Rehearsal Gray | `#B8A9AC` | Disabled states, subtle borders, captions |
| Curtain Burgundy | `#7A3B4E` | Dark accent for emphasis, footer backgrounds |

### CSS Custom Properties

```css
:root {
  --ballet-pink: #F2D1CB;
  --ballet-pointe-satin: #FDEEF4;
  --ballet-blush-tulle: #F8E0E6;
  --ballet-warm-ivory: #FFF8F3;
  --ballet-studio-white: #FFFBF8;
  --ballet-champagne-silk: #F7E7CE;
  --ballet-dusty-rose: #D4A5A5;
  --ballet-stage-mauve: #C9929D;
  --ballet-ribbon-pink: #E8A0B5;
  --ballet-chiffon-lavender: #E6D5E8;
  --ballet-leotard-nude: #EDBBA8;
  --ballet-barre-charcoal: #5C4A4F;
  --ballet-spotlight-gold: #D4B896;
  --ballet-rehearsal-gray: #B8A9AC;
  --ballet-curtain-burgundy: #7A3B4E;
}
```

---

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Cormorant Garamond** | 300, 400, 500, 600 | Primary heading font; high-contrast serif with elongated proportions | [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) |
| **Libre Baskerville** | 400, 400i, 700 | Body text; elegant, readable serif with classical refinement | [Libre Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) |
| **Josefin Sans** | 200, 300, 400, 600 | UI elements, navigation, and captions; geometric sans with vintage grace | [Josefin Sans](https://fonts.google.com/specimen/Josefin+Sans) |
| **Italiana** | 400 | Display headings; tall, narrow letterforms that mirror a dancer's posture | [Italiana](https://fonts.google.com/specimen/Italiana) |
| **Dancing Script** | 400, 500, 600, 700 | Decorative accents and pull quotes; fluid cursive with natural rhythm | [Dancing Script](https://fonts.google.com/specimen/Dancing+Script) |
| **Tenor Sans** | 400 | Subheadings and labels; clean sans-serif with classical proportions | [Tenor Sans](https://fonts.google.com/specimen/Tenor+Sans) |
| **Lora** | 400, 500, 600, 700 | Alternative body serif; refined with subtle brush contrast | [Lora](https://fonts.google.com/specimen/Lora) |
| **Playfair Display** | 400, 500, 600, 700 | Alternative display heading; high-contrast transitional serif | [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Cormorant Garamond 300 | Libre Baskerville 400 | Airy elegance, classical poise |
| Italiana 400 | Josefin Sans 300 | Tall and refined, modern ballet program |
| Playfair Display 500 italic | Lora 400 | Romantic editorial, warm sophistication |
| Cormorant Garamond 600 | Tenor Sans 400 | Structured grace, studio formality |
| Dancing Script 500 | Josefin Sans 400 | Whimsical movement, rehearsal journal |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Josefin+Sans:wght@200;300;400;600&family=Dancing+Script:wght@400;500;600&display=swap');

body {
  font-family: 'Libre Baskerville', 'Georgia', serif;
  font-size: 1.05rem;
  line-height: 1.85;
  color: var(--ballet-barre-charcoal);
  background: var(--ballet-warm-ivory);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Cormorant Garamond', 'Garamond', serif;
  font-weight: 300;
  letter-spacing: 0.04em;
  line-height: 1.3;
  color: var(--ballet-curtain-burgundy);
}

h1 {
  font-size: 3.2rem;
  font-style: italic;
}

h2 {
  font-size: 2rem;
  font-weight: 400;
}

.nav-link {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 300;
  font-size: 0.8rem;
  letter-spacing: 0.18em;
  text-transform: uppercase;
}

.script-accent {
  font-family: 'Dancing Script', cursive;
  font-size: 1.6rem;
  color: var(--ballet-ribbon-pink);
}
```

---

## Layout Principles

- **Tall, centered compositions**: Use narrow content columns (600-780px max-width) to create a vertical, portrait-oriented reading experience that mirrors the upright posture of a dancer
- **Generous vertical spacing**: Allow 80-120px between major sections; the rhythm of space creates visual breathing room, like rests in a musical score
- **Asymmetric grace**: Offset images and decorative elements slightly from center to create the elegant asymmetry of a ballet pose (arabesque, attitude)
- **Layered translucency**: Stack semi-transparent panels and overlays to create depth reminiscent of tulle layers, using rgba values with low alpha
- **Horizontal barre lines**: Use thin horizontal rules (1px, low-opacity pinks) as section dividers that reference the ballet barre — clean, structural, and understated
- **Full-bleed imagery with soft overlays**: Hero images and feature photos extend edge-to-edge but are softened with gradient overlays in warm ivory or blush
- **Responsive fluidity**: On smaller screens, maintain the vertical emphasis and tonal softness; collapse grid layouts to single columns and increase line-height for readability
- **Card elevation through glow**: Prefer soft, warm-toned box-shadows over sharp drop-shadows; cards should appear to float on a cushion of light rather than casting hard edges

---

## CSS / Design Techniques

### Satin Card

```css
.ballet-card {
  background: linear-gradient(135deg, var(--ballet-pointe-satin) 0%, var(--ballet-warm-ivory) 100%);
  border: 1px solid rgba(232, 160, 181, 0.20);
  border-radius: 20px;
  padding: 40px 36px;
  box-shadow:
    0 8px 32px rgba(242, 209, 203, 0.30),
    0 2px 8px rgba(92, 74, 79, 0.04);
  transition: transform 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94),
              box-shadow 0.4s ease;
}

.ballet-card:hover {
  transform: translateY(-4px);
  box-shadow:
    0 12px 40px rgba(242, 209, 203, 0.40),
    0 4px 12px rgba(92, 74, 79, 0.06);
}

.ballet-card h3 {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 400;
  font-size: 1.5rem;
  color: var(--ballet-curtain-burgundy);
  margin-bottom: 12px;
}

.ballet-card p {
  color: var(--ballet-barre-charcoal);
  font-size: 0.95rem;
  line-height: 1.8;
}
```

### Ribbon Button

```css
.ballet-button {
  background: linear-gradient(135deg, var(--ballet-ribbon-pink) 0%, var(--ballet-stage-mauve) 100%);
  color: var(--ballet-studio-white);
  border: none;
  border-radius: 50px;
  padding: 14px 40px;
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 400;
  font-size: 0.8rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  cursor: pointer;
  box-shadow: 0 4px 20px rgba(232, 160, 181, 0.35);
  transition: all 0.35s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  position: relative;
  overflow: hidden;
}

.ballet-button::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.15), transparent);
  transition: left 0.5s ease;
}

.ballet-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 28px rgba(232, 160, 181, 0.50);
}

.ballet-button:hover::before {
  left: 100%;
}
```

### Studio Navigation Bar

```css
.ballet-nav {
  background: rgba(255, 248, 243, 0.95);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(212, 165, 165, 0.15);
  padding: 24px 48px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: sticky;
  top: 0;
  z-index: 100;
}

.ballet-nav .logo {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 300;
  font-size: 1.4rem;
  letter-spacing: 0.08em;
  color: var(--ballet-curtain-burgundy);
  text-decoration: none;
}

.ballet-nav .links {
  display: flex;
  gap: 36px;
  align-items: center;
}

.ballet-nav .links a {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 300;
  font-size: 0.75rem;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  text-decoration: none;
  color: var(--ballet-barre-charcoal);
  position: relative;
  transition: color 0.3s ease;
}

.ballet-nav .links a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 50%;
  width: 0;
  height: 1px;
  background: var(--ballet-ribbon-pink);
  transition: width 0.3s ease, left 0.3s ease;
}

.ballet-nav .links a:hover {
  color: var(--ballet-curtain-burgundy);
}

.ballet-nav .links a:hover::after {
  width: 100%;
  left: 0;
}
```

### Ethereal Hero Section

```css
.ballet-hero {
  background: linear-gradient(
    180deg,
    var(--ballet-pointe-satin) 0%,
    var(--ballet-blush-tulle) 40%,
    var(--ballet-warm-ivory) 100%
  );
  text-align: center;
  padding: 140px 40px 120px;
  position: relative;
  overflow: hidden;
}

.ballet-hero::before {
  content: '';
  position: absolute;
  top: -30%;
  left: 50%;
  transform: translateX(-50%);
  width: 120%;
  height: 120%;
  background: radial-gradient(
    ellipse at 50% 40%,
    rgba(242, 209, 203, 0.30) 0%,
    transparent 55%
  );
  pointer-events: none;
}

.ballet-hero::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 1px;
  background: linear-gradient(
    to right,
    transparent,
    var(--ballet-dusty-rose),
    transparent
  );
}

.ballet-hero h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 4rem;
  font-weight: 300;
  font-style: italic;
  color: var(--ballet-curtain-burgundy);
  position: relative;
  margin-bottom: 16px;
}

.ballet-hero .subtitle {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 200;
  font-size: 0.85rem;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: var(--ballet-stage-mauve);
  position: relative;
}

.ballet-hero .description {
  max-width: 520px;
  margin: 24px auto 0;
  font-family: 'Libre Baskerville', serif;
  font-size: 1rem;
  line-height: 1.9;
  color: var(--ballet-barre-charcoal);
  position: relative;
}
```

### Tulle Overlay Panel

```css
.ballet-tulle-panel {
  background: rgba(253, 238, 244, 0.45);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  border: 1px solid rgba(232, 160, 181, 0.12);
  border-radius: 16px;
  padding: 48px 40px;
  position: relative;
}

.ballet-tulle-panel::before {
  content: '';
  position: absolute;
  inset: 0;
  border-radius: 16px;
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.20) 0%,
    rgba(248, 224, 230, 0.08) 50%,
    rgba(255, 255, 255, 0.15) 100%
  );
  pointer-events: none;
}

.ballet-tulle-panel > * {
  position: relative;
  z-index: 1;
}
```

### Barre Divider

```css
.ballet-barre-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
  margin: 64px auto;
  max-width: 400px;
}

.ballet-barre-divider::before,
.ballet-barre-divider::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(
    to var(--direction, right),
    transparent,
    var(--ballet-dusty-rose)
  );
}

.ballet-barre-divider::before {
  --direction: right;
}

.ballet-barre-divider::after {
  --direction: left;
}

.ballet-barre-divider .ornament {
  width: 6px;
  height: 6px;
  background: var(--ballet-ribbon-pink);
  border-radius: 50%;
  box-shadow: 0 0 8px rgba(232, 160, 181, 0.40);
}
```

### Pointe Shoe Lace-Up Detail

```css
.ballet-laceup {
  position: relative;
  padding-left: 32px;
  margin: 24px 0;
}

.ballet-laceup::before {
  content: '';
  position: absolute;
  left: 12px;
  top: 0;
  bottom: 0;
  width: 1px;
  background: repeating-linear-gradient(
    to bottom,
    var(--ballet-ribbon-pink) 0px,
    var(--ballet-ribbon-pink) 8px,
    transparent 8px,
    transparent 16px
  );
}

.ballet-laceup::after {
  content: '';
  position: absolute;
  left: 8px;
  top: 4px;
  width: 9px;
  height: 9px;
  border: 1.5px solid var(--ballet-ribbon-pink);
  border-radius: 50%;
  background: var(--ballet-warm-ivory);
}

.ballet-laceup li {
  list-style: none;
  padding: 8px 0;
  font-family: 'Libre Baskerville', serif;
  font-size: 0.95rem;
  color: var(--ballet-barre-charcoal);
  line-height: 1.7;
}
```

---

## Design Do's and Don'ts

### Do

- Use a tonal palette that stays within the blush-pink-to-ivory range, shifting values subtly rather than introducing competing hues
- Favor light font weights (300, 400) for headings to maintain the sense of weightlessness and elongation
- Apply smooth, long-duration transitions (0.3-0.5s) with ease-in-out or cubic-bezier curves that mimic graceful movement
- Use generous padding and margin to create breathing room — negative space is as important as content
- Layer semi-transparent elements (tulle panels, frosted overlays) to build soft visual depth
- Include thin horizontal rules as structural barre references between sections
- Treat imagery with warm, soft-focus overlays that evoke stage lighting
- Use rounded corners (16-24px) for cards and panels to maintain the softness of the aesthetic
- Let italic serif headings carry the expressive elegance of the design

### Don't

- Use sharp geometric angles, hard borders, or boxy containers that contradict the fluid grace of ballet
- Apply heavy, bold font weights for headings — this breaks the lightness and elongated feel
- Use saturated neon or primary colors that shatter the tonal blush palette
- Add aggressive animations, bounces, or jarring transitions — all motion should feel controlled and deliberate
- Overuse script or cursive fonts; reserve them for small decorative accents to avoid illegibility
- Create dense, cluttered layouts — Balletcore demands the discipline of simplicity and intentional placement
- Mix with grunge, brutalist, cyberpunk, or industrial aesthetics that fundamentally oppose its graceful philosophy
- Use pure black (#000000) for text; opt for warm charcoal tones instead
- Apply heavy drop shadows or dark overlays that add visual weight

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Coquette** | Closest sibling; both are hyper-feminine with pink palettes, but Coquette leans more Rococo-ornamental with bows and pearls, while Balletcore is more athletic, disciplined, and studio-inspired |
| **Danish Pastel** | Shares the soft pastel palette and gentle aesthetic, but Danish Pastel is more playful and graphic with checks and daisies versus Balletcore's fluid elegance |
| **Cottagecore** | Both celebrate femininity and softness; Cottagecore is rustic and pastoral while Balletcore is urban, polished, and performative |
| **Light Academia** | Overlaps in warmth and classical refinement; Light Academia draws from literary and scholarly traditions while Balletcore draws from movement and performance |
| **Glassmorphism** | Shares the translucent, frosted layering approach; Glassmorphism is more tech-oriented while Balletcore uses the technique to evoke tulle and chiffon |
| **Grandmillennial** | Both embrace traditional femininity and refined aesthetics, but Grandmillennial is more rooted in interior decor, wallpaper patterns, and grandmother-chic |
| **Fairycore** | Shares ethereal lightness and soft palettes, but Fairycore is more fantastical and nature-infused while Balletcore is grounded in human artistry and discipline |
| **Art Nouveau** | Both value flowing organic curves and elegant form; Art Nouveau is more botanical and architectural while Balletcore is kinetic and body-centered |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Balletcore — Grace in Every Detail</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Josefin+Sans:wght@200;300;400;600&family=Dancing+Script:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      --ballet-pink: #F2D1CB;
      --ballet-pointe-satin: #FDEEF4;
      --ballet-blush-tulle: #F8E0E6;
      --ballet-warm-ivory: #FFF8F3;
      --ballet-studio-white: #FFFBF8;
      --ballet-champagne-silk: #F7E7CE;
      --ballet-dusty-rose: #D4A5A5;
      --ballet-stage-mauve: #C9929D;
      --ballet-ribbon-pink: #E8A0B5;
      --ballet-chiffon-lavender: #E6D5E8;
      --ballet-leotard-nude: #EDBBA8;
      --ballet-barre-charcoal: #5C4A4F;
      --ballet-spotlight-gold: #D4B896;
      --ballet-rehearsal-gray: #B8A9AC;
      --ballet-curtain-burgundy: #7A3B4E;
    }

    body {
      font-family: 'Libre Baskerville', Georgia, serif;
      font-size: 1.05rem;
      line-height: 1.85;
      color: var(--ballet-barre-charcoal);
      background: var(--ballet-warm-ivory);
      min-height: 100vh;
      -webkit-font-smoothing: antialiased;
    }

    /* ---- Navigation ---- */
    .nav {
      background: rgba(255, 248, 243, 0.95);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(212, 165, 165, 0.15);
      padding: 22px 48px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav .logo {
      font-family: 'Cormorant Garamond', serif;
      font-weight: 300;
      font-size: 1.4rem;
      letter-spacing: 0.08em;
      color: var(--ballet-curtain-burgundy);
      text-decoration: none;
    }

    .nav .logo em {
      font-style: italic;
    }

    .nav .links {
      display: flex;
      gap: 36px;
      align-items: center;
    }

    .nav .links a {
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 300;
      font-size: 0.72rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      text-decoration: none;
      color: var(--ballet-barre-charcoal);
      position: relative;
      transition: color 0.3s ease;
    }

    .nav .links a::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 50%;
      width: 0;
      height: 1px;
      background: var(--ballet-ribbon-pink);
      transition: width 0.3s ease, left 0.3s ease;
    }

    .nav .links a:hover {
      color: var(--ballet-curtain-burgundy);
    }

    .nav .links a:hover::after {
      width: 100%;
      left: 0;
    }

    /* ---- Hero Section ---- */
    .hero {
      background: linear-gradient(
        180deg,
        var(--ballet-pointe-satin) 0%,
        var(--ballet-blush-tulle) 40%,
        var(--ballet-warm-ivory) 100%
      );
      text-align: center;
      padding: 140px 40px 120px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: -30%;
      left: 50%;
      transform: translateX(-50%);
      width: 120%;
      height: 120%;
      background: radial-gradient(
        ellipse at 50% 40%,
        rgba(242, 209, 203, 0.30) 0%,
        transparent 55%
      );
      pointer-events: none;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 1px;
      background: linear-gradient(to right, transparent, var(--ballet-dusty-rose), transparent);
    }

    .hero .overline {
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 200;
      font-size: 0.8rem;
      letter-spacing: 0.3em;
      text-transform: uppercase;
      color: var(--ballet-stage-mauve);
      position: relative;
      display: block;
      margin-bottom: 12px;
    }

    .hero h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 4.2rem;
      font-weight: 300;
      font-style: italic;
      color: var(--ballet-curtain-burgundy);
      position: relative;
      line-height: 1.15;
      margin-bottom: 20px;
    }

    .hero p {
      max-width: 500px;
      margin: 0 auto 36px;
      font-size: 0.95rem;
      color: var(--ballet-barre-charcoal);
      position: relative;
      line-height: 1.9;
    }

    .hero .btn {
      display: inline-block;
      background: linear-gradient(135deg, var(--ballet-ribbon-pink) 0%, var(--ballet-stage-mauve) 100%);
      color: var(--ballet-studio-white);
      border: none;
      border-radius: 50px;
      padding: 14px 44px;
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 400;
      font-size: 0.75rem;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 0 4px 20px rgba(232, 160, 181, 0.35);
      transition: all 0.35s cubic-bezier(0.25, 0.46, 0.45, 0.94);
      position: relative;
      overflow: hidden;
    }

    .hero .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 28px rgba(232, 160, 181, 0.50);
    }

    /* ---- Barre Divider ---- */
    .barre-divider {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      margin: 0 auto;
      max-width: 300px;
      padding: 64px 0;
    }

    .barre-divider::before,
    .barre-divider::after {
      content: '';
      flex: 1;
      height: 1px;
    }

    .barre-divider::before {
      background: linear-gradient(to right, transparent, var(--ballet-dusty-rose));
    }

    .barre-divider::after {
      background: linear-gradient(to left, transparent, var(--ballet-dusty-rose));
    }

    .barre-divider span {
      width: 6px;
      height: 6px;
      background: var(--ballet-ribbon-pink);
      border-radius: 50%;
      box-shadow: 0 0 8px rgba(232, 160, 181, 0.40);
    }

    /* ---- Section Title ---- */
    .section-title {
      text-align: center;
      margin-bottom: 48px;
    }

    .section-title .script-label {
      font-family: 'Dancing Script', cursive;
      font-size: 1.4rem;
      color: var(--ballet-ribbon-pink);
      display: block;
      margin-bottom: 4px;
    }

    .section-title h2 {
      font-family: 'Cormorant Garamond', serif;
      font-weight: 400;
      font-size: 2.2rem;
      color: var(--ballet-curtain-burgundy);
      letter-spacing: 0.03em;
    }

    /* ---- Card Grid ---- */
    .card-grid {
      max-width: 900px;
      margin: 0 auto;
      padding: 0 40px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 32px;
    }

    .card {
      background: linear-gradient(135deg, var(--ballet-pointe-satin) 0%, var(--ballet-warm-ivory) 100%);
      border: 1px solid rgba(232, 160, 181, 0.18);
      border-radius: 20px;
      padding: 40px 32px;
      box-shadow:
        0 8px 32px rgba(242, 209, 203, 0.25),
        0 2px 8px rgba(92, 74, 79, 0.04);
      transition: transform 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94),
                  box-shadow 0.4s ease;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow:
        0 12px 40px rgba(242, 209, 203, 0.40),
        0 4px 12px rgba(92, 74, 79, 0.06);
    }

    .card .card-icon {
      font-size: 2rem;
      margin-bottom: 16px;
      display: block;
    }

    .card h3 {
      font-family: 'Cormorant Garamond', serif;
      font-weight: 500;
      font-size: 1.4rem;
      color: var(--ballet-curtain-burgundy);
      margin-bottom: 12px;
    }

    .card p {
      font-size: 0.9rem;
      line-height: 1.8;
      color: var(--ballet-barre-charcoal);
    }

    /* ---- Tulle Feature Panel ---- */
    .tulle-panel {
      max-width: 720px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .tulle-panel-inner {
      background: rgba(253, 238, 244, 0.45);
      backdrop-filter: blur(8px);
      -webkit-backdrop-filter: blur(8px);
      border: 1px solid rgba(232, 160, 181, 0.12);
      border-radius: 24px;
      padding: 56px 48px;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .tulle-panel-inner::before {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: 24px;
      background: linear-gradient(
        135deg,
        rgba(255, 255, 255, 0.20) 0%,
        rgba(248, 224, 230, 0.08) 50%,
        rgba(255, 255, 255, 0.15) 100%
      );
      pointer-events: none;
    }

    .tulle-panel-inner blockquote {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.6rem;
      font-weight: 300;
      font-style: italic;
      color: var(--ballet-curtain-burgundy);
      line-height: 1.6;
      position: relative;
      z-index: 1;
      margin-bottom: 16px;
    }

    .tulle-panel-inner cite {
      font-family: 'Josefin Sans', sans-serif;
      font-style: normal;
      font-weight: 300;
      font-size: 0.75rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--ballet-stage-mauve);
      position: relative;
      z-index: 1;
    }

    /* ---- Rehearsal List ---- */
    .rehearsal-list {
      max-width: 600px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .rehearsal-list ul {
      position: relative;
      padding-left: 32px;
    }

    .rehearsal-list ul::before {
      content: '';
      position: absolute;
      left: 12px;
      top: 0;
      bottom: 0;
      width: 1px;
      background: repeating-linear-gradient(
        to bottom,
        var(--ballet-ribbon-pink) 0px,
        var(--ballet-ribbon-pink) 8px,
        transparent 8px,
        transparent 16px
      );
    }

    .rehearsal-list li {
      list-style: none;
      padding: 10px 0 10px 8px;
      font-size: 0.95rem;
      color: var(--ballet-barre-charcoal);
      line-height: 1.7;
      position: relative;
    }

    .rehearsal-list li::before {
      content: '';
      position: absolute;
      left: -24px;
      top: 50%;
      transform: translateY(-50%);
      width: 7px;
      height: 7px;
      border: 1.5px solid var(--ballet-ribbon-pink);
      border-radius: 50%;
      background: var(--ballet-warm-ivory);
    }

    /* ---- Footer ---- */
    .footer {
      background: var(--ballet-curtain-burgundy);
      color: rgba(255, 248, 243, 0.7);
      text-align: center;
      padding: 48px 40px;
      margin-top: 80px;
    }

    .footer .footer-brand {
      font-family: 'Cormorant Garamond', serif;
      font-weight: 300;
      font-size: 1.3rem;
      font-style: italic;
      color: var(--ballet-ballet-pink, #F2D1CB);
      margin-bottom: 12px;
    }

    .footer p {
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 300;
      font-size: 0.7rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
    }

    .footer .footer-links {
      margin-top: 20px;
      display: flex;
      justify-content: center;
      gap: 24px;
    }

    .footer .footer-links a {
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 300;
      font-size: 0.68rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: rgba(255, 248, 243, 0.5);
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .footer .footer-links a:hover {
      color: var(--ballet-pink);
    }

    /* ---- Responsive ---- */
    @media (max-width: 768px) {
      .nav {
        padding: 18px 24px;
      }

      .nav .links {
        gap: 20px;
      }

      .nav .links a {
        font-size: 0.65rem;
        letter-spacing: 0.12em;
      }

      .hero {
        padding: 100px 24px 80px;
      }

      .hero h1 {
        font-size: 2.8rem;
      }

      .card-grid {
        padding: 0 24px;
        grid-template-columns: 1fr;
      }

      .tulle-panel {
        padding: 0 24px;
      }

      .tulle-panel-inner {
        padding: 40px 28px;
      }

      .tulle-panel-inner blockquote {
        font-size: 1.3rem;
      }

      .rehearsal-list {
        padding: 0 24px;
      }

      .footer .footer-links {
        flex-direction: column;
        gap: 12px;
      }
    }

    @media (max-width: 480px) {
      .nav .links {
        gap: 14px;
      }

      .hero h1 {
        font-size: 2.2rem;
      }

      .hero .overline {
        font-size: 0.7rem;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav class="nav">
    <a href="#" class="logo"><em>Balletcore</em></a>
    <div class="links">
      <a href="#">Studio</a>
      <a href="#">Collection</a>
      <a href="#">Movement</a>
      <a href="#">About</a>
    </div>
  </nav>

  <!-- Hero Section -->
  <header class="hero">
    <span class="overline">An Aesthetic of Grace</span>
    <h1>Balletcore</h1>
    <p>Satin, tulle, and the quiet discipline of movement — where every detail is a gesture and every space breathes like a studio before curtain rise.</p>
    <a href="#" class="btn">Enter the Studio</a>
  </header>

  <!-- Divider -->
  <div class="barre-divider"><span></span></div>

  <!-- Cards Section -->
  <section>
    <div class="section-title">
      <span class="script-label">The Elements</span>
      <h2>Core Inspirations</h2>
    </div>
    <div class="card-grid">
      <div class="card">
        <span class="card-icon">&#129526;</span>
        <h3>Satin &amp; Ribbon</h3>
        <p>The luminous sheen of satin pointe shoes and the graceful wrap of ribbons lacing up the ankle — smooth, tactile, and deeply personal.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#9728;&#65039;</span>
        <h3>Stage Light</h3>
        <p>Warm amber and rose washes that transform the studio into a dream. Soft gradients and gentle glows that frame without overwhelming.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#127932;</span>
        <h3>Tulle Layers</h3>
        <p>Translucent, weightless, and endlessly layerable. Tulle brings depth through subtlety, each layer softening the one beneath it.</p>
      </div>
    </div>
  </section>

  <!-- Divider -->
  <div class="barre-divider"><span></span></div>

  <!-- Quote Panel -->
  <section>
    <div class="tulle-panel">
      <div class="tulle-panel-inner">
        <blockquote>The body says what words cannot.</blockquote>
        <cite>Martha Graham</cite>
      </div>
    </div>
  </section>

  <!-- Divider -->
  <div class="barre-divider"><span></span></div>

  <!-- Rehearsal List Section -->
  <section>
    <div class="section-title">
      <span class="script-label">The Practice</span>
      <h2>Design Principles</h2>
    </div>
    <div class="rehearsal-list">
      <ul>
        <li>Let every element breathe — generous white space is the silence between movements</li>
        <li>Build depth through translucency rather than shadow, like tulle over warm skin</li>
        <li>Choose elongated, light-weight typography that echoes the lines of a dancer</li>
        <li>Animate with intention — smooth, controlled transitions that feel choreographed</li>
        <li>Maintain a tonal palette; let values shift gently like light across a studio floor</li>
        <li>Balance softness with discipline — Balletcore is romantic, but never careless</li>
      </ul>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="footer-brand">Balletcore</div>
    <p>Grace in every pixel</p>
    <div class="footer-links">
      <a href="#">Studio</a>
      <a href="#">Collection</a>
      <a href="#">Movement</a>
      <a href="#">About</a>
    </div>
  </footer>

</body>
</html>
```
