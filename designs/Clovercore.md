# Clovercore Design Reference

Clovercore is a nature-inspired, hyper-cute aesthetic rooted in **late 1990s to early 2000s Japanese stationery culture**. It centers on the four-leaf clover as a symbol of luck, happiness, and innocence, blending **organic, earthy greens** with **glossy, pastel sweetness**. The look channels the era of Kamio Japan, Q-Lia, Mind Wave, San-X, and Crux memo pads -- tiny collectible stationery sheets covered in nameless mascot animals, sparkle graphics, lace borders, and optimistic "Engrish" phrases about luck and dreams. Clovercore evokes **anemoia** (nostalgia for a time you never experienced), childhood wonder, and a distinctly Y2K-era Japanese kawaii sensibility.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Four-leaf clovers** -- the central, defining motif; used as icons, repeating patterns, borders, and background fills
- **Ladybugs** -- small, cheerful insect companions frequently paired with clover imagery
- **Musical notes** -- scattered decoratively to suggest lightheartedness and melody
- **Lace borders** -- delicate, scalloped or doily-style edges framing content areas
- **Polka dots** -- soft, rounded dot patterns in pastel or white used as backgrounds
- **Sparkle / glitter graphics** -- star-shaped highlights and shimmer effects scattered across compositions
- **Nameless mascot animals** -- simple, rounded bears, pandas, hamsters, and bunnies with minimal features
- **Rainbows** -- small pastel arcs used as accent decorations
- **Bubbles** -- translucent circular shapes adding an airy, dreamy quality
- **Hearts and stars** -- secondary decorative elements reinforcing the kawaii language

### Design Principles

- **Hyper-cute, kawaii visual language** -- everything is rounded, soft, friendly, and approachable
- **Nature-meets-glossy** -- earthy green tones combined with glossy, high-sheen pastel finishes
- **Dense but cheerful decoration** -- surfaces are richly patterned without feeling heavy; decoration is joyful, not oppressive
- **Centered and symmetrical compositions** -- content tends toward balanced, centered layouts
- **White or light backgrounds** -- generous use of white space or very pale backgrounds to let colorful elements pop
- **Small-scale, collectible feel** -- designs echo the intimate scale of memo pads and stickers (think 80x80mm)
- **Playful typography with "Engrish" phrases** -- broken English messages about luck, dreams, happiness, and friendship
- **Soft edges and rounded shapes** -- no sharp corners; border-radius is generous everywhere

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Primary accent** | Lime green, grass green, clover green |
| **Secondary accent** | Soft pink, rose pink |
| **Base / Background** | White, cream, very pale green |
| **Supporting pastels** | Pastel yellow, sky blue, lavender |
| **Neutral** | Warm light gray, pale beige |

### Detailed Color Table

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Clover Green | `#4CAF50` | Primary accent, clover motifs, headings |
| Lime Green | `#8BC34A` | Secondary green, highlights, hover states |
| Pale Leaf Green | `#C8E6C9` | Light backgrounds, card fills, subtle tints |
| Mint Cream | `#E8F5E9` | Page backgrounds, section alternates |
| Soft Pink | `#F8BBD0` | Secondary accent, mascot cheeks, borders |
| Rose Pink | `#E91E63` | Emphasis elements, hearts, small accents (used sparingly) |
| Pale Pink | `#FCE4EC` | Alternating backgrounds, soft highlights |
| Pastel Yellow | `#FFF9C4` | Sparkle accents, star decorations, badges |
| Sunshine Yellow | `#FFD54F` | Ladybug accents, warm highlights |
| Sky Blue | `#B3E5FC` | Bubble elements, secondary decorations |
| Lavender | `#E1BEE7` | Tertiary accent, rainbow elements |
| White | `#FFFFFF` | Primary background, text areas |
| Cream | `#FFF8E7` | Warm background alternative |
| Warm Gray | `#F5F5F5` | Subtle section dividers, neutral zones |
| Soft Charcoal | `#5D4037` | Body text (warm, never pure black) |

### Suggested CSS Custom Properties

