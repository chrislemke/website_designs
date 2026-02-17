# Manguebeat Design Reference

Manguebeat (also spelled Mangue Beat or Mangue bit) is a cultural and musical movement that emerged circa 1991 in Recife, Pernambuco, northeastern Brazil, as a reaction to the cultural and economic stagnation of the city. Founded by musicians Chico Science and Fred Zero Quatro, the movement fuses **traditional Pernambucan rhythms** (maracatu, frevo, coco, embolada) with **global contemporary genres** (rock, hip-hop, funk, electronic, raggamuffin). Visually, Manguebeat represents a **raw, tropical-urban collision aesthetic** -- mangrove mud meets satellite dishes, Afro-Brazilian carnival vibrancy meets DIY punk grit, and psychedelic folk patterns meet digital-age collage. The movement's manifesto, "Caranguejos com Cerebro" (Crabs with Brains, 1992), established the core visual metaphor: a parabolic antenna stuck in the mud, receiving signals from the entire world.

---

## Visual Characteristics

### Core Motifs and Symbols

- **The Crab (Caranguejo)** -- central emblem of the movement; represents resilience, mangrove life, and the people of Recife's impoverished waterfront communities
- **Parabolic antenna in mud** -- the defining manifesto symbol; a satellite dish planted in mangrove sludge, embodying the fusion of local tradition with global modernity
- **Mangrove ecosystem imagery** -- tangled roots, brackish water, mud flats, tidal zones; the organic chaos of coastal wetlands
- **Maracatu patterns** -- psychedelic visual language drawn from Afro-Brazilian carnival processions: embroidered banners, feathered headdresses, mirrored costumes
- **Frevo umbrellas** -- small, colorful spinning umbrellas iconic to Pernambuco carnival, representing energy and movement
- **Collage and pixelation** -- the "Da Lama ao Caos" album cover (designed by Hilton Lacerda) pioneered a collage-mosaic style where each "pixel" is a different layered image
- **Graffiti and street murals** -- urban wall art depicting crabs, mangroves, and movement iconography across Recife
- **Straw hats (chapeu de palha)** -- traditional Pernambucan headwear, often juxtaposed with modern urban accessories

### Design Principles

- **Collision of tradition and technology** -- deliberate juxtaposition of folk/organic elements with digital/electronic elements
- **Raw, unpolished texture** -- gritty, muddy, DIY quality; not clean or corporate
- **Tropical maximalism** -- dense, vibrant, saturated compositions drawing from carnival excess
- **Anti-elitist, resourceful aesthetic** -- thrifted, repurposed, and improvised visual language
- **Cultural layering** -- Afro-Brazilian, Indigenous, Portuguese colonial, and global pop culture references stacked together
- **Ecological grounding** -- persistent references to mangrove ecosystems, water, mud, and organic life
- **Urban-rural tension** -- city grit meets coastal nature; concrete meets mangrove

---

## Color Palette

### Primary Scheme

The Manguebeat palette draws from two sources: the **earthy, organic tones of the mangrove** (mud brown, brackish green, murky water) and the **explosive vibrancy of Pernambucan carnival** (maracatu reds, golds, blues; frevo primary colors). These combine to create a distinctive warm-tropical-meets-gritty-earth palette.

| Role | Colors |
|------|--------|
| **Mangrove earth tones** | Mud brown, dark olive, brackish teal, silty ochre |
| **Carnival vibrancy** | Vibrant red, royal blue, bright yellow, emerald green |
| **Accent / energy** | Hot coral, gold/amber, electric turquoise |
| **Ground / darkness** | Rich black-brown, deep mangrove green |

### Color Details

