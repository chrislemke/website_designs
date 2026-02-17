# Puppycore Design Reference

Puppycore is a kawaii aesthetic centered around the **hyper-feminine, pastel, and deliberately exaggerated depiction of puppies and dog-related motifs**. It draws heavily from early 2000s Japanese merchandise and stationery culture (San-X, Artlist, The Dog), wrapping themes of cuteness, innocence, comfort, and nostalgia in soft pastel warmth, dreamy filters, and sparkle-laden imagery. The visual language emphasizes **gentle affection and comfort** -- everything is soft, plush, and glowing with a fantasy-like warmth. Unlike edgier kawaii sub-aesthetics, Puppycore is purely wholesome, evoking the feeling of cuddling a small puppy in a pastel-colored room.

---

## Visual Characteristics

### Core Motifs and Patterns

**Puppy / Animal Layer:**
- Small dog breeds: Corgis, Pugs, Golden Retrievers, Shih-Tzus
- Puppies depicted with exaggerated features: oversized eyes, digitally added cheek blush, ribbons or bows clipped to ears
- Paw prints as repeating background patterns and decorative accents
- Dog bones rendered as cookies, charms, ornaments, and divider elements

**Sweet / Innocent Layer:**
- Heart shapes rendered as cookies, charms, or plush toys
- Bows and ribbons as decorative flourishes and border accents
- Sparkles and digital glitter layered throughout
- Pacifiers and soft cloth toys as secondary motifs
- Baby-associated items integrated into the visual language
- Stars and small flower accents scattered as visual seasoning

**Environmental / Textural:**
- Soft focus and blurry/hazy filters creating a dreamlike quality
- Overlays that enhance cuteness and innocence
- Fluffy textures overlaid for a fantasy effect
- Digital sparkles and glitter applied liberally
- Warm, diffused lighting as if seen through a gentle haze
- Plush, stuffed-animal-like textures on surfaces

### Design Principles

- **Pure wholesomeness** -- every element should radiate warmth, comfort, and gentleness; no edge, no irony
- **Soft focus dreaminess** -- the visual world should feel slightly hazy, as if viewed through a soft-focus lens
- **Exaggerated cuteness** -- features are enlarged, simplified, and sweetened; oversized eyes, rosy cheeks, tiny bows
- **Sparkle saturation** -- glitter and sparkle effects are essential, not optional; they create the magical, fantasy quality
- **Pastel dominance** -- the palette is exclusively soft pastels with white and cream; no dark or harsh colors
- **Rounded everything** -- all shapes are soft, curved, and pillow-like; no sharp edges or angular geometry
- **Textural softness** -- surfaces should feel plush, fluffy, and touchable; like a stuffed animal brought to screen
- **Nostalgic warmth** -- evoke early 2000s Japanese stationery and pet merchandise culture

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base / Background** | Cream white, warm white, very soft pink |
| **Primary accent** | Soft pink, baby pink, rose pink |
| **Secondary accent** | Baby blue, powder blue |
| **Tertiary accents** | Soft lavender, pastel yellow |
| **Warm tones** | Peach, soft apricot |
| **Highlight / Sparkle** | White, shimmer gold, sparkle white |
| **Blush / Cheek** | Warm rosy pink |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Cream White | `#FFF8F0`, `#FFFAF5` | Primary background, page base |
| Warm White | `#FFF5EE`, `#FFF0F5` | Card surfaces, content areas |
| Baby Pink | `#FFB6C1`, `#FFC0CB` | Primary accent, section backgrounds, borders |
| Rose Pink | `#F8A4B8`, `#F4889E` | Headings, active elements, buttons |
| Blush Pink | `#FFDBDF`, `#FFD1D6` | Hover states, subtle backgrounds |
| Baby Blue | `#AED8F0`, `#B5E0F7` | Secondary accent, alternating sections, tags |
| Powder Blue | `#CCE5F5`, `#D6EBF8` | Light accent backgrounds |
| Soft Lavender | `#E6D8F5`, `#DCC8F0` | Tertiary accent, decorative elements |
| Pastel Yellow | `#FFF5B8`, `#FFEEA0` | Sparkle accents, star motifs, warm highlights |
| Peach | `#FFDAB9`, `#FFD5B0` | Warm accent, badge backgrounds |
| Apricot | `#FFCDA8`, `#FFCBA4` | Warm secondary accent |
| Cheek Blush | `#F8A0B0`, `#F5909E` | Kawaii blush circles, decorative dots |
| Shimmer Gold | `#FFE4A0`, `#FFD97D` | Sparkle highlights, star accents |
| Puppy Brown | `#D4A574`, `#C49A6C` | Soft warm brown for puppy-themed accents, outlines |
| Nose Brown | `#8B7355`, `#7A6548` | Dark warm accent, small detail elements |
| Soft Black | `#5C4A3D`, `#6B5B4F` | Text color (warm brown-black, never pure black) |