```css
:root {
  /* Greens -- primary identity */
  --clover-green: #4CAF50;
  --clover-green-dark: #388E3C;
  --clover-lime: #8BC34A;
  --clover-pale-green: #C8E6C9;
  --clover-mint: #E8F5E9;

  /* Pinks -- secondary warmth */
  --clover-pink: #F8BBD0;
  --clover-rose: #E91E63;
  --clover-pale-pink: #FCE4EC;

  /* Accent pastels */
  --clover-yellow: #FFF9C4;
  --clover-sunshine: #FFD54F;
  --clover-sky: #B3E5FC;
  --clover-lavender: #E1BEE7;

  /* Neutrals */
  --clover-white: #FFFFFF;
  --clover-cream: #FFF8E7;
  --clover-gray: #F5F5F5;
  --clover-text: #5D4037;
  --clover-text-light: #8D6E63;

  /* Functional */
  --clover-bg-primary: var(--clover-white);
  --clover-bg-secondary: var(--clover-mint);
  --clover-bg-card: var(--clover-pale-green);
  --clover-accent: var(--clover-green);
  --clover-accent-secondary: var(--clover-pink);
  --clover-border: var(--clover-pale-green);
}
```

### Approaches

- **Green-dominant with pink accents** -- use clover greens for 60-70% of colored elements, pink for 20-30%, other pastels for the remaining 10%
- **High white-space ratio** -- backgrounds are predominantly white or very pale; color appears in motifs, borders, and accents
- **Pastel layering** -- stack translucent pastel washes for depth without heaviness
- **Warm, never stark** -- avoid pure black text; use warm brown-grays instead
- **Glossy, candy-like finishes** -- subtle gradients and highlights that suggest shininess

---

## Typography

### Typeface Characteristics

Clovercore typography features:

- **Rounded, friendly sans-serif typefaces** -- soft terminals, no sharp corners on letterforms
- **Slightly playful proportions** -- not strictly geometric; a little bouncy or handwritten in feel
- **Lightweight to medium weights** -- heavy bold is rare; the mood is light and airy
- **Mixed-case with decorative capitals** -- title case preferred over all-caps
- **Occasional handwritten / script accents** -- for "Engrish" phrases and decorative labels
- **Small text sizes for charm** -- body text can be modest in size, echoing stationery memo-pad scale

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Nunito** | Rounded sans-serif, friendly | Primary headings, UI elements |
| **Quicksand** | Geometric rounded sans | Subheadings, navigation, labels |
| **Varela Round** | Simple rounded sans | Body text, clean sections |
| **Patrick Hand** | Casual handwritten | "Engrish" phrases, decorative quotes, captions |
| **Caveat** | Natural handwriting | Accent text, annotations, whimsical labels |
| **M PLUS Rounded 1c** | Japanese-inspired rounded | Bilingual designs, authentic kawaii feel |
| **Comfortaa** | Rounded geometric | Display text, hero headings |
| **Baloo 2** | Rounded, bubbly | Fun headings, call-to-action text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700&family=Quicksand:wght@400;500;600&family=Patrick+Hand&family=Varela+Round&display=swap');

/* Headings */
h1, h2, h3 {
  font-family: 'Nunito', 'Quicksand', sans-serif;
  color: var(--clover-green-dark);
  font-weight: 700;
  letter-spacing: 0.02em;
  line-height: 1.3;
}

/* Display / Hero text */
.clover-display {
  font-family: 'Comfortaa', 'Nunito', sans-serif;
  font-size: clamp(2rem, 6vw, 4.5rem);
  font-weight: 700;
  color: var(--clover-green);
  letter-spacing: 0.03em;
}

/* Body text */
body {
  font-family: 'Varela Round', 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  letter-spacing: 0.01em;
  line-height: 1.8;
  color: var(--clover-text);
}

/* Kawaii / Engrish accent phrases */
.clover-phrase {
  font-family: 'Patrick Hand', 'Caveat', cursive;
  font-size: 1.1rem;
  color: var(--clover-text-light);
  font-style: italic;
  letter-spacing: 0.04em;
}

/* Labels and tags */
.clover-label {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--clover-green);
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, single-column primary layout** -- content flows down a central axis, echoing the vertical format of Japanese memo pads
- **Card-based sections** -- individual content blocks are presented as rounded cards or "sticker" panels
- **Generous padding and margins** -- lots of breathing room; nothing should feel cramped
- **Rounded containers everywhere** -- border-radius on all cards, images, buttons, and panels (12px-24px minimum)
- **Max content width of 800-960px** -- the intimate stationery feel is lost on ultra-wide layouts
- **Soft grid with organic placement** -- while underlying grid is structured, elements can slightly overlap or float to feel handmade