| Color | Hex | Usage |
|-------|-----|-------|
| Mangrove Mud | `#4A3728` | Dark backgrounds, grounding elements |
| Brackish Green | `#2D5A27` | Secondary backgrounds, organic accents |
| Silty Ochre | `#C4943A` | Warm midtones, border accents |
| Tidal Teal | `#1A6B5A` | Waterline accents, secondary surfaces |
| Maracatu Red | `#D42020` | Primary accent, headlines, energy |
| Carnival Gold | `#F0B816` | Highlights, icons, star elements |
| Royal Blue | `#1848B0` | Secondary accent, contrast blocks |
| Emerald Green | `#10A848` | Tertiary accent, ecological references |
| Frevo White | `#F5F0E6` | Text on dark backgrounds, light accents |
| Crab Coral | `#E85530` | Hot accent, call-to-action elements |
| Deep Black-Brown | `#1A1410` | Deepest background, text shadows |
| Antenna Silver | `#A0A8B0` | Metallic/tech references, subtle UI elements |

### Suggested CSS Custom Properties

```css
:root {
  /* Mangrove Earth Tones */
  --mangue-mud: #4a3728;
  --mangue-mud-dark: #2e2118;
  --mangue-mud-light: #6b5340;
  --mangue-brackish: #2d5a27;
  --mangue-ochre: #c4943a;
  --mangue-teal: #1a6b5a;

  /* Carnival Vibrancy */
  --mangue-red: #d42020;
  --mangue-gold: #f0b816;
  --mangue-blue: #1848b0;
  --mangue-green: #10a848;
  --mangue-coral: #e85530;

  /* Neutrals */
  --mangue-white: #f5f0e6;
  --mangue-off-white: #e8e0d0;
  --mangue-silver: #a0a8b0;
  --mangue-black: #1a1410;
  --mangue-near-black: #231c14;

  /* Functional */
  --mangue-bg-primary: var(--mangue-black);
  --mangue-bg-secondary: var(--mangue-mud-dark);
  --mangue-bg-card: var(--mangue-mud);
  --mangue-text-primary: var(--mangue-white);
  --mangue-text-secondary: var(--mangue-off-white);
  --mangue-text-accent: var(--mangue-gold);
  --mangue-accent-primary: var(--mangue-red);
  --mangue-accent-secondary: var(--mangue-coral);
  --mangue-accent-cool: var(--mangue-teal);
}
```

### Color Usage Approaches

- **Earth-grounded vibrancy** -- vibrant carnival colors always anchored by dark, muddy earth tones underneath
- **Warm dominance** -- reds, golds, oranges, and corals dominate; cooler blues and greens serve as contrast accents
- **High saturation on dark grounds** -- bright, saturated colors placed against deep brown-black backgrounds (not pure black -- use warm dark tones)
- **Mud gradient** -- use gradients that transition from dark mud to brackish green, evoking the mangrove waterline
- **Carnival bursts** -- moments of full-spectrum primary color used sparingly for maximum impact (red + blue + yellow + green together)
- **Gold as connective tissue** -- carnival gold/amber used for borders, highlights, and linking elements

---

## Typography

### Typeface Characteristics

Manguebeat typography fuses:

- **Raw, hand-painted street art lettering** -- graffiti influence from Recife's urban walls
- **Bold, condensed, high-impact display type** -- designed to be seen on concert posters and murals
- **Irregular, organic letterforms** -- imperfect baselines, varied weight, handmade quality
- **Stencil and spray-paint textures** -- DIY punk influence on type treatment
- **Mixed case and mixed styles** -- combining script, sans-serif, and decorative faces in a single composition
- **Carnival poster typography** -- large, colorful, attention-grabbing event type from frevo and maracatu flyers

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Archivo Black** | Ultra-bold, condensed sans | Primary headlines, impact text |
| **Barrio** | Hand-drawn, irregular display | Hero text, decorative headings |
| **Permanent Marker** | Hand-drawn marker | Subheadings, street-art feel |
| **Bebas Neue** | Tall, condensed sans | Section headers, all-caps titles |
| **Patua One** | Bold slab serif with warmth | Secondary headings, statements |
| **Bungee** | Bold geometric display | Accent text, labels |
| **Stint Ultra Expanded** | Wide, bold serif | Dramatic display moments |
| **Amaranth** | Humanist sans, slightly irregular | Body headings, navigation |
| **Source Sans 3** | Clean humanist sans-serif | Body text, readable content |
| **Lora** | Transitional serif | Body text alternative, longer passages |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Archivo+Black&family=Barrio&family=Permanent+Marker&family=Bebas+Neue&family=Patua+One&family=Source+Sans+3:wght@400;600;700&display=swap');

