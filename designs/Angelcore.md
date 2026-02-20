# Angelcore - Design Reference

Angelcore is a contemporary internet aesthetic rooted in the imagery and mythology of angels drawn primarily from European Renaissance, Baroque, and Rococo art. It evokes the ethereal beauty of heaven through soft glowing whites, gilded gold accents, and dreamy celestial imagery -- cherubs, halos, wings, doves, clouds, and divine light. The palette centers on luminous whites and creams warmed by pale gold, baby blue, and blush pink, creating an atmosphere of purity, innocence, and transcendence. In digital design, Angelcore translates into airy layouts bathed in radiant light effects, delicate serif typography reminiscent of classical inscriptions, ornamental gold borders, translucent overlays that mimic heavenly mist, and imagery that channels the soft sfumato of Renaissance angel paintings. Every surface should feel as if it is glowing from within, suspended in an endless expanse of cloud and light.

## Visual Characteristics

### Core Design Traits

- **Celestial light and radiance**: Soft, diffused glows, crepuscular rays, and radial light bursts that emanate from behind content, simulating divine illumination breaking through clouds
- **Gold leaf and gilded accents**: Ornamental gold borders, thin gold rules, metallic gradient highlights, and filigree details inspired by illuminated manuscripts and gilded altar frames
- **Cherub and putti motifs**: Decorative references to Renaissance cherubs used as ornamental elements, section dividers, or watermark-style background imagery
- **Cloud and mist textures**: Soft, billowing cloud shapes used as backgrounds, section transitions, and container edges, creating a sensation of floating in the heavens
- **Halo and aureole shapes**: Circular and elliptical golden ring motifs used as decorative frames around headings, avatars, or focal imagery
- **Wing and feather details**: Stylized angel wing silhouettes and individual feather shapes used as icons, dividers, and ornamental flourishes
- **Renaissance painting influence**: Soft sfumato edges, warm chiaroscuro lighting, muted fresco-like textures, and compositions echoing classical religious paintings
- **Translucent white layering**: Multiple overlapping semi-transparent white panels that create ethereal depth, as though peering through layers of heavenly cloud

### Design Principles

- Bathe every surface in soft, warm light; nothing should feel cold, harsh, or shadowed in darkness
- Use white space as sacred space -- generous, open, and reverent in its emptiness
- Apply gold sparingly as a divine accent; it should highlight, not overwhelm
- Maintain an atmosphere of serenity and stillness; avoid aggressive motion or harsh transitions
- Layer translucent whites and creams to build depth without weight
- Reference classical art composition: centered subjects, symmetrical balance, and upward visual flow
- Treat typography as inscription -- elegant, measured, and timeless
- Let every element feel weightless, as though floating on air or ascending upward

## Color Palette

| Color Name | Hex | Role/Usage |
|------------|-----|------------|
| Heavenly White | `#FFFEF9` | Primary page background, sacred white space |
| Cloud Ivory | `#FBF8F1` | Card backgrounds, content surfaces |
| Angelic Cream | `#F5EFE0` | Secondary surfaces, soft contrast panels |
| Divine Gold | `#D4A843` | Primary accent, gilded borders, ornamental details |
| Halo Gold | `#E8C766` | Lighter gold for gradients, glow effects |
| Pale Aureate | `#F2E4B3` | Muted gold for backgrounds, subtle warmth |
| Cherub Blush | `#F2D7D5` | Soft pink accent, warm highlights |
| Seraphim Blue | `#D4E4F1` | Cool accent, sky tones, airy contrast |
| Celestial Lavender | `#E3DAF0` | Tertiary accent, ethereal purple tint |
| Dove Grey | `#C8C3B8` | Muted text accents, subtle borders |
| Fresco Umber | `#8A7D6B` | Body text on light backgrounds |
| Altar Dark | `#3D362B` | Headings, high-contrast text |

### CSS Custom Properties

