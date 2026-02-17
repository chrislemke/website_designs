# Steampunk Design Reference

Steampunk is a retro-futuristic aesthetic set in an alternate Victorian era where steam power, clockwork mechanisms, and brass engineering have advanced to fantastical levels. It depicts a world of copper pipes, leather straps, ornate clockwork gears, sepia-toned adventure, and baroque mechanical invention. The visual language draws from 19th-century industrial design, Jules Verne and H.G. Wells science fiction, and the ornamental craftsmanship of the Victorian period. In web design, Steampunk translates to warm sepia and copper color palettes, ornate serif typography, textured parchment backgrounds, brass UI elements, gear motifs, and a handcrafted quality that rejects the sterile precision of modern digital design.

---

## Visual Characteristics

### Core Design Traits

- **Warm sepia and amber tones** -- everything is filtered through a warm, aged lens suggesting antique photographs and candlelit workshops
- **Brass, copper, and bronze metallics** -- UI elements appear to be forged from polished metal, with specular highlights and warm reflections
- **Clockwork gears and cog motifs** -- interlocking gear shapes used as decorative elements, borders, and visual metaphors
- **Parchment and aged paper textures** -- backgrounds evoke old manuscripts, patent drawings, and Victorian-era documents
- **Ornate borders and filigree** -- decorative Victorian-style frames, corner ornaments, and flourishes
- **Leather and rivets** -- button and panel styling suggests stitched leather straps fastened with brass rivets
- **Exposed mechanical components** -- visible pipes, valves, gauges, and dials as UI metaphors
- **Victorian typography** -- ornamental serif typefaces, blackletter accents, and engraved lettering
- **Hand-drawn technical illustrations** -- patent-drawing-style line art, blueprints, and schematic diagrams
- **Warm atmospheric lighting** -- amber candlelight, gas lamp glow, and warm vignettes at the edges

### Design Principles

- Embrace ornamentation -- unlike minimalist aesthetics, Steampunk values decorative detail and craftsmanship
- Every element should feel handmade, mechanical, and tangible -- never sterile or purely digital
- Use warm color temperatures throughout -- cool blues and stark whites are foreign to this aesthetic
- Create a sense of layered materiality: metal over leather over parchment over wood
- Functional elements should look like Victorian-era instruments: gauges, dials, switches, levers
- Typography should feel engraved, stamped, or printed on a letterpress -- never pixel-perfect
- Borders and frames are features, not obstacles -- ornate framing elevates content
- The overall mood should feel like an inventor's workshop: cluttered, warm, fascinating, and alive
- Reference real Victorian engineering and design: Brunel's bridges, Victorian railway posters, patent office drawings

---

## Color Palette

### Victorian Workshop Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Polished Brass** | `#C8A84E` | Primary accent, buttons, key interactive elements |
| **Dark Brass** | `#9A7B2F` | Hover states, borders, active elements |
| **Antique Gold** | `#D4A843` | Highlights, star ratings, premium indicators |
| **Copper Pipe** | `#B87333` | Secondary accent, warm highlights |
| **Dark Copper** | `#8B5E3C` | Tertiary accent, deep warm tones |
| **Aged Parchment** | `#F4E8C1` | Light backgrounds, card surfaces |
| **Warm Cream** | `#FFF8E7` | Primary light background |
| **Sepia** | `#704214` | Primary text, headings |
| **Dark Leather** | `#3C2415` | Darkest text, footer backgrounds, nav bars |
| **Rich Mahogany** | `#4E1E0E` | Deep accent, dark section backgrounds |
| **Burnt Sienna** | `#A0522D` | Warm mid-tone accent |
| **Parchment Shadow** | `#D4C5A0` | Borders, dividers, subtle backgrounds |
| **Steel Gray** | `#6B6B6B` | Secondary text, captions, muted elements |
| **Iron Dark** | `#2C2C2C` | Heavy contrast elements, structural borders |
| **Rust Red** | `#8B3A1A` | Warning states, danger accents |
| **Verdigris** | `#43B3AE` | Oxidized copper accent, subtle cool contrast |

### CSS Custom Properties