### Suggested CSS Custom Properties

```css
:root {
  /* Soft pastel base tones */
  --puppy-cream: #fff8f0;
  --puppy-warm-white: #fff5ee;
  --puppy-snow: #fffaf5;
  --puppy-blush-bg: #fff0f5;

  /* Pink spectrum */
  --puppy-baby-pink: #ffb6c1;
  --puppy-rose: #f8a4b8;
  --puppy-blush: #ffdbdf;
  --puppy-deep-pink: #f4889e;

  /* Cool pastels */
  --puppy-baby-blue: #aed8f0;
  --puppy-powder-blue: #cce5f5;
  --puppy-lavender: #e6d8f5;

  /* Warm accents */
  --puppy-yellow: #fff5b8;
  --puppy-peach: #ffdab9;
  --puppy-apricot: #ffcda8;

  /* Character accents */
  --puppy-cheek-blush: #f8a0b0;
  --puppy-shimmer: #ffe4a0;
  --puppy-brown: #d4a574;
  --puppy-nose: #8b7355;

  /* Text */
  --puppy-text-primary: #5c4a3d;
  --puppy-text-secondary: #8b7a6e;
  --puppy-text-heading: #f4889e;

  /* Functional mappings */
  --puppy-bg-primary: var(--puppy-cream);
  --puppy-bg-secondary: var(--puppy-snow);
  --puppy-bg-card: var(--puppy-warm-white);
  --puppy-accent: var(--puppy-rose);
  --puppy-accent-secondary: var(--puppy-baby-blue);
  --puppy-border: var(--puppy-baby-pink);
  --puppy-link: var(--puppy-deep-pink);
  --puppy-link-hover: var(--puppy-rose);
  --puppy-shadow: rgba(248, 164, 184, 0.2);
  --puppy-glow: rgba(255, 182, 193, 0.35);
}
```

### Color Approaches

- **Pink is the heart** -- baby pink and rose pink form the backbone of the palette; other pastels are supporting players
- **Always warm** -- even the blues and lavenders lean warm; avoid cool, clinical, or saturated tones
- **White is cream-tinted** -- backgrounds are never stark white; always warmed with a hint of pink, peach, or yellow
- **Brown over black** -- text and outlines use warm brown tones, never pure black; this keeps everything soft
- **Sparkle as color** -- shimmer gold and sparkle white act as accent colors in their own right
- **Glow over shadow** -- prefer pink-tinted, diffused glowing box-shadows over traditional gray drop shadows
- **No dark sections** -- unlike related aesthetics, Puppycore has no dark or contrasting moody sections

---

## Typography

### Typeface Characteristics

Puppycore typography is bubbly, cheerful, and playful:

- **Bold, rounded bubble-letter display fonts** -- headlines should feel like they come from a cute sticker sheet or Japanese stationery set
- **Handwriting-style script fonts** -- for slogans and affectionate phrases like "I WOOF YOU"
- **Pixel art-inspired display** -- for a nostalgic early-2000s touch in decorative headings
- **Rounded, friendly body fonts** -- soft sans-serifs with generous curves for readability
- **Emoji and Unicode decoration** -- paw print, heart, sparkle, star, dog, and bone emoji used as visual punctuation
- **Never angular or corporate** -- typography must feel handmade, playful, and soft

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Baloo 2** | Bubbly, rounded display | Hero text, large headings, slogans |
| **Comfortaa** | Rounded, wide sans-serif | Headlines, section titles |
| **Quicksand** | Rounded geometric sans-serif | Body text, UI elements |
| **Nunito** | Rounded, friendly sans-serif | Body text, navigation |
| **Patrick Hand** | Handwritten, casual | Accent text, affectionate phrases |
| **Caveat** | Handwritten, natural | Captions, decorative labels |
| **Fredoka One** | Bold, rounded display | Large playful headings |
| **Bubblegum Sans** | Bouncy, cartoon display | Fun headlines, decorative text |
| **Pangolin** | Rounded handwriting hybrid | Subheadings, callouts |
| **Indie Flower** | Handwritten, whimsical | Scattered decorative text, notes |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;600;700;800&family=Quicksand:wght@400;500;600;700&family=Patrick+Hand&family=Comfortaa:wght@400;700&family=Caveat:wght@400;700&display=swap');

