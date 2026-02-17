# Rococo Design Reference

Rococo is an exceptionally ornamental and theatrical decorative style that emerged in 1720s Paris as a reaction against the imposing grandeur and rigid formality of the preceding Baroque style. It is characterized by **lightness, elegance, and exuberant use of curving natural forms** in ornamentation. The aesthetic celebrates **frivolity, pleasure, intimacy, leisure**, and **playful ornamentation**, favoring smaller, intimate salon environments over grand ceremonial spaces. Asymmetry, pastel palettes, gilded surfaces, and nature-derived motifs create an atmosphere of aristocratic charm and romantic delicacy.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Rocaille** -- shell-shaped ornamental forms derived from shells, icicles, and grotto rock-work; the defining Rococo motif and the origin of the name
- **C-scrolls and S-scrolls** -- flowing curvilinear scroll forms used in borders, frames, cartouches, and transitions
- **Acanthus leaves** -- stylized foliage with serrated-edged raffle leaf forms, twisting and sinuous, often bordering abstract ornament
- **Putti (cherubs)** -- plump winged infant figures used as decorative elements on furniture, ceilings, wall panels, and architectural keystones
- **Garlands and festoons** -- draped floral swags and ribbon-tied bouquets of flowers
- **Cartouches** -- ornamental frames with scrollwork borders enclosing central motifs or text
- **Mascarons** -- relief human faces used on architectural keystones and decorative panels
- **Pastoral and mythological scenes** -- depictions of aristocratic pastimes, courtship, and playful mythology in soft colors and hazy light
- **Chinoiserie elements** -- pagodas, dragons, monkeys, bizarre flowers, bamboo, and Chinese figures reflecting Far Eastern influence
- **Love symbols** -- quivers, arrows, arrowed hearts, and other romantic motifs
- **Mirrors** -- extensively used as decorative and spatial elements, especially above fireplaces

### Design Principles

- **Asymmetrical composition** -- dynamic, off-center arrangements that create visual movement and playfulness
- **Lightness and delicacy** -- airy, graceful forms that avoid heaviness or severity
- **Curvilinear construction** -- abundant curves, scrolls, and flowing organic shapes throughout all elements
- **Intimate scale** -- smaller rooms and compositions reflecting domestic warmth rather than monumental grandeur
- **Exuberant ornamentation** -- rich decorative detail that is playful rather than imposing
- **Integration of nature** -- foliage, shells, flowers, and organic forms woven throughout all decoration
- **Theatrical elegance** -- every surface treated as an opportunity for refined decorative expression

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | Ivory white, cream, warm pearl |
| **Pastels** | Light pink, powder blue, mint green, lavender, soft peach |
| **Metallic accents** | Gold leaf, gilded gold, soft champagne gold |
| **Dark accents** | Black lacquer (Chinoiserie panels), charcoal (used sparingly) |

### Suggested Hex Values

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Ivory White | `#FEFCF3`, `#FBF8EF` | Primary backgrounds, light surfaces |
| Cream | `#F5EDE0`, `#F0E8D8` | Secondary backgrounds, panel fills |
| Blush Pink | `#F2C4C4`, `#E8B4B8` | Accent panels, decorative elements, highlights |
| Rose Pink | `#D4919A`, `#C27D88` | Stronger pink accents, headings, ornamental details |
| Powder Blue | `#B3CCE6`, `#A3BFD9` | Accent panels, secondary highlights, backgrounds |
| Mint Green | `#B8D8C8`, `#A5CCBA` | Decorative accents, secondary panels |
| Lavender | `#C8B8D8`, `#B5A3CA` | Soft accents, decorative fills |
| Soft Peach | `#F5D6C6`, `#EBC8B4` | Warm accents, backgrounds |
| Gilded Gold | `#C9A84C`, `#D4B85C` | Ornamental borders, scroll details, text accents |
| Champagne Gold | `#E8D5A3`, `#DCC68E` | Subtle gold fills, light metallic accents |
| Warm Charcoal | `#3A3335`, `#4A4245` | Text on light surfaces, fine ornamental lines |
| Black Lacquer | `#1A1618`, `#0F0D0E` | Chinoiserie-inspired dark panels (used sparingly) |