/* Primary headlines -- bold, raw, impactful */
h1 {
  font-family: 'Archivo Black', 'Bebas Neue', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.03em;
  color: var(--mangue-gold);
  text-shadow:
    3px 3px 0 var(--mangue-red),
    6px 6px 0 rgba(26, 20, 16, 0.6);
  line-height: 0.95;
}

/* Hero / Display text -- hand-drawn, organic */
.mangue-display {
  font-family: 'Barrio', 'Permanent Marker', cursive;
  font-size: clamp(3rem, 10vw, 8rem);
  letter-spacing: 0.02em;
  line-height: 1.0;
  color: var(--mangue-red);
  text-shadow:
    2px 2px 0 var(--mangue-gold),
    4px 4px 0 var(--mangue-mud);
}

/* Section headings */
h2 {
  font-family: 'Patua One', 'Permanent Marker', serif;
  color: var(--mangue-coral);
  letter-spacing: 0.02em;
  text-shadow:
    2px 2px 0 var(--mangue-mud-dark);
}

/* Subheadings */
h3 {
  font-family: 'Bebas Neue', 'Archivo Black', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--mangue-gold);
}

/* Body text */
body {
  font-family: 'Source Sans 3', sans-serif;
  font-weight: 400;
  letter-spacing: 0.01em;
  line-height: 1.7;
  color: var(--mangue-text-primary);
}
```

---

## Layout Principles

### Grid and Structure

- **Organic, asymmetric composition** -- avoid rigid, uniform grids; use offset and overlapping elements
- **Collage-style layering** -- elements overlap, text sits on images, borders bleed
- **Dense but not claustrophobic** -- fill space with content and texture, but allow breathing room through contrast rather than whitespace
- **Full-bleed color blocks** -- large sections of saturated carnival color, edge to edge
- **Mud-to-sky vertical flow** -- dark/earthy tones at the bottom, lighter/brighter elements rising upward (echoing mangrove-to-canopy)
- **Broken grid moments** -- elements that intentionally break the layout grid, jutting out or overlapping section boundaries

### Section Organization

- Use **thick, textured dividers** between sections (mud-colored bars, tangled root patterns, carnival stripe borders)
- Create **hierarchy through color temperature** -- warm reds/golds for primary content, cooler teals/blues for secondary
- Employ **rough-edged containers** -- irregular borders, torn-paper effects, organic shapes
- Mix **card-based content** with **full-width statement sections** for rhythm variation
- Apply **collage overlaps** at section boundaries -- elements from one section bleeding into the next
- Use **crab or antenna icons** as section markers or bullet points

### Responsive Approach

- Mobile: single column, stacked carnival-color blocks, large bold type
- Tablet: offset two-column, asymmetric card layouts
- Desktop: three-column collage grid with overlapping elements and full-width hero sections

---

## CSS/Design Techniques

### Mud Gradient Background

```css
/* Mangrove mud gradient -- the foundational Manguebeat surface */
.mangue-mud-bg {
  background: linear-gradient(
    180deg,
    var(--mangue-black) 0%,
    var(--mangue-mud-dark) 30%,
    var(--mangue-mud) 60%,
    var(--mangue-brackish) 100%
  );
}