```css
:root {
  /* Metallics */
  --steam-brass: #c8a84e;
  --steam-brass-dark: #9a7b2f;
  --steam-gold: #d4a843;
  --steam-copper: #b87333;
  --steam-copper-dark: #8b5e3c;

  /* Backgrounds */
  --steam-bg-parchment: #f4e8c1;
  --steam-bg-cream: #fff8e7;
  --steam-bg-dark: #3c2415;
  --steam-bg-mahogany: #4e1e0e;

  /* Text */
  --steam-text-sepia: #704214;
  --steam-text-dark: #3c2415;
  --steam-text-muted: #6b6b6b;
  --steam-text-light: #f4e8c1;

  /* Accents */
  --steam-sienna: #a0522d;
  --steam-rust: #8b3a1a;
  --steam-verdigris: #43b3ae;

  /* Borders */
  --steam-border-light: #d4c5a0;
  --steam-border-dark: #9a7b2f;

  /* Textures (subtle gradients simulating material) */
  --steam-leather: linear-gradient(145deg, #4a3020 0%, #3c2415 50%, #4a3020 100%);
  --steam-brass-surface: linear-gradient(145deg, #d4a843 0%, #c8a84e 40%, #9a7b2f 60%, #c8a84e 100%);
  --steam-parchment: linear-gradient(180deg, #fff8e7 0%, #f4e8c1 100%);
}
```

---

## Typography

### Typeface Characteristics

Steampunk typography is:

- **Ornate serif and slab serif** -- typefaces that feel engraved, stamped, or printed on a letterpress
- **Victorian-era display faces** -- decorative, high-contrast serifs with thick-thin stroke variation
- **Blackletter accents** -- gothic/fraktur letterforms used sparingly for decorative emphasis
- **Medium to heavy weights** -- bold presence that feels stamped into metal or embossed into leather
- **Uppercase for labels and headings** -- evoking brass nameplates and industrial signage
- **Monospaced for data** -- typewriter-style fonts suggesting technical notes and logbook entries
- **Generous line-height for body** -- comfortable reading on parchment-colored backgrounds

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Playfair Display** | High-contrast serif, elegant | Headlines, hero text, display |
| **Cinzel** | Roman-inscribed capitals, regal | Titles, headers, decorative text |
| **Spectral** | Refined transitional serif | Body text, readable long-form content |
| **Crimson Text** | Old-style serif, bookish | Body text, editorial content |
| **Libre Baskerville** | Classic Baskerville revival | Body text, elegant readability |
| **UnifrakturMaguntia** | Blackletter / Fraktur | Decorative accents, drop caps, logos |
| **Special Elite** | Typewriter | Technical notes, code, labels |
| **IM Fell English** | Historical printed text | Decorative body, Victorian feel |
| **Cormorant Garamond** | Elegant, high-contrast serif | Refined headlines, subheadings |
| **Bitter** | Contemporary slab serif | UI text, labels, readable at small sizes |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Cinzel** (700) | **Spectral** (400) | Regal and refined, Victorian formality |
| **Playfair Display** (700) | **Crimson Text** (400) | Elegant contrast, bookish warmth |
| **Cinzel** (700) | **Libre Baskerville** (400) | Classic, authoritative, engraved |
| **Cormorant Garamond** (600) | **Spectral** (400) | Refined, delicate, literary |
| **Playfair Display** (700) | **Special Elite** (400) | Dramatic heading, typewriter body |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700;900&family=Spectral:ital,wght@0,400;0,600;1,400&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Cinzel', 'Playfair Display', serif;
  font-weight: 700;
  color: var(--steam-text-sepia);
  line-height: 1.2;
  letter-spacing: 0.03em;
}

/* Display / Hero text */
.steam-display {
  font-family: 'Cinzel', serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  color: var(--steam-brass);
  text-shadow: 1px 1px 0 var(--steam-brass-dark), 2px 2px 4px rgba(0, 0, 0, 0.3);
}

/* Body text */
body {
  font-family: 'Spectral', 'Crimson Text', serif;
  font-weight: 400;
  font-size: 1.05rem;
  line-height: 1.8;
  color: var(--steam-text-sepia);
}

/* Industrial labels */
.steam-label {
  font-family: 'Cinzel', serif;
  font-weight: 700;
  font-size: 0.75rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--steam-text-muted);
}