/* Headlines -- bubbly, rounded display */
h1, h2, h3 {
  font-family: 'Baloo 2', 'Comfortaa', cursive;
  font-weight: 700;
  color: var(--puppy-text-heading);
  line-height: 1.2;
  letter-spacing: 0.02em;
}

h1 { font-size: clamp(2.4rem, 5vw, 4.2rem); }
h2 { font-size: clamp(1.6rem, 3.5vw, 2.5rem); }
h3 { font-size: clamp(1.2rem, 2.5vw, 1.8rem); }

/* Body text -- rounded, friendly */
body {
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-weight: 500;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--puppy-text-primary);
}

/* Handwritten affectionate text */
.puppy-handwritten {
  font-family: 'Patrick Hand', 'Caveat', cursive;
  font-size: 1.4em;
  color: var(--puppy-rose);
  transform: rotate(-1.5deg);
  display: inline-block;
}

/* Emoji decorative text */
.puppy-emoji-text {
  font-size: 0.85rem;
  letter-spacing: 0.3em;
  text-align: center;
  line-height: 2;
  user-select: none;
  opacity: 0.7;
}

/* Tags and badges */
.puppy-tag {
  font-family: 'Quicksand', sans-serif;
  font-size: 0.7rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: #fff;
}
```

---

## Layout Principles

### Grid and Structure

- **Soft, airy arrangements** -- generous whitespace with warm-tinted backgrounds; content should feel like it's resting on a fluffy cloud
- **Centered, single-column flow** -- content flows vertically with comfortable breathing room between sections
- **Card-based sections** -- rounded pastel cards containing content, each feeling like a soft cushion or pillow
- **Rounded containers** -- heavy use of border-radius (20px+) for a plush, toy-like feeling
- **Floating sticker quality** -- elements should look like they could be peeled off the page
- **Glow-based visual hierarchy** -- use pink glowing box-shadows and soft borders to draw attention
- **Balanced but playful** -- overall layout is orderly and sweet, not chaotic

### Section Organization

- Use **soft pastel gradient washes** between sections for seamless, dreamy flow
- Apply **paw print, heart, or sparkle emoji dividers** between content blocks
- Create **gentle alternating backgrounds** -- cream, then blush pink, then powder blue tints
- Employ **sticker-like floating elements** -- small paw prints, bones, hearts that break the grid as decoration
- Use **scalloped or wavy borders** between sections for a soft, playful edge
- Incorporate **sparkle overlays** on hero and feature sections
- Keep sections **light and warm** -- no dark or contrasting sections

---

## CSS/Design Techniques

### Dreamy Pastel Background

```css
/* Soft warm cream background with pink glow */
.puppy-bg {
  background-color: var(--puppy-cream);
  background-image:
    radial-gradient(
      ellipse at 25% 15%,
      rgba(255, 182, 193, 0.12) 0%,
      transparent 50%
    ),
    radial-gradient(
      ellipse at 75% 85%,
      rgba(174, 216, 240, 0.10) 0%,
      transparent 50%
    ),
    radial-gradient(
      ellipse at 50% 50%,
      rgba(230, 216, 245, 0.08) 0%,
      transparent 60%
    );
}

/* Soft focus / dreamy haze overlay */
.puppy-haze::before {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(
    135deg,
    rgba(255, 240, 245, 0.3) 0%,
    rgba(255, 248, 240, 0.1) 50%,
    rgba(255, 219, 223, 0.2) 100%
  );
  pointer-events: none;
  z-index: 0;
}
```

### Sparkle / Glitter Overlay

```css
/* CSS sparkle dots scattered across a section */
.puppy-sparkle {
  position: relative;
}