/* Tidal waterline effect */
.mangue-waterline {
  background:
    linear-gradient(
      180deg,
      var(--mangue-mud-dark) 0%,
      var(--mangue-mud-dark) 48%,
      var(--mangue-teal) 48%,
      var(--mangue-teal) 52%,
      var(--mangue-mud-dark) 52%,
      var(--mangue-mud-dark) 100%
    );
}
```

### Carnival Stripe Divider

```css
/* Maracatu / frevo-inspired carnival stripe */
.mangue-carnival-stripe {
  width: 100%;
  height: 8px;
  background: repeating-linear-gradient(
    90deg,
    var(--mangue-red) 0px,
    var(--mangue-red) 40px,
    var(--mangue-gold) 40px,
    var(--mangue-gold) 80px,
    var(--mangue-blue) 80px,
    var(--mangue-blue) 120px,
    var(--mangue-green) 120px,
    var(--mangue-green) 160px
  );
}

/* Thicker carnival bar with texture */
.mangue-carnival-bar {
  width: 100%;
  height: 24px;
  background: repeating-linear-gradient(
    -45deg,
    var(--mangue-red) 0px,
    var(--mangue-red) 12px,
    var(--mangue-gold) 12px,
    var(--mangue-gold) 24px,
    var(--mangue-blue) 24px,
    var(--mangue-blue) 36px,
    var(--mangue-green) 36px,
    var(--mangue-green) 48px
  );
  box-shadow:
    0 2px 8px rgba(212, 32, 32, 0.4),
    0 -2px 8px rgba(240, 184, 22, 0.3);
}
```

### Collage / Pixel-Mosaic Effect

```css
/* Inspired by the Da Lama ao Caos album cover collage style */
.mangue-collage-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(80px, 1fr));
  gap: 2px;
}

.mangue-collage-grid > * {
  aspect-ratio: 1;
  overflow: hidden;
  border: 1px solid var(--mangue-mud-dark);
}

/* Pixelated image treatment */
.mangue-pixelate {
  image-rendering: pixelated;
  filter: contrast(1.3) saturate(1.4);
}
```

### Gritty Texture Overlay

```css
/* Mud/grain texture overlay -- simulates the raw, unpolished Manguebeat feel */
.mangue-grit::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    radial-gradient(circle, rgba(196, 148, 58, 0.04) 1px, transparent 1px),
    radial-gradient(circle, rgba(74, 55, 40, 0.06) 1px, transparent 1px);
  background-size: 4px 4px, 7px 7px;
  background-position: 0 0, 3px 3px;
  pointer-events: none;
  mix-blend-mode: overlay;
}

/* Noise texture for that analog, street-art feel */
.mangue-noise::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
  pointer-events: none;
  opacity: 0.5;
}
```

### Manguebeat Card / Panel

```css
.mangue-card {
  background: var(--mangue-mud);
  border: 3px solid var(--mangue-ochre);
  border-left: 6px solid var(--mangue-red);
  border-radius: 2px;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    4px 4px 0 var(--mangue-mud-dark),
    8px 8px 0 rgba(26, 20, 16, 0.3);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.mangue-card:hover {
  transform: translate(-2px, -2px);
  box-shadow:
    6px 6px 0 var(--mangue-mud-dark),
    10px 10px 0 rgba(26, 20, 16, 0.3);
}

/* Carnival accent bar at top of card */
.mangue-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(
    90deg,
    var(--mangue-red),
    var(--mangue-gold),
    var(--mangue-blue),
    var(--mangue-green)
  );
}
```

### Crab Icon (CSS-only)

```css
/* Stylized crab symbol -- the Manguebeat emblem */
.mangue-crab {
  display: inline-block;
  width: 40px;
  height: 28px;
  background: var(--mangue-coral);
  border-radius: 50% 50% 30% 30%;
  position: relative;
}

.mangue-crab::before,
.mangue-crab::after {
  content: '';
  position: absolute;
  width: 20px;
  height: 3px;
  background: var(--mangue-coral);
  top: 4px;
  border-radius: 2px;
}

.mangue-crab::before {
  left: -14px;
  transform: rotate(-30deg);
}

