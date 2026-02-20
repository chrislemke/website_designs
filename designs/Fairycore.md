# Fairycore

## Overview

Fairycore is a dreamy, nature-enchanted aesthetic that romanticizes the mythology of fairies, woodland spirits, and the hidden magic of the natural world. It conjures an atmosphere of enchanted forests, dew-kissed moss, luminous fireflies drifting through twilight glades, delicate fairy wings, and mushroom-dotted clearings bathed in soft golden light. In digital design, Fairycore translates into ethereal soft-focus visuals, shimmering particle effects, pastel-and-earth color palettes, translucent layering, and typography that feels hand-lettered by woodland creatures. Every element should evoke a sense of gentle wonder, as if the viewer has stumbled into a secret glen where the boundary between the natural and the magical has dissolved entirely.

## Visual Characteristics

### Core Design Traits

- **Ethereal soft focus**: Backgrounds and decorative imagery employ gaussian blur, soft glows, and diffused lighting to create a dreamlike, out-of-focus atmosphere reminiscent of early morning mist in a forest
- **Bioluminescent accents**: Subtle glowing elements such as firefly particles, dewdrop highlights, and faint luminous trails suggest hidden magic woven through the interface
- **Organic layering and transparency**: Overlapping translucent shapes, frosted glass panels, and layered botanical silhouettes create a sense of depth and enchantment
- **Mushroom and moss motifs**: Toadstools, bracket fungi, lichen textures, and mossy surfaces serve as recurring decorative elements and visual anchors
- **Fairy wing iridescence**: Delicate iridescent shimmer effects on borders, hover states, and decorative accents that catch the light like dragonfly or fairy wings
- **Woodland flora and fauna**: Ferns, wildflowers, trailing ivy, butterflies, moths, rabbits, and deer as illustrative elements throughout the layout
- **Sparkle and pixie dust effects**: Subtle CSS particle animations, star-shaped glints, and shimmering gradients that evoke scattered fairy dust
- **Dewdrop and water highlights**: Small circular highlights and radial gradients that mimic water droplets resting on leaves and petals

### Design Principles

- **Whispered enchantment**: Magic should feel gentle and discovered, never loud or forced; subtlety is the hallmark of true Fairycore
- **Nature as architecture**: Let organic forms define the structure; curves of branches, arcs of fern fronds, and the spirals of unfurling leaves should guide layout decisions
- **Layered depth**: Build visual depth through translucency, overlapping elements, and soft shadows to create the feeling of peering through forest canopy layers
- **Luminous warmth**: Even in cool greens and purples, maintain an underlying warmth through golden highlights and soft amber glows
- **Imperfect beauty**: Embrace organic asymmetry and natural irregularity over rigid geometric precision
- **Seasonal stillness**: The design should feel timeless and unhurried, like a perpetual golden hour in an ancient woodland

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Moonlit Cream | `#F5F0E8` | Primary background |
| Morning Mist | `#EDE8E0` | Card / surface background |
| Moss Green | `#6B8F6B` | Primary accent |
| Fern Shadow | `#4A7453` | Dark green accent |
| Dewdrop Lilac | `#B8A5CC` | Secondary accent |
| Toadstool Rose | `#C4917E` | Warm highlight |
| Firefly Gold | `#D4B96A` | Luminous accent / glow |
| Fairy Wing Pink | `#E0C4D0` | Tertiary accent |
| Twilight Lavender | `#8E7BA8` | Interactive elements |
| Bark Brown | `#5C4A3A` | Primary text |
| Cobweb Silver | `#C8C4BE` | Muted borders / dividers |
| Enchanted Teal | `#6A9E9E` | Alternate accent |
| Mushroom Beige | `#D5C8B5` | Alternate surface |
| Foxglove Purple | `#9B6B8A` | Highlight accent |
| Canopy Dark | `#2E3D2E` | Deep contrast / footer |
| Petal White | `#FAF7F2` | Highlight background |

### CSS Custom Properties

```css
:root {
  --fc-cream: #F5F0E8;
  --fc-mist: #EDE8E0;
  --fc-moss: #6B8F6B;
  --fc-fern: #4A7453;
  --fc-lilac: #B8A5CC;
  --fc-toadstool: #C4917E;
  --fc-firefly: #D4B96A;
  --fc-wing-pink: #E0C4D0;
  --fc-twilight: #8E7BA8;
  --fc-bark: #5C4A3A;
  --fc-cobweb: #C8C4BE;
  --fc-teal: #6A9E9E;
  --fc-mushroom: #D5C8B5;
  --fc-foxglove: #9B6B8A;
  --fc-canopy: #2E3D2E;
  --fc-petal: #FAF7F2;
}
```

## Typography

### Typeface Characteristics