```css
:root {
  --angel-white: #FFFEF9;
  --angel-ivory: #FBF8F1;
  --angel-cream: #F5EFE0;
  --angel-gold: #D4A843;
  --angel-halo: #E8C766;
  --angel-pale-gold: #F2E4B3;
  --angel-blush: #F2D7D5;
  --angel-blue: #D4E4F1;
  --angel-lavender: #E3DAF0;
  --angel-dove: #C8C3B8;
  --angel-umber: #8A7D6B;
  --angel-dark: #3D362B;
}
```

## Typography

### Typeface Characteristics

Angelcore typography draws from the tradition of classical inscriptions, Renaissance title pages, and illuminated manuscripts. Headings should feel carved in stone or penned with a quill -- refined, high-contrast serifs with elegant proportions. Body text should be warm and readable with a bookish, timeless quality. Decorative script accents can evoke the hand of a celestial scribe, used sparingly for labels and ornamental phrases. Avoid anything that feels industrial, techy, or aggressively modern; every letterform should feel as though it belongs on a chapel ceiling or the page of a prayer book.

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Cormorant Garamond** | Elegant high-contrast serif | Headings, display text, titles |
| **EB Garamond** | Classical old-style serif | Body text, long-form reading |
| **Cinzel** | All-caps inscriptional serif | Section headers, navigation labels |
| **Great Vibes** | Flowing calligraphic script | Decorative accents, pull quotes |
| **Quattrocento** | Sturdy classical serif | Subheadings, supporting text |
| **Josefin Sans** | Geometric light sans-serif | UI labels, captions, small text |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Cormorant Garamond 600 | EB Garamond 400 | Renaissance editorial, warm and classical |
| Cinzel 700 | Quattrocento 400 | Inscriptional grandeur, chapel-inspired |
| Great Vibes 400 | Josefin Sans 300 | Celestial script meets airy modern clarity |
| Cormorant Garamond 700 | Josefin Sans 400 | High-contrast elegance with clean legibility |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=EB+Garamond:wght@400;500;600&family=Cinzel:wght@400;700&family=Great+Vibes&display=swap');

body {
  font-family: 'EB Garamond', 'Georgia', serif;
  font-size: 1.125rem;
  line-height: 1.85;
  color: var(--angel-umber);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Cormorant Garamond', 'Garamond', serif;
  font-weight: 600;
  letter-spacing: 0.02em;
  color: var(--angel-dark);
}

h1 {
  font-size: 3rem;
  line-height: 1.2;
}

h2 {
  font-size: 2rem;
  line-height: 1.3;
}

.inscriptional {
  font-family: 'Cinzel', serif;
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  font-size: 0.85rem;
}

.celestial-script {
  font-family: 'Great Vibes', cursive;
  font-size: 2rem;
  color: var(--angel-gold);
}
```

## Layout Principles

### Grid and Structure

- Content areas are centered and narrow (640-860px max-width) to create a reverent, focused reading experience reminiscent of a manuscript page
- Use generous internal padding (40-60px) within containers to let content breathe within its gilded frame
- Symmetrical layouts are preferred; center-aligned headings and balanced two-column grids echo the compositional harmony of Renaissance altarpieces
- Vertical stacking is the primary layout strategy; content flows downward like a scroll or illuminated page
- Gold border accents and thin rule lines define section boundaries without creating visual heaviness

### Section Organization

- Open with a radiant hero section featuring a central heading bathed in soft light and cloud imagery
- Use ornamental gold dividers between major sections rather than hard horizontal rules
- Cards and content panels should feel like they float above the background, separated by soft shadows and glowing edges
- Group related content within cream or ivory panels that contrast gently against the white page background
- End with a footer that echoes the heavenly theme, using muted gold and soft typography

### Responsive Approach

- On mobile, maintain the single-column vertical scroll and generous padding; reduce heading sizes but preserve the airy spaciousness
- Scale down ornamental gold borders and halo motifs rather than removing them entirely; the divine atmosphere should persist at every viewport
- Cloud backgrounds and radial light effects should use viewport-relative units to remain proportional
- Touch targets should be generous (48px minimum) and styled with soft rounded edges and subtle gold highlights
- Navigation collapses into a simple centered stack or minimal icon menu, maintaining the serene, uncluttered feel

## CSS / Design Techniques

### Celestial Card

```css
.angel-card {
  background: var(--angel-ivory);
  border: 1px solid var(--angel-pale-gold);
  border-radius: 20px;
  padding: 44px;
  position: relative;
  box-shadow:
    0 4px 24px rgba(212, 168, 67, 0.08),
    0 1px 6px rgba(61, 54, 43, 0.04);
}

