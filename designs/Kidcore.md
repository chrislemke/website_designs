# Kidcore - Design Reference

## Overview

Kidcore is a maximalist, nostalgia-fueled web aesthetic that celebrates the unbridled joy and sensory overload of 1990s and early 2000s childhood. Rooted in hyper-saturated primary colors, toy-box imagery, and the visual language of Lisa Frank folders, Nickelodeon bumpers, and cereal box packaging, Kidcore treats the screen as a playground where more is always more. Layouts favor collage-style compositions with tilted elements, sticker-like decorations, crayon textures, and chunky rounded shapes that evoke arts-and-crafts tables and playroom floors. Typography is bubbly, hand-drawn, and deliberately imperfect, rejecting sophistication in favor of exuberant, childlike energy. Rainbow gradients, checkerboard patterns, smiley faces, stars, hearts, and cartoon doodles are layered without restraint, creating a scrapbook-like density that rewards exploration. The philosophy is joyful maximalism -- every pixel should feel like it was decorated by a kid with unlimited markers, stickers, and glitter glue.

---

## Visual Characteristics

### Core Design Traits

- **Hyper-saturated primary colors**: Pure reds, blues, and yellows dominate every surface, pushed to maximum saturation and paired with equally bold greens, oranges, and pinks to create a relentlessly vibrant palette
- **Collage-style layouts**: Elements are layered, overlapped, and slightly rotated as if pasted into a scrapbook, rejecting grid alignment in favor of intentional visual chaos
- **Sticker and doodle decorations**: Stars, hearts, smiley faces, rainbows, clouds, flowers, and squiggly lines are scattered across the design as decorative accents, mimicking the sticker sheets and notebook doodles of childhood
- **Rounded and bubbly shapes**: All containers, buttons, and decorative elements use exaggerated border-radius values, evoking toy blocks, gumballs, and inflatable furniture
- **Rainbow gradients**: Multi-color gradients spanning the full spectrum appear on backgrounds, borders, text, and decorative bands, reinforcing the more-is-more philosophy
- **Crayon and marker textures**: Rough, hand-drawn borders, wobbly lines, and textured fills simulate the imperfect mark-making of crayons, finger paint, and colored pencils
- **Toy and cartoon motifs**: Visual references to building blocks, alphabet magnets, board games, gummy bears, ball pits, and cartoon characters anchor the design in tactile childhood objects
- **Checkerboard and playful patterns**: Bold checkerboard grids, polka dots, zigzag borders, and rainbow stripes serve as background patterns and section dividers
- **Thick, visible outlines**: All elements carry heavy dark outlines reminiscent of coloring book illustrations and cartoon cel animation
- **Playful drop shadows**: Chunky, hard-offset shadows in contrasting colors give elements a sticker-peel or pop-up book dimensionality

### Design Principles

- **Joy over elegance**: Every design decision prioritizes fun, energy, and visual excitement over refinement, sophistication, or subtlety
- **Maximalism as philosophy**: Empty space is an opportunity for another sticker, another color, another pattern; whitespace is minimized in favor of visual density
- **Nostalgic authenticity**: References should feel genuine to the 90s/Y2K childhood experience rather than ironic or cynical; the tone is warm and earnest
- **Imperfection is charm**: Slightly misaligned elements, wobbly borders, and hand-drawn textures are features, not bugs; over-polished designs lose the handmade quality
- **Accessibility through contrast**: Despite the visual complexity, text must remain readable through strong color contrast and generous sizing
- **Layered discovery**: Dense compositions should reward exploration, with decorative details that reveal themselves on closer inspection

---

## Color Palette

Kidcore demands a palette that hits like a box of 64 crayons spilled across a table. Primary colors form the foundation, supported by a full rainbow of secondary and accent hues at maximum saturation.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| Crayon Red | `#FF2D2D` | Primary accent, buttons, hearts, alert states |
| Sunshine Yellow | `#FFD600` | Backgrounds, highlights, star decorations, hover states |
| True Blue | `#2979FF` | Links, headers, borders, sky elements |
| Grass Green | `#00C853` | Success states, nature motifs, checkerboard fills |
| Bubblegum Pink | `#FF6EC7` | Decorative accents, badges, sticker outlines |
| Tangerine Orange | `#FF6D00` | Secondary buttons, callouts, warm accents |
| Grape Purple | `#AA00FF` | Tags, decorative shadows, alternating pattern fills |
| Cloud White | `#FFFEF5` | Page background, card surfaces, breathing room |
| Chalkboard Black | `#1A1A2E` | Text, outlines, thick borders, cartoon strokes |
| Robin Egg Blue | `#00E5FF` | Secondary links, decorative borders, water motifs |
| Candy Apple | `#D50000` | Deep accent, important labels, bold emphasis |
| Lemon Lime | `#C6FF00` | Highlight backgrounds, tag fills, energetic accents |
| Cotton Candy | `#F8BBD0` | Soft backgrounds, alternating rows, gentle sections |
| Royal Blue | `#304FFE` | Dark link variant, footer backgrounds, contrast text |
| Rainbow Gradient Start | `#FF0000` | Left/top edge of rainbow gradient bands |
| Rainbow Gradient End | `#8B00FF` | Right/bottom edge of rainbow gradient bands |

### CSS Custom Properties

```css
:root {
  /* Primary colors */
  --kid-red: #FF2D2D;
  --kid-yellow: #FFD600;
  --kid-blue: #2979FF;
  --kid-green: #00C853;

  /* Secondary colors */
  --kid-pink: #FF6EC7;
  --kid-orange: #FF6D00;
  --kid-purple: #AA00FF;
  --kid-cyan: #00E5FF;

  /* Supporting colors */
  --kid-candy-red: #D50000;
  --kid-lime: #C6FF00;
  --kid-cotton-candy: #F8BBD0;
  --kid-royal-blue: #304FFE;

  /* Neutrals */
  --kid-white: #FFFEF5;
  --kid-black: #1A1A2E;

  /* Rainbow gradient */
  --kid-rainbow: linear-gradient(
    90deg,
    #FF0000, #FF8800, #FFD600,
    #00C853, #2979FF, #AA00FF, #8B00FF
  );

  /* Functional tokens */
  --kid-bg: var(--kid-white);
  --kid-text: var(--kid-black);
  --kid-border: var(--kid-black);
  --kid-accent: var(--kid-red);
  --kid-highlight: var(--kid-yellow);
  --kid-link: var(--kid-blue);
  --kid-shadow-color: var(--kid-pink);
  --kid-radius: 20px;
  --kid-radius-lg: 30px;
  --kid-radius-pill: 999px;
  --kid-outline: 3px;
  --kid-shadow-offset: 5px;
}
```