### Section Organization

- Use **decorative dividers** between sections -- clover icons, dotted lines, lace-pattern borders, or small mascot illustrations
- Apply **alternating pastel backgrounds** -- white, then pale green, then white, then pale pink for visual rhythm
- Create **hierarchy through color and roundness** rather than size contrast -- headings are distinguished by color (green) more than by dramatic size differences
- Employ **floating decorative elements** -- small clovers, stars, and sparkles positioned around content areas using absolute positioning
- Keep **dense but organized decoration** -- the charm is in the rich detail, but maintain clear content hierarchy

### Responsive Considerations

- Stack cards vertically on mobile; 2-column grid on tablet; max 3 columns on desktop
- Reduce decorative floating elements on smaller screens
- Maintain generous padding even at small sizes -- the "breathing room" is essential to the aesthetic

---

## CSS/Design Techniques

### Lace Border Effect

```css
/* Scalloped lace-style border using radial gradients */
.clover-lace-border {
  position: relative;
  padding: 2rem;
  background: var(--clover-white);
  border: 2px solid var(--clover-pale-green);
  border-radius: 16px;
}

.clover-lace-border::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 10%;
  right: 10%;
  height: 10px;
  background: radial-gradient(
    circle at 10px 0,
    transparent 8px,
    var(--clover-pale-green) 8px,
    var(--clover-pale-green) 10px,
    transparent 10px
  );
  background-size: 20px 10px;
  background-repeat: repeat-x;
}
```

### Sparkle / Glitter Effect

```css
/* Animated sparkle using CSS */
@keyframes sparkle {
  0%, 100% { opacity: 0; transform: scale(0) rotate(0deg); }
  50% { opacity: 1; transform: scale(1) rotate(180deg); }
}

.clover-sparkle {
  position: absolute;
  width: 12px;
  height: 12px;
  background: var(--clover-sunshine);
  clip-path: polygon(
    50% 0%, 61% 35%, 98% 35%, 68% 57%,
    79% 91%, 50% 70%, 21% 91%, 32% 57%,
    2% 35%, 39% 35%
  );
  animation: sparkle 2s ease-in-out infinite;
}

.clover-sparkle:nth-child(2) { animation-delay: 0.5s; }
.clover-sparkle:nth-child(3) { animation-delay: 1.0s; }
.clover-sparkle:nth-child(4) { animation-delay: 1.5s; }
```

### Four-Leaf Clover Shape (CSS-only)

```css
/* Pure CSS four-leaf clover */
.clover-icon {
  position: relative;
  width: 40px;
  height: 40px;
}

.clover-icon::before,
.clover-icon::after,
.clover-icon span::before,
.clover-icon span::after {
  content: '';
  position: absolute;
  width: 20px;
  height: 20px;
  background: var(--clover-green);
  border-radius: 50% 50% 50% 0;
}

.clover-icon::before { top: 0; left: 10px; transform: rotate(45deg); }
.clover-icon::after { top: 10px; right: 0; transform: rotate(135deg); }
.clover-icon span::before { bottom: 0; left: 10px; transform: rotate(-135deg); }
.clover-icon span::after { top: 10px; left: 0; transform: rotate(-45deg); }
```

### Polka Dot Background Pattern

```css
/* Soft polka dot pattern */
.clover-polka-bg {
  background-color: var(--clover-white);
  background-image: radial-gradient(
    circle,
    var(--clover-pale-green) 8px,
    transparent 8px
  );
  background-size: 40px 40px;
}

/* Offset polka dots for a more organic feel */
.clover-polka-bg-offset {
  background-color: var(--clover-white);
  background-image:
    radial-gradient(circle, var(--clover-pale-green) 6px, transparent 6px),
    radial-gradient(circle, var(--clover-pale-pink) 4px, transparent 4px);
  background-size: 50px 50px, 50px 50px;
  background-position: 0 0, 25px 25px;
}
```

### Glossy / Candy Card Effect

```css
/* Glossy card with kawaii sheen */
.clover-card {
  background: linear-gradient(
    135deg,
    var(--clover-white) 0%,
    var(--clover-pale-green) 100%
  );
  border: 2px solid var(--clover-pale-green);
  border-radius: 20px;
  padding: 2rem;
  box-shadow:
    0 4px 12px rgba(76, 175, 80, 0.1),
    inset 0 1px 0 rgba(255, 255, 255, 0.8);
  position: relative;
  overflow: hidden;
}

/* Glossy sheen overlay */
.clover-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.4) 0%,
    rgba(255, 255, 255, 0) 100%
  );
  border-radius: 20px 20px 0 0;
  pointer-events: none;
}
```