.mangue-crab::after {
  right: -14px;
  transform: rotate(30deg);
}
```

### Mangrove Root Border Pattern

```css
/* Organic, tangled mangrove-root border effect */
.mangue-root-border {
  border-image: repeating-linear-gradient(
    -45deg,
    var(--mangue-brackish) 0px,
    var(--mangue-mud) 4px,
    var(--mangue-teal) 4px,
    var(--mangue-brackish) 8px
  ) 8;
  border-width: 4px;
  border-style: solid;
}

/* Wavy, organic section divider evoking tidal motion */
.mangue-wave-divider {
  width: 100%;
  height: 30px;
  background: var(--mangue-teal);
  clip-path: polygon(
    0% 60%, 3% 40%, 7% 55%, 12% 35%, 18% 50%, 24% 30%,
    30% 55%, 36% 35%, 42% 50%, 48% 30%, 54% 55%, 60% 35%,
    66% 50%, 72% 30%, 78% 55%, 84% 35%, 90% 50%, 95% 35%,
    100% 55%, 100% 100%, 0% 100%
  );
  opacity: 0.7;
}
```

### Antenna / Technology Accent

```css
/* Satellite dish / antenna metallic accent line */
.mangue-antenna-line {
  width: 100%;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    var(--mangue-silver) 20%,
    var(--mangue-white) 50%,
    var(--mangue-silver) 80%,
    transparent 100%
  );
  position: relative;
}

.mangue-antenna-line::after {
  content: '';
  position: absolute;
  right: 50%;
  top: -4px;
  width: 10px;
  height: 10px;
  background: var(--mangue-silver);
  border-radius: 50%;
  box-shadow: 0 0 6px var(--mangue-silver);
}
```

### Psychedelic Maracatu Background

```css
/* Layered radial gradients evoking carnival energy */
.mangue-carnival-bg {
  background: var(--mangue-black);
  background-image:
    radial-gradient(ellipse at 15% 60%, rgba(212, 32, 32, 0.15) 0%, transparent 50%),
    radial-gradient(ellipse at 75% 20%, rgba(240, 184, 22, 0.12) 0%, transparent 45%),
    radial-gradient(ellipse at 50% 80%, rgba(24, 72, 176, 0.1) 0%, transparent 50%),
    radial-gradient(ellipse at 85% 70%, rgba(16, 168, 72, 0.08) 0%, transparent 40%);
}

/* Animated shimmer -- like sunlight on tidal water */
@keyframes mangue-shimmer {
  0%   { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}

.mangue-shimmer {
  background: linear-gradient(
    90deg,
    transparent 0%,
    rgba(240, 184, 22, 0.08) 25%,
    rgba(196, 148, 58, 0.15) 50%,
    rgba(240, 184, 22, 0.08) 75%,
    transparent 100%
  );
  background-size: 200% 100%;
  animation: mangue-shimmer 6s ease-in-out infinite;
}
```

### Oversaturation / Tropical Filter

```css
/* Apply to images for that hyper-vivid tropical-carnival look */
.mangue-saturate {
  filter: saturate(160%) contrast(1.15) brightness(1.05);
}

/* Warm mud-tone overlay on images */
.mangue-mud-overlay {
  position: relative;
}

.mangue-mud-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(
    180deg,
    rgba(74, 55, 40, 0.2) 0%,
    rgba(26, 20, 16, 0.4) 100%
  );
  mix-blend-mode: multiply;
  pointer-events: none;
}

/* Carnival color-shift overlay */
.mangue-carnival-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(
    135deg,
    rgba(212, 32, 32, 0.15),
    rgba(240, 184, 22, 0.1),
    rgba(16, 168, 72, 0.1)
  );
  mix-blend-mode: screen;
  pointer-events: none;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Manguebeat materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Mangrove mud, silt, organic matter | Dark warm-brown backgrounds with grain/noise texture overlay |