.angel-card::before {
  content: '';
  position: absolute;
  top: -1px;
  left: 15%;
  right: 15%;
  height: 2px;
  background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
}

.angel-card::after {
  content: '';
  position: absolute;
  top: 12px;
  left: 12px;
  right: 12px;
  bottom: 12px;
  border: 1px solid rgba(212, 168, 67, 0.15);
  border-radius: 14px;
  pointer-events: none;
}
```

### Divine Button

```css
.angel-button {
  background: linear-gradient(135deg, var(--angel-gold) 0%, var(--angel-halo) 100%);
  color: var(--angel-white);
  border: none;
  border-radius: 50px;
  padding: 14px 40px;
  font-family: 'Cinzel', serif;
  font-weight: 700;
  font-size: 0.8rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  cursor: pointer;
  box-shadow:
    0 4px 16px rgba(212, 168, 67, 0.30),
    inset 0 1px 0 rgba(255, 255, 255, 0.30);
  transition: all 0.4s ease;
}

.angel-button:hover {
  transform: translateY(-2px);
  box-shadow:
    0 8px 28px rgba(212, 168, 67, 0.40),
    inset 0 1px 0 rgba(255, 255, 255, 0.40);
}
```

### Gilded Navigation

```css
.angel-nav {
  background: var(--angel-white);
  border-bottom: 1px solid var(--angel-pale-gold);
  padding: 20px 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 48px;
  position: relative;
}

.angel-nav::after {
  content: '';
  position: absolute;
  bottom: -1px;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
}

.angel-nav a {
  color: var(--angel-umber);
  font-family: 'Cinzel', serif;
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  text-decoration: none;
  transition: color 0.3s ease;
}

.angel-nav a:hover {
  color: var(--angel-gold);
}
```

### Radiant Hero Section

```css
.angel-hero {
  background: linear-gradient(180deg, var(--angel-ivory) 0%, var(--angel-white) 100%);
  text-align: center;
  padding: 120px 40px;
  position: relative;
  overflow: hidden;
}

.angel-hero::before {
  content: '';
  position: absolute;
  top: -30%;
  left: 25%;
  width: 50%;
  height: 160%;
  background: radial-gradient(ellipse at 50% 40%, rgba(232, 199, 102, 0.12) 0%, transparent 60%);
  pointer-events: none;
}

.angel-hero::after {
  content: '';
  position: absolute;
  top: 10%;
  left: 50%;
  transform: translateX(-50%);
  width: 300px;
  height: 300px;
  border: 1px solid rgba(212, 168, 67, 0.15);
  border-radius: 50%;
  pointer-events: none;
}

.angel-hero h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 3.5rem;
  font-weight: 600;
  color: var(--angel-dark);
  position: relative;
}

.angel-hero .script {
  font-family: 'Great Vibes', cursive;
  font-size: 1.6rem;
  color: var(--angel-gold);
  display: block;
  margin-bottom: 8px;
  position: relative;
}

.angel-hero p {
  max-width: 540px;
  margin: 20px auto 0;
  color: var(--angel-umber);
  position: relative;
}
```

### Halo Divider

```css
.angel-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
  margin: 56px 0;
}

.angel-divider::before,
.angel-divider::after {
  content: '';
  width: 100px;
  height: 1px;
  background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
}