---

## Typography

Kidcore typography should feel hand-drawn, bubbly, and exuberant. Letters should look like they were written with fat markers, stamped with alphabet blocks, or inflated like balloons. Readability matters, but personality matters more.

### Typeface Characteristics

- **Rounded terminals and stroke endings** -- no sharp serifs or angular cuts; every letterform should feel soft and approachable
- **Heavy weight bias** -- bold and extra-bold weights dominate; thin or light weights feel too delicate for the playful energy required
- **Irregular or hand-drawn quality** -- slight variation in stroke width, baseline alignment, or letter spacing mimics real handwriting and hand-lettering
- **Large x-heights** -- generous lowercase proportions improve readability at the smaller sizes used in body text while maintaining a childlike openness
- **Decorative display faces for headings** -- headings can push into novelty territory with bubble letters, block shapes, or crayon textures that would be unreadable at small sizes

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| Bubblegum Sans | Rounded, playful display | Headlines, hero text, feature titles |
| Fredoka | Variable weight, rounded | Headings, subheadings, UI labels |
| Gaegu | Childlike handwriting | Body text, captions, personal notes |
| Patrick Hand | Casual handwritten | Body text, descriptions, informal content |
| Bungee | Bold block display | Hero titles, banners, large display text |
| Sniglet | Rounded, friendly sans | Navigation, buttons, card titles |
| Schoolbell | Notebook handwriting | Decorative text, annotations, asides |
| Baloo 2 | Heavy rounded sans | Subheadings, callouts, badge labels |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Bubblegum Sans | Patrick Hand | Toy packaging meets notebook scribbles; playful and readable |
| Fredoka (700) | Gaegu | Chunky rounded headers with casual handwritten body; arts-and-crafts |
| Bungee | Patrick Hand | Bold block-letter impact paired with friendly handwriting; cereal box energy |
| Sniglet | Gaegu | Friendly rounded headers with childlike body text; storybook feel |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Bubblegum+Sans&family=Fredoka:wght@400;500;600;700&family=Patrick+Hand&display=swap');

/* === Base Typography === */
body {
  font-family: 'Patrick Hand', 'Comic Sans MS', 'Segoe Print', cursive;
  font-size: 18px;
  line-height: 1.7;
  color: var(--kid-text);
  background-color: var(--kid-bg);
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Bubblegum Sans', 'Fredoka', 'Comic Sans MS', cursive;
  line-height: 1.2;
  color: var(--kid-text);
  text-shadow: 3px 3px 0 var(--kid-yellow);
}

h1 {
  font-size: clamp(2.5rem, 8vw, 5rem);
  text-shadow: 4px 4px 0 var(--kid-pink);
}

h2 {
  font-family: 'Fredoka', 'Comic Sans MS', cursive;
  font-weight: 700;
  font-size: clamp(1.8rem, 4vw, 3rem);
}

h3 {
  font-family: 'Fredoka', 'Comic Sans MS', cursive;
  font-weight: 600;
  font-size: clamp(1.3rem, 3vw, 2rem);
}

a {
  color: var(--kid-link);
  text-decoration: underline wavy;
  text-underline-offset: 4px;
  transition: color 0.2s, transform 0.2s;
}

a:hover {
  color: var(--kid-pink);
  transform: scale(1.05);
}