/* Typewriter text */
.steam-typewriter {
  font-family: 'Special Elite', 'Courier New', monospace;
  font-size: 0.95rem;
  color: var(--steam-text-sepia);
  line-height: 1.6;
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, framed containers** -- content wrapped in ornate borders suggesting Victorian picture frames or patent documents
- **Parchment-colored backgrounds** -- warm cream and sepia tones throughout, never stark white
- **Ornate section dividers** -- decorative horizontal rules with gear, flourish, or filigree motifs
- **Asymmetric, workshop-style layouts** -- slightly imperfect arrangements suggesting a cluttered inventor's desk
- **Bordered cards and panels** -- every content block has a visible frame, like a brass nameplate or framed certificate
- **Header banners** -- section headings presented in banner-style frames with decorative corners
- **Two or three-column layouts** -- balanced, formal arrangements referencing newspaper and broadsheet design

### Section Organization

- **Navigation**: Dark leather-colored bar with brass-styled links, ornate logo, gear icon accents
- **Hero**: Parchment background with large serif headline, decorative border frame, technical illustration
- **Features**: Card grid with ornate borders, gear/cog icon accents, sepia-toned
- **Content rows**: Alternating parchment and darker sections with illustrated technical diagrams
- **Quote / Testimonial**: Ornate quotation marks, italicized serif text, decorative border
- **CTA section**: Dark leather background with brass-colored headline and metallic button
- **Footer**: Dark mahogany background, ornate top border, organized link columns

### Responsive Approach

- Maintain warm color temperatures across all breakpoints
- Simplify ornate borders on mobile -- reduce corner decorations but keep the border itself
- Stack columns vertically on mobile; maintain framed card styling
- Reduce decorative gear/filigree elements on small screens for clarity
- Typography remains serif-based at all sizes; increase line-height on mobile for readability

---

## CSS / Design Techniques

### Steampunk Card Component

```css
.steam-card {
  background: var(--steam-bg-parchment);
  border: 2px solid var(--steam-border-dark);
  border-radius: 2px;
  padding: 32px;
  position: relative;
  box-shadow: 0 2px 8px rgba(60, 36, 21, 0.15);
}

/* Corner rivets */
.steam-card::before,
.steam-card::after {
  content: '';
  position: absolute;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: radial-gradient(circle, var(--steam-gold) 30%, var(--steam-brass-dark) 70%);
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.3);
}

.steam-card::before { top: 8px; left: 8px; }
.steam-card::after { top: 8px; right: 8px; }

/* Card grid */
.steam-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 28px;
}
```

### Steampunk Button

```css
.steam-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--steam-brass-surface);
  color: var(--steam-bg-dark);
  border: 2px solid var(--steam-brass-dark);
  border-radius: 3px;
  padding: 12px 32px;
  font-family: 'Cinzel', serif;
  font-weight: 700;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2), inset 0 1px 0 rgba(255, 255, 255, 0.2);
  transition: all 0.2s ease;
}

.steam-button:hover {
  background: linear-gradient(145deg, #e0c060 0%, #d4a843 50%, #b08830 100%);
  box-shadow: 0 3px 8px rgba(0, 0, 0, 0.3), inset 0 1px 0 rgba(255, 255, 255, 0.3);
}

.steam-button:active {
  box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.3);
  transform: translateY(1px);
}

/* Dark variant */
.steam-button--dark {
  background: var(--steam-leather);
  color: var(--steam-gold);
  border-color: var(--steam-copper-dark);
}

.steam-button--dark:hover {
  background: linear-gradient(145deg, #5a3828 0%, #4a3020 50%, #5a3828 100%);
}

/* Outline variant */
.steam-button--outline {
  background: transparent;
  color: var(--steam-brass);
  border: 2px solid var(--steam-brass);
  box-shadow: none;
}

.steam-button--outline:hover {
  background: rgba(200, 168, 78, 0.1);
}
```

### Navigation Bar

```css
.steam-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 16px 40px;
  background: var(--steam-leather);
  border-bottom: 3px solid var(--steam-brass-dark);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
}

.steam-nav__logo {
  font-family: 'Cinzel', serif;
  font-weight: 900;
  font-size: 1.3rem;
  color: var(--steam-gold);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
}

.steam-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.steam-nav__links a {
  font-family: 'Cinzel', serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--steam-border-light);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  transition: color 0.2s;
}

.steam-nav__links a:hover {
  color: var(--steam-gold);
}
```

### Hero Section

```css
.steam-hero {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 100px 40px;
  background: var(--steam-parchment);
  position: relative;
}

/* Ornate top border */
.steam-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 5%;
  right: 5%;
  height: 4px;
  background: repeating-linear-gradient(
    90deg,
    var(--steam-brass) 0px,
    var(--steam-brass) 20px,
    transparent 20px,
    transparent 24px,
    var(--steam-brass-dark) 24px,
    var(--steam-brass-dark) 28px,
    transparent 28px,
    transparent 32px
  );
}

.steam-hero__content {
  max-width: 700px;
  border: 3px double var(--steam-border-dark);
  padding: 48px;
  background: rgba(255, 248, 231, 0.8);
}

.steam-hero__content h1 {
  font-size: clamp(2rem, 5vw, 3.5rem);
  color: var(--steam-brass);
  text-shadow: 1px 1px 0 var(--steam-brass-dark), 2px 2px 4px rgba(0, 0, 0, 0.2);
  margin-bottom: 1rem;
  text-transform: uppercase;
  letter-spacing: 0.06em;
}

.steam-hero__content p {
  font-size: 1.1rem;
  color: var(--steam-text-sepia);
  margin-bottom: 2rem;
  font-style: italic;
}

@media (max-width: 768px) {
  .steam-hero { padding: 60px 20px; }
  .steam-hero__content { padding: 28px; }
}
```

### Ornate Section Divider

```css
.steam-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
  margin: 48px auto;
  max-width: 400px;
}

.steam-divider::before,
.steam-divider::after {
  content: '';
  flex: 1;
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--steam-brass), transparent);
}

.steam-divider__gear {
  width: 28px;
  height: 28px;
  border: 3px solid var(--steam-brass);
  border-radius: 50%;
  position: relative;
}

.steam-divider__gear::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--steam-brass);
}
```

### Gauge / Meter Component

```css
.steam-gauge {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 12px;
}

.steam-gauge__dial {
  width: 100px;
  height: 50px;
  border: 3px solid var(--steam-brass);
  border-radius: 100px 100px 0 0;
  background: var(--steam-bg-parchment);
  position: relative;
  overflow: hidden;
}

.steam-gauge__fill {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  background: linear-gradient(0deg, var(--steam-rust), var(--steam-copper), var(--steam-gold));
  transition: height 0.5s ease;
}

.steam-gauge__label {
  font-family: 'Cinzel', serif;
  font-weight: 700;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--steam-text-muted);
}
```

---

## Design Do's and Don'ts

### Do

- Use warm, sepia-toned color palettes throughout -- brass, copper, amber, cream, dark brown
- Apply ornate borders, corner decorations, and Victorian-style frames to content containers
- Choose serif typefaces with character: Cinzel, Playfair Display, or Spectral
- Add tactile material textures: parchment backgrounds, leather panels, metallic button surfaces
- Include clockwork gear motifs as decorative elements and visual metaphors
- Use `box-shadow` and subtle gradients to create metallic, three-dimensional surfaces
- Reference real Victorian engineering aesthetics: rivet patterns, gauge instruments, blueprint drawings
- Make buttons and interactive elements feel like brass switches or leather-wrapped controls

### Don't

- Use cool colors (blue, green, pure white) as primary palette colors -- they break the warm Victorian atmosphere
- Apply flat, shadow-free styling -- Steampunk embraces material depth and tactile surfaces
- Use sans-serif typefaces for headings -- they feel too modern and digital
- Strip away ornamentation -- unlike minimalist aesthetics, Steampunk values decorative richness
- Use neon or electric glow effects -- the light sources are candles, gas lamps, and fire
- Make layouts too clean and grid-perfect -- some organic imperfection adds character
- Forget the materiality -- every surface should suggest a physical material (metal, leather, paper, wood)
- Mix in modern digital UI patterns (flat toggles, pill buttons) that break the period illusion

---

## Related Aesthetics

| Aesthetic | Relationship to Steampunk |
|-----------|--------------------------|
| **Art Nouveau** | Contemporary of the Victorian era; shares organic ornamentation but favors flowing natural curves over mechanical geometry |
| **Art Deco** | Later successor (1920s-30s); shares the love of ornamentation and metallic materials but is more geometric and streamlined |
| **Arts and Crafts** | Parallel Victorian movement; shares the handmade ethos and rejection of industrial mass production |
| **Gothic** | Shares the Victorian architectural vocabulary; darker and more ecclesiastical than Steampunk's workshop warmth |
| **Baroque** | Shares the love of ornamentation and richness; Baroque is royal and religious, Steampunk is industrial and inventive |
| **Cyberpunk** | Fellow "-punk" aesthetic; both critique technology and society, but Steampunk looks to a Victorian past, Cyberpunk to a digital future |
| **Dieselpunk** | Direct sibling; shifts the era from Victorian steam to 1920s-40s diesel and Art Deco industrial |
| **Clockpunk** | Sub-aesthetic focused specifically on clockwork and Renaissance-era mechanics |
| **Skeuomorphism** | Shares the desire for digital elements that feel like physical objects; Steampunk applies this with Victorian materials |

---

## Quick-Start: Minimal Steampunk Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Steampunk Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700;900&family=Spectral:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
  <style>
    :root {
      --steam-brass: #c8a84e;
      --steam-brass-dark: #9a7b2f;
      --steam-gold: #d4a843;
      --steam-copper: #b87333;
      --steam-bg-parchment: #f4e8c1;
      --steam-bg-cream: #fff8e7;
      --steam-bg-dark: #3c2415;
      --steam-bg-mahogany: #4e1e0e;
      --steam-text-sepia: #704214;
      --steam-text-muted: #6b6b6b;
      --steam-text-light: #f4e8c1;
      --steam-border-light: #d4c5a0;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--steam-bg-cream);
      color: var(--steam-text-sepia);
      font-family: 'Spectral', serif;
      font-size: 1.05rem;
      line-height: 1.8;
    }

    h1, h2, h3 {
      font-family: 'Cinzel', serif;
      font-weight: 700;
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 14px 40px;
      background: linear-gradient(145deg, #4a3020, #3c2415, #4a3020);
      border-bottom: 3px solid var(--steam-brass-dark);
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
    }

    nav a.logo {
      font-family: 'Cinzel', serif;
      font-weight: 900;
      font-size: 1.2rem;
      color: var(--steam-gold);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'Cinzel', serif;
      font-weight: 500;
      font-size: 0.85rem;
      color: var(--steam-border-light);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--steam-gold); }

    /* Hero */
    .hero {
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 100px 40px;
      background: linear-gradient(180deg, var(--steam-bg-cream), var(--steam-bg-parchment));
    }

    .hero-content {
      max-width: 680px;
      border: 3px double var(--steam-brass-dark);
      padding: 48px;
      background: rgba(255, 248, 231, 0.85);
    }

    .hero h1 {
      font-size: clamp(2rem, 5vw, 3.5rem);
      color: var(--steam-brass);
      text-shadow: 1px 1px 0 var(--steam-brass-dark), 2px 2px 4px rgba(0, 0, 0, 0.2);
      text-transform: uppercase;
      letter-spacing: 0.06em;
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.1rem;
      font-style: italic;
      color: var(--steam-text-sepia);
      margin-bottom: 2rem;
    }

    .btn {
      display: inline-block;
      background: linear-gradient(145deg, #d4a843, #c8a84e, #9a7b2f, #c8a84e);
      color: var(--steam-bg-dark);
      border: 2px solid var(--steam-brass-dark);
      border-radius: 3px;
      padding: 12px 36px;
      font-family: 'Cinzel', serif;
      font-weight: 700;
      font-size: 0.85rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2), inset 0 1px 0 rgba(255, 255, 255, 0.2);
      transition: all 0.2s;
    }

    .btn:hover {
      background: linear-gradient(145deg, #e0c060, #d4a843, #b08830);
      box-shadow: 0 3px 8px rgba(0, 0, 0, 0.3), inset 0 1px 0 rgba(255, 255, 255, 0.3);
    }

    /* Divider */
    .divider {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      margin: 0 auto;
      max-width: 300px;
      padding: 32px 0;
    }

    .divider::before, .divider::after {
      content: '';
      flex: 1;
      height: 2px;
      background: linear-gradient(90deg, transparent, var(--steam-brass), transparent);
    }

    .divider-gear {
      width: 22px; height: 22px;
      border: 3px solid var(--steam-brass);
      border-radius: 50%;
      position: relative;
    }

    .divider-gear::before {
      content: '';
      position: absolute;
      top: 50%; left: 50%;
      transform: translate(-50%, -50%);
      width: 6px; height: 6px;
      border-radius: 50%;
      background: var(--steam-brass);
    }

    /* Features */
    .features {
      padding: 60px 0;
      background: var(--steam-bg-parchment);
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--steam-text-sepia);
      text-transform: uppercase;
      letter-spacing: 0.04em;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 28px;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: var(--steam-bg-cream);
      border: 2px solid var(--steam-brass-dark);
      padding: 28px;
      position: relative;
      box-shadow: 0 2px 6px rgba(60, 36, 21, 0.12);
    }

    /* Corner rivets */
    .feature::before, .feature::after {
      content: '';
      position: absolute;
      width: 8px; height: 8px;
      border-radius: 50%;
      background: radial-gradient(circle, var(--steam-gold) 30%, var(--steam-brass-dark) 70%);
      box-shadow: 0 1px 2px rgba(0, 0, 0, 0.3);
    }

    .feature::before { top: 8px; left: 8px; }
    .feature::after { top: 8px; right: 8px; }

    .feature h3 { font-size: 1.1rem; margin-bottom: 0.5rem; color: var(--steam-copper); }
    .feature p { color: var(--steam-text-muted); font-size: 0.95rem; }

    /* CTA */
    .cta {
      background: linear-gradient(145deg, #4a3020, #3c2415, #4e1e0e);
      text-align: center;
      padding: 80px 40px;
      border-top: 3px solid var(--steam-brass-dark);
      border-bottom: 3px solid var(--steam-brass-dark);
    }

    .cta h2 {
      font-size: 2rem;
      color: var(--steam-gold);
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
      text-transform: uppercase;
      letter-spacing: 0.04em;
      margin-bottom: 1rem;
    }

    .cta p {
      color: var(--steam-border-light);
      font-style: italic;
      margin-bottom: 2rem;
    }

    .cta .btn {
      background: transparent;
      color: var(--steam-gold);
      border: 2px solid var(--steam-gold);
      box-shadow: none;
    }

    .cta .btn:hover {
      background: rgba(200, 168, 78, 0.15);
    }

    /* Footer */
    footer {
      background: var(--steam-bg-mahogany);
      text-align: center;
      padding: 30px 40px;
      color: var(--steam-text-muted);
      font-size: 0.9rem;
      border-top: 2px solid var(--steam-brass-dark);
    }

    @media (max-width: 768px) {
      .hero { padding: 60px 20px; }
      .hero-content { padding: 28px; }
      nav { padding: 12px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Aetheric Co.</a>
    <ul>
      <li><a href="#">Workshop</a></li>
      <li><a href="#">Inventions</a></li>
      <li><a href="#">Patents</a></li>
      <li><a href="#">Journal</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>The Grand Apparatus</h1>
      <p>Precision clockwork engineering for the discerning inventor. Brass-forged instruments of extraordinary capability, crafted in our London workshop since 1887.</p>
      <a href="#" class="btn">View Catalogue</a>
    </div>
  </section>

  <div class="divider">
    <div class="divider-gear"></div>
  </div>

  <section class="features">
    <h2>Apparatus & Instruments</h2>
    <div class="features-grid">
      <div class="feature">
        <h3>Chronometric Engine</h3>
        <p>A self-winding temporal calculator of unparalleled accuracy. Measures the passage of moments down to the thousandth of a second.</p>
      </div>
      <div class="feature">
        <h3>Aether Compass</h3>
        <p>Navigate the invisible currents of the luminiferous aether with this handcrafted brass instrument, fitted with precision crystal lenses.</p>
      </div>
      <div class="feature">
        <h3>Pneumatic Relay</h3>
        <p>Steam-powered message transmission across vast distances. Copper-piped communication networks for the modern empire.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Commission a Bespoke Instrument</h2>
    <p>Our master artificers await your specifications. Every creation is forged by hand, tested by fire, and guaranteed for a lifetime.</p>
    <a href="#" class="btn">Enquire</a>
  </section>

  <footer>
    <p>The Aetheric Company, Ltd. -- Established 1887, London -- Purveyors of Fine Clockwork</p>
  </footer>
</body>
</html>
```