.puppy-sparkle::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    radial-gradient(circle 1.5px, rgba(255, 228, 160, 0.7) 100%, transparent 100%),
    radial-gradient(circle 1px, rgba(255, 255, 255, 0.8) 100%, transparent 100%),
    radial-gradient(circle 2px, rgba(255, 228, 160, 0.5) 100%, transparent 100%),
    radial-gradient(circle 1px, rgba(255, 255, 255, 0.6) 100%, transparent 100%),
    radial-gradient(circle 1.5px, rgba(248, 164, 184, 0.4) 100%, transparent 100%);
  background-size: 150px 120px, 100px 90px, 130px 140px, 80px 110px, 170px 130px;
  background-position: 10px 20px, 60px 70px, 90px 10px, 30px 100px, 120px 50px;
  pointer-events: none;
  z-index: 1;
  opacity: 0.6;
}

/* Animated twinkle sparkle */
@keyframes puppy-twinkle {
  0%, 100% { opacity: 0.3; transform: scale(1); }
  50% { opacity: 1; transform: scale(1.3); }
}

.puppy-sparkle-animated {
  animation: puppy-twinkle 2s ease-in-out infinite;
}
```

### Paw Print Pattern Background

```css
/* Repeating paw print pattern */
.puppy-paw-pattern {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='60' height='60' viewBox='0 0 60 60'%3E%3Cg fill='%23f8a4b8' opacity='0.12'%3E%3Cellipse cx='30' cy='38' rx='8' ry='10'/%3E%3Ccircle cx='20' cy='26' r='4.5'/%3E%3Ccircle cx='40' cy='26' r='4.5'/%3E%3Ccircle cx='16' cy='34' r='3.5'/%3E%3Ccircle cx='44' cy='34' r='3.5'/%3E%3C/g%3E%3C/svg%3E");
  background-size: 80px 80px;
}
```

### Puppy Card Styles

```css
/* Base puppy card -- rounded, soft, glowing */
.puppy-card {
  background: var(--puppy-bg-card);
  border: 2px solid var(--puppy-baby-pink);
  border-radius: 24px;
  padding: 2rem;
  position: relative;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  box-shadow: 0 4px 20px var(--puppy-shadow);
  overflow: hidden;
}

.puppy-card:hover {
  transform: translateY(-4px) scale(1.01);
  box-shadow: 0 8px 32px var(--puppy-glow);
  border-color: var(--puppy-rose);
}

/* Pastel blue variant */
.puppy-card--blue {
  border-color: var(--puppy-baby-blue);
  box-shadow: 0 4px 20px rgba(174, 216, 240, 0.25);
}

/* Lavender variant */
.puppy-card--lavender {
  border-color: var(--puppy-lavender);
  box-shadow: 0 4px 20px rgba(230, 216, 245, 0.25);
}

/* Sticker-style floating badge */
.puppy-sticker {
  background: var(--puppy-bg-card);
  border: 3px solid var(--puppy-rose);
  border-radius: 28px;
  padding: 0.8rem 1.5rem;
  display: inline-block;
  transform: rotate(-2deg);
  box-shadow:
    2px 3px 0 var(--puppy-blush),
    4px 6px 14px var(--puppy-shadow);
}
```

### Bone-Shaped Divider

```css
/* Dog bone divider element */
.puppy-bone-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem 0;
  gap: 1rem;
}

.puppy-bone-divider::before,
.puppy-bone-divider::after {
  content: '';
  flex: 1;
  max-width: 200px;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--puppy-baby-pink),
    transparent
  );
}

/* Bone shape using CSS */
.puppy-bone {
  width: 48px;
  height: 18px;
  background: var(--puppy-baby-pink);
  border-radius: 4px;
  position: relative;
}

.puppy-bone::before,
.puppy-bone::after {
  content: '';
  position: absolute;
  width: 16px;
  height: 22px;
  background: var(--puppy-baby-pink);
  border-radius: 50%;
  top: -2px;
}

.puppy-bone::before { left: -6px; }
.puppy-bone::after { right: -6px; }
```

### Kawaii Blush Cheek Effect

```css
/* Add kawaii blush circles to any element */
.puppy-blush {
  position: relative;
}

.puppy-blush::before,
.puppy-blush::after {
  content: '';
  position: absolute;
  width: 24px;
  height: 14px;
  border-radius: 50%;
  background: var(--puppy-cheek-blush);
  opacity: 0.35;
  bottom: 20%;
}