### Kawaii Button

```css
.clover-button {
  display: inline-block;
  padding: 0.75rem 2rem;
  font-family: 'Nunito', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: var(--clover-white);
  background: linear-gradient(
    180deg,
    var(--clover-lime) 0%,
    var(--clover-green) 100%
  );
  border: none;
  border-radius: 50px;
  box-shadow:
    0 4px 0 var(--clover-green-dark),
    0 6px 12px rgba(76, 175, 80, 0.25);
  cursor: pointer;
  transition: all 0.15s ease;
  letter-spacing: 0.03em;
}

.clover-button:hover {
  transform: translateY(-2px);
  box-shadow:
    0 6px 0 var(--clover-green-dark),
    0 8px 16px rgba(76, 175, 80, 0.3);
}

.clover-button:active {
  transform: translateY(2px);
  box-shadow:
    0 2px 0 var(--clover-green-dark),
    0 3px 6px rgba(76, 175, 80, 0.2);
}
```

### Decorative Divider with Clover

```css
/* Section divider with centered clover motif */
.clover-divider {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin: 3rem auto;
  max-width: 400px;
}

.clover-divider::before,
.clover-divider::after {
  content: '';
  flex: 1;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--clover-pale-green),
    var(--clover-green),
    var(--clover-pale-green),
    transparent
  );
}

/* The clover symbol sits between the lines (use an actual icon or emoji in HTML) */
```

### Floating Decorative Elements

```css
/* Container for floating decorations */
.clover-decorations {
  position: fixed;
  inset: 0;
  pointer-events: none;
  overflow: hidden;
  z-index: -1;
}

/* Gently floating clover leaf */
@keyframes float-drift {
  0% { transform: translateY(0) rotate(0deg); opacity: 0.3; }
  50% { transform: translateY(-20px) rotate(10deg); opacity: 0.6; }
  100% { transform: translateY(0) rotate(0deg); opacity: 0.3; }
}

.clover-float {
  position: absolute;
  font-size: 1.5rem;
  animation: float-drift 4s ease-in-out infinite;
  color: var(--clover-green);
  opacity: 0.3;
}

.clover-float:nth-child(1) { top: 10%; left: 5%; animation-delay: 0s; }
.clover-float:nth-child(2) { top: 30%; right: 8%; animation-delay: 1s; }
.clover-float:nth-child(3) { top: 60%; left: 3%; animation-delay: 2s; }
.clover-float:nth-child(4) { top: 80%; right: 5%; animation-delay: 3s; }
```

### Mascot Character Placeholder