### Suggested CSS Custom Properties

```css
:root {
  /* Base */
  --rococo-ivory: #fefcf3;
  --rococo-cream: #f5ede0;
  --rococo-pearl: #f8f4ec;
  --rococo-charcoal: #3a3335;
  --rococo-warm-black: #1a1618;

  /* Pastels */
  --rococo-blush: #f2c4c4;
  --rococo-rose: #d4919a;
  --rococo-powder-blue: #b3cce6;
  --rococo-mint: #b8d8c8;
  --rococo-lavender: #c8b8d8;
  --rococo-peach: #f5d6c6;

  /* Metallics */
  --rococo-gold: #c9a84c;
  --rococo-gold-light: #e8d5a3;
  --rococo-champagne: #dcc68e;

  /* Functional */
  --rococo-bg-primary: var(--rococo-ivory);
  --rococo-bg-secondary: var(--rococo-cream);
  --rococo-text-primary: var(--rococo-charcoal);
  --rococo-accent: var(--rococo-gold);
  --rococo-border: var(--rococo-gold-light);
}
```

### Approaches

- **Pastel palette with gilded accents** -- soft, delicate hues paired with warm gold ornamental details
- **Ivory/cream base with rosy warmth** -- light backgrounds tinted pink or peach, never stark white
- **Abundant gold** -- used for borders, scrollwork, dividers, and ornamental frames (not text body)
- **Optional dark variant** -- black lacquer Chinoiserie-inspired backgrounds with gold and pastel accents
- **Tonal harmony** -- colors should feel soft, harmonious, and never jarring; pastels sit alongside each other gently

---

## Typography

### Typeface Characteristics

Rococo typography features:

- **Ornamental serif letterforms** with refined, elegant proportions
- **Calligraphic flourishes** -- swash capitals, decorative terminals, and flowing curves
- **Light to medium weight** -- avoiding heaviness, reflecting the aesthetic's emphasis on delicacy
- **Generous, graceful proportions** -- tall ascenders, elegant descenders, open counter shapes
- **Italic and script forms** preferred for display text, evoking handwritten aristocratic correspondence
- **Decorative initial capitals** -- oversized, ornate drop caps with scroll and floral embellishment
- **Refined spacing** -- generous letter-spacing and word-spacing that feels open and airy

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Cormorant Garamond** | Elegant, high-contrast serif | Body text, subheadings |
| **Playfair Display** | Refined serif with contrast and curves | Headlines, section titles |
| **Great Vibes** | Flowing calligraphic script with ornamental character | Decorative titles, accent text |
| **Tangerine** | Delicate calligraphic script | Decorative subtitles, pull quotes |
| **Cormorant** | Display serif with flowing elegance | Feature headlines |
| **Libre Baskerville** | Classical serif with refined weight | Body copy, reading text |
| **Spectral** | Organic serif with visible stroke variation | Body text |
| **Pinyon Script** | Formal copperplate script | Decorative accents, monograms |
| **Cinzel** | Refined inscriptional serif | Formal headings, navigation |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Playfair Display', 'Cormorant Garamond', serif;
  letter-spacing: 0.04em;
  color: var(--rococo-charcoal);
  font-weight: 400;
  line-height: 1.25;
}

/* Display / Hero text */
.rococo-display {
  font-family: 'Cormorant', 'Playfair Display', serif;
  font-size: clamp(2.5rem, 7vw, 5.5rem);
  letter-spacing: 0.06em;
  line-height: 1.1;
  font-weight: 300;
  font-style: italic;
}

/* Decorative script accents */
.rococo-script {
  font-family: 'Great Vibes', 'Tangerine', 'Pinyon Script', cursive;
  font-size: 2em;
  color: var(--rococo-gold);
}