.rainbow-text {
  background: var(--kid-rainbow);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

---

## Layout Principles

### Grid and Structure

- **Collage over grid**: Prefer overlapping, rotated, and irregularly placed elements over strict grid alignment; use CSS Grid and Flexbox as foundations but break the regularity with transforms and negative margins
- **Generous border-radius everywhere**: All containers, cards, buttons, and images should use rounded corners (20px minimum) to maintain the soft, toylike feel
- **Thick dark outlines on every element**: A 3px solid border in the dark color around cards, images, and interactive elements creates the coloring-book look essential to the aesthetic
- **Sticker-style layering**: Use absolute positioning, z-index stacking, and slight rotations (2 to 5 degrees) to create a pasted-on, scrapbook depth
- **Rainbow dividers between sections**: Replace standard horizontal rules with gradient bars spanning the full width in the rainbow spectrum
- **Visible, chunky spacing**: Padding and margins should be generous and visually obvious; tight spacing feels adult and corporate

### Section Organization

- **Hero with oversized display text**: Lead with a massive, colorful headline surrounded by floating decorative elements (stars, clouds, hearts)
- **Card-based content zones**: Present information in rounded, outlined cards with colored backgrounds that alternate through the palette
- **Feature strips with alternating colors**: Full-width colored bands that alternate between palette colors, each containing a single feature or content block
- **Sticker sidebar or floating elements**: Decorative elements positioned in margins or overlapping section boundaries to break the rectangular monotony
- **Footer as a playground**: The footer continues the playful energy with bright colors, doodle borders, and a rainbow gradient cap

### Responsive Approach

- **Stack and scale rather than hide**: On smaller screens, collage elements stack vertically but maintain their rotations, colors, and decorative elements
- **Maintain border-radius proportions**: Round corners should scale with the viewport but never drop below 12px; sharp corners break the aesthetic
- **Fluid typography with generous minimums**: Use clamp() for all text sizes with minimum values large enough to remain bubbly and readable on mobile
- **Preserve decorative elements**: Unlike minimal designs that strip decoration on mobile, Kidcore should keep its stickers, doodles, and color variety at all breakpoints
- **Touch-friendly oversized targets**: Buttons and interactive elements should be large (minimum 48px tap targets) which naturally aligns with the chunky, oversized aesthetic

---

## CSS / Design Techniques

### Kidcore Card

A bubbly content card with thick outlines, colored shadow, and rounded corners that looks like a sticker peeled off a sheet.

```css
.kid-card {
  background-color: var(--kid-white);
  border: var(--kid-outline) solid var(--kid-black);
  border-radius: var(--kid-radius);
  padding: 1.5rem;
  box-shadow: var(--kid-shadow-offset) var(--kid-shadow-offset) 0 var(--kid-shadow-color);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  position: relative;
  overflow: visible;
}

.kid-card:hover {
  transform: translateY(-4px) rotate(-1deg);
  box-shadow: 8px 8px 0 var(--kid-purple);
}

.kid-card::before {
  content: '';
  position: absolute;
  top: -10px;
  right: -10px;
  width: 40px;
  height: 40px;
  background: var(--kid-yellow);
  border: 2px solid var(--kid-black);
  border-radius: 50%;
  z-index: 1;
}

.kid-card h3 {
  font-family: 'Fredoka', cursive;
  font-weight: 700;
  font-size: 1.4rem;
  margin-bottom: 0.75rem;
  color: var(--kid-blue);
}

.kid-card p {
  font-size: 1rem;
  line-height: 1.6;
  margin-bottom: 1rem;
}

.kid-card .tag {
  display: inline-block;
  font-family: 'Fredoka', cursive;
  font-size: 0.75rem;
  font-weight: 600;
  padding: 0.25rem 0.75rem;
  border-radius: var(--kid-radius-pill);
  border: 2px solid var(--kid-black);
  background-color: var(--kid-lime);
  margin-right: 0.4rem;
  margin-bottom: 0.4rem;
}
```

### Kidcore Button

Chunky, rounded buttons with bold outlines and a playful press effect that feels like pushing a toy.

```css
.kid-btn {
  display: inline-block;
  font-family: 'Fredoka', 'Comic Sans MS', cursive;
  font-size: 1.1rem;
  font-weight: 600;
  padding: 0.8rem 2rem;
  border: var(--kid-outline) solid var(--kid-black);
  border-radius: var(--kid-radius-pill);
  background-color: var(--kid-red);
  color: var(--kid-white);
  cursor: pointer;
  text-decoration: none;
  text-align: center;
  box-shadow: 4px 4px 0 var(--kid-black);
  transition: transform 0.15s ease, box-shadow 0.15s ease;
  position: relative;
}

.kid-btn:hover {
  transform: translateY(-2px);
  box-shadow: 6px 6px 0 var(--kid-black);
}

.kid-btn:active {
  transform: translateY(3px);
  box-shadow: 1px 1px 0 var(--kid-black);
}

.kid-btn--blue { background-color: var(--kid-blue); }
.kid-btn--green { background-color: var(--kid-green); color: var(--kid-black); }
.kid-btn--pink { background-color: var(--kid-pink); }
.kid-btn--yellow { background-color: var(--kid-yellow); color: var(--kid-black); }
.kid-btn--orange { background-color: var(--kid-orange); }

.kid-btn--outline {
  background-color: var(--kid-white);
  color: var(--kid-black);
}
```

### Kidcore Navigation

A colorful top navigation bar with pill-shaped links and rainbow underline, like alphabet magnets on a fridge.

```css
.kid-nav {
  background-color: var(--kid-yellow);
  border-bottom: var(--kid-outline) solid var(--kid-black);
  padding: 0.75rem 1.5rem;
  position: relative;
}

.kid-nav::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 0;
  right: 0;
  height: 5px;
  background: var(--kid-rainbow);
}

.kid-nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 0.5rem;
}

.kid-nav .logo {
  font-family: 'Bubblegum Sans', cursive;
  font-size: 1.5rem;
  color: var(--kid-black);
  text-decoration: none;
  margin-right: 1rem;
}

.kid-nav a {
  display: block;
  padding: 0.5rem 1rem;
  font-family: 'Fredoka', cursive;
  font-weight: 600;
  font-size: 1rem;
  color: var(--kid-black);
  text-decoration: none;
  border-radius: var(--kid-radius-pill);
  border: 2px solid transparent;
  transition: background-color 0.2s, border-color 0.2s;
}

.kid-nav a:hover {
  background-color: var(--kid-white);
  border-color: var(--kid-black);
}

.kid-nav a.active {
  background-color: var(--kid-red);
  color: var(--kid-white);
  border-color: var(--kid-black);
}
```

### Kidcore Hero Section

A loud, celebratory hero with oversized rainbow text, floating decorative elements, and a patterned background.

```css
.kid-hero {
  min-height: 85vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 3rem 2rem;
  background-color: var(--kid-cyan);
  background-image:
    radial-gradient(circle, var(--kid-white) 1px, transparent 1px),
    radial-gradient(circle, var(--kid-white) 1px, transparent 1px);
  background-size: 30px 30px;
  background-position: 0 0, 15px 15px;
  border-bottom: var(--kid-outline) solid var(--kid-black);
  position: relative;
  overflow: hidden;
}

.kid-hero h1 {
  font-family: 'Bubblegum Sans', cursive;
  font-size: clamp(3rem, 10vw, 7rem);
  line-height: 1.1;
  color: var(--kid-black);
  text-shadow:
    4px 4px 0 var(--kid-yellow),
    -2px -2px 0 var(--kid-pink);
  position: relative;
  z-index: 2;
}

.kid-hero p {
  font-family: 'Patrick Hand', cursive;
  font-size: clamp(1.1rem, 2.5vw, 1.6rem);
  max-width: 50ch;
  margin-top: 1.5rem;
  color: var(--kid-black);
  position: relative;
  z-index: 2;
  background-color: rgba(255, 254, 245, 0.85);
  padding: 1rem 2rem;
  border-radius: var(--kid-radius);
  border: 2px solid var(--kid-black);
}

.kid-hero .btn-row {
  margin-top: 2rem;
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
  position: relative;
  z-index: 2;
}

/* Floating decorative star */
.kid-hero .deco-star {
  position: absolute;
  font-size: 3rem;
  animation: float 3s ease-in-out infinite;
  z-index: 1;
  filter: drop-shadow(2px 2px 0 var(--kid-black));
}

@keyframes float {
  0%, 100% { transform: translateY(0) rotate(0deg); }
  50% { transform: translateY(-15px) rotate(10deg); }
}
```

### Rainbow Divider

A full-width gradient strip that replaces boring horizontal rules with childhood energy.

```css
.kid-divider {
  height: 8px;
  border: none;
  background: var(--kid-rainbow);
  border-top: 2px solid var(--kid-black);
  border-bottom: 2px solid var(--kid-black);
  margin: 0;
}

.kid-divider--thick {
  height: 16px;
  border-radius: 8px;
  margin: 2rem 1rem;
  border: 2px solid var(--kid-black);
}

.kid-divider--wavy {
  height: 20px;
  background: var(--kid-rainbow);
  border: 2px solid var(--kid-black);
  border-radius: 10px;
  margin: 2rem 1rem;
  position: relative;
}
```

### Sticker Badge

Small decorative labels that mimic adhesive stickers, used for tags, categories, and decorative callouts.

```css
.kid-sticker {
  display: inline-flex;
  align-items: center;
  gap: 0.3rem;
  font-family: 'Fredoka', cursive;
  font-weight: 600;
  font-size: 0.85rem;
  padding: 0.4rem 1rem;
  border: 2px solid var(--kid-black);
  border-radius: var(--kid-radius-pill);
  background-color: var(--kid-pink);
  color: var(--kid-black);
  box-shadow: 2px 2px 0 var(--kid-black);
  transform: rotate(-2deg);
  transition: transform 0.2s;
  white-space: nowrap;
}

.kid-sticker:hover {
  transform: rotate(2deg) scale(1.08);
}

.kid-sticker--red { background-color: var(--kid-red); color: var(--kid-white); }
.kid-sticker--blue { background-color: var(--kid-blue); color: var(--kid-white); }
.kid-sticker--green { background-color: var(--kid-green); }
.kid-sticker--yellow { background-color: var(--kid-yellow); }
.kid-sticker--purple { background-color: var(--kid-purple); color: var(--kid-white); }
.kid-sticker--orange { background-color: var(--kid-orange); }
```

### Checkerboard Section

A patterned background section using CSS-generated checkerboard, a signature Kidcore texture.

```css
.kid-checkerboard {
  padding: 3rem 2rem;
  background-color: var(--kid-white);
  background-image:
    linear-gradient(45deg, var(--kid-yellow) 25%, transparent 25%),
    linear-gradient(-45deg, var(--kid-yellow) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, var(--kid-yellow) 75%),
    linear-gradient(-45deg, transparent 75%, var(--kid-yellow) 75%);
  background-size: 40px 40px;
  background-position: 0 0, 0 20px, 20px -20px, -20px 0;
  border-top: var(--kid-outline) solid var(--kid-black);
  border-bottom: var(--kid-outline) solid var(--kid-black);
}

.kid-checkerboard .content-box {
  max-width: 800px;
  margin: 0 auto;
  background-color: var(--kid-white);
  border: var(--kid-outline) solid var(--kid-black);
  border-radius: var(--kid-radius-lg);
  padding: 2.5rem;
  box-shadow: 6px 6px 0 var(--kid-black);
}
```

### Kidcore Feature Strip

Full-width colored bands for showcasing features, alternating through the palette.

```css
.kid-feature-strip {
  padding: 3rem 2rem;
  border-bottom: var(--kid-outline) solid var(--kid-black);
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 2rem;
}

.kid-feature-strip:nth-child(odd) { background-color: var(--kid-cotton-candy); }
.kid-feature-strip:nth-child(even) { background-color: var(--kid-lime); }

.kid-feature-strip .icon-circle {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: var(--kid-outline) solid var(--kid-black);
  background-color: var(--kid-yellow);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2.5rem;
  flex-shrink: 0;
  box-shadow: 4px 4px 0 var(--kid-black);
}

.kid-feature-strip .feature-text {
  flex: 1;
  min-width: 200px;
}

.kid-feature-strip .feature-text h3 {
  font-family: 'Fredoka', cursive;
  font-weight: 700;
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
  color: var(--kid-black);
}

.kid-feature-strip .feature-text p {
  font-size: 1.05rem;
  line-height: 1.6;
}
```

---

## Design Do's and Don'ts

### Do

- **Saturate everything** -- push colors to their brightest, boldest values; muted or pastel-leaning tones weaken the toy-box energy
- **Round every corner** -- cards, buttons, images, and containers all need generous border-radius; sharp corners feel corporate and adult
- **Layer decorative elements** -- scatter stars, hearts, smiley faces, and doodle accents across the layout like stickers on a notebook cover
- **Use thick dark outlines** -- a consistent 3px solid border on all major elements creates the coloring-book look essential to the aesthetic
- **Mix multiple colors per section** -- each card, button, or badge can be a different color; chromatic variety is a feature, not a bug
- **Include rainbow gradients** -- use them for dividers, borders, text highlights, and background accents wherever energy feels low
- **Embrace CSS animations** -- gentle bounces, wobbles, and floats on decorative elements add the kinetic, alive quality of a toy store
- **Keep text large and readable** -- chunky fonts at generous sizes maintain both the playful look and practical accessibility
- **Use emoji and Unicode symbols** -- stars, hearts, sparkles, and smiley faces as inline text decorations reinforce the childlike tone
- **Test with real content** -- the design should feel joyful even with actual text and images, not just with placeholder lorem ipsum

### Don't

- **Don't use thin, elegant typefaces** -- serif fonts, light weights, and tightly tracked lettering contradict the bubbly, handmade aesthetic
- **Don't pursue minimal whitespace** -- Kidcore is maximalist, but don't confuse density with cramped text; generous padding inside elements is essential
- **Don't default to grayscale** -- gray text, gray borders, and gray backgrounds drain the life from the palette; use the full color spectrum instead
- **Don't use subtle hover states** -- interactions should be obvious and delightful with noticeable color changes, scale bumps, and rotations
- **Don't add ironic or cynical tone** -- Kidcore nostalgia should feel warm and sincere; sarcasm and dark humor undercut the joyful spirit
- **Don't forget accessibility** -- despite the visual complexity, maintain WCAG contrast ratios, keyboard navigation, and screen reader support
- **Don't use stock corporate photography** -- if images are needed, lean toward illustrations, cartoon-style graphics, or photos with heavy color filters and sticker overlays
- **Don't create perfectly symmetrical layouts** -- slight rotations, offset elements, and intentional irregularity maintain the handmade, scrapbook energy
- **Don't neglect mobile** -- the dense, layered aesthetic needs careful responsive adjustment so elements do not overlap into unreadable piles on small screens

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Y2K Futurism](Y2K_Futurism.md) | Overlaps in the late-90s/early-2000s nostalgia timeline, but Y2K leans chrome, cyber, and futuristic where Kidcore stays grounded in toys and craft supplies |
| [Maximalism](Maximalism.md) | Shares the more-is-more philosophy and rejection of empty space, but Maximalism draws from luxury and eclectic fine art rather than childhood play |
| [Neubrutalism](Neubrutalism.md) | Both use thick dark outlines and hard-offset colored shadows, but Neubrutalism is geometric and adult where Kidcore is rounded and childlike |
| [Wacky Postmodernism](Wacky_Pomo.md) | Related in the playful rejection of design rules and love of clashing colors, but Wacky Pomo is more ironic and intellectual in its rule-breaking |
| [Memphis Design](Memphis_Design.md) | A direct visual ancestor through its bold geometric patterns, clashing colors, and rejection of minimalist good taste popular in 80s/90s kids products |
| [Cottagecore](Cottagecore.md) | Both are nostalgia-driven internet aesthetics, but Cottagecore yearns for pastoral simplicity while Kidcore celebrates urban, plastic, screen-lit childhood |
| [Vaporwave](Vaporwave.md) | Shares 90s nostalgia roots but processes it through irony, melancholy, and lo-fi digital artifacts rather than Kidcore's earnest, bright optimism |
| [Whimsigothic](Whimsigothic.md) | Both embrace maximalism and decorative excess, but Whimsigothic channels dark mysticism while Kidcore channels sunny, daytime play energy |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Playtown Creative Studio</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bubblegum+Sans&family=Fredoka:wght@400;500;600;700&family=Patrick+Hand&display=swap" rel="stylesheet">
  <style>
    /* --- Custom Properties --- */
    :root {
      --kid-red: #FF2D2D;
      --kid-yellow: #FFD600;
      --kid-blue: #2979FF;
      --kid-green: #00C853;
      --kid-pink: #FF6EC7;
      --kid-orange: #FF6D00;
      --kid-purple: #AA00FF;
      --kid-cyan: #00E5FF;
      --kid-candy-red: #D50000;
      --kid-lime: #C6FF00;
      --kid-cotton-candy: #F8BBD0;
      --kid-royal-blue: #304FFE;
      --kid-white: #FFFEF5;
      --kid-black: #1A1A2E;
      --kid-rainbow: linear-gradient(90deg, #FF0000, #FF8800, #FFD600, #00C853, #2979FF, #AA00FF, #8B00FF);
      --kid-radius: 20px;
      --kid-radius-lg: 30px;
      --kid-radius-pill: 999px;
      --kid-outline: 3px;
      --kid-shadow-offset: 5px;
    }

    /* --- Reset & Base --- */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Patrick Hand', 'Comic Sans MS', 'Segoe Print', cursive;
      font-size: 18px;
      line-height: 1.7;
      color: var(--kid-black);
      background-color: var(--kid-white);
    }

    /* --- Typography --- */
    h1, h2, h3, h4 {
      font-family: 'Bubblegum Sans', 'Comic Sans MS', cursive;
      line-height: 1.2;
    }

    h2 {
      font-family: 'Fredoka', cursive;
      font-weight: 700;
    }

    h3 {
      font-family: 'Fredoka', cursive;
      font-weight: 600;
    }

    a {
      color: var(--kid-blue);
      text-decoration: underline wavy;
      text-underline-offset: 4px;
      transition: color 0.2s;
    }

    a:hover {
      color: var(--kid-pink);
    }

    /* --- Navigation --- */
    .nav {
      background-color: var(--kid-yellow);
      border-bottom: var(--kid-outline) solid var(--kid-black);
      padding: 0.75rem 1.5rem;
      position: relative;
      z-index: 100;
    }

    .nav::after {
      content: '';
      position: absolute;
      bottom: -8px;
      left: 0;
      right: 0;
      height: 5px;
      background: var(--kid-rainbow);
    }

    .nav-inner {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 0.5rem;
    }

    .nav .logo {
      font-family: 'Bubblegum Sans', cursive;
      font-size: 1.6rem;
      color: var(--kid-black);
      text-decoration: none;
      margin-right: auto;
      text-shadow: 2px 2px 0 var(--kid-pink);
    }

    .nav .logo:hover { text-shadow: 2px 2px 0 var(--kid-cyan); }

    .nav ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 0.25rem;
    }

    .nav ul a {
      display: block;
      padding: 0.4rem 1rem;
      font-family: 'Fredoka', cursive;
      font-weight: 600;
      font-size: 1rem;
      color: var(--kid-black);
      text-decoration: none;
      border-radius: var(--kid-radius-pill);
      border: 2px solid transparent;
      transition: background-color 0.2s, border-color 0.2s;
    }

    .nav ul a:hover {
      background-color: var(--kid-white);
      border-color: var(--kid-black);
    }

    /* --- Hero --- */
    .hero {
      min-height: 85vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 4rem 2rem;
      background-color: var(--kid-cyan);
      background-image:
        radial-gradient(circle, rgba(255,254,245,0.5) 2px, transparent 2px);
      background-size: 32px 32px;
      border-bottom: var(--kid-outline) solid var(--kid-black);
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-size: clamp(2.8rem, 9vw, 6.5rem);
      color: var(--kid-black);
      text-shadow:
        4px 4px 0 var(--kid-yellow),
        -2px -2px 0 var(--kid-pink);
      position: relative;
      z-index: 2;
    }

    .hero .subtitle {
      font-family: 'Patrick Hand', cursive;
      font-size: clamp(1.1rem, 2.5vw, 1.5rem);
      max-width: 50ch;
      margin-top: 1.5rem;
      background: rgba(255,254,245,0.88);
      padding: 1rem 2rem;
      border-radius: var(--kid-radius);
      border: 2px solid var(--kid-black);
      position: relative;
      z-index: 2;
    }

    .hero .btn-row {
      margin-top: 2rem;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
      position: relative;
      z-index: 2;
    }

    /* Floating decorations */
    .deco {
      position: absolute;
      font-size: 2.5rem;
      z-index: 1;
      filter: drop-shadow(2px 2px 0 var(--kid-black));
      animation: float 4s ease-in-out infinite;
    }

    .deco:nth-child(1) { top: 12%; left: 8%; animation-delay: 0s; }
    .deco:nth-child(2) { top: 20%; right: 10%; animation-delay: 0.8s; font-size: 3rem; }
    .deco:nth-child(3) { bottom: 18%; left: 12%; animation-delay: 1.5s; }
    .deco:nth-child(4) { bottom: 25%; right: 8%; animation-delay: 2.2s; font-size: 2rem; }
    .deco:nth-child(5) { top: 45%; left: 3%; animation-delay: 0.5s; font-size: 2rem; }
    .deco:nth-child(6) { top: 55%; right: 4%; animation-delay: 1.8s; }

    @keyframes float {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      50% { transform: translateY(-12px) rotate(8deg); }
    }

    /* --- Buttons --- */
    .btn {
      display: inline-block;
      font-family: 'Fredoka', cursive;
      font-size: 1.1rem;
      font-weight: 600;
      padding: 0.8rem 2rem;
      border: var(--kid-outline) solid var(--kid-black);
      border-radius: var(--kid-radius-pill);
      cursor: pointer;
      text-decoration: none;
      text-align: center;
      box-shadow: 4px 4px 0 var(--kid-black);
      transition: transform 0.15s ease, box-shadow 0.15s ease;
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 6px 6px 0 var(--kid-black);
      text-decoration: none;
    }

    .btn:active {
      transform: translateY(3px);
      box-shadow: 1px 1px 0 var(--kid-black);
    }

    .btn--red { background-color: var(--kid-red); color: var(--kid-white); }
    .btn--blue { background-color: var(--kid-blue); color: var(--kid-white); }
    .btn--green { background-color: var(--kid-green); color: var(--kid-black); }
    .btn--pink { background-color: var(--kid-pink); color: var(--kid-black); }
    .btn--yellow { background-color: var(--kid-yellow); color: var(--kid-black); }
    .btn--outline { background-color: var(--kid-white); color: var(--kid-black); }

    /* --- Rainbow Divider --- */
    .rainbow-divider {
      height: 8px;
      border: none;
      background: var(--kid-rainbow);
      border-top: 2px solid var(--kid-black);
      border-bottom: 2px solid var(--kid-black);
      margin: 0;
    }

    /* --- Section --- */
    .section {
      padding: 4rem 2rem;
      border-bottom: var(--kid-outline) solid var(--kid-black);
    }

    .section-inner {
      max-width: 1100px;
      margin: 0 auto;
    }

    .section h2 {
      font-size: clamp(1.8rem, 4vw, 3rem);
      margin-bottom: 0.5rem;
      text-shadow: 3px 3px 0 var(--kid-yellow);
    }

    .section .lead {
      font-size: 1.1rem;
      max-width: 60ch;
      margin-bottom: 2rem;
    }

    /* --- Card Grid --- */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 1.5rem;
    }

    .card {
      background-color: var(--kid-white);
      border: var(--kid-outline) solid var(--kid-black);
      border-radius: var(--kid-radius);
      padding: 1.5rem;
      box-shadow: 5px 5px 0 var(--kid-pink);
      transition: transform 0.2s ease, box-shadow 0.2s ease;
      position: relative;
    }

    .card:nth-child(2) { box-shadow: 5px 5px 0 var(--kid-blue); }
    .card:nth-child(3) { box-shadow: 5px 5px 0 var(--kid-green); }
    .card:nth-child(4) { box-shadow: 5px 5px 0 var(--kid-orange); }
    .card:nth-child(5) { box-shadow: 5px 5px 0 var(--kid-purple); }
    .card:nth-child(6) { box-shadow: 5px 5px 0 var(--kid-cyan); }

    .card:hover {
      transform: translateY(-5px) rotate(-1deg);
    }

    .card .card-icon {
      font-size: 2.5rem;
      margin-bottom: 0.75rem;
    }

    .card h3 {
      font-size: 1.3rem;
      margin-bottom: 0.5rem;
      color: var(--kid-blue);
    }

    .card p {
      font-size: 0.95rem;
      line-height: 1.6;
      margin-bottom: 1rem;
    }

    .sticker {
      display: inline-block;
      font-family: 'Fredoka', cursive;
      font-weight: 600;
      font-size: 0.75rem;
      padding: 0.2rem 0.7rem;
      border: 2px solid var(--kid-black);
      border-radius: var(--kid-radius-pill);
      margin-right: 0.3rem;
      margin-bottom: 0.3rem;
    }

    .sticker--red { background-color: var(--kid-red); color: var(--kid-white); }
    .sticker--blue { background-color: var(--kid-blue); color: var(--kid-white); }
    .sticker--green { background-color: var(--kid-green); color: var(--kid-black); }
    .sticker--yellow { background-color: var(--kid-yellow); color: var(--kid-black); }
    .sticker--pink { background-color: var(--kid-pink); color: var(--kid-black); }
    .sticker--purple { background-color: var(--kid-purple); color: var(--kid-white); }
    .sticker--orange { background-color: var(--kid-orange); color: var(--kid-black); }

    /* --- Checkerboard Section --- */
    .checker-section {
      padding: 4rem 2rem;
      background-color: var(--kid-white);
      background-image:
        linear-gradient(45deg, var(--kid-lime) 25%, transparent 25%),
        linear-gradient(-45deg, var(--kid-lime) 25%, transparent 25%),
        linear-gradient(45deg, transparent 75%, var(--kid-lime) 75%),
        linear-gradient(-45deg, transparent 75%, var(--kid-lime) 75%);
      background-size: 40px 40px;
      background-position: 0 0, 0 20px, 20px -20px, -20px 0;
      border-bottom: var(--kid-outline) solid var(--kid-black);
    }

    .checker-section .content-box {
      max-width: 750px;
      margin: 0 auto;
      background: var(--kid-white);
      border: var(--kid-outline) solid var(--kid-black);
      border-radius: var(--kid-radius-lg);
      padding: 2.5rem;
      box-shadow: 6px 6px 0 var(--kid-black);
      text-align: center;
    }

    .checker-section .content-box h2 {
      text-shadow: 3px 3px 0 var(--kid-pink);
    }

    /* --- Feature Strips --- */
    .feature-strip {
      padding: 3rem 2rem;
      border-bottom: var(--kid-outline) solid var(--kid-black);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 2rem;
    }

    .feature-strip .strip-inner {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 2rem;
      width: 100%;
    }

    .feature-strip:nth-child(odd) { background-color: var(--kid-cotton-candy); }
    .feature-strip:nth-child(even) { background-color: #E1F5FE; }

    .feature-strip .icon-circle {
      width: 90px;
      height: 90px;
      border-radius: 50%;
      border: var(--kid-outline) solid var(--kid-black);
      background-color: var(--kid-yellow);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2.2rem;
      flex-shrink: 0;
      box-shadow: 4px 4px 0 var(--kid-black);
    }

    .feature-strip .feature-text { flex: 1; min-width: 200px; }
    .feature-strip .feature-text h3 { font-size: 1.4rem; margin-bottom: 0.4rem; }

    /* --- Testimonials --- */
    .testimonial-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 1.5rem;
    }

    .testimonial {
      background-color: var(--kid-cotton-candy);
      border: var(--kid-outline) solid var(--kid-black);
      border-radius: var(--kid-radius);
      padding: 1.5rem;
      box-shadow: 4px 4px 0 var(--kid-red);
      position: relative;
    }

    .testimonial:nth-child(2) {
      background-color: #E1F5FE;
      box-shadow: 4px 4px 0 var(--kid-blue);
    }

    .testimonial:nth-child(3) {
      background-color: #F1F8E9;
      box-shadow: 4px 4px 0 var(--kid-green);
    }

    .testimonial .stars {
      font-size: 1.3rem;
      margin-bottom: 0.5rem;
      letter-spacing: 2px;
    }

    .testimonial p {
      font-size: 1rem;
      line-height: 1.6;
      margin-bottom: 0.75rem;
    }

    .testimonial .author {
      font-family: 'Fredoka', cursive;
      font-weight: 600;
      font-size: 0.9rem;
      color: var(--kid-purple);
    }

    /* --- Footer --- */
    .footer {
      background-color: var(--kid-royal-blue);
      color: var(--kid-white);
      padding: 3rem 2rem;
      position: relative;
    }

    .footer::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 8px;
      background: var(--kid-rainbow);
    }

    .footer-inner {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
      justify-content: space-between;
    }

    .footer h4 {
      font-family: 'Bubblegum Sans', cursive;
      font-size: 1.3rem;
      margin-bottom: 0.75rem;
      color: var(--kid-yellow);
    }

    .footer ul {
      list-style: none;
    }

    .footer ul li { margin-bottom: 0.4rem; }

    .footer a {
      color: var(--kid-white);
      text-decoration: none;
      text-underline-offset: 3px;
    }

    .footer a:hover {
      text-decoration: underline wavy;
      color: var(--kid-yellow);
    }

    .footer .copyright {
      width: 100%;
      text-align: center;
      margin-top: 2rem;
      padding-top: 1.5rem;
      border-top: 2px solid rgba(255,255,255,0.2);
      font-size: 0.9rem;
    }

    /* --- Utilities --- */
    .text-center { text-align: center; }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      .hero { min-height: 70vh; padding: 3rem 1.5rem; }
      .hero h1 { font-size: clamp(2.2rem, 10vw, 4rem); }
      .deco { font-size: 1.8rem !important; }
      .section { padding: 3rem 1.5rem; }
      .feature-strip .strip-inner { flex-direction: column; text-align: center; }
      .feature-strip .icon-circle { margin: 0 auto; }
      .footer-inner { flex-direction: column; }
    }

    @media (max-width: 480px) {
      .nav-inner { justify-content: center; }
      .nav .logo { margin-right: 0; width: 100%; text-align: center; }
      .nav ul { justify-content: center; }
      .hero { min-height: 60vh; }
      .card-grid { grid-template-columns: 1fr; }
      .testimonial-grid { grid-template-columns: 1fr; }
      .btn { width: 100%; }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="nav">
    <div class="nav-inner">
      <a href="#" class="logo">Playtown Studio</a>
      <ul>
        <li><a href="#services">Services</a></li>
        <li><a href="#work">Our Work</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#reviews">Reviews</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </nav>

  <!-- HERO -->
  <section class="hero">
    <span class="deco">&#11088;</span>
    <span class="deco">&#127752;</span>
    <span class="deco">&#10084;&#65039;</span>
    <span class="deco">&#127775;</span>
    <span class="deco">&#9728;&#65039;</span>
    <span class="deco">&#127848;</span>
    <h1>Where Creativity Comes to Play!</h1>
    <p class="subtitle">
      We are Playtown Creative Studio, a design team that believes the best ideas come from play.
      We build brands, websites, and campaigns bursting with color, joy, and unapologetic fun.
    </p>
    <div class="btn-row">
      <a href="#work" class="btn btn--red">See Our Work</a>
      <a href="#contact" class="btn btn--outline">Say Hello</a>
    </div>
  </section>

  <!-- RAINBOW DIVIDER -->
  <hr class="rainbow-divider">

  <!-- SERVICES -->
  <section class="section" id="services" style="background-color: #FFF9C4;">
    <div class="section-inner">
      <h2>What We Do</h2>
      <p class="lead">
        From brand identities to full-blown digital playgrounds, we bring bold ideas to life
        with the energy of a Saturday morning cartoon marathon.
      </p>
      <div class="card-grid">
        <div class="card">
          <div class="card-icon">&#127912;</div>
          <h3>Brand Identity</h3>
          <p>Logos, color systems, and visual guidelines that make your brand impossible to ignore. We craft identities that pop off the shelf and stick in memory.</p>
          <span class="sticker sticker--red">Logos</span>
          <span class="sticker sticker--blue">Guidelines</span>
          <span class="sticker sticker--yellow">Color</span>
        </div>
        <div class="card">
          <div class="card-icon">&#128187;</div>
          <h3>Web Design</h3>
          <p>Websites that feel like an adventure. We build responsive, accessible sites with personality to spare, designed to delight every visitor who lands on the page.</p>
          <span class="sticker sticker--green">Responsive</span>
          <span class="sticker sticker--pink">Interactive</span>
        </div>
        <div class="card">
          <div class="card-icon">&#128247;</div>
          <h3>Social Media</h3>
          <p>Scroll-stopping content for every platform. We design posts, stories, and campaigns that bring your feed to life with color-drenched, thumb-pausing visuals.</p>
          <span class="sticker sticker--purple">Campaigns</span>
          <span class="sticker sticker--orange">Content</span>
        </div>
        <div class="card">
          <div class="card-icon">&#127880;</div>
          <h3>Event Design</h3>
          <p>From launch parties to trade shows, we design physical and digital event experiences that transform spaces into immersive, playful brand environments.</p>
          <span class="sticker sticker--yellow">Spaces</span>
          <span class="sticker sticker--red">Immersive</span>
        </div>
        <div class="card">
          <div class="card-icon">&#128230;</div>
          <h3>Packaging</h3>
          <p>Product packaging that kids and adults alike want to keep. We design boxes, labels, and unboxing experiences that turn products into collectible moments.</p>
          <span class="sticker sticker--blue">Unboxing</span>
          <span class="sticker sticker--green">Shelf Impact</span>
        </div>
        <div class="card">
          <div class="card-icon">&#127916;</div>
          <h3>Motion Graphics</h3>
          <p>Animated logos, explainer videos, and social media motion content that brings your brand to life with bouncy, energetic movement and vivid color.</p>
          <span class="sticker sticker--pink">Animation</span>
          <span class="sticker sticker--purple">Video</span>
        </div>
      </div>
    </div>
  </section>

  <hr class="rainbow-divider">

  <!-- CHECKERBOARD ABOUT SECTION -->
  <section class="checker-section" id="about">
    <div class="content-box">
      <h2>About Our Studio</h2>
      <p style="margin-top: 1rem;">
        Founded in 2019 by a team of designers who never outgrew their love for bold colors and
        Saturday morning cartoons, Playtown Creative Studio operates from a paint-splattered
        warehouse in Portland filled with vintage toys and an irresponsible number of marker sets.
        We believe design should spark joy first and ask questions later. Our clients range from
        indie toy companies to major snack brands, and every project gets the same treatment:
        maximum color, maximum fun, zero corporate boredom.
      </p>
      <div style="margin-top: 1.5rem; display: flex; flex-wrap: wrap; gap: 0.5rem; justify-content: center;">
        <span class="sticker sticker--red">Portland, OR</span>
        <span class="sticker sticker--blue">Est. 2019</span>
        <span class="sticker sticker--green">12 Creatives</span>
        <span class="sticker sticker--yellow">200+ Projects</span>
        <span class="sticker sticker--purple">100% Fun</span>
      </div>
    </div>
  </section>

  <hr class="rainbow-divider">

  <!-- FEATURED WORK -->
  <section class="section" id="work">
    <div class="section-inner">
      <h2>Featured Work</h2>
      <p class="lead">A handful of projects we are especially proud of. Each one started as play and ended as something wonderful.</p>
    </div>
    <div class="feature-strip" style="background-color: var(--kid-cotton-candy);">
      <div class="strip-inner">
        <div class="icon-circle">&#127850;</div>
        <div class="feature-text">
          <h3>SugarPop Candy Rebrand</h3>
          <p>Complete visual overhaul for a gummy candy company, including new packaging, a bubbly wordmark, and a social campaign that boosted their Instagram following by 340% in three months.</p>
        </div>
      </div>
    </div>
    <div class="feature-strip" style="background-color: #E1F5FE;">
      <div class="strip-inner">
        <div class="icon-circle" style="background-color: var(--kid-cyan);">&#128302;</div>
        <div class="feature-text">
          <h3>WonderBox Subscription Service</h3>
          <p>Brand identity and e-commerce website for a monthly kids' activity box. We designed the full unboxing experience from outer carton to tissue paper to the collectible sticker sheet inside.</p>
        </div>
      </div>
    </div>
    <div class="feature-strip" style="background-color: #F1F8E9;">
      <div class="strip-inner">
        <div class="icon-circle" style="background-color: var(--kid-lime);">&#127922;</div>
        <div class="feature-text">
          <h3>TinyTown Board Game Launch</h3>
          <p>Complete go-to-market design for an indie board game, including box art, rule book illustration, Kickstarter page design, and animated social teasers that helped the campaign fund in under 48 hours.</p>
        </div>
      </div>
    </div>
  </section>

  <hr class="rainbow-divider">

  <!-- TESTIMONIALS -->
  <section class="section" id="reviews" style="background-color: #FFF3E0;">
    <div class="section-inner">
      <h2>Kind Words</h2>
      <p class="lead">What our clients say about working with us.</p>
      <div class="testimonial-grid">
        <div class="testimonial">
          <div class="stars">&#11088;&#11088;&#11088;&#11088;&#11088;</div>
          <p>"Playtown completely transformed our brand. Our packaging went from forgettable to the kind of thing kids refuse to throw away. Sales jumped 28% in the first quarter after launch."</p>
          <div class="author">-- Jamie Chen, CEO of SugarPop</div>
        </div>
        <div class="testimonial">
          <div class="stars">&#11088;&#11088;&#11088;&#11088;&#11088;</div>
          <p>"They made our Kickstarter page look like a theme park. We funded in two days and backers kept telling us the page itself was half the reason they pledged. Incredible team."</p>
          <div class="author">-- Priya Sharma, TinyTown Games</div>
        </div>
        <div class="testimonial">
          <div class="stars">&#11088;&#11088;&#11088;&#11088;&#11088;</div>
          <p>"Working with Playtown felt like recess. They brought so much energy and creativity to every meeting. The final website is the most fun thing on the internet, and our subscribers agree."</p>
          <div class="author">-- Marcus Li, Founder of WonderBox</div>
        </div>
      </div>
    </div>
  </section>

  <hr class="rainbow-divider">

  <!-- CONTACT CTA -->
  <section class="checker-section" id="contact">
    <div class="content-box">
      <h2>Let's Make Something Fun!</h2>
      <p style="margin-top: 1rem; margin-bottom: 1.5rem;">
        Got a project that needs more color, more energy, more joy? We would love to hear about it.
        Drop us a line and let's turn your next big idea into a playground.
      </p>
      <div style="display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center;">
        <a href="mailto:hello@playtownstudio.com" class="btn btn--pink">Email Us</a>
        <a href="#" class="btn btn--blue">Book a Call</a>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="footer">
    <div class="footer-inner">
      <div>
        <h4>Playtown Studio</h4>
        <p>Creative design for brands<br>that refuse to be boring.</p>
      </div>
      <div>
        <h4>Services</h4>
        <ul>
          <li><a href="#">Brand Identity</a></li>
          <li><a href="#">Web Design</a></li>
          <li><a href="#">Social Media</a></li>
          <li><a href="#">Packaging</a></li>
        </ul>
      </div>
      <div>
        <h4>Connect</h4>
        <ul>
          <li><a href="#">Instagram</a></li>
          <li><a href="#">Dribbble</a></li>
          <li><a href="#">TikTok</a></li>
          <li><a href="#">LinkedIn</a></li>
        </ul>
      </div>
      <div>
        <h4>Studio</h4>
        <ul>
          <li><a href="#">About Us</a></li>
          <li><a href="#">Careers</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Press Kit</a></li>
        </ul>
      </div>
      <div class="copyright">
        Made with &#10084;&#65039; and way too many stickers by Playtown Creative Studio.
      </div>
    </div>
  </footer>

</body>
</html>
```