Fairycore typography should feel organic, slightly fantastical, and hand-touched. Headings benefit from elegant serifs with soft, flowing terminals or decorative display faces that evoke calligraphic fairy-tale lettering. Body text should remain highly readable while retaining warmth and personality through gentle serif or humanist sans-serif forms. Accent text, such as quotes, labels, and decorative flourishes, can employ handwritten or script faces to reinforce the hand-crafted, woodland journal quality of the aesthetic.

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Cormorant Infant** | Elegant display serif with soft, slightly whimsical terminals | Headings and hero text |
| **EB Garamond** | Classic old-style serif with warm, organic letterforms | Body text and long-form reading |
| **Caveat** | Casual handwritten script with natural bounce | Decorative labels, quotes, annotations |
| **Cinzel Decorative** | Ornate display serif with fairy-tale grandeur | Feature titles and section headers |
| **Quicksand** | Rounded geometric sans-serif with gentle, friendly forms | UI elements, navigation, captions |
| **Tangerine** | Delicate calligraphic script with elegant flourishes | Pull quotes, decorative accents |
| **Spectral** | Warm, readable serif with organic character | Alternate body text |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Cormorant Infant 600 | EB Garamond 400 | Elegant woodland editorial |
| Cinzel Decorative 400 | Spectral 400 | Grand fairy-tale storytelling |
| Cormorant Infant 500 | Quicksand 400 | Ethereal yet modern and approachable |
| Caveat 600 | EB Garamond 400 | Hand-written forest journal |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Infant:wght@400;500;600;700&family=EB+Garamond:wght@400;500;600&family=Caveat:wght@400;600&family=Quicksand:wght@400;500;600&display=swap');

body {
  font-family: 'EB Garamond', 'Georgia', serif;
  font-size: 1.1rem;
  line-height: 1.85;
  color: #5C4A3A;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Cormorant Infant', 'Garamond', serif;
  font-weight: 600;
  letter-spacing: 0.02em;
  color: #4A7453;
}

.handwritten {
  font-family: 'Caveat', cursive;
  font-size: 1.4rem;
  color: #8E7BA8;
}