| Brackish tidal water | Teal-green gradients, subtle shimmer animations |
| Maracatu embroidered banners (red/gold thread) | Bold red/gold border accents, decorative stripe patterns |
| Frevo spinning umbrellas | Rotating color elements, carnival stripe dividers |
| Street graffiti on weathered concrete | Rough textures, hand-drawn fonts, offset layering |
| Album cover collage / pixel mosaic | CSS grid mosaics, overlapping image layers |
| Straw hat weave | Subtle crosshatch or woven background patterns |
| Satellite dish metal | Metallic silver gradients, antenna-line accents |
| Carnival sequins and mirrors | Shimmer animations, reflective highlights |
| Screen-printed concert flyer | Bold type, limited color blocks, visible print texture |

---

## Sub-styles and Variations

### Mangue-Roots (Traditional Focus)

- Emphasis on maracatu and frevo visual traditions
- Richer earth tones, less technology reference
- Embroidery-inspired borders and ornamentation
- Carnival costume colors dominate (deep red, royal blue, gold)
- Handcraft textures and woven patterns

### Mangue-Cyber / Afrociberdelia

- Named after Chico Science's second album "Afrociberdelia"
- Stronger technology and digital references
- Pixelation and collage effects
- Satellite and antenna motifs more prominent
- More electric/neon color accents mixed with earth tones
- Glitch and data-moshing visual effects blended with organic textures

### Mangue-Street (Urban Graffiti)

- Graffiti and mural art dominant
- Spray-paint textures and stencil typography
- Concrete and urban surfaces as backgrounds
- Hip-hop visual culture influence
- Bolder, more graphic compositions
- Black and white photography mixed with color splashes

---

## Notable Visual Practitioners

| Artist / Designer | Role |
|-------------------|------|
| **Hilton Lacerda** | Director and designer of "Da Lama ao Caos" album cover; key visual architect |
| **Jorge du Peixe** | Nação Zumbi percussionist; graffiti artist and designer who shaped movement's visual identity |
| **Ayode Franca** | Black artist/illustrator from Pernambuco; visual language exploring local popular culture and Afro-Brazilian archetypes |
| **Kboco** | Recife graffiti artist; signature style influenced by African, Mayan, and Indigenous Brazilian design |
| **Fred Zero Quatro** | Mundo Livre S/A frontman; co-author of the manifesto; shaped the movement's conceptual visual identity |
| **Chico Science** | Movement founder; his personal style (straw hat + sunglasses + printed shirts) became the iconic Manguebeat look |

---

## Related Aesthetics

| Aesthetic | Relationship to Manguebeat |
|-----------|----------------------------|
| **Psychedelia** | Direct influence on swirling patterns, saturated colors, and expanded-consciousness visual language |
| **Hip-Hop** | Shared urban culture roots: graffiti, street wear, DIY poster art, bold typography |
| **Rave** | Electronic music crossover; shared energy in visual dynamism and color intensity |
| **Funk** | Musical and visual kinship through Afro-Brazilian rhythmic culture and bold expression |
| **DIY Punk** | Shared anti-establishment ethos; raw, unpolished, hand-made visual aesthetic |
| **Tropical** | Lush vegetation, warm saturated colors, coastal imagery |
| **Afrofuturism** | Parallel exploration of African diasporic identity through technology and tradition |
| **Chicha** | South American musical-visual movement with similar fusion of folk tradition and urban popular culture |
| **Graffiti Pop** | Shared street art origins and bold, graphic visual language |
| **Lowbrow** | Common outsider-art positioning and celebration of popular culture over fine art |

---