/* Body text */
body {
  font-family: 'Cormorant Garamond', 'Libre Baskerville', 'Spectral', serif;
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.8;
  color: var(--rococo-charcoal);
}
```

---

## Layout Principles

### Grid and Structure

- **Asymmetrical yet balanced layouts** -- compositions that feel dynamic and playful, not rigidly centered
- **Intimate proportions** -- content areas feel enclosed and cozy rather than expansive or monumental
- **Curvilinear containers** -- panels and frames with rounded, scrolling edges rather than sharp rectangles
- **Layered ornamentation** -- decorative elements frame and overlap content, creating visual depth
- **Central cartouche focus** -- key content framed within ornamental scroll-bordered panels

### Section Organization

- Use **ornamental scroll dividers** between sections (C-scroll and S-scroll separators, shell motifs, floral garlands)
- Apply **generous whitespace** with soft tonal backgrounds that shift between pastel hues per section
- Create **hierarchy through ornamental framing** -- more important content receives richer decorative borders
- Employ **garland and festoon borders** -- floral swag decorations along tops and bottoms of sections
- **Cartouche framing** -- key headings and featured content enclosed in ornate scroll-bordered frames
- **Mirror-like symmetry in ornament** -- decorative borders may be symmetrical even when content layout is asymmetrical

---

## CSS/Design Techniques

### Ornamental Scroll Dividers (SVG + CSS)

```css
/* C-scroll and shell-inspired ornamental divider */
.rococo-divider {
  height: 50px;
  background: no-repeat center / 50% auto;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 50'%3E%3Cpath d='M160,25 C160,10 140,5 130,15 C120,25 130,35 145,30 M240,25 C240,10 260,5 270,15 C280,25 270,35 255,30' fill='none' stroke='%23c9a84c' stroke-width='1.5'/%3E%3Cpath d='M145,30 C160,28 180,35 200,25 C220,35 240,28 255,30' fill='none' stroke='%23c9a84c' stroke-width='1.5'/%3E%3Cellipse cx='200' cy='22' rx='12' ry='10' fill='none' stroke='%23c9a84c' stroke-width='1'/%3E%3Cpath d='M194,22 C196,18 200,16 204,18 C206,20 204,24 200,24 C196,24 194,22 194,22Z' fill='%23c9a84c' opacity='0.3'/%3E%3C/svg%3E");
  margin: 2.5rem auto;
  opacity: 0.7;
}

/* Floral garland divider */
.rococo-garland-divider {
  height: 40px;
  position: relative;
  margin: 2rem auto;
  width: 60%;
  background: no-repeat center / 100% auto;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 40'%3E%3Cpath d='M0,15 Q50,35 100,20 Q150,5 200,20 Q250,35 300,20 Q350,5 400,15' fill='none' stroke='%23e8d5a3' stroke-width='1.5'/%3E%3Ccircle cx='100' cy='20' r='4' fill='%23f2c4c4'/%3E%3Ccircle cx='200' cy='20' r='5' fill='%23d4919a'/%3E%3Ccircle cx='300' cy='20' r='4' fill='%23f2c4c4'/%3E%3C/svg%3E");
  opacity: 0.8;
}
```

### Cartouche Frame (Ornamental Panel)

```css
/* Ornamental scroll-bordered panel inspired by Rococo cartouches */
.rococo-cartouche {
  background: var(--rococo-pearl);
  border: 1.5px solid var(--rococo-gold-light);
  border-radius: 30px 10px 30px 10px; /* asymmetric organic rounding */
  padding: 3rem 2.5rem;
  position: relative;
  box-shadow:
    0 4px 20px rgba(201, 168, 76, 0.08),
    inset 0 0 40px rgba(242, 196, 196, 0.06);
}

/* Corner scroll ornaments */
.rococo-cartouche::before,
.rococo-cartouche::after {
  content: '';
  position: absolute;
  width: 50px;
  height: 50px;
  background: no-repeat center / contain;
  opacity: 0.5;
}