.ui-label {
  font-family: 'Quicksand', 'Helvetica Neue', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
}
```

## Layout Principles

### Grid and Structure

- **Organic, flowing single-column layouts**: Prefer a natural vertical reading flow that mimics wandering along a forest path; avoid rigid multi-column grids
- **Asymmetric accent placement**: Position decorative botanical elements, sparkle effects, and illustrative motifs off-grid for a natural, discovered quality
- **Layered card stacking**: Overlap cards and content panels slightly, with varying border-radius values, to create a collage-like depth reminiscent of layered leaves
- **Generous whitespace**: Maintain airy breathing room (40-60px between sections, 32-48px card padding) so the design feels like an open glade, not a dense thicket
- **Max-width content areas**: Keep readable content at 720-880px max-width, centered on the page, with decorative elements allowed to extend beyond

### Section Organization

- **Hero as a clearing**: The hero section should feel like stepping into an enchanted clearing; large, open, softly lit, with a single focal heading and atmospheric background effects
- **Content cards as discovered objects**: Present content blocks as artifacts found in the forest, such as mossy stones, bark scrolls, or leaf-wrapped parcels, each with unique but harmonious styling
- **Botanical dividers between sections**: Use decorative separators featuring fern fronds, mushroom clusters, or trailing vine motifs instead of plain horizontal rules
- **Footer as forest floor**: The footer should feel grounded and earthy with darker tones, as if one has reached the mossy roots at the base of an ancient tree

### Responsive Approach

- **Graceful stacking**: Cards and content blocks stack vertically on smaller screens while maintaining generous padding and rounded forms
- **Scaled-down decorations**: Reduce particle effects, sparkle counts, and decorative element sizes on mobile to preserve performance without sacrificing atmosphere
- **Touch-friendly targets**: Buttons and interactive elements maintain minimum 44px touch targets with ample padding on mobile
- **Preserved atmosphere**: Even at small viewports, maintain the soft background gradients, rounded corners, and warm color palette that define the enchanted feel

## CSS / Design Techniques

### Fairycore Card

```css
.fairy-card {
  background: linear-gradient(135deg, #FAF7F2 0%, #EDE8E0 100%);
  border: 1px solid rgba(184, 165, 204, 0.3);
  border-radius: 20px;
  padding: 36px;
  box-shadow:
    0 2px 12px rgba(74, 116, 83, 0.08),
    0 0 40px rgba(184, 165, 204, 0.06);
  position: relative;
  overflow: hidden;
}

.fairy-card::before {
  content: '';
  position: absolute;
  top: -50%;
  right: -50%;
  width: 100%;
  height: 100%;
  background: radial-gradient(circle, rgba(212, 185, 106, 0.08) 0%, transparent 70%);
  pointer-events: none;
}

.fairy-card::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: linear-gradient(90deg, #6B8F6B, #B8A5CC, #D4B96A, #E0C4D0);
  border-radius: 0 0 20px 20px;
}
```

### Fairycore Button

```css
.fairy-button {
  background: linear-gradient(135deg, #6B8F6B 0%, #4A7453 100%);
  color: #FAF7F2;
  border: none;
  border-radius: 28px;
  padding: 14px 36px;
  font-family: 'EB Garamond', serif;
  font-size: 1.05rem;
  font-weight: 500;
  cursor: pointer;
  transition: all 0.4s ease;
  box-shadow:
    0 2px 8px rgba(74, 116, 83, 0.3),
    0 0 20px rgba(107, 143, 107, 0.1);
  position: relative;
  overflow: hidden;
}

.fairy-button::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  width: 0;
  height: 0;
  background: radial-gradient(circle, rgba(212, 185, 106, 0.4) 0%, transparent 70%);
  transform: translate(-50%, -50%);
  transition: width 0.5s ease, height 0.5s ease;
  pointer-events: none;
}

.fairy-button:hover {
  transform: translateY(-2px);
  box-shadow:
    0 6px 20px rgba(74, 116, 83, 0.35),
    0 0 30px rgba(184, 165, 204, 0.15);
}

.fairy-button:hover::before {
  width: 300px;
  height: 300px;
}
```

### Navigation Bar

```css
.fairy-nav {
  background: rgba(245, 240, 232, 0.9);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(200, 196, 190, 0.5);
  padding: 16px 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: sticky;
  top: 0;
  z-index: 100;
}

.fairy-nav .logo {
  font-family: 'Cormorant Infant', serif;
  font-size: 1.4rem;
  font-weight: 600;
  color: #4A7453;
  text-decoration: none;
}

.fairy-nav a {
  font-family: 'Quicksand', sans-serif;
  font-size: 0.9rem;
  font-weight: 500;
  color: #5C4A3A;
  text-decoration: none;
  padding: 8px 18px;
  border-radius: 20px;
  transition: all 0.3s ease;
}

.fairy-nav a:hover {
  background: rgba(107, 143, 107, 0.12);
  color: #4A7453;
  box-shadow: 0 0 12px rgba(184, 165, 204, 0.15);
}
```

### Hero Section

```css
.fairy-hero {
  background: linear-gradient(180deg, #F5F0E8 0%, #EDE8E0 60%, #E0C4D0 100%);
  padding: 100px 40px 80px;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.fairy-hero::before {
  content: '';
  position: absolute;
  top: 20%;
  left: 50%;
  transform: translateX(-50%);
  width: 600px;
  height: 600px;
  background: radial-gradient(circle, rgba(212, 185, 106, 0.12) 0%, transparent 65%);
  pointer-events: none;
}

.fairy-hero h1 {
  font-family: 'Cormorant Infant', serif;
  font-size: 3.4rem;
  font-weight: 600;
  color: #4A7453;
  margin-bottom: 16px;
  position: relative;
}

.fairy-hero .subtitle {
  font-family: 'Caveat', cursive;
  font-size: 1.6rem;
  color: #8E7BA8;
  margin-bottom: 24px;
}

.fairy-hero p {
  font-family: 'EB Garamond', serif;
  font-size: 1.2rem;
  color: #5C4A3A;
  max-width: 580px;
  margin: 0 auto;
  line-height: 1.85;
}
```

### Firefly Particle Effect

```css
.firefly-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  overflow: hidden;
}

.firefly {
  position: absolute;
  width: 6px;
  height: 6px;
  background: radial-gradient(circle, #D4B96A 0%, rgba(212, 185, 106, 0) 70%);
  border-radius: 50%;
  animation: fireflyFloat 8s ease-in-out infinite, fireflyGlow 3s ease-in-out infinite alternate;
}

@keyframes fireflyFloat {
  0%, 100% { transform: translate(0, 0); }
  25% { transform: translate(40px, -60px); }
  50% { transform: translate(-20px, -100px); }
  75% { transform: translate(60px, -40px); }
}

@keyframes fireflyGlow {
  0% { opacity: 0.2; box-shadow: 0 0 4px rgba(212, 185, 106, 0.3); }
  100% { opacity: 0.8; box-shadow: 0 0 12px rgba(212, 185, 106, 0.6); }
}

.firefly:nth-child(2) { animation-delay: -2s; animation-duration: 10s, 4s; }
.firefly:nth-child(3) { animation-delay: -4s; animation-duration: 7s, 2.5s; }
.firefly:nth-child(4) { animation-delay: -1s; animation-duration: 9s, 3.5s; }
.firefly:nth-child(5) { animation-delay: -5s; animation-duration: 11s, 2s; }
```

### Botanical Divider

```css
.fairy-divider {
  text-align: center;
  margin: 48px 0;
  position: relative;
  height: 24px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.fairy-divider::before,
.fairy-divider::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(90deg, transparent, #C8C4BE, transparent);
  max-width: 200px;
}

.fairy-divider span {
  padding: 0 20px;
  color: #6B8F6B;
  font-size: 1.3rem;
  opacity: 0.6;
}
```

### Dewdrop Tooltip

```css
.fairy-tooltip {
  position: relative;
  cursor: help;
  border-bottom: 1px dotted #B8A5CC;
}

.fairy-tooltip::after {
  content: attr(data-tip);
  position: absolute;
  bottom: calc(100% + 10px);
  left: 50%;
  transform: translateX(-50%) scale(0.9);
  background: rgba(250, 247, 242, 0.95);
  backdrop-filter: blur(8px);
  border: 1px solid rgba(184, 165, 204, 0.3);
  border-radius: 14px;
  padding: 10px 18px;
  font-family: 'Quicksand', sans-serif;
  font-size: 0.82rem;
  color: #5C4A3A;
  white-space: nowrap;
  opacity: 0;
  pointer-events: none;
  transition: opacity 0.3s ease, transform 0.3s ease;
  box-shadow:
    0 4px 16px rgba(74, 116, 83, 0.1),
    0 0 20px rgba(184, 165, 204, 0.08);
}

.fairy-tooltip:hover::after {
  opacity: 1;
  transform: translateX(-50%) scale(1);
}
```

### Mushroom Badge

```css
.fairy-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  background: linear-gradient(135deg, #D5C8B5 0%, #EDE8E0 100%);
  border: 1px solid rgba(196, 145, 126, 0.3);
  border-radius: 20px;
  padding: 6px 16px;
  font-family: 'Quicksand', sans-serif;
  font-size: 0.8rem;
  font-weight: 500;
  color: #5C4A3A;
  transition: all 0.3s ease;
}

.fairy-badge::before {
  content: '\1F344';
  font-size: 0.9rem;
}

.fairy-badge:hover {
  background: linear-gradient(135deg, #E0C4D0 0%, #FAF7F2 100%);
  box-shadow: 0 0 16px rgba(184, 165, 204, 0.2);
  transform: translateY(-1px);
}
```

## Design Do's and Don'ts

### Do

- Use soft gaussian blur on background images and decorative layers to create an ethereal, dreamlike atmosphere
- Incorporate subtle glow and shimmer effects on hover states to evoke fairy dust and bioluminescence
- Pair elegant serif headings with handwritten accent text for a woodland journal quality
- Apply warm golden radial gradients as ambient light sources behind content areas
- Use translucent, frosted-glass panels with backdrop-filter for cards and overlays
- Include organic CSS shapes (using border-radius variations and clip-path) for containers rather than perfect rectangles
- Maintain a muted, low-saturation palette with occasional pops of golden warmth and soft purple
- Add gentle CSS animations for floating, glowing, and fading elements that feel natural and unhurried
- Use cream and warm off-white backgrounds instead of pure white
- Layer multiple subtle box-shadows with green and purple tints for depth that feels organic

### Don't

- Avoid harsh neon colors, electric blues, or high-contrast corporate palettes that shatter the enchanted mood
- Avoid sharp angular shapes, hard geometric grids, or brutalist design elements
- Do not use pure black text or backgrounds; the aesthetic requires softened, warm darks like deep forest green or bark brown
- Avoid fast, aggressive animations or abrupt transitions; all motion should be slow, gentle, and flowing
- Do not overcrowd layouts with too many decorative elements; enchantment requires breathing room and negative space
- Avoid modern tech-forward imagery, stock photos of offices, or corporate iconography
- Do not use heavy, blocky sans-serif fonts exclusively; serifs and scripts are essential to the fairy-tale feel
- Avoid flat, shadowless design; Fairycore relies on layered depth and atmospheric lighting
- Do not use jarring drop shadows with pure black; tint all shadows with forest green or soft purple
- Avoid overly saturated or artificially vivid colors; Fairycore colors should feel sun-dappled and naturally muted

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Cottagecore** | Closest relative; both celebrate romanticized nature, but Fairycore adds explicit magical and fantastical elements like fairy wings, sparkles, and bioluminescence |
| **Goblincore** | Shares the love of mushrooms, moss, and forest floor treasures, but Goblincore is earthier and more chaotic where Fairycore is ethereal and delicate |
| **Whimsigothic** | Both employ an enchanted, slightly otherworldly atmosphere, but Whimsigothic leans dark and moody while Fairycore stays luminous and gentle |
| **Art Nouveau** | Shares the emphasis on organic, flowing natural forms and botanical motifs, though Art Nouveau is more stylized and architecturally formal |
| **Danish Pastel** | Both use soft, muted pastel palettes, but Danish Pastel is modern and minimal while Fairycore is layered and nature-enchanted |
| **Dreamcore** | Both create surreal, atmospheric experiences, but Dreamcore tends toward unsettling liminal spaces while Fairycore remains warm and inviting |
| **Frutiger Eco** | Shares nature-positive themes and green palettes, but Frutiger Eco is clean and corporate while Fairycore is handcrafted and mythical |
| **Wabi-Sabi** | Both appreciate natural imperfection and organic beauty, but Wabi-Sabi is austere and Japanese-inflected while Fairycore is lush and European-fantastical |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Mossy Grimoire &mdash; An Enchanted Herbarium</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Infant:wght@400;500;600;700&family=EB+Garamond:wght@400;500;600&family=Caveat:wght@400;600&family=Quicksand:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'EB Garamond', Georgia, serif;
      font-size: 1.1rem;
      line-height: 1.85;
      color: #5C4A3A;
      background-color: #F5F0E8;
      min-height: 100vh;
      overflow-x: hidden;
    }

    /* --- Firefly Particles --- */
    .fireflies {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      pointer-events: none;
      z-index: 0;
    }

    .firefly {
      position: absolute;
      width: 5px; height: 5px;
      background: radial-gradient(circle, #D4B96A 0%, rgba(212,185,106,0) 70%);
      border-radius: 50%;
      animation: ffFloat 8s ease-in-out infinite, ffGlow 3s ease-in-out infinite alternate;
    }

    .firefly:nth-child(1) { top: 15%; left: 10%; }
    .firefly:nth-child(2) { top: 30%; left: 80%; animation-delay: -2s; animation-duration: 10s, 4s; }
    .firefly:nth-child(3) { top: 55%; left: 25%; animation-delay: -4s; animation-duration: 7s, 2.5s; }
    .firefly:nth-child(4) { top: 70%; left: 65%; animation-delay: -1s; animation-duration: 9s, 3.5s; }
    .firefly:nth-child(5) { top: 40%; left: 50%; animation-delay: -5s; animation-duration: 11s, 2s; }
    .firefly:nth-child(6) { top: 85%; left: 35%; animation-delay: -3s; animation-duration: 8.5s, 3s; }

    @keyframes ffFloat {
      0%, 100% { transform: translate(0, 0); }
      25% { transform: translate(30px, -50px); }
      50% { transform: translate(-15px, -80px); }
      75% { transform: translate(45px, -30px); }
    }

    @keyframes ffGlow {
      0% { opacity: 0.15; box-shadow: 0 0 3px rgba(212,185,106,0.3); }
      100% { opacity: 0.7; box-shadow: 0 0 10px rgba(212,185,106,0.5); }
    }

    /* --- Navigation --- */
    .nav {
      background: rgba(245,240,232,0.88);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(200,196,190,0.5);
      padding: 14px 32px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav-logo {
      font-family: 'Cormorant Infant', serif;
      font-size: 1.4rem;
      font-weight: 600;
      color: #4A7453;
      text-decoration: none;
    }

    .nav-links { display: flex; gap: 4px; }

    .nav-links a {
      font-family: 'Quicksand', sans-serif;
      font-size: 0.88rem;
      font-weight: 500;
      color: #5C4A3A;
      text-decoration: none;
      padding: 8px 18px;
      border-radius: 20px;
      transition: all 0.3s ease;
    }

    .nav-links a:hover {
      background: rgba(107,143,107,0.12);
      color: #4A7453;
    }

    /* --- Hero --- */
    .hero {
      text-align: center;
      padding: 90px 24px 70px;
      position: relative;
      background: linear-gradient(180deg, #F5F0E8 0%, #EDE8E0 50%, rgba(224,196,208,0.3) 100%);
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 15%;
      left: 50%;
      transform: translateX(-50%);
      width: 500px;
      height: 500px;
      background: radial-gradient(circle, rgba(212,185,106,0.1) 0%, transparent 65%);
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Cormorant Infant', serif;
      font-size: 3.2rem;
      font-weight: 600;
      color: #4A7453;
      margin-bottom: 12px;
      position: relative;
    }

    .hero .tagline {
      font-family: 'Caveat', cursive;
      font-size: 1.5rem;
      color: #8E7BA8;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 1.15rem;
      max-width: 560px;
      margin: 0 auto 32px;
      color: #5C4A3A;
    }

    /* --- Buttons --- */
    .btn {
      display: inline-block;
      background: linear-gradient(135deg, #6B8F6B 0%, #4A7453 100%);
      color: #FAF7F2;
      border: none;
      border-radius: 28px;
      padding: 14px 36px;
      font-family: 'EB Garamond', serif;
      font-size: 1.05rem;
      font-weight: 500;
      cursor: pointer;
      text-decoration: none;
      transition: all 0.4s ease;
      box-shadow: 0 2px 10px rgba(74,116,83,0.3), 0 0 20px rgba(107,143,107,0.08);
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 24px rgba(74,116,83,0.35), 0 0 30px rgba(184,165,204,0.12);
    }

    .btn-outline {
      background: transparent;
      color: #4A7453;
      border: 1.5px solid rgba(107,143,107,0.4);
      box-shadow: none;
    }

    .btn-outline:hover {
      background: rgba(107,143,107,0.08);
      box-shadow: 0 0 20px rgba(107,143,107,0.1);
    }

    /* --- Container --- */
    .container {
      max-width: 840px;
      margin: 0 auto;
      padding: 0 24px;
      position: relative;
      z-index: 1;
    }

    /* --- Divider --- */
    .divider {
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 48px 0;
    }

    .divider::before,
    .divider::after {
      content: '';
      flex: 1;
      height: 1px;
      background: linear-gradient(90deg, transparent, #C8C4BE, transparent);
      max-width: 180px;
    }

    .divider span {
      padding: 0 18px;
      color: #6B8F6B;
      font-size: 1.2rem;
      opacity: 0.5;
    }

    /* --- Section headings --- */
    .section-title {
      font-family: 'Cormorant Infant', serif;
      font-size: 2rem;
      font-weight: 600;
      color: #4A7453;
      text-align: center;
      margin-bottom: 12px;
    }

    .section-subtitle {
      font-family: 'Caveat', cursive;
      font-size: 1.25rem;
      color: #8E7BA8;
      text-align: center;
      margin-bottom: 40px;
    }

    /* --- Cards --- */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
      margin-bottom: 48px;
    }

    .card {
      background: linear-gradient(135deg, #FAF7F2 0%, #EDE8E0 100%);
      border: 1px solid rgba(184,165,204,0.25);
      border-radius: 20px;
      padding: 32px;
      position: relative;
      overflow: hidden;
      transition: all 0.4s ease;
    }

    .card::before {
      content: '';
      position: absolute;
      top: -40%;
      right: -40%;
      width: 80%;
      height: 80%;
      background: radial-gradient(circle, rgba(212,185,106,0.06) 0%, transparent 70%);
      pointer-events: none;
    }

    .card::after {
      content: '';
      position: absolute;
      bottom: 0; left: 0; right: 0;
      height: 3px;
      background: linear-gradient(90deg, #6B8F6B, #B8A5CC, #D4B96A);
      border-radius: 0 0 20px 20px;
      opacity: 0.6;
    }

    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 28px rgba(74,116,83,0.1), 0 0 40px rgba(184,165,204,0.06);
    }

    .card-icon {
      font-size: 2rem;
      margin-bottom: 14px;
      display: block;
    }

    .card h3 {
      font-family: 'Cormorant Infant', serif;
      font-size: 1.35rem;
      font-weight: 600;
      color: #4A7453;
      margin-bottom: 10px;
    }

    .card p {
      font-size: 1rem;
      line-height: 1.75;
    }

    /* --- Badge --- */
    .badge {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      background: linear-gradient(135deg, #D5C8B5 0%, #EDE8E0 100%);
      border: 1px solid rgba(196,145,126,0.25);
      border-radius: 20px;
      padding: 5px 14px;
      font-family: 'Quicksand', sans-serif;
      font-size: 0.78rem;
      font-weight: 500;
      color: #5C4A3A;
    }

    /* --- Feature block --- */
    .feature {
      display: flex;
      align-items: flex-start;
      gap: 28px;
      margin-bottom: 36px;
      padding: 28px 32px;
      background: rgba(250,247,242,0.6);
      border-radius: 18px;
      border: 1px solid rgba(200,196,190,0.3);
    }

    .feature-icon {
      font-size: 2.4rem;
      flex-shrink: 0;
      margin-top: 4px;
    }

    .feature h3 {
      font-family: 'Cormorant Infant', serif;
      font-size: 1.25rem;
      font-weight: 600;
      color: #4A7453;
      margin-bottom: 6px;
    }

    .feature p {
      font-size: 1rem;
      line-height: 1.75;
    }

    /* --- Testimonial / Quote --- */
    .quote-block {
      text-align: center;
      padding: 48px 40px;
      margin: 48px 0;
      background: linear-gradient(180deg, rgba(184,165,204,0.08) 0%, rgba(224,196,208,0.06) 100%);
      border-radius: 24px;
      border: 1px solid rgba(184,165,204,0.15);
      position: relative;
    }

    .quote-block::before {
      content: '\201C';
      font-family: 'Cormorant Infant', serif;
      font-size: 5rem;
      color: #B8A5CC;
      opacity: 0.3;
      position: absolute;
      top: 10px;
      left: 30px;
      line-height: 1;
    }

    .quote-block p {
      font-family: 'Cormorant Infant', serif;
      font-size: 1.5rem;
      font-weight: 500;
      font-style: italic;
      color: #4A7453;
      max-width: 580px;
      margin: 0 auto 14px;
      line-height: 1.6;
    }

    .quote-block cite {
      font-family: 'Caveat', cursive;
      font-size: 1.15rem;
      color: #8E7BA8;
      font-style: normal;
    }

    /* --- Footer --- */
    .footer {
      background: linear-gradient(180deg, #EDE8E0 0%, #2E3D2E 100%);
      padding: 60px 24px 32px;
      text-align: center;
      margin-top: 60px;
    }

    .footer h3 {
      font-family: 'Cormorant Infant', serif;
      font-size: 1.6rem;
      font-weight: 600;
      color: #D4B96A;
      margin-bottom: 8px;
    }

    .footer p {
      font-family: 'EB Garamond', serif;
      font-size: 0.95rem;
      color: #C8C4BE;
      max-width: 480px;
      margin: 0 auto 24px;
      line-height: 1.7;
    }

    .footer-links {
      display: flex;
      justify-content: center;
      gap: 24px;
      margin-bottom: 32px;
      flex-wrap: wrap;
    }

    .footer-links a {
      font-family: 'Quicksand', sans-serif;
      font-size: 0.85rem;
      color: #C8C4BE;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .footer-links a:hover { color: #D4B96A; }

    .footer-copy {
      font-family: 'Quicksand', sans-serif;
      font-size: 0.75rem;
      color: rgba(200,196,190,0.5);
    }

    /* --- Responsive --- */
    @media (max-width: 640px) {
      .hero h1 { font-size: 2.2rem; }
      .hero { padding: 60px 20px 50px; }
      .nav { padding: 12px 16px; }
      .nav-links a { padding: 6px 12px; font-size: 0.82rem; }
      .feature { flex-direction: column; gap: 12px; padding: 24px; }
      .card { padding: 24px; }
      .quote-block { padding: 36px 24px; }
      .quote-block p { font-size: 1.25rem; }
      .section-title { font-size: 1.7rem; }
      .card-grid { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

  <!-- Firefly particles -->
  <div class="fireflies">
    <div class="firefly"></div>
    <div class="firefly"></div>
    <div class="firefly"></div>
    <div class="firefly"></div>
    <div class="firefly"></div>
    <div class="firefly"></div>
  </div>

  <!-- Navigation -->
  <nav class="nav">
    <a href="#" class="nav-logo">The Mossy Grimoire</a>
    <div class="nav-links">
      <a href="#herbarium">Herbarium</a>
      <a href="#enchantments">Enchantments</a>
      <a href="#woodland">Woodland</a>
      <a href="#about">About</a>
    </div>
  </nav>

  <!-- Hero -->
  <header class="hero">
    <h1>The Mossy Grimoire</h1>
    <p class="tagline">whispered secrets from the enchanted wood</p>
    <p>A hand-gathered collection of woodland herbs, fairy-ring fungi, and ancient botanical wisdom passed down through generations of forest keepers who tend the hidden glades.</p>
    <div style="margin-top: 28px; display: flex; gap: 14px; justify-content: center; flex-wrap: wrap;">
      <a href="#herbarium" class="btn">Explore the Herbarium</a>
      <a href="#woodland" class="btn btn-outline">Wander the Woods</a>
    </div>
  </header>

  <div class="container">

    <!-- Divider -->
    <div class="divider"><span>&#10047; &#10047; &#10047;</span></div>

    <!-- Herbarium Cards -->
    <section id="herbarium">
      <h2 class="section-title">The Living Herbarium</h2>
      <p class="section-subtitle">pressed between pages of bark and moonlight</p>

      <div class="card-grid">
        <div class="card">
          <span class="card-icon">&#127812;</span>
          <h3>Silver Fern</h3>
          <p>Found unfurling in damp hollows beneath elder oaks. Its fronds collect morning dew that shimmers with a faint iridescence, prized by healers for calming restless dreams.</p>
          <div style="margin-top: 14px;"><span class="badge">&#127807; Shade-dwelling</span></div>
        </div>
        <div class="card">
          <span class="card-icon">&#127344;</span>
          <h3>Foxglove Bell</h3>
          <p>The tall purple spires nod gently in forest clearings, each bell-shaped bloom said to house a sleeping fairy. Gather only the fallen petals and never disturb the sleeping residents within.</p>
          <div style="margin-top: 14px;"><span class="badge">&#127800; Meadow bloom</span></div>
        </div>
        <div class="card">
          <span class="card-icon">&#127804;</span>
          <h3>Moonpetal Moss</h3>
          <p>This luminescent moss grows on the north faces of ancient standing stones. Under a full moon its surface glows faintly silver-green, guiding lost travellers back to familiar paths.</p>
          <div style="margin-top: 14px;"><span class="badge">&#127761; Nocturnal</span></div>
        </div>
      </div>
    </section>

    <!-- Divider -->
    <div class="divider"><span>&#10047;</span></div>

    <!-- Enchantments -->
    <section id="enchantments">
      <h2 class="section-title">Woodland Enchantments</h2>
      <p class="section-subtitle">gentle magic for everyday tending</p>

      <div class="feature">
        <span class="feature-icon">&#128171;</span>
        <div>
          <h3>Dewdrop Preservation</h3>
          <p>Collect morning dew from clover leaves before the first light touches them. Stored in a glass vial sealed with beeswax, the dew retains its clarity for a full cycle of the moon and can be added to tinctures for gentle renewal.</p>
        </div>
      </div>

      <div class="feature">
        <span class="feature-icon">&#127812;</span>
        <div>
          <h3>Fern Spiral Compass</h3>
          <p>The unfurling direction of young fern fiddleheads in spring indicates the nearest source of fresh water. Follow the spiral inward and then trace the direction it points at its tightest coil.</p>
        </div>
      </div>

      <div class="feature">
        <span class="feature-icon">&#129476;</span>
        <div>
          <h3>Mushroom Ring Etiquette</h3>
          <p>When you encounter a fairy ring of toadstools, walk three times clockwise around its perimeter before stepping inside. Leave a small offering of dried lavender or a smooth river stone at the northern edge as thanks.</p>
        </div>
      </div>
    </section>

    <!-- Quote -->
    <div class="quote-block">
      <p>Between the roots and the reaching branches, there is a stillness where the old magic breathes.</p>
      <cite>&mdash; The Keeper of the Eastern Glade</cite>
    </div>

    <!-- Woodland Guide -->
    <section id="woodland">
      <h2 class="section-title">Paths Through the Woodland</h2>
      <p class="section-subtitle">where every trail tells a story</p>

      <div class="card-grid">
        <div class="card">
          <span class="card-icon">&#127795;</span>
          <h3>The Elder Oak Trail</h3>
          <p>A winding path through the oldest part of the forest, where the canopy is so thick that sunlight falls in scattered golden coins on the mossy floor. Listen for the hollow knocking of woodpeckers overhead.</p>
        </div>
        <div class="card">
          <span class="card-icon">&#128167;</span>
          <h3>Willowbrook Crossing</h3>
          <p>Follow the clear stream where watercress grows in slow eddies and dragonflies rest on sun-warmed stones. The crossing is shallow here and the stepping stones are smooth from centuries of careful feet.</p>
        </div>
      </div>
    </section>

    <!-- Divider -->
    <div class="divider"><span>&#10047; &#10047; &#10047;</span></div>

    <!-- About -->
    <section id="about" style="text-align: center; padding: 20px 0 40px;">
      <h2 class="section-title">About the Grimoire</h2>
      <p class="section-subtitle">tended with care since the first acorn fell</p>
      <p style="max-width: 560px; margin: 0 auto; font-size: 1.05rem;">
        The Mossy Grimoire has been kept by the woodland stewards for as long as the forest has stood. Each entry is gathered by hand, dried between pages of birch bark, and inscribed by candlelight. We share this knowledge so that the gentle arts of forest-keeping may continue for generations to come.
      </p>
      <div style="margin-top: 28px;">
        <a href="#herbarium" class="btn">Begin Your Journey</a>
      </div>
    </section>

  </div>

  <!-- Footer -->
  <footer class="footer">
    <h3>The Mossy Grimoire</h3>
    <p>Gathered from the quiet places between root and branch, where the old knowledge still grows green.</p>
    <div class="footer-links">
      <a href="#herbarium">Herbarium</a>
      <a href="#enchantments">Enchantments</a>
      <a href="#woodland">Woodland Paths</a>
      <a href="#about">About</a>
    </div>
    <p class="footer-copy">&copy; 2026 The Mossy Grimoire. Tended with care in the Eastern Glade.</p>
  </footer>

</body>
</html>
```

## Implementation Tips

- **Firefly particles**: Use CSS-only animations with `radial-gradient` dots and staggered `animation-delay` values for performant floating glow effects without JavaScript; limit to 6-8 particles for subtlety
- **Warm-tinted shadows**: Always tint box-shadows with forest green (`rgba(74, 116, 83, 0.08)`) or soft purple (`rgba(184, 165, 204, 0.06)`) rather than pure black for organic warmth
- **Ambient glow effects**: Use large `radial-gradient` pseudo-elements as ambient light sources behind hero sections and content areas to simulate golden-hour forest light
- **Frosted glass panels**: Apply `backdrop-filter: blur(12px)` with semi-transparent backgrounds for navigation bars and overlay cards that feel like peering through morning mist
- **Avoid pure white and pure black**: Use `#FAF7F2` or `#F5F0E8` instead of `#FFFFFF` for backgrounds, and `#5C4A3A` or `#2E3D2E` instead of `#000000` for text
- **Iridescent hover effects**: Create fairy-wing shimmer on hover by transitioning `box-shadow` to include a spread of soft purple and gold glows simultaneously
- **Botanical SVG dividers**: Inline simple single-color SVG fern or mushroom motifs at low opacity for section dividers; keep them lightweight and decorative rather than illustrative
- **Image treatment**: Apply `filter: saturate(0.85) brightness(1.05)` to photographs to maintain the soft, slightly sun-faded quality of the palette
- **Performance on mobile**: Reduce or disable firefly particle animations on screens below 640px using `prefers-reduced-motion` media queries and viewport-based conditionals