.puppy-blush::before { left: 15%; }
.puppy-blush::after { right: 15%; }
```

### Soft Glow Hover Effects

```css
/* Pink glow border for interactive elements */
.puppy-glow-border {
  border: 2px solid var(--puppy-baby-pink);
  transition: box-shadow 0.3s ease, border-color 0.3s ease;
}

.puppy-glow-border:hover {
  border-color: var(--puppy-rose);
  box-shadow:
    0 0 12px rgba(255, 182, 193, 0.3),
    0 0 30px rgba(255, 182, 193, 0.15);
}

/* Soft pink button with glow */
.puppy-button {
  background: var(--puppy-rose);
  color: #fff;
  border: none;
  border-radius: 999px;
  padding: 12px 28px;
  font-family: 'Quicksand', sans-serif;
  font-weight: 700;
  font-size: 0.95rem;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.3s ease;
  box-shadow: 0 4px 14px rgba(248, 164, 184, 0.35);
}

.puppy-button:hover {
  transform: translateY(-2px);
  box-shadow:
    0 6px 20px rgba(248, 164, 184, 0.5),
    0 0 15px rgba(255, 182, 193, 0.2);
}
```

### Scalloped / Wavy Border

```css
/* Scalloped edge divider between sections */
.puppy-scallop {
  position: relative;
  overflow: hidden;
}

.puppy-scallop::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 100%;
  height: 20px;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 120 20'%3E%3Cpath d='M0,20 C15,0 30,0 45,10 C60,20 75,20 90,10 C105,0 120,0 120,20 Z' fill='%23fff8f0'/%3E%3C/svg%3E") repeat-x;
  background-size: 120px 20px;
}
```

### Heart Pattern Background

```css
/* Subtle heart scatter pattern */
.puppy-hearts {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='50' height='50' viewBox='0 0 50 50'%3E%3Cpath d='M25,40 L5,22 C-1,15 5,6 12,6 C17,6 21,9 25,14 C29,9 33,6 38,6 C45,6 51,15 45,22 Z' fill='%23ffb6c1' opacity='0.08'/%3E%3C/svg%3E");
  background-size: 70px 70px;
}
```

### Emoji / Paw Print Decorative Divider

```css
/* Paw-and-heart emoji divider */
.puppy-divider {
  text-align: center;
  padding: 2rem 0;
  font-size: 1.2rem;
  letter-spacing: 0.6em;
  user-select: none;
  opacity: 0.6;
}

/* Usage: <div class="puppy-divider">content here</div> */

/* Sparkle text decoration on headings */
.puppy-sparkle-text {
  position: relative;
}

.puppy-sparkle-text::before {
  content: '\2728';
  position: absolute;
  top: -6px;
  left: -14px;
  font-size: 0.7rem;
  opacity: 0.5;
}

.puppy-sparkle-text::after {
  content: '\2728';
  position: absolute;
  bottom: -6px;
  right: -14px;
  font-size: 0.55rem;
  opacity: 0.35;
}
```

### Ribbon / Bow Accent

```css
/* Decorative bow ribbon on top of cards */
.puppy-ribbon {
  position: relative;
}

.puppy-ribbon::before {
  content: '';
  position: absolute;
  top: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 50px;
  height: 16px;
  background: var(--puppy-rose);
  border-radius: 50%;
  opacity: 0.7;
}

