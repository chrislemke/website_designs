# Shoe Diva Design Reference

Shoe Diva is a commercial illustration and design aesthetic prevalent from the late 1990s through the 2000s, primarily on products and media targeting adult women. It is defined by a **whimsical, hand-drawn illustration style** with "loopy" and sketchy linework, a **bright and feminine color palette**, and an aspirational depiction of the **glamorous urban single woman** obsessed with fashion, shoes, and shopping. The style is playful, sophisticated, and unapologetically feminine -- a more mature and worldly counterpart to Parisian Girly. It shares its bright, feminine color palette with McBling and its fashion-illustration sensibility with Curly Girly. The cultural archetype is Carrie Bradshaw from *Sex and the City*.

---

## Visual Characteristics

### Core Motifs and Patterns

- **High-heeled shoes** -- the single most iconic motif; stilettos, pumps, and Manolo Blahnik-style heels rendered as whimsical illustrations
- **Shopping bags** -- luxury department store bags (often with ribbon handles) as symbols of indulgence and retail therapy
- **Cocktails** -- Cosmopolitan glasses, martinis, and champagne flutes as lifestyle icons
- **Makeup and cosmetics** -- lipstick, compacts, perfume bottles, and nail polish as decorative elements
- **Parisian iconography** -- Eiffel Tower silhouettes and references evoking fashion-capital sophistication
- **Stylized female figures** -- thin, fashionable women in exaggerated poses, often carrying shopping bags or wearing statement heels
- **Hearts and bows** -- decorative romantic flourishes scattered throughout compositions
- **Sparkles and glitter** -- small star bursts, shine highlights, and shimmer effects conveying glamour
- **Fluffy textures** -- feathery, plush, and soft tactile accents (boas, fur trims, powder puffs)
- **Decorative flourishes** -- curling swashes, looping ornamental lines, and ribbon-like scrollwork
- **Handbags and clutches** -- designer purse illustrations as secondary fashion motifs
- **Fashion accessories** -- sunglasses, tiaras, pearl necklaces, and charm bracelets

### Illustration Style

- **Hand-drawn and sketchy** -- linework is deliberately loose, organic, and imperfect rather than precise or geometric
- **Thin, loopy lines** -- fine-weight strokes with exaggerated curves and swooping movement
- **Free-flowing quality** -- lines convey energy, whimsy, and spontaneity as if sketched quickly in a fashion notebook
- **Flat color fills with line overlays** -- areas of bright, solid color contained by or layered with the sketchy linework
- **Watercolor-adjacent washes** -- soft, semi-transparent color areas suggesting watercolor or marker rendering
- **Vector-fashion hybrid** -- the look of hand illustration translated into clean, reproducible commercial graphics

### Design Principles

- **Playful sophistication** -- fun and lighthearted but with an aspirational, grown-up polish
- **Feminine maximalism** -- abundant decorative detail; ornate, embellished, and busy over minimal
- **Bright saturation** -- colors are vivid, cheerful, and unapologetic; nothing muted or moody
- **Whimsy over precision** -- deliberate imperfection and looseness in illustration and layout
- **Aspirational glamour** -- every element reinforces a fantasy of fashionable urban living
- **Consumerist celebration** -- shopping, fashion, and luxury goods presented joyfully and without irony
- **Sketch-like energy** -- the aesthetic should feel like a chic fashion illustration come to life

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Primary / Dominant** | Hot pink, rose pink, bubblegum pink |
| **Secondary** | Bright yellow, sunny gold |
| **Tertiary** | Lime green, mint green |
| **Accent** | Sky blue, periwinkle, lavender purple |
| **Neutral / Background** | White, soft cream, pale pink |
| **Contrast** | Black (for linework and text) |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Hot Pink | `#FF69B4`, `#FF1493` | Primary brand color, headings, key decorative elements |
| Rose Pink | `#F472B6`, `#E8558A` | Cards, secondary fills, hover states |
| Blush Pink | `#FFD6E0`, `#FFC0CB` | Light backgrounds, soft fills, panels |
| Pale Pink | `#FFF0F5`, `#FFF5F8` | Page backgrounds, subtle surfaces |
| Sunny Yellow | `#FFD700`, `#FFEB3B` | Accent highlights, badges, star sparkles |
| Soft Yellow | `#FFF8DC`, `#FFFACD` | Warm background sections, secondary panels |
| Lime Green | `#77DD77`, `#98E698` | Tertiary accent, fresh contrast elements |
| Mint Green | `#B2F5B2`, `#D4EDDA` | Soft accent backgrounds, alternating sections |
| Sky Blue | `#87CEEB`, `#89CFF0` | Cool accent, links, decorative touches |
| Periwinkle | `#CCCCFF`, `#B0B0E8` | Soft secondary accent, subtle borders |
| Lavender | `#E6C8FF`, `#D8B4FE` | Light accent surfaces, card backgrounds |
| Sketch Black | `#2A2A2A`, `#333333` | Linework, body text, borders |
| Pure White | `#FFFFFF` | Base backgrounds, text on dark surfaces |
| Soft Cream | `#FFFEF5`, `#FFF9F0` | Warm white alternative background |
| Champagne Gold | `#D4AF37`, `#C5A55A` | Metallic accents, sparkle effects, luxury feel |