.angel-divider span {
  width: 12px;
  height: 12px;
  border: 1.5px solid var(--angel-gold);
  border-radius: 50%;
  background: transparent;
  box-shadow: 0 0 8px rgba(212, 168, 67, 0.25);
}
```

### Cloud Background Section

```css
.angel-cloud-section {
  background:
    radial-gradient(ellipse at 20% 80%, rgba(212, 228, 241, 0.3) 0%, transparent 50%),
    radial-gradient(ellipse at 80% 20%, rgba(242, 228, 179, 0.2) 0%, transparent 50%),
    radial-gradient(ellipse at 50% 50%, rgba(242, 215, 213, 0.15) 0%, transparent 60%),
    var(--angel-white);
  padding: 80px 40px;
  position: relative;
}

.angel-cloud-section::before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 120px;
  background: linear-gradient(to top, var(--angel-white), transparent);
  pointer-events: none;
}
```

### Aureate Image Frame

```css
.angel-frame {
  position: relative;
  display: inline-block;
  padding: 8px;
  background: linear-gradient(135deg, var(--angel-halo) 0%, var(--angel-gold) 50%, var(--angel-halo) 100%);
  border-radius: 16px;
  box-shadow:
    0 4px 20px rgba(212, 168, 67, 0.20),
    inset 0 1px 0 rgba(255, 255, 255, 0.40);
}

.angel-frame img {
  display: block;
  border-radius: 12px;
  width: 100%;
  height: auto;
}

.angel-frame::after {
  content: '';
  position: absolute;
  top: 4px;
  left: 4px;
  right: 4px;
  bottom: 4px;
  border: 1px solid rgba(255, 255, 255, 0.25);
  border-radius: 14px;
  pointer-events: none;
}
```

### Ethereal Footer

```css
.angel-footer {
  background: var(--angel-cream);
  border-top: 1px solid var(--angel-pale-gold);
  padding: 48px 40px;
  text-align: center;
  position: relative;
}

.angel-footer::before {
  content: '';
  position: absolute;
  top: -1px;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
}

.angel-footer p {
  font-family: 'EB Garamond', serif;
  font-size: 0.95rem;
  color: var(--angel-dove);
  letter-spacing: 0.02em;
}