.rococo-cartouche::before {
  top: -10px;
  left: -10px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 50 50'%3E%3Cpath d='M5,40 C5,20 15,10 35,5 C25,10 15,20 15,35 C15,40 20,42 25,38 C18,42 10,40 10,32 C10,24 20,15 35,10' fill='none' stroke='%23c9a84c' stroke-width='1.2'/%3E%3C/svg%3E");
}

.rococo-cartouche::after {
  bottom: -10px;
  right: -10px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 50 50'%3E%3Cpath d='M45,10 C45,30 35,40 15,45 C25,40 35,30 35,15 C35,10 30,8 25,12 C32,8 40,10 40,18 C40,26 30,35 15,40' fill='none' stroke='%23c9a84c' stroke-width='1.2'/%3E%3C/svg%3E");
}
```

### Gilded Gold Border Effect

```css
/* Gold ornamental border mimicking gilded frame */
.rococo-gold-border {
  border: 2px solid var(--rococo-gold-light);
  outline: 1px solid var(--rococo-champagne);
  outline-offset: 4px;
  box-shadow:
    0 0 0 6px var(--rococo-ivory),
    0 0 0 7px var(--rococo-gold-light);
  padding: 2rem;
}

/* Gold accent line with shell centerpiece */
.rococo-gold-line {
  width: 40%;
  margin: 2rem auto;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--rococo-champagne) 15%,
    var(--rococo-gold) 50%,
    var(--rococo-champagne) 85%,
    transparent
  );
  position: relative;
}

.rococo-gold-line::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 16px;
  height: 14px;
  background: no-repeat center / contain;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 14'%3E%3Cpath d='M8,2 C6,0 2,1 2,5 C2,8 5,11 8,13 C11,11 14,8 14,5 C14,1 10,0 8,2Z' fill='%23c9a84c' opacity='0.6'/%3E%3C/svg%3E");
}
```

### Rococo Card / Panel

```css
.rococo-card {
  background: linear-gradient(
    160deg,
    var(--rococo-ivory) 0%,
    var(--rococo-pearl) 50%,
    var(--rococo-cream) 100%
  );
  border: 1px solid var(--rococo-gold-light);
  border-radius: 16px 6px 16px 6px;
  padding: 2.5rem;
  position: relative;
  overflow: hidden;
  transition: box-shadow 0.4s ease;
}

.rococo-card:hover {
  box-shadow:
    0 8px 30px rgba(201, 168, 76, 0.12),
    0 2px 10px rgba(212, 145, 154, 0.08);
}

/* Subtle pastel wash in corner */
.rococo-card::before {
  content: '';
  position: absolute;
  top: -40px;
  right: -40px;
  width: 150px;
  height: 150px;
  background: radial-gradient(
    circle,
    rgba(242, 196, 196, 0.15) 0%,
    rgba(200, 184, 216, 0.08) 40%,
    transparent 70%
  );
  pointer-events: none;
  border-radius: 50%;
}
```

### Cherub / Shell Decorative Element

```css
/* Shell (rocaille) decorative motif */
.rococo-shell {
  width: 80px;
  height: 70px;
  margin: 0 auto;
  position: relative;
}

.rococo-shell::before {
  content: '';
  position: absolute;
  inset: 0;
  background: no-repeat center / contain;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 80 70'%3E%3Cpath d='M40,5 C30,5 10,15 8,35 C6,50 20,62 40,65 C60,62 74,50 72,35 C70,15 50,5 40,5Z' fill='none' stroke='%23c9a84c' stroke-width='1.2'/%3E%3Cpath d='M40,15 L35,55 M40,15 L28,52 M40,15 L22,45 M40,15 L45,55 M40,15 L52,52 M40,15 L58,45' fill='none' stroke='%23e8d5a3' stroke-width='0.8'/%3E%3C/svg%3E");
  opacity: 0.6;
}
```

### Pastel Section Backgrounds

```css
/* Alternating pastel section backgrounds */
.rococo-section:nth-child(odd) {
  background: var(--rococo-ivory);
}