### Suggested CSS Custom Properties

```css
:root {
  /* Pinks -- the dominant family */
  --diva-hot-pink: #ff69b4;
  --diva-deep-pink: #ff1493;
  --diva-rose: #f472b6;
  --diva-blush: #ffd6e0;
  --diva-pale-pink: #fff0f5;

  /* Yellows -- sunny secondary */
  --diva-sunny-yellow: #ffd700;
  --diva-soft-yellow: #fff8dc;
  --diva-bright-yellow: #ffeb3b;

  /* Greens -- fresh tertiary */
  --diva-lime-green: #77dd77;
  --diva-mint: #b2f5b2;

  /* Blues and purples -- cool accents */
  --diva-sky-blue: #87ceeb;
  --diva-periwinkle: #ccccff;
  --diva-lavender: #e6c8ff;

  /* Neutrals */
  --diva-black: #2a2a2a;
  --diva-charcoal: #555555;
  --diva-white: #ffffff;
  --diva-cream: #fffef5;

  /* Metallic accent */
  --diva-gold: #d4af37;

  /* Functional mappings */
  --diva-bg-primary: var(--diva-pale-pink);
  --diva-bg-secondary: var(--diva-cream);
  --diva-bg-card: var(--diva-white);
  --diva-text-primary: var(--diva-black);
  --diva-text-secondary: var(--diva-charcoal);
  --diva-text-heading: var(--diva-deep-pink);
  --diva-accent: var(--diva-hot-pink);
  --diva-accent-secondary: var(--diva-sunny-yellow);
  --diva-border: rgba(42, 42, 42, 0.3);
  --diva-border-sketch: var(--diva-black);
  --diva-link: var(--diva-deep-pink);
  --diva-link-hover: var(--diva-hot-pink);

  /* Gradients */
  --diva-gradient-pink: linear-gradient(135deg, #ff69b4, #ff1493);
  --diva-gradient-warm: linear-gradient(135deg, #ffd6e0, #fff8dc);
  --diva-gradient-shimmer: linear-gradient(135deg, #ffd6e0, #e6c8ff, #87ceeb);
}
```

### Palette Approaches

- **Pink dominance** -- hot pink and its variants are the primary visual identity; 50-60% of colored surfaces
- **Yellow as sunshine punch** -- bright yellow used for highlights, badges, and sparkle accents to energize the pink base
- **Green as fresh contrast** -- lime and mint greens appear sparingly for visual breathing room
- **Cool blue-purple touches** -- sky blue and lavender provide softness and variety without competing with pink
- **Sketch-black for structure** -- dark linework grounds the bright palette and provides the hand-drawn feel
- **White as clean canvas** -- generous white space keeps the busy decorative elements from becoming overwhelming
- **Gold for luxury** -- champagne and gold metallics used sparingly for shimmer and glamour cues
- **Never dark or moody** -- the palette stays bright, warm, and cheerful at all times