.angel-footer .script {
  font-family: 'Great Vibes', cursive;
  font-size: 1.4rem;
  color: var(--angel-gold);
  display: block;
  margin-bottom: 8px;
}
```

## Design Do's and Don'ts

### Do

- Use soft, diffused radial gradients of gold and warm white to simulate divine light emanating from behind content
- Apply thin gold borders and gilded accent lines to create a sense of sacred ornamentation
- Choose high-contrast classical serif typefaces that evoke Renaissance inscriptions and illuminated manuscripts
- Maintain generous white space to create an atmosphere of openness, purity, and transcendence
- Use translucent cream and ivory overlays to build ethereal depth without visual heaviness
- Reference classical symmetry and centered composition in your layouts
- Apply subtle warm-toned box shadows that feel like ambient heavenly glow rather than hard drop shadows
- Use circular and elliptical shapes (halos, aureoles) as decorative framing devices

### Don't

- Use harsh black shadows, dark backgrounds, or high-contrast dark modes that contradict the heavenly lightness
- Apply bold saturated colors (neon, electric, primary) that overpower the soft, muted celestial palette
- Choose industrial, brutalist, or monospaced typefaces; the aesthetic demands classical elegance
- Crowd the layout with dense content or cluttered navigation; celestial spaces require breathing room
- Use sharp geometric angles, hard corners, or aggressive diagonal lines
- Overdo the gold accents to the point of gaudiness; gold should feel like candlelight, not a jewelry store
- Combine Angelcore with grunge, cyberpunk, or dark gothic aesthetics that undermine the purity and light
- Apply heavy animation or rapid motion; movement should be slow, gentle, and ascending

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Coquette** | Shares soft femininity, blush pink tones, and delicate ornamentation; Coquette is boudoir-romantic while Angelcore is sacred-ethereal |
| **Baroque** | Direct art-historical ancestor; both use gold, ornament, and religious imagery, but Baroque is dramatic, heavy, and theatrical while Angelcore is soft and serene |
| **Rococo** | Shares pastel palette, gilded details, and cherub motifs; Rococo is playful and decorative while Angelcore is reverent and celestial |
| **Cottagecore** | Both celebrate innocence, purity, and soft natural beauty; Cottagecore is rural and earthbound while Angelcore is heavenly and transcendent |
| **Ethereal** | Near-synonym in mood; Ethereal is broader and more abstract while Angelcore specifically references angel iconography and religious art |
| **Fairycore** | Shares the dreamy, magical atmosphere and soft palette; Fairycore draws from woodland folklore while Angelcore draws from sacred mythology |
| **Light Academia** | Both favor warm whites, classical references, and elegant typography; Light Academia is scholarly while Angelcore is devotional |
| **Devilcore** | Direct opposite; Devilcore embraces darkness, red-black palettes, and demonic imagery as the anti-thesis to Angelcore's heavenly purity |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Seraphina - Angelcore Collection</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=EB+Garamond:wght@400;500&family=Cinzel:wght@400;700&family=Great+Vibes&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --angel-white: #FFFEF9;
      --angel-ivory: #FBF8F1;
      --angel-cream: #F5EFE0;
      --angel-gold: #D4A843;
      --angel-halo: #E8C766;
      --angel-pale-gold: #F2E4B3;
      --angel-blush: #F2D7D5;
      --angel-blue: #D4E4F1;
      --angel-lavender: #E3DAF0;
      --angel-dove: #C8C3B8;
      --angel-umber: #8A7D6B;
      --angel-dark: #3D362B;
    }

    body {
      font-family: 'EB Garamond', Georgia, serif;
      font-size: 1.125rem;
      line-height: 1.85;
      color: var(--angel-umber);
      background: var(--angel-white);
      min-height: 100vh;
    }

    /* --- Navigation --- */
    .nav {
      background: var(--angel-white);
      border-bottom: 1px solid var(--angel-pale-gold);
      padding: 20px 40px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 48px;
      position: relative;
    }

    .nav::after {
      content: '';
      position: absolute;
      bottom: -1px;
      left: 10%;
      right: 10%;
      height: 1px;
      background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
    }

    .nav a {
      color: var(--angel-umber);
      font-family: 'Cinzel', serif;
      font-size: 0.72rem;
      font-weight: 700;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .nav a:hover {
      color: var(--angel-gold);
    }

    /* --- Hero --- */
    .hero {
      background: linear-gradient(180deg, var(--angel-ivory) 0%, var(--angel-white) 100%);
      text-align: center;
      padding: 120px 40px 100px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: -30%;
      left: 25%;
      width: 50%;
      height: 160%;
      background: radial-gradient(ellipse at 50% 40%, rgba(232, 199, 102, 0.12) 0%, transparent 60%);
      pointer-events: none;
    }

    .hero::after {
      content: '';
      position: absolute;
      top: 10%;
      left: 50%;
      transform: translateX(-50%);
      width: 320px;
      height: 320px;
      border: 1px solid rgba(212, 168, 67, 0.12);
      border-radius: 50%;
      pointer-events: none;
    }

    .hero .script {
      font-family: 'Great Vibes', cursive;
      font-size: 1.6rem;
      color: var(--angel-gold);
      display: block;
      margin-bottom: 4px;
      position: relative;
    }

    .hero h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 3.5rem;
      font-weight: 600;
      color: var(--angel-dark);
      position: relative;
      line-height: 1.15;
    }

    .hero p {
      max-width: 520px;
      margin: 20px auto 0;
      color: var(--angel-umber);
      position: relative;
      font-size: 1.05rem;
    }

    .hero .cta {
      display: inline-block;
      margin-top: 32px;
      background: linear-gradient(135deg, var(--angel-gold) 0%, var(--angel-halo) 100%);
      color: var(--angel-white);
      border: none;
      border-radius: 50px;
      padding: 14px 40px;
      font-family: 'Cinzel', serif;
      font-weight: 700;
      font-size: 0.78rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      text-decoration: none;
      box-shadow: 0 4px 16px rgba(212, 168, 67, 0.30), inset 0 1px 0 rgba(255, 255, 255, 0.30);
      transition: all 0.4s ease;
      position: relative;
    }

    .hero .cta:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 28px rgba(212, 168, 67, 0.40), inset 0 1px 0 rgba(255, 255, 255, 0.40);
    }

    /* --- Divider --- */
    .divider {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      margin: 0 auto;
      padding: 48px 0;
      max-width: 400px;
    }

    .divider::before, .divider::after {
      content: '';
      flex: 1;
      height: 1px;
      background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
    }

    .divider span {
      width: 12px;
      height: 12px;
      border: 1.5px solid var(--angel-gold);
      border-radius: 50%;
      box-shadow: 0 0 8px rgba(212, 168, 67, 0.25);
    }

    /* --- Content Grid --- */
    .content {
      max-width: 860px;
      margin: 0 auto;
      padding: 0 40px 60px;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 32px;
    }

    .content.full-width {
      grid-template-columns: 1fr;
    }

    /* --- Cards --- */
    .card {
      background: var(--angel-ivory);
      border: 1px solid var(--angel-pale-gold);
      border-radius: 20px;
      padding: 40px;
      position: relative;
      box-shadow: 0 4px 24px rgba(212, 168, 67, 0.08), 0 1px 6px rgba(61, 54, 43, 0.04);
    }

    .card::before {
      content: '';
      position: absolute;
      top: -1px;
      left: 15%;
      right: 15%;
      height: 2px;
      background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
    }

    .card h2 {
      font-family: 'Cormorant Garamond', serif;
      font-weight: 600;
      font-size: 1.5rem;
      color: var(--angel-dark);
      margin-bottom: 12px;
    }

    .card p {
      color: var(--angel-umber);
      line-height: 1.8;
    }

    .card .tag {
      display: inline-block;
      margin-top: 16px;
      font-family: 'Cinzel', serif;
      font-size: 0.68rem;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--angel-gold);
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .card .tag:hover {
      color: var(--angel-dark);
    }

    /* --- Cloud Section --- */
    .cloud-section {
      background:
        radial-gradient(ellipse at 20% 80%, rgba(212, 228, 241, 0.3) 0%, transparent 50%),
        radial-gradient(ellipse at 80% 20%, rgba(242, 228, 179, 0.2) 0%, transparent 50%),
        radial-gradient(ellipse at 50% 50%, rgba(242, 215, 213, 0.15) 0%, transparent 60%),
        var(--angel-white);
      padding: 80px 40px;
      text-align: center;
    }

    .cloud-section h2 {
      font-family: 'Cormorant Garamond', serif;
      font-weight: 600;
      font-size: 2.2rem;
      color: var(--angel-dark);
      margin-bottom: 8px;
    }

    .cloud-section .script {
      font-family: 'Great Vibes', cursive;
      font-size: 1.4rem;
      color: var(--angel-gold);
      display: block;
      margin-bottom: 4px;
    }

    .cloud-section p {
      max-width: 520px;
      margin: 16px auto 0;
      color: var(--angel-umber);
    }

    /* --- Testimonial / Quote --- */
    .quote {
      max-width: 640px;
      margin: 0 auto;
      padding: 60px 40px;
      text-align: center;
    }

    .quote blockquote {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.5rem;
      font-style: italic;
      font-weight: 400;
      color: var(--angel-dark);
      line-height: 1.7;
      border: none;
      padding: 0;
      margin: 0;
    }

    .quote cite {
      display: block;
      margin-top: 16px;
      font-family: 'Cinzel', serif;
      font-size: 0.7rem;
      font-style: normal;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--angel-dove);
    }

    /* --- Footer --- */
    .footer {
      background: var(--angel-cream);
      border-top: 1px solid var(--angel-pale-gold);
      padding: 48px 40px;
      text-align: center;
      position: relative;
    }

    .footer::before {
      content: '';
      position: absolute;
      top: -1px;
      left: 10%;
      right: 10%;
      height: 1px;
      background: linear-gradient(to right, transparent, var(--angel-gold), transparent);
    }

    .footer .script {
      font-family: 'Great Vibes', cursive;
      font-size: 1.4rem;
      color: var(--angel-gold);
      display: block;
      margin-bottom: 8px;
    }

    .footer p {
      font-size: 0.9rem;
      color: var(--angel-dove);
    }

    /* --- Responsive --- */
    @media (max-width: 640px) {
      .nav { gap: 24px; padding: 16px 20px; }
      .nav a { font-size: 0.65rem; letter-spacing: 0.1em; }
      .hero { padding: 80px 24px 60px; }
      .hero h1 { font-size: 2.4rem; }
      .hero .script { font-size: 1.3rem; }
      .content { grid-template-columns: 1fr; padding: 0 24px 40px; }
      .card { padding: 28px; }
      .cloud-section { padding: 60px 24px; }
      .cloud-section h2 { font-size: 1.7rem; }
      .quote { padding: 40px 24px; }
      .quote blockquote { font-size: 1.2rem; }
    }
  </style>
</head>
<body>
  <nav class="nav">
    <a href="#">Sanctum</a>
    <a href="#">Collection</a>
    <a href="#">Devotion</a>
    <a href="#">About</a>
  </nav>

  <header class="hero">
    <span class="script">touched by grace</span>
    <h1>Seraphina</h1>
    <p>A collection inspired by celestial light, Renaissance angels,
       and the quiet beauty of things divine and eternal.</p>
    <a href="#" class="cta">Enter the Sanctum</a>
  </header>

  <div class="divider"><span></span></div>

  <main class="content">
    <div class="card">
      <h2>Wings of Gold</h2>
      <p>Draped in gilded light and soft ivory silk, each piece
         channels the radiance of a Renaissance cherub emerging
         from clouds of gold leaf and warm candlelight.</p>
      <a href="#" class="tag">Explore Collection &rarr;</a>
    </div>
    <div class="card">
      <h2>Heavenly Lace</h2>
      <p>Delicate lace and sheer organza layered like wisps of
         cloud, capturing the ethereal lightness of angel wings
         caught in a beam of morning sun.</p>
      <a href="#" class="tag">View Details &rarr;</a>
    </div>
  </main>

  <section class="cloud-section">
    <span class="script">a higher calling</span>
    <h2>The Celestial Atelier</h2>
    <p>Every creation begins with a meditation on light -- the way it
       falls through stained glass, halos a marble face, or turns
       ordinary clouds into cathedrals of the sky.</p>
  </section>

  <div class="divider"><span></span></div>

  <section class="quote">
    <blockquote>
      &ldquo;There is something in the softness of light, in the warmth of gold
      against white, that reminds us we were made for something
      more than the heaviness of this world.&rdquo;
    </blockquote>
    <cite>Seraphina Atelier, On Beauty and Light</cite>
  </section>

  <div class="divider"><span></span></div>

  <section class="content full-width">
    <div class="card">
      <h2>Our Philosophy</h2>
      <p>We believe that beauty is a form of devotion. Each design
         is crafted to evoke the serenity of a chapel at dawn -- golden
         light pouring through high windows, the scent of aged wood
         and white flowers, the hush of sacred space. Our materials
         are chosen for their ability to catch and hold light: silk that
         shimmers like a halo, lace as intricate as carved marble,
         and gold accents that glow with the warmth of votive candles.</p>
    </div>
  </section>

  <footer class="footer">
    <span class="script">with grace</span>
    <p>Seraphina Atelier &middot; Crafted in devotion to light and beauty</p>
  </footer>
</body>
</html>
```