.rococo-section:nth-child(even) {
  background: linear-gradient(
    180deg,
    var(--rococo-cream) 0%,
    rgba(242, 196, 196, 0.08) 50%,
    var(--rococo-cream) 100%
  );
}

/* Blush-tinted feature section */
.rococo-section-blush {
  background: linear-gradient(
    135deg,
    var(--rococo-ivory) 0%,
    rgba(242, 196, 196, 0.12) 30%,
    rgba(200, 184, 216, 0.08) 60%,
    var(--rococo-ivory) 100%
  );
}

/* Powder-blue tinted section */
.rococo-section-blue {
  background: linear-gradient(
    135deg,
    var(--rococo-ivory) 0%,
    rgba(179, 204, 230, 0.1) 40%,
    var(--rococo-pearl) 100%
  );
}
```

### Soft Ornamental Shadow/Depth

```css
/* Soft, diffused shadow evoking gilded frame depth */
.rococo-shadow {
  box-shadow:
    0 2px 8px rgba(201, 168, 76, 0.08),
    0 8px 25px rgba(58, 51, 53, 0.06);
}

/* Inner glow for intimate warmth */
.rococo-inner-glow {
  box-shadow:
    inset 0 0 40px rgba(242, 196, 196, 0.08),
    inset 0 0 80px rgba(232, 213, 163, 0.04),
    0 4px 20px rgba(201, 168, 76, 0.08);
}
```

### Background Texture Pattern

```css
/* Subtle damask-like repeating pattern */
.rococo-pattern-bg {
  background-color: var(--rococo-ivory);
  background-image:
    radial-gradient(ellipse at 30% 50%, rgba(242, 196, 196, 0.06) 0%, transparent 50%),
    radial-gradient(ellipse at 70% 50%, rgba(200, 184, 216, 0.05) 0%, transparent 50%);
  background-size: 250px 250px;
}