---

## Typography

### Typeface Characteristics

Shoe Diva typography mirrors the hand-drawn, sketchy illustration style:

- **Loopy, flowing script fonts** -- connected cursive letterforms with exaggerated curves and swashes
- **Sketch-like quality** -- fonts that appear hand-lettered rather than mechanical or geometric
- **Thin, elegant strokes** -- lightweight lines matching the fine linework of the illustrations
- **Bouncy baselines** -- letters that dance and move rather than sitting rigidly
- **Fashion-magazine influence** -- elegant, aspirational display type evoking editorial fashion layouts
- **Mixed type pairing** -- decorative scripts for display paired with clean sans-serifs for readability
- **Feminine without being childish** -- sophisticated and grown-up, not tween or juvenile

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Great Vibes** | Flowing calligraphic script | Hero headlines, decorative titles, glamour text |
| **Parisienne** | Elegant French-inspired script | Section titles, accent phrases, fashion references |
| **Dancing Script** | Casual, bouncy cursive | Subheadings, callout text, feature labels |
| **Sacramento** | Thin, flowing monoline script | Subtitle text, pull quotes, delicate accents |
| **Alex Brush** | Formal brush script | Display text, decorative headings |
| **Satisfy** | Retro-flavored flowing script | Accent text, badges, decorative labels |
| **Playfair Display** | High-contrast elegant serif | Structured headings, editorial feel |
| **Cormorant Garamond** | Refined, high-contrast serif | Body headings, sophisticated readability |
| **Quicksand** | Rounded, modern sans-serif | Body text, readable contrast to script display |
| **Poppins** | Geometric, friendly sans-serif | Body copy, UI elements, labels |
| **Montserrat** | Clean geometric sans-serif | Navigation, structured labels, subheadings |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Parisienne&family=Dancing+Script:wght@400;700&family=Sacramento&family=Playfair+Display:wght@400;700&family=Quicksand:wght@400;500;600&family=Montserrat:wght@400;600&display=swap');

/* Hero / display headlines -- signature flowing script */
h1 {
  font-family: 'Great Vibes', 'Parisienne', cursive;
  font-weight: 400;
  color: var(--diva-text-heading);
  line-height: 1.2;
  font-size: clamp(2.5rem, 7vw, 5.5rem);
  letter-spacing: 0.02em;
}

/* Section headings -- elegant serif or script */
h2 {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 700;
  color: var(--diva-black);
  font-size: clamp(1.6rem, 3.5vw, 2.5rem);
  letter-spacing: 0.03em;
  line-height: 1.3;
}

/* Subheadings -- lighter script accent */
h3 {
  font-family: 'Dancing Script', 'Sacramento', cursive;
  font-weight: 700;
  color: var(--diva-hot-pink);
  font-size: clamp(1.2rem, 2.5vw, 1.8rem);
  line-height: 1.4;
}

/* Body text -- clean and readable */
body {
  font-family: 'Quicksand', 'Poppins', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  letter-spacing: 0.02em;
  color: var(--diva-text-primary);
}

/* Decorative accent text -- fashion phrases, quotes */
.diva-accent-text {
  font-family: 'Parisienne', 'Sacramento', cursive;
  font-size: 1.5em;
  color: var(--diva-deep-pink);
  font-style: italic;
}