```css
/* Circular mascot avatar frame */
.clover-mascot {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background: var(--clover-pale-pink);
  border: 3px solid var(--clover-pink);
  box-shadow:
    0 0 0 4px var(--clover-white),
    0 0 0 6px var(--clover-pale-green);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2rem;
  margin: 0 auto;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Clovercore materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Glossy sticker / stationery paper | Subtle white-to-pastel gradients with inset highlight |
| Glitter / holographic accents | Sparkle animations, shimmer gradient overlays |
| Lace trim / doily edges | CSS scalloped borders, repeating radial gradient edges |
| Polka-dot fabric | CSS radial-gradient background patterns |
| Soft rubber / silicone (pencil toppers) | Heavy border-radius, 3D-like button shadows |
| Translucent / frosted plastic | `backdrop-filter: blur()` with semi-transparent backgrounds |
| Memo pad paper | White cards with faint ruled or dotted grid lines |
| Washi tape | Colored semi-transparent strips as decorative accents |

---

## Mood and Tone

### Emotional Language

Clovercore designs should evoke:

- **Luck and optimism** -- "good luck," "happy days," "wishing you happiness"
- **Childhood innocence** -- simple pleasures, collecting, wonder at small things
- **Nature appreciation** -- gentle celebration of leaves, flowers, insects, seasons
- **Nostalgic warmth** -- Y2K-era Japanese design sensibility, pre-smartphone simplicity
- **Gentle encouragement** -- phrases like "follow your dreams," "you can do it," "every day is a gift"

### Sample Decorative Phrases (Engrish Style)

These are the kinds of text fragments that appear on Clovercore stationery and can be used as decorative elements:

- "Happy Clover Days"
- "A little luck for you"
- "Sweet dream time"
- "Nature is my friend"
- "Lucky lucky happy days"
- "Gentle breeze and clover fields"

---

## Related Aesthetics

| Aesthetic | Relationship to Clovercore |
|-----------|----------------------------|
| **Frutiger Eco** | Shares nature-meets-technology glossy optimism; Clovercore is cuter and more stationery-focused |
| **Global Village Coffeehouse** | Overlapping earthy, friendly vibes; Coffeehouse is more mature and multicultural |
| **Heisei Retro** | Same era (late Heisei period Japan); broader Japanese retro vs. Clovercore's specific stationery niche |
| **Juminocore** | Similar kawaii Japanese stationery roots; Juminocore is broader in motif range |
| **Puppycore** | Shares cute animal mascot focus; Puppycore centers specifically on dogs/puppies |
| **Whimsy Twee** | Overlapping cute, handmade, nature-loving sensibility; Twee is more Western indie-craft |
| **Cottagecore** | Shared nature romanticism; Cottagecore is rural Western, Clovercore is urban Japanese kawaii |
| **Sanriocore** | Adjacent kawaii stationery culture; Sanriocore focuses on named Sanrio characters specifically |

---

## Quick-Start: Minimal Clovercore Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clovercore Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700&family=Quicksand:wght@400;500;600&family=Patrick+Hand&family=Varela+Round&display=swap" rel="stylesheet">
  <style>
    :root {
      --clover-green: #4CAF50;
      --clover-green-dark: #388E3C;
      --clover-lime: #8BC34A;
      --clover-pale-green: #C8E6C9;
      --clover-mint: #E8F5E9;
      --clover-pink: #F8BBD0;
      --clover-pale-pink: #FCE4EC;
      --clover-sunshine: #FFD54F;
      --clover-white: #FFFFFF;
      --clover-cream: #FFF8E7;
      --clover-text: #5D4037;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--clover-white);
      color: var(--clover-text);
      font-family: 'Varela Round', 'Quicksand', sans-serif;
      font-weight: 400;
      line-height: 1.8;
      letter-spacing: 0.01em;
    }

    h1, h2, h3 {
      font-family: 'Nunito', sans-serif;
      color: var(--clover-green-dark);
      font-weight: 700;
    }

    .hero {
      text-align: center;
      padding: 5rem 2rem;
      background: linear-gradient(180deg, var(--clover-mint) 0%, var(--clover-white) 100%);
    }

    .hero h1 {
      font-size: clamp(2.2rem, 5vw, 4rem);
      color: var(--clover-green);
    }

    .hero .phrase {
      font-family: 'Patrick Hand', cursive;
      color: var(--clover-text);
      opacity: 0.7;
      font-size: 1.2rem;
      margin-top: 0.5rem;
    }

    .clover-divider {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 0.75rem;
      margin: 2.5rem auto;
      max-width: 300px;
      color: var(--clover-green);
      font-size: 1.2rem;
    }

    .clover-divider::before,
    .clover-divider::after {
      content: '';
      flex: 1;
      height: 2px;
      background: linear-gradient(90deg, transparent, var(--clover-pale-green), transparent);
    }

    section {
      max-width: 800px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    section:nth-child(even) {
      background: var(--clover-mint);
      max-width: 100%;
    }

    section:nth-child(even) > * {
      max-width: 800px;
      margin-left: auto;
      margin-right: auto;
    }

    .card {
      background: linear-gradient(135deg, var(--clover-white), var(--clover-pale-green));
      border: 2px solid var(--clover-pale-green);
      border-radius: 20px;
      padding: 2rem;
      box-shadow: 0 4px 12px rgba(76, 175, 80, 0.1);
      margin: 1.5rem 0;
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p class="phrase">Happy clover days</p>
  </div>

  <div class="clover-divider">&#9752;</div>

  <section>
    <h2>Section Heading</h2>
    <div class="card">
      <p>Content styled with the Clovercore aesthetic -- soft, rounded, green-and-pink, full of gentle optimism.</p>
    </div>
  </section>

  <section>
    <h2>Another Section</h2>
    <p>Alternating pale green backgrounds create visual rhythm.</p>
  </section>
</body>
</html>
```