/* Scroll-work inspired subtle pattern */
.rococo-scroll-bg {
  background-color: var(--rococo-cream);
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Cpath d='M50,20 C40,20 30,30 30,40 C30,50 40,55 50,50 C60,45 65,35 60,25 C55,18 50,20 50,20Z' fill='none' stroke='%23c9a84c' stroke-width='0.4' opacity='0.08'/%3E%3Cpath d='M50,80 C60,80 70,70 70,60 C70,50 60,45 50,50 C40,55 35,65 40,75 C45,82 50,80 50,80Z' fill='none' stroke='%23c9a84c' stroke-width='0.4' opacity='0.08'/%3E%3C/svg%3E");
  background-size: 120px 120px;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Rococo materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Gold leaf / Gilding | Gold gradient accents on borders, ornamental details, and text highlights (`linear-gradient` with gold tones) |
| Porcelain | Smooth, luminous white/cream surfaces with subtle warm sheen (gentle gradient) |
| Chinese lacquer | Deep black backgrounds with subtle glossy reflection gradients (Chinoiserie variant) |
| Marble | Cool off-white surfaces with faint veining texture (SVG or subtle gradient noise) |
| Silk brocade | Soft pastel backgrounds with subtle damask-like repeating patterns |
| Carved and gilded wood | Ornamental gold borders and frame details, warm brown structural lines |
| Mirrors | Subtle reflective gradient overlays, glass-like highlight effects (`backdrop-filter: blur`) |
| Painted ceiling fresco | Soft gradient backgrounds suggesting atmospheric depth with pastel color washes |
| Wrought iron scrollwork | Ornamental dark line work in scroll and curve patterns, decorative borders |
| Soft flowing fabric | Gentle gradient transitions, flowing SVG shapes, pastel layered backgrounds |

---

## Painting and Graphic Style

Rococo visual art has distinct characteristics useful for web design mood and composition:

- **Soft, hazy light** -- paintings bathed in warm, diffused illumination; no harsh shadows or dramatic chiaroscuro
- **Pastel color harmony** -- pinks, blues, greens, and creams blended in gentle tonal relationships
- **Pastoral and romantic scenes** -- idyllic countryside settings, gardens, courtship, aristocratic leisure (fete galante)
- **Flowing, sinuous composition** -- figures and forms arranged in gentle curves and diagonal movements
- **Atmospheric depth** -- soft backgrounds fading into misty distance, suggesting dreamy spaciousness
- **Abundant floral detail** -- flowers, garlands, and bouquets as decorative fills and compositional anchors
- **Playful, lighthearted tone** -- whimsical rather than solemn, charming rather than awe-inspiring
- **Notable artists:** Jean-Antoine Watteau (fete galante scenes), Francois Boucher (sensuous mythological paintings), Jean-Honore Fragonard (romantic garden scenes)

---

## Architecture and Interior Influence

Key architectural and interior design principles relevant to layout and spatial thinking:

| Architectural Feature | Web Design Translation |
|-----------------------|------------------------|
| Intimate salon proportions | Contained, cozy content widths; avoid overly wide layouts |
| Ornamental ceiling medallions | Decorative centered motifs above or within hero sections |
| Gilded wall paneling (boiserie) | Ornamental gold-bordered content panels and card frames |
| Mirrors amplifying light and space | Light, luminous backgrounds with reflective highlight effects |
| Asymmetrical rocaille ornament | Decorative elements placed off-center for dynamic visual interest |
| Pastel-painted wall panels | Alternating soft-tinted section backgrounds in different pastels |
| Chinoiserie lacquer panels | Optional dark accent sections with Asian-inspired motifs |
| Wrought-iron scrollwork | Ornamental SVG curve patterns used as dividers and borders |
| Elaborate door surrounds | Rich ornamental framing around key content entries and headings |

---

## Sub-styles and Variations

### French Rococo (1720s-1760s)
- The original and most refined expression
- Emphasis on intimate interiors, gilded boiserie, and salon culture
- Pastel palette with abundant gold
- Associated with Louis XV, Madame de Pompadour, and the Parisian aristocracy

### German/Bavarian Rococo
- More exuberant and theatrical than the French original
- Elaborate painted ceiling frescoes in palaces and churches
- Complex ornamental programs covering entire interiors
- Notable: Pilgrimage Church of Wies, Hall of Mirrors at Amalienburg (Munich)

### Portuguese Rococo
- Integration with local architectural traditions
- Notable: Palace of Queluz
- Rich gilded interiors blending Rococo with Iberian decorative traditions

### Chinoiserie Rococo
- Fusion of Rococo ornamentation with Far Eastern motifs
- Chinese lacquer panels, pagodas, dragons, bamboo, exotic flowers
- Black lacquer backgrounds with gold and pastel accents
- Notable: Coromandel lacquer room at Schloss Falkenlust, Bruhl, Germany

### Rococopunk
- Modern speculative fiction reimagining of Rococo aesthetics
- Blends 18th-century ornamental excess with futuristic or fantastical technology
- Maintains pastel palettes and scrollwork but adds mechanical or sci-fi elements

---

## Related Aesthetics

| Aesthetic | Relationship to Rococo |
|-----------|------------------------|
| **Baroque** | Direct predecessor; Rococo emerged as a lighter, more intimate reaction against Baroque grandeur |
| **Chinoiserie** | Major decorative influence; Far Eastern motifs integrated throughout Rococo interiors |
| **Neoclassicism** | Direct successor; replaced Rococo's ornamentation with classical restraint and symmetry |
| **Gustavian** | Scandinavian interpretation blending Rococo elegance with Nordic restraint |
| **Decadence** | Shares themes of luxury, excess, and aesthetic pleasure-seeking |
| **Angelcore** | Modern aesthetic echoing Rococo's cherubs, softness, and ethereal pastel palette |
| **Coquette** | Contemporary aesthetic drawing on Rococo's femininity, ribbons, bows, and romantic charm |
| **Princesscore** | Modern aesthetic inspired by Rococo's palatial elegance and pink-and-gold palette |
| **Rococopunk** | Speculative reimagining that fuses Rococo ornament with futuristic elements |
| **Art Nouveau** | Later movement sharing Rococo's love of organic curves and nature-derived ornament |

---

## Quick-Start: Minimal Rococo Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rococo Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Cormorant+Garamond:ital,wght@0,300;0,400;1,400&family=Great+Vibes&display=swap" rel="stylesheet">
  <style>
    :root {
      --rococo-ivory: #fefcf3;
      --rococo-cream: #f5ede0;
      --rococo-pearl: #f8f4ec;
      --rococo-charcoal: #3a3335;
      --rococo-blush: #f2c4c4;
      --rococo-rose: #d4919a;
      --rococo-powder-blue: #b3cce6;
      --rococo-mint: #b8d8c8;
      --rococo-lavender: #c8b8d8;
      --rococo-gold: #c9a84c;
      --rococo-gold-light: #e8d5a3;
      --rococo-champagne: #dcc68e;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--rococo-ivory);
      color: var(--rococo-charcoal);
      font-family: 'Cormorant Garamond', serif;
      font-weight: 400;
      letter-spacing: 0.02em;
      line-height: 1.8;
    }

    h1, h2, h3 {
      font-family: 'Playfair Display', serif;
      letter-spacing: 0.04em;
      color: var(--rococo-charcoal);
      font-weight: 400;
    }

    .hero {
      text-align: center;
      padding: 6rem 2rem;
      background: linear-gradient(
        180deg,
        var(--rococo-ivory) 0%,
        rgba(242, 196, 196, 0.08) 50%,
        var(--rococo-ivory) 100%
      );
      position: relative;
    }

    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2.5rem, 7vw, 5.5rem);
      font-style: italic;
      font-weight: 400;
      letter-spacing: 0.06em;
    }

    .hero .subtitle {
      font-family: 'Great Vibes', cursive;
      font-size: 2rem;
      color: var(--rococo-gold);
      margin-top: 0.5rem;
    }

    /* Ornamental scroll divider */
    .rococo-divider {
      height: 50px;
      width: 50%;
      margin: 2rem auto;
      background: no-repeat center / 100% auto;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 50'%3E%3Cpath d='M160,25 C160,10 140,5 130,15 C120,25 130,35 145,30 M240,25 C240,10 260,5 270,15 C280,25 270,35 255,30' fill='none' stroke='%23c9a84c' stroke-width='1.5'/%3E%3Cpath d='M145,30 C160,28 180,35 200,25 C220,35 240,28 255,30' fill='none' stroke='%23c9a84c' stroke-width='1.5'/%3E%3Cellipse cx='200' cy='22' rx='10' ry='8' fill='none' stroke='%23c9a84c' stroke-width='1'/%3E%3C/svg%3E");
      opacity: 0.6;
    }

    section {
      max-width: 800px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    section h2 {
      text-align: center;
      margin-bottom: 1.5rem;
    }

    section p {
      text-align: justify;
      text-indent: 1.5em;
    }

    /* Gilded card panel */
    .rococo-panel {
      background: var(--rococo-pearl);
      border: 1.5px solid var(--rococo-gold-light);
      border-radius: 30px 10px 30px 10px;
      padding: 2.5rem;
      box-shadow:
        0 4px 20px rgba(201, 168, 76, 0.08),
        inset 0 0 40px rgba(242, 196, 196, 0.06);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <div class="subtitle">An elegant subtitle in flowing script</div>
    <div class="rococo-divider"></div>
  </div>
  <section>
    <h2>Section Heading</h2>
    <p>Content with Rococo styling applied. The soft pastel palette, gilded ornamental accents, and flowing typographic elegance create an atmosphere of aristocratic charm and intimate refinement.</p>
  </section>
</body>
</html>
```