/* Labels and structured text */
.diva-label {
  font-family: 'Montserrat', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  font-size: 0.8rem;
  font-weight: 600;
  color: var(--diva-charcoal);
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, airy compositions** -- content organized with generous whitespace evoking fashion magazine layouts
- **Sketch-framed panels** -- content containers with hand-drawn-style borders (slightly irregular, thin strokes)
- **Generous padding** -- spacious interiors within cards and sections for an upscale, editorial feel
- **Mixed illustration and text** -- decorative motifs (shoes, bags, cocktails) interspersed with content
- **Card-based layouts** -- content grouped into elegant, lightly bordered cards
- **Vertical flow** -- sections stack top-to-bottom with decorative dividers between them
- **Fashion-editorial grid** -- asymmetric arrangements inspired by magazine page layouts

### Section Organization

- Use **decorative motif dividers** between sections (stiletto silhouettes, bow ribbons, sparkle clusters)
- Apply **alternating soft backgrounds** -- rotate between pale pink, soft cream, white, and light lavender sections
- Create **hierarchy through color warmth** -- hot pink for primary elements, blush for secondary, white for tertiary
- Employ **sketch-style borders** -- thin, slightly wavy or hand-drawn-effect borders on containers
- Use **fashion-icon section markers** -- small shoe, handbag, or cocktail glass illustrations to introduce sections
- Incorporate **sparkle accents** -- small glitter dots and star bursts as decorative seasoning
- Feature **fashion illustration vignettes** -- stylized figures or accessory sketches as section decorations

---

## CSS/Design Techniques

### Hand-Drawn Sketch Border Effect

```css
/* Simulated hand-drawn border using wavy outline */
.diva-sketch-border {
  border: 2px solid var(--diva-black);
  border-radius: 2px 8px 2px 6px;
  position: relative;
}

/* Double-line sketch frame */
.diva-sketch-frame {
  border: 1.5px solid var(--diva-black);
  outline: 1px solid var(--diva-black);
  outline-offset: 4px;
  border-radius: 3px 6px 2px 5px;
  padding: 2rem;
  background: var(--diva-white);
}

/* Slightly irregular border for hand-drawn feel */
.diva-loose-border {
  border: 2px solid var(--diva-black);
  border-radius: 4px 12px 4px 10px / 10px 4px 12px 4px;
}
```

### Sparkle / Glitter Overlay

```css
/* Scattered sparkle dots */
.diva-sparkle::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    radial-gradient(1px 1px at 15% 20%, rgba(255, 215, 0, 0.6), transparent),
    radial-gradient(1.5px 1.5px at 35% 65%, rgba(255, 255, 255, 0.8), transparent),
    radial-gradient(1px 1px at 55% 15%, rgba(255, 215, 0, 0.5), transparent),
    radial-gradient(1px 1px at 75% 70%, rgba(255, 255, 255, 0.7), transparent),
    radial-gradient(1.5px 1.5px at 90% 35%, rgba(255, 215, 0, 0.4), transparent),
    radial-gradient(1px 1px at 45% 85%, rgba(255, 255, 255, 0.6), transparent),
    radial-gradient(1px 1px at 10% 50%, rgba(212, 175, 55, 0.5), transparent);
  pointer-events: none;
  opacity: 0.7;
}

/* Shimmer gradient for glamour surfaces */
.diva-shimmer {
  background: linear-gradient(
    135deg,
    #ffd6e0, #fff0f5, #ffd6e0, #fff8dc, #ffd6e0
  );
  background-size: 200% 200%;
  animation: diva-shimmer 4s ease-in-out infinite;
}

@keyframes diva-shimmer {
  0%, 100% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
}
```

### Stiletto Shoe Divider (SVG)

```css
/* Stiletto silhouette section divider */
.diva-shoe-divider {
  height: 50px;
  background: no-repeat center / auto 100%;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 120 50'%3E%3Cpath d='M30,45 L35,20 Q37,10 45,8 Q55,5 60,8 L65,12 Q68,15 75,14 L85,12 Q90,11 90,14 L90,18 Q90,22 85,22 L40,22 L35,45 Z' fill='none' stroke='%23ff69b4' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
  margin: 2rem auto;
  width: 120px;
  opacity: 0.6;
}
```

### Shoe Diva Card

```css
/* Elegant sketch-framed card */
.diva-card {
  background: var(--diva-white);
  border: 1.5px solid var(--diva-black);
  border-radius: 4px 12px 4px 10px;
  padding: 2rem;
  position: relative;
  box-shadow: 3px 3px 0 0 var(--diva-blush);
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.diva-card:hover {
  box-shadow: 5px 5px 0 0 var(--diva-hot-pink);
  transform: translate(-2px, -2px);
}

/* Heart accent in corner */
.diva-card::before {
  content: '\2665';
  position: absolute;
  top: -8px;
  right: 12px;
  background: var(--diva-white);
  padding: 0 0.3rem;
  color: var(--diva-hot-pink);
  font-size: 0.9rem;
}
```

### Loopy Line Decorative Border

```css
/* Wavy, loopy top border evoking the sketchy linework */
.diva-loopy-border {
  border: none;
  height: 20px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 20'%3E%3Cpath d='M0 10 Q10 0 20 10 T40 10 T60 10 T80 10 T100 10 T120 10 T140 10 T160 10 T180 10 T200 10' fill='none' stroke='%23ff69b4' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-size: 200px 20px;
  background-position: center;
}
```

### Bow Ribbon Divider

```css
/* Decorative bow divider */
.diva-bow-divider {
  text-align: center;
  margin: 2.5rem 0;
  position: relative;
}

.diva-bow-divider::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--diva-hot-pink),
    transparent
  );
}

.diva-bow-divider::after {
  content: '\1F380';
  position: relative;
  z-index: 1;
  background: var(--diva-bg-primary);
  padding: 0 1rem;
  font-size: 1.3rem;
}
```

### Pink Gradient Backgrounds

```css
/* Soft pink-to-cream hero gradient */
.diva-hero-bg {
  background: linear-gradient(
    180deg,
    var(--diva-pale-pink) 0%,
    var(--diva-cream) 60%,
    var(--diva-white) 100%
  );
}

/* Warm pink-to-lavender section gradient */
.diva-section-warm {
  background: linear-gradient(
    135deg,
    var(--diva-blush) 0%,
    var(--diva-lavender) 100%
  );
}

/* Bright pink accent gradient */
.diva-bold-gradient {
  background: linear-gradient(
    135deg,
    var(--diva-hot-pink) 0%,
    var(--diva-rose) 50%,
    var(--diva-blush) 100%
  );
}
```

### Fashion Motif Scatter

```css
/* Decorative shoe and bag icons scattered on sections */
.diva-motifs::before {
  content: '\1F460'; /* high heel */
  position: absolute;
  top: 8%;
  left: 5%;
  font-size: 1.4rem;
  transform: rotate(-15deg);
  opacity: 0.25;
  pointer-events: none;
}

.diva-motifs::after {
  content: '\1F6CD'; /* shopping bags */
  position: absolute;
  bottom: 6%;
  right: 4%;
  font-size: 1.3rem;
  transform: rotate(10deg);
  opacity: 0.2;
  pointer-events: none;
}

/* Cocktail and sparkle secondary scatter */
.diva-motifs-alt::before {
  content: '\1F378'; /* cocktail glass */
  position: absolute;
  top: 5%;
  right: 7%;
  font-size: 1.2rem;
  transform: rotate(8deg);
  opacity: 0.2;
  pointer-events: none;
}

.diva-motifs-alt::after {
  content: '\2728'; /* sparkles */
  position: absolute;
  bottom: 8%;
  left: 6%;
  font-size: 1rem;
  opacity: 0.3;
  pointer-events: none;
}
```

### Button Styles

```css
/* Primary pink button with sketch energy */
.diva-btn {
  display: inline-block;
  padding: 0.7rem 2rem;
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  border: 1.5px solid var(--diva-black);
  border-radius: 4px 10px 4px 8px;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
}

.diva-btn--primary {
  background: var(--diva-hot-pink);
  color: var(--diva-white);
  border-color: var(--diva-deep-pink);
}

.diva-btn--primary:hover {
  background: var(--diva-deep-pink);
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(255, 20, 147, 0.3);
}

.diva-btn--outline {
  background: transparent;
  color: var(--diva-hot-pink);
  border-color: var(--diva-hot-pink);
}

.diva-btn--outline:hover {
  background: var(--diva-hot-pink);
  color: var(--diva-white);
}
```

### Alternating Section Backgrounds

```css
/* Pale pink section */
.diva-section--pink {
  background: linear-gradient(180deg, var(--diva-blush), var(--diva-pale-pink));
  padding: 4rem 2rem;
}

/* Cream / warm white section */
.diva-section--cream {
  background: var(--diva-cream);
  padding: 4rem 2rem;
}

/* Lavender section */
.diva-section--lavender {
  background: linear-gradient(180deg, #f5f0ff, #faf5ff);
  padding: 4rem 2rem;
}

/* Clean white section */
.diva-section--white {
  background: var(--diva-white);
  padding: 4rem 2rem;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Shoe Diva materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Sketchy pen-and-ink illustration | Thin, slightly irregular CSS borders; SVG linework; hand-drawn-style fonts |
| Watercolor washes | Semi-transparent gradient fills; soft pastel background blends |
| Glitter and sparkle | Tiny radial-gradient dots overlay; animated shimmer gradients; gold accents |
| Satin ribbon | Smooth pink gradient strips as dividers; bow emoji decorations |
| Fluffy textures (feathers, fur trim) | Soft box-shadows; blur effects; layered translucent overlays |
| Glossy magazine paper | Clean white card backgrounds; subtle sheen gradients; crisp edges |
| Designer shopping bag tissue paper | Pale, warm-tinted background colors; soft cream and blush surfaces |
| Champagne bubbles | Scattered small radial gradient circles; gentle floating animations |
| Lipstick / nail polish | High-saturation pink accent blocks; glossy gradient buttons |
| Fashion illustration paper | White or off-white card backgrounds with fine sketch-style line borders |
| Perfume bottle glass | Translucent pink overlays with `backdrop-filter: blur`; soft glow effects |

---

## Key Visual Values

- **Playful sophistication** -- lighthearted and fun, but aimed at adult women rather than children or tweens
- **Aspirational glamour** -- the aesthetic sells a fantasy of fashionable urban living, shopping sprees, and cocktail culture
- **Hand-drawn whimsy** -- the sketch-like, loopy illustration style is the defining visual signature
- **Unapologetic femininity** -- everything is bright, pink, sparkly, and confidently girly without restraint
- **Consumerist joy** -- shopping, shoes, fashion, and luxury goods are celebrated as sources of happiness
- **Urban chic** -- rooted in a glamorized vision of New York and Paris as fashion capitals
- **Editorial polish** -- despite the hand-drawn looseness, the overall presentation is polished and commercial-ready

---

## Related Aesthetics

| Aesthetic | Relationship to Shoe Diva |
|-----------|--------------------------|
| **Parisian Girly** | Closely related; Shoe Diva is the more mature, worldly counterpart with adult women as the target audience |
| **Curly Girly** | Shares the fashion-illustration sensibility and pink palette; Curly Girly is more tween-oriented with curled serif typography |
| **McBling** | Contemporary trend (2003-2008); shares bright, feminine color palette and commercial glamour |
| **Vectordelia** | Related through the vector illustration and decorative line art traditions |

---

## Associated Brands and Media

### Literature
- Sophie Kinsella's *Confessions of a Shopaholic* series (book covers are quintessential examples)
- Lauren Weisberger's *The Devil Wears Prada* (2003)
- Madonna's *The English Roses* book series

### Television and Film
- *Sex and the City* (1998-2004) -- Carrie Bradshaw as the cultural archetype
- *Legally Blonde* (2001)
- *Ugly Betty* (2006-2010)
- *Confessions of a Shopaholic* (2009 film)

### Brands
- Manolo Blahnik
- Chanel
- Skinny Girl Cocktails
- My Scene (Mattel doll franchise)

---

## Quick-Start: Minimal Shoe Diva Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Shoe Diva Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@400;700&family=Dancing+Script:wght@400;700&family=Quicksand:wght@400;500;600&family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --diva-hot-pink: #ff69b4;
      --diva-deep-pink: #ff1493;
      --diva-rose: #f472b6;
      --diva-blush: #ffd6e0;
      --diva-pale-pink: #fff0f5;
      --diva-sunny-yellow: #ffd700;
      --diva-lime-green: #77dd77;
      --diva-sky-blue: #87ceeb;
      --diva-lavender: #e6c8ff;
      --diva-black: #2a2a2a;
      --diva-white: #ffffff;
      --diva-cream: #fffef5;
      --diva-gold: #d4af37;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--diva-pale-pink);
      color: var(--diva-black);
      font-family: 'Quicksand', sans-serif;
      font-weight: 400;
      letter-spacing: 0.02em;
      line-height: 1.7;
    }

    h1, h2 {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      letter-spacing: 0.03em;
    }

    h3 {
      font-family: 'Dancing Script', cursive;
      font-weight: 700;
    }

    .hero {
      text-align: center;
      padding: 5rem 2rem 4rem;
      background: linear-gradient(
        180deg,
        var(--diva-pale-pink) 0%,
        var(--diva-cream) 100%
      );
    }

    .hero h1 {
      font-family: 'Great Vibes', cursive;
      font-size: clamp(3rem, 8vw, 6rem);
      color: var(--diva-hot-pink);
      font-weight: 400;
      letter-spacing: 0.02em;
      line-height: 1.2;
    }

    .hero .subtitle {
      font-family: 'Montserrat', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      font-size: 0.85rem;
      color: var(--diva-black);
      margin-top: 0.5rem;
    }

    /* Bow ribbon divider */
    .diva-divider {
      text-align: center;
      margin: 2rem 0;
      position: relative;
    }

    .diva-divider::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 15%;
      right: 15%;
      height: 1px;
      background: linear-gradient(90deg, transparent, var(--diva-hot-pink), transparent);
    }

    .diva-divider::after {
      content: '\1F460';
      position: relative;
      z-index: 1;
      background: var(--diva-pale-pink);
      padding: 0 0.8rem;
      font-size: 1.2rem;
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 3rem 2rem;
      text-align: center;
    }

    section h2 {
      margin-bottom: 1rem;
      color: var(--diva-black);
    }

    .card {
      background: var(--diva-white);
      border: 1.5px solid var(--diva-black);
      border-radius: 4px 12px 4px 10px;
      padding: 2rem;
      margin: 1.5rem 0;
      box-shadow: 3px 3px 0 0 var(--diva-blush);
      transition: box-shadow 0.3s ease, transform 0.3s ease;
      text-align: left;
    }

    .card:hover {
      box-shadow: 5px 5px 0 0 var(--diva-hot-pink);
      transform: translate(-2px, -2px);
    }

    .card h3 {
      font-size: 1.4rem;
      color: var(--diva-deep-pink);
      margin-bottom: 0.5rem;
    }

    /* Loopy decorative line */
    .loopy-line {
      height: 20px;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 20'%3E%3Cpath d='M0 10 Q10 0 20 10 T40 10 T60 10 T80 10 T100 10 T120 10 T140 10 T160 10 T180 10 T200 10' fill='none' stroke='%23ff69b4' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: repeat-x;
      background-size: 200px 20px;
      background-position: center;
      margin: 1rem 0;
    }
  </style>
</head>
<body>
  <div class="loopy-line"></div>
  <div class="hero">
    <h1>Title Here</h1>
    <p class="subtitle">A Shoe Diva Presentation</p>
    <div class="diva-divider"></div>
  </div>
  <section>
    <h2>Section Heading</h2>
    <div class="card">
      <h3>Fabulous Content</h3>
      <p>Styled with the Shoe Diva aesthetic -- whimsical hand-drawn energy, bright pinks, and the glamour of fashion-forward urban living.</p>
    </div>
    <div class="card">
      <h3>Shopping Spree</h3>
      <p>Every element celebrates playful sophistication, from the loopy linework to the sparkle-dusted accents and sketch-style borders.</p>
    </div>
  </section>
  <div class="loopy-line"></div>
</body>
</html>
```