## Quick-Start: Minimal Manguebeat Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Manguebeat Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Archivo+Black&family=Barrio&family=Permanent+Marker&family=Patua+One&family=Bebas+Neue&family=Source+Sans+3:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --mangue-mud: #4a3728;
      --mangue-mud-dark: #2e2118;
      --mangue-mud-light: #6b5340;
      --mangue-brackish: #2d5a27;
      --mangue-ochre: #c4943a;
      --mangue-teal: #1a6b5a;
      --mangue-red: #d42020;
      --mangue-gold: #f0b816;
      --mangue-blue: #1848b0;
      --mangue-green: #10a848;
      --mangue-coral: #e85530;
      --mangue-white: #f5f0e6;
      --mangue-off-white: #e8e0d0;
      --mangue-silver: #a0a8b0;
      --mangue-black: #1a1410;
      --mangue-near-black: #231c14;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--mangue-black);
      color: var(--mangue-white);
      font-family: 'Source Sans 3', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1 {
      font-family: 'Archivo Black', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.03em;
      color: var(--mangue-gold);
      text-shadow:
        3px 3px 0 var(--mangue-red),
        6px 6px 0 rgba(26, 20, 16, 0.6);
      line-height: 0.95;
    }

    h2 {
      font-family: 'Patua One', serif;
      color: var(--mangue-coral);
      text-shadow: 2px 2px 0 var(--mangue-mud-dark);
    }

    h3 {
      font-family: 'Bebas Neue', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--mangue-gold);
    }

    /* Hero section */
    .hero {
      text-align: center;
      padding: 6rem 2rem;
      position: relative;
      overflow: hidden;
      background:
        radial-gradient(ellipse at 20% 60%, rgba(212, 32, 32, 0.15) 0%, transparent 50%),
        radial-gradient(ellipse at 75% 30%, rgba(240, 184, 22, 0.12) 0%, transparent 45%),
        linear-gradient(180deg, var(--mangue-black) 0%, var(--mangue-mud-dark) 100%);
    }

    .hero h1 {
      font-size: clamp(3rem, 10vw, 8rem);
    }

    .hero .subtitle {
      font-family: 'Barrio', cursive;
      color: var(--mangue-coral);
      font-size: 1.5rem;
      margin-top: 1rem;
    }

    /* Carnival stripe divider */
    .carnival-stripe {
      width: 100%;
      height: 8px;
      background: repeating-linear-gradient(
        90deg,
        var(--mangue-red) 0px,
        var(--mangue-red) 40px,
        var(--mangue-gold) 40px,
        var(--mangue-gold) 80px,
        var(--mangue-blue) 80px,
        var(--mangue-blue) 120px,
        var(--mangue-green) 120px,
        var(--mangue-green) 160px
      );
    }

    /* Content section */
    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    /* Card */
    .card {
      background: var(--mangue-mud);
      border: 3px solid var(--mangue-ochre);
      border-left: 6px solid var(--mangue-red);
      border-radius: 2px;
      padding: 2rem;
      margin: 1.5rem 0;
      position: relative;
      box-shadow:
        4px 4px 0 var(--mangue-mud-dark),
        8px 8px 0 rgba(26, 20, 16, 0.3);
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 4px;
      background: linear-gradient(
        90deg,
        var(--mangue-red),
        var(--mangue-gold),
        var(--mangue-blue),
        var(--mangue-green)
      );
    }

    /* Links */
    a {
      color: var(--mangue-gold);
      text-decoration: underline;
      text-decoration-color: var(--mangue-ochre);
      text-underline-offset: 3px;
      transition: color 0.2s;
    }

    a:hover {
      color: var(--mangue-coral);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p class="subtitle">Subtitle in Barrio font</p>
  </div>
  <div class="carnival-stripe"></div>
  <section>
    <h2>Section Heading</h2>
    <p>Content with Manguebeat styling applied. The mangrove mud anchors everything in warm, earthy darkness while carnival colors burst through for energy and life.</p>
    <div class="card">
      <h3>Card Title</h3>
      <p>A card component with the characteristic left-border accent, carnival gradient top bar, and hard shadow offset.</p>
    </div>
  </section>
  <div class="carnival-stripe"></div>
</body>
</html>
```