.puppy-ribbon::after {
  content: '';
  position: absolute;
  top: -3px;
  left: 50%;
  transform: translateX(-50%);
  width: 10px;
  height: 10px;
  background: var(--puppy-deep-pink);
  border-radius: 50%;
  z-index: 1;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Puppycore materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Plush / stuffed animal fabric | Rounded corners (20px+), soft pink box-shadows, warm pastel gradients |
| Ribbons and bows | Decorative top borders with soft curved shapes, scalloped edges |
| Glitter and sparkle | Radial-gradient dot patterns with gold/white, twinkling animations |
| Soft focus photography | Backdrop-filter blur, gradient overlays with low opacity |
| Puppy paw prints | SVG paw print repeat patterns at low opacity on backgrounds |
| Dog bone shapes | CSS-drawn bone shapes for dividers, badges, and decorative elements |
| Sticker sheets | Pill-shaped badges with thick pastel borders, slight rotation, soft shadows |
| Baby pink fluffy blankets | Gradient backgrounds from cream to blush with soft radial glows |
| Heart-shaped charms | SVG heart patterns, heart emoji as decorative punctuation |
| Japanese stationery | Clean pastel cards with rounded edges, kawaii character accents, grid layouts |
| Cookies and treats | Warm brown-tinted small card elements with rounded corners |

---

## Typography and Text Culture

### Characteristic Phrases and Text Style

- Bold, colorful bubble-letter slogans: "I WOOF YOU", "PAW-SOME"
- Pun-based wordplay with puppy/dog themes
- Affectionate, wholesome messaging
- Emoji used as visual punctuation between words and in dividers
- Mix of uppercase bubble text for emphasis with lowercase handwritten text for warmth

---

## Key Differences from Related Aesthetics

| Aspect | Puppycore | Cutecore | Kawaii | Sanriocore |
|--------|-----------|----------|-------|------------|
| **Subject focus** | Puppies and dogs exclusively | Broad cute imagery + horror | General cute culture | Sanrio brand characters |
| **Color approach** | Soft warm pastels, pink-dominant | Pastels undercut by reds/darks | Pure bright pastels | Character-specific palettes |
| **Emotional tone** | Wholesome, comforting, nostalgic | Dissonant, anxious, obsessive | Joyful, cheerful | Brand-loyal, collectible |
| **Edge / darkness** | None; purely innocent | Explicit (blood, weapons) | None | None |
| **Texture** | Soft focus, dreamy, sparkly | Cluttered, glitchy, degraded | Clean, crisp | Clean, branded |
| **Cultural root** | Early 2000s Japanese pet merchandise | 2010s internet subculture | Japanese cute culture broadly | Sanrio corporation |
| **Overall feel** | Cuddling a puppy on a cloud | Disturbing fan shrine | Children's shop | Character gift store |

---

## Related Aesthetics

| Aesthetic | Relationship to Puppycore |
|-----------|--------------------------|
| **Cutecore** | Shares kawaii visual language but Cutecore adds horror/edge; Puppycore is its wholesome counterpart |
| **Kawaii** | Parent aesthetic; Puppycore is a niche sub-application of kawaii focused specifically on puppy/dog motifs |
| **Sanriocore** | Shares the Japanese character-merchandise culture and pastel palette; Sanriocore is brand-specific |
| **Heisei Retro** | Shares early 2000s Japanese merchandise nostalgia; Puppycore draws from this era's pet-themed products |
| **Clovercore** | Adjacent wholesome aesthetic; shares the gentle, innocent, nature-adjacent quality |

---

## Quick-Start: Minimal Puppycore Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Puppycore Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;600;700;800&family=Quicksand:wght@400;500;600;700&family=Patrick+Hand&family=Caveat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --puppy-cream: #fff8f0;
      --puppy-warm-white: #fff5ee;
      --puppy-snow: #fffaf5;
      --puppy-baby-pink: #ffb6c1;
      --puppy-rose: #f8a4b8;
      --puppy-blush: #ffdbdf;
      --puppy-deep-pink: #f4889e;
      --puppy-baby-blue: #aed8f0;
      --puppy-lavender: #e6d8f5;
      --puppy-yellow: #fff5b8;
      --puppy-peach: #ffdab9;
      --puppy-cheek-blush: #f8a0b0;
      --puppy-shimmer: #ffe4a0;
      --puppy-brown: #d4a574;
      --puppy-text: #5c4a3d;
      --puppy-text-heading: #f4889e;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--puppy-cream);
      color: var(--puppy-text);
      font-family: 'Quicksand', sans-serif;
      font-weight: 500;
      line-height: 1.7;
      background-image:
        radial-gradient(ellipse at 25% 15%, rgba(255, 182, 193, 0.10) 0%, transparent 50%),
        radial-gradient(ellipse at 75% 85%, rgba(174, 216, 240, 0.08) 0%, transparent 50%);
    }

    h1, h2, h3 {
      font-family: 'Baloo 2', cursive;
      font-weight: 700;
      color: var(--puppy-text-heading);
      line-height: 1.2;
    }

    .hero {
      text-align: center;
      padding: 5rem 2rem 3rem;
      background: linear-gradient(
        170deg,
        var(--puppy-snow) 0%,
        var(--puppy-blush) 50%,
        var(--puppy-snow) 100%
      );
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 5vw, 4.5rem);
      margin-bottom: 0.5rem;
    }

    .hero .subtitle {
      font-family: 'Patrick Hand', cursive;
      font-size: 1.5rem;
      color: var(--puppy-brown);
      transform: rotate(-1deg);
      display: inline-block;
    }

    .paw-divider {
      text-align: center;
      padding: 1.5rem 0;
      font-size: 1.2rem;
      letter-spacing: 0.6em;
      user-select: none;
      opacity: 0.5;
    }

    .puppy-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 1.5rem;
      max-width: 1100px;
      margin: 0 auto;
      padding: 2rem;
    }

    .puppy-card {
      background: var(--puppy-warm-white);
      border: 2px solid var(--puppy-baby-pink);
      border-radius: 24px;
      padding: 2rem;
      box-shadow: 0 4px 20px rgba(248, 164, 184, 0.2);
      position: relative;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .puppy-card:hover {
      transform: translateY(-4px) scale(1.01);
      box-shadow: 0 8px 32px rgba(255, 182, 193, 0.35);
      border-color: var(--puppy-rose);
    }

    .puppy-card h3 {
      font-size: 1.3rem;
      margin-bottom: 0.5rem;
    }

    .tag {
      display: inline-block;
      padding: 0.2rem 0.7rem;
      font-family: 'Quicksand', sans-serif;
      font-size: 0.65rem;
      font-weight: 700;
      text-transform: uppercase;
      border-radius: 100px;
      margin-bottom: 0.8rem;
      color: #fff;
    }

    .tag--pink { background: var(--puppy-rose); }
    .tag--blue { background: #8abdd4; }
    .tag--lavender { background: #b8a0d4; }
    .tag--peach { background: var(--puppy-brown); }

    .feature-section {
      background: linear-gradient(
        135deg,
        var(--puppy-blush) 0%,
        var(--puppy-snow) 50%,
        rgba(174, 216, 240, 0.15) 100%
      );
      padding: 3rem 2rem;
      text-align: center;
    }

    .feature-section h2 {
      margin-bottom: 0.5rem;
    }

    .feature-section .subtitle {
      font-family: 'Caveat', cursive;
      font-size: 1.3rem;
      color: var(--puppy-brown);
    }

    .feature-section p {
      max-width: 600px;
      margin: 1rem auto 0;
      color: var(--puppy-text);
      opacity: 0.85;
    }

    footer {
      text-align: center;
      padding: 2.5rem;
      background: var(--puppy-blush);
      border-radius: 40px 40px 0 0;
      margin-top: 2rem;
      font-family: 'Patrick Hand', cursive;
      font-size: 1.2rem;
      color: var(--puppy-brown);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Pawfect Friends</h1>
    <span class="subtitle">I woof you so much!</span>
  </div>

  <div class="paw-divider">...</div>

  <section class="puppy-grid">
    <div class="puppy-card">
      <span class="tag tag--pink">Pupper</span>
      <h3>Golden Sunshine</h3>
      <p>A golden retriever puppy napping in a patch of warm afternoon light, wrapped in a pastel pink blanket.</p>
    </div>
    <div class="puppy-card">
      <span class="tag tag--blue">Tiny</span>
      <h3>Little Loaf</h3>
      <p>A corgi curled up like a bread loaf, wearing a tiny bow on one ear, surrounded by heart-shaped treats.</p>
    </div>
    <div class="puppy-card">
      <span class="tag tag--lavender">Dreamy</span>
      <h3>Cloud Pup</h3>
      <p>Soft focus, sparkles drifting down, a shih-tzu with ribbons looking up with oversized gentle eyes.</p>
    </div>
    <div class="puppy-card">
      <span class="tag tag--peach">Cozy</span>
      <h3>Snuggle Time</h3>
      <p>A pug wrapped in a cream-colored fleece, surrounded by plush toys and tiny paw-print pillows.</p>
    </div>
  </section>

  <div class="feature-section">
    <h2>Paw-some Moments</h2>
    <span class="subtitle">Every day is a puppy day</span>
    <p>Soft, sparkly, and endlessly comforting. A world where everything is as gentle as a puppy's first nap.</p>
  </div>

  <footer>
    <p>Made with warmth, sparkles, and puppy kisses</p>
  </footer>
</body>
</html>
```
