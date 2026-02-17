# Superflat Pop

A commercial graphic design aesthetic prevalent from the late 2000s to the early 2010s, derived from Takashi Murakami's Superflat fine art movement. Superflat Pop strips away the subversive and disturbing undertones of the original movement, retaining its vibrant colors, bold outlines, flat dimensionality, and kawaii sensibility for mass-market appeal. The style fuses Japanese pop culture imagery -- anime characters, kawaii mascots, "sweet and sunny" florals -- with Western pop art, graffiti, and toy culture. It appears across animation, video games, advertising, fashion, and product design, sharing DNA with Y2K Futurism, McBling, Frutiger Aero, and Vectordelia but distinguished by its emphasis on kawaii motifs and deliberate visual flatness.

---

## Color Palette

### Core Principles

- **Vibrant rainbow spectrum** -- the default palette spans the full rainbow, rendered in either high-saturation neon or soft pastel variants depending on context
- **Flat, solid color fills** -- colors are applied as uniform, unmodulated fields with no shading, no gradients within shapes, and no naturalistic modeling
- **High chroma** -- every hue is pushed toward maximum saturation; nothing is muted, dusty, or desaturated
- **White or pale backgrounds** -- compositions sit on clean white or near-white grounds to maximize the luminosity and pop of the colored elements

### Primary Neon Palette

| Color | Hex | Role |
|-------|-----|------|
| **Hot Pink** | `#FF4DA6` | Primary accent, character highlights, floral petals |
| **Electric Yellow** | `#FFE500` | Cheerful accents, sunburst backgrounds, petal fills |
| **Vivid Cyan** | `#00D4FF` | Cool contrast accent, secondary fills, sky elements |
| **Lime Green** | `#7FFF00` | Organic accents, character details, leaf fills |
| **Tangerine Orange** | `#FF6B2B` | Warm accent, energetic highlights |
| **Violet** | `#9B30FF` | Playful contrast, secondary character fills |
| **Cherry Red** | `#FF1744` | Bold emphasis, lips, hearts, graphic elements |

### Pastel Variant Palette

| Color | Hex | Role |
|-------|-----|------|
| **Pastel Pink** | `#FFB3D9` | Soft backgrounds, kawaii character fills |
| **Pastel Yellow** | `#FFF59D` | Gentle accents, petal highlights |
| **Pastel Blue** | `#81D4FA` | Cool backgrounds, sky fills |
| **Pastel Green** | `#B9F6CA` | Organic accents, leaf fills |
| **Pastel Lavender** | `#CE93D8` | Whimsical accents, secondary fills |
| **Pastel Peach** | `#FFCCBC` | Warm accents, character skin tones |

### Neutral and Background Colors

| Color | Hex | Role |
|-------|-----|------|
| **Pure White** | `#FFFFFF` | Primary background, negative space |
| **Soft White** | `#FAFAFA` | Subtle background variation |
| **Black** | `#000000` | Bold outlines, high-contrast text |
| **Soft Black** | `#222222` | Outline alternative, body text |

### CSS Custom Properties

```css
:root {
  /* Neon primaries */
  --sfp-hot-pink:       #FF4DA6;
  --sfp-yellow:         #FFE500;
  --sfp-cyan:           #00D4FF;
  --sfp-lime:           #7FFF00;
  --sfp-orange:         #FF6B2B;
  --sfp-violet:         #9B30FF;
  --sfp-red:            #FF1744;

  /* Pastel variants */
  --sfp-pastel-pink:    #FFB3D9;
  --sfp-pastel-yellow:  #FFF59D;
  --sfp-pastel-blue:    #81D4FA;
  --sfp-pastel-green:   #B9F6CA;
  --sfp-pastel-lavender:#CE93D8;
  --sfp-pastel-peach:   #FFCCBC;

  /* Backgrounds */
  --sfp-white:          #FFFFFF;
  --sfp-soft-white:     #FAFAFA;

  /* Outlines and text */
  --sfp-black:          #000000;
  --sfp-soft-black:     #222222;

  /* Functional aliases */
  --sfp-bg-primary:     var(--sfp-white);
  --sfp-bg-secondary:   var(--sfp-soft-white);
  --sfp-text-primary:   var(--sfp-soft-black);
  --sfp-accent:         var(--sfp-hot-pink);
  --sfp-outline:        var(--sfp-black);
}
```

### Color Usage Guidelines

- **Use the full rainbow** -- unlike minimal palettes, Superflat Pop encourages using many colors simultaneously; 5-7 hues in a single composition is normal
- **Flat fills only** -- no gradients within individual shapes; each shape is a single solid color
- **Bold outline contrast** -- black outlines at 2-4px weight separate color fields and define all shapes
- **Background stays clean** -- white or very pale background lets the saturated elements do the visual work
- **Mix neon and pastel** -- within a single composition, some elements can be neon while others are pastel, creating depth through color temperature rather than shading
- **Avoid** -- earth tones, muted colors, natural/organic palettes, monochromatic schemes, gradient fills

---

## Typography

### Font Characteristics

- **Rounded, bubbly letterforms** -- the defining typographic trait; every letter has soft, inflated, friendly curves with no sharp terminals
- **Bold to ultra-bold weights** -- heavy, chunky type that feels solid and playful
- **Soft terminals** -- stroke endings are rounded, never flat-cut or bracketed
- **Clean and legible** -- despite the playfulness, type remains highly readable
- **No serifs, no sharp geometry** -- strictly rounded sans-serif faces that mirror the kawaii softness of the illustrations

### Specific Typefaces (Period-Authentic)

| Font | Notes |
|------|-------|
| **VAG Rounded** | The quintessential Superflat Pop typeface; originally designed for Volkswagen, widely adopted in this era for its perfectly rounded geometry |
| **Roundhouse** (House Industries) | Display font with exaggerated roundness and retro-futuristic character |
| **Billo** (Fontalicious) | Free rounded display font with a chunky, toy-like quality |

### Recommended Web Fonts (Google Fonts)

| Role | Fonts |
|------|-------|
| **Display / Headings** | `Fredoka One`, `Baloo 2` (700-800), `Bubblegum Sans` |
| **Rounded Sans-Serif** | `Nunito` (700-900), `Varela Round`, `M PLUS Rounded 1c` (700-900) |
| **Body Text** | `Nunito` (400-600), `Quicksand` (500-600), `M PLUS Rounded 1c` (400-500) |
| **Playful Display** | `Boogaloo`, `Luckiest Guy`, `Lilita One` |

### CSS Typography Example

```css
@import url('https://fonts.googleapis.com/css2?family=Fredoka+One&family=Nunito:wght@400;600;700;800;900&family=Varela+Round&display=swap');

h1, h2, h3, h4, h5, h6 {
  font-family: 'Fredoka One', 'Nunito', 'VAG Rounded', sans-serif;
  font-weight: 700;
  color: var(--sfp-soft-black);
  line-height: 1.2;
  letter-spacing: 0.01em;
}

/* Hero / display headings */
.sfp-display {
  font-family: 'Fredoka One', sans-serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  color: var(--sfp-hot-pink);
  -webkit-text-stroke: 2px var(--sfp-black);
  paint-order: stroke fill;
  line-height: 1.1;
  letter-spacing: 0.02em;
}

body {
  font-family: 'Nunito', 'Varela Round', 'VAG Rounded', sans-serif;
  font-weight: 600;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--sfp-text-primary);
}

/* Bold rainbow text effect */
.sfp-rainbow-text {
  background: linear-gradient(
    90deg,
    var(--sfp-red),
    var(--sfp-orange),
    var(--sfp-yellow),
    var(--sfp-lime),
    var(--sfp-cyan),
    var(--sfp-violet),
    var(--sfp-hot-pink)
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  font-weight: 900;
}
```

---

## Key Design Elements and Motifs

### Defining Visual Motifs

- **Bold black outlines** -- the signature Superflat Pop device; every shape, character, and element is defined by strong, uniform-weight outlines (typically black, occasionally colored). Outlines are clean and vector-sharp, never sketchy or hand-drawn
- **"Sweet and Sunny" flowers** -- stylized, simplified floral forms with perfectly round petals, bold outlines, and flat saturated fills. Often feature a kawaii smiley face in the center. Directly inspired by Murakami's iconic flower motifs
- **Kawaii faces** -- simple dot eyes and tiny curved mouths applied to characters, objects, flowers, and abstract shapes. Blush cheek circles are common
- **Geometric shapes** -- circles, ovals, rounded rectangles, and simple polygons used as compositional building blocks; always with rounded corners and bold outlines
- **Urban vinyl / toy figures** -- character designs that look like they could be molded as collectible vinyl toys; rounded, simplified, 3D-implied forms rendered flat
- **Graffiti elements** -- drips, tags, and spray-paint motifs integrated as decorative accents, connecting to street art and urban culture
- **Anime/otaku references** -- large-eyed characters, exaggerated proportions, and visual language borrowed from Japanese animation and manga
- **Rainbow color blocking** -- sections or elements filled with rainbow-ordered color sequences as both decoration and structural device

### Murakami Flower Pattern (CSS)

```css
/* Simplified Murakami-inspired flower using radial gradients */
.sfp-flower {
  width: 120px;
  height: 120px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}

.sfp-flower::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(circle at 50% 15%, var(--sfp-hot-pink) 18%, transparent 19%),
    radial-gradient(circle at 83% 35%, var(--sfp-yellow) 18%, transparent 19%),
    radial-gradient(circle at 83% 70%, var(--sfp-cyan) 18%, transparent 19%),
    radial-gradient(circle at 50% 88%, var(--sfp-lime) 18%, transparent 19%),
    radial-gradient(circle at 17% 70%, var(--sfp-orange) 18%, transparent 19%),
    radial-gradient(circle at 17% 35%, var(--sfp-violet) 18%, transparent 19%);
}

.sfp-flower::after {
  content: '\263A';  /* smiley face */
  font-size: 2rem;
  z-index: 1;
  color: var(--sfp-soft-black);
}

/* Bold outline ring overlay */
.sfp-outline-ring {
  border: 3px solid var(--sfp-black);
  border-radius: 50%;
}
```

### Decorative CSS Patterns

```css
/* Polka dot pattern (toylike, playful) */
.sfp-polka-dots {
  background-image:
    radial-gradient(circle, var(--sfp-hot-pink) 8px, transparent 8px),
    radial-gradient(circle, var(--sfp-yellow) 8px, transparent 8px);
  background-size: 48px 48px;
  background-position: 0 0, 24px 24px;
  background-color: var(--sfp-white);
}

/* Rainbow stripe accent bar */
.sfp-rainbow-bar {
  height: 8px;
  background: linear-gradient(
    90deg,
    var(--sfp-red) 0%,
    var(--sfp-orange) 14%,
    var(--sfp-yellow) 28%,
    var(--sfp-lime) 42%,
    var(--sfp-cyan) 57%,
    var(--sfp-violet) 71%,
    var(--sfp-hot-pink) 85%,
    var(--sfp-red) 100%
  );
  border-radius: 4px;
}

/* Kawaii face applied to any container */
.sfp-kawaii-face {
  position: relative;
}

.sfp-kawaii-face::after {
  content: '\2022  \2022';  /* dot eyes */
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translateX(-50%);
  font-size: 1.2rem;
  letter-spacing: 0.8em;
  color: var(--sfp-black);
}
```

---

## Composition and Layout Principles

### Core Layout Traits

- **Clean, open compositions** -- unlike the maximalist density of Colorful Pop, Superflat Pop uses generous white space to let each element pop against the background
- **Flat dimensionality** -- all elements exist on the same visual plane; no drop shadows, no depth simulation, no perspective. The flatness is the point
- **Bold outlined containers** -- cards, sections, and interactive elements are defined by thick black outlines (2-4px) rather than shadows or subtle borders
- **Centered and symmetrical** -- compositions tend toward balanced, centered arrangements that feel designed and intentional
- **Grid-based but playful** -- underlying grid structure with elements occasionally breaking alignment for energy and fun
- **Character integration** -- mascot characters and kawaii illustrations are embedded naturally within the layout, not isolated in image blocks

### Grid and Spacing

```css
.sfp-layout {
  max-width: 1100px;
  margin: 0 auto;
  padding: 3rem 2rem;
}

.sfp-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

/* Outlined card -- the core Superflat Pop container */
.sfp-card {
  background: var(--sfp-white);
  border: 3px solid var(--sfp-black);
  border-radius: 16px;
  padding: 2rem;
  position: relative;
  transition: transform 0.2s ease;
}

.sfp-card:hover {
  transform: translateY(-3px) rotate(-0.5deg);
}

/* Colored card variant */
.sfp-card--pink {
  background: var(--sfp-pastel-pink);
}

.sfp-card--yellow {
  background: var(--sfp-pastel-yellow);
}

.sfp-card--blue {
  background: var(--sfp-pastel-blue);
}
```

### Hero Section

```css
.sfp-hero {
  text-align: center;
  padding: 5rem 2rem;
  background: var(--sfp-white);
  position: relative;
  overflow: hidden;
}

.sfp-hero h1 {
  font-family: 'Fredoka One', sans-serif;
  font-size: clamp(3rem, 7vw, 5.5rem);
  color: var(--sfp-hot-pink);
  -webkit-text-stroke: 3px var(--sfp-black);
  paint-order: stroke fill;
  margin-bottom: 1rem;
  position: relative;
  z-index: 1;
}

.sfp-hero p {
  font-family: 'Nunito', sans-serif;
  font-size: 1.25rem;
  font-weight: 600;
  color: var(--sfp-soft-black);
  max-width: 600px;
  margin: 0 auto 2rem;
  position: relative;
  z-index: 1;
}

/* Decorative background circles */
.sfp-hero::before,
.sfp-hero::after {
  content: '';
  position: absolute;
  border-radius: 50%;
  border: 3px solid var(--sfp-black);
}

.sfp-hero::before {
  width: 200px;
  height: 200px;
  background: var(--sfp-pastel-yellow);
  top: -60px;
  right: -40px;
}

.sfp-hero::after {
  width: 150px;
  height: 150px;
  background: var(--sfp-pastel-blue);
  bottom: -40px;
  left: -30px;
}
```

### Section Color Blocking

```css
.sfp-section {
  padding: 4rem 0;
  position: relative;
}

.sfp-section--white {
  background: var(--sfp-white);
}

.sfp-section--pink {
  background: var(--sfp-pastel-pink);
}

.sfp-section--yellow {
  background: var(--sfp-pastel-yellow);
}

.sfp-section--blue {
  background: var(--sfp-pastel-blue);
}

/* Bold divider between sections */
.sfp-section + .sfp-section {
  border-top: 3px solid var(--sfp-black);
}
```

---

## Textures and Surface Effects

### Surface Treatment Principles

- **Completely flat** -- no textures, no noise, no paper grain. Surfaces are smooth, uniform, digital-clean
- **No shadows** -- strictly no drop shadows, box shadows, or any depth simulation. This is a defining rule
- **No gradients within shapes** -- each shape is one solid color. Gradients are only acceptable as rainbow accent bars or background washes at section scale
- **Bold outlines replace shadows** -- where other aesthetics use shadows for separation and hierarchy, Superflat Pop uses thick black outlines
- **Matte, not glossy** -- surfaces read as flat and opaque, not reflective or translucent
- **Sticker / vinyl quality** -- elements feel like flat vinyl stickers or screen-printed graphics applied to a surface

### CSS Surface Techniques

```css
/* Bold-outlined element (core technique replacing shadows) */
.sfp-outlined {
  border: 3px solid var(--sfp-black);
  border-radius: 12px;
  box-shadow: none;
  background: var(--sfp-white);
}

/* Pop-out effect using offset border (no shadow) */
.sfp-pop-out {
  border: 3px solid var(--sfp-black);
  border-radius: 12px;
  position: relative;
}

.sfp-pop-out::after {
  content: '';
  position: absolute;
  inset: 0;
  border: 3px solid var(--sfp-black);
  border-radius: 12px;
  transform: translate(4px, 4px);
  background: var(--sfp-black);
  z-index: -1;
}

/* Flat vinyl sticker feel */
.sfp-sticker {
  display: inline-block;
  background: var(--sfp-hot-pink);
  color: var(--sfp-white);
  border: 2px solid var(--sfp-black);
  border-radius: 100px;
  padding: 0.5em 1.5em;
  font-family: 'Fredoka One', sans-serif;
  font-size: 0.9rem;
}
```

---

## Animation and Motion

- **Bouncy entrances** -- elements pop in with overshoot easing, mimicking the springy feel of vinyl toys
- **Gentle hover rotations** -- cards and elements tilt slightly on hover for a playful, tactile feel
- **No aggressive motion** -- Superflat Pop is cheerful, not frenetic; animations should feel friendly and toy-like

### CSS Animation Examples

```css
/* Bouncy pop-in */
.sfp-pop-in {
  animation: sfp-bounce 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275) both;
}

@keyframes sfp-bounce {
  0% { transform: scale(0); opacity: 0; }
  60% { transform: scale(1.1); }
  100% { transform: scale(1); opacity: 1; }
}

/* Playful hover tilt */
.sfp-tilt:hover {
  transform: rotate(-2deg) scale(1.03);
  transition: transform 0.25s ease;
}

/* Slow float for decorative elements */
.sfp-float {
  animation: sfp-float 3s ease-in-out infinite;
}

@keyframes sfp-float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-8px); }
}
```

---

## CSS Techniques Summary

| Technique | CSS Property / Approach |
|-----------|------------------------|
| Bold outlines | `border: 3px solid #000` on all containers, cards, buttons, and decorative shapes |
| Flat color fills | Solid `background` color; never use gradients within individual shape fills |
| Rounded everything | `border-radius: 12px-16px` on containers; `border-radius: 50%` on circular motifs |
| No shadows at all | `box-shadow: none`; separation comes from outlines and color contrast |
| Outlined text | `-webkit-text-stroke: 2-3px #000` with `paint-order: stroke fill` for bold display type |
| Pop-out offset | Pseudo-element with `transform: translate(4px, 4px)` and black background behind outlined card |
| Rainbow gradient | `linear-gradient(90deg, ...)` with 7 rainbow stops for accent bars and text fills |
| Kawaii face details | Unicode characters or small pseudo-element dots for simple face expressions |
| Sticker tags | `border-radius: 100px` pill shape + bold outline + solid fill for badge/tag elements |
| Playful hover | `transform: rotate(-2deg) scale(1.03)` for toy-like interactive feel |
| Color blocking sections | Full-width pastel background blocks separated by `border-top: 3px solid #000` |
| Bouncy animation | `cubic-bezier(0.175, 0.885, 0.32, 1.275)` for spring overshoot entrance effects |

---

## Design Do's and Don'ts

### Do

- Use bold, uniform-weight black outlines on every element
- Fill shapes with flat, solid, highly saturated colors
- Employ the full rainbow -- many colors at once is encouraged
- Keep backgrounds white or very pale to let colors pop
- Use rounded, bubbly typography (VAG Rounded, Fredoka One, Nunito)
- Include kawaii faces, stylized flowers, and playful mascot characters
- Maintain clean, generous white space between elements
- Make everything feel like a flat vinyl sticker or screen print
- Apply rounded corners liberally (12-16px on containers, full circles on decorative shapes)

### Don't

- Use drop shadows, box shadows, or any depth simulation
- Apply gradients within individual shapes (rainbow bars at section scale are acceptable)
- Use textures, noise, paper grain, or any surface variation
- Use thin, delicate, serif, or script typefaces
- Employ muted, desaturated, or earth-tone palettes
- Create complex perspective or 3D depth (the "flat" is fundamental)
- Use photographic elements or realistic rendering
- Make compositions cluttered or dense -- this is cheerful and open, not maximalist
- Omit outlines -- the bold outline is the defining visual device

---

## Button Component

```css
.sfp-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--sfp-hot-pink);
  color: var(--sfp-white);
  border: 3px solid var(--sfp-black);
  border-radius: 100px;
  padding: 14px 36px;
  font-family: 'Fredoka One', 'Nunito', sans-serif;
  font-size: 1rem;
  cursor: pointer;
  text-decoration: none;
  position: relative;
  transition: transform 0.15s ease;
}

.sfp-button::after {
  content: '';
  position: absolute;
  inset: 0;
  border: 3px solid var(--sfp-black);
  border-radius: 100px;
  transform: translate(3px, 3px);
  background: var(--sfp-black);
  z-index: -1;
  transition: transform 0.15s ease;
}

.sfp-button:hover {
  transform: translate(-1px, -1px);
}

.sfp-button:hover::after {
  transform: translate(5px, 5px);
}

.sfp-button:active {
  transform: translate(3px, 3px);
}

.sfp-button:active::after {
  transform: translate(0, 0);
}

/* Color variants */
.sfp-button--yellow { background: var(--sfp-yellow); color: var(--sfp-black); }
.sfp-button--cyan { background: var(--sfp-cyan); color: var(--sfp-black); }
.sfp-button--lime { background: var(--sfp-lime); color: var(--sfp-black); }
```

---

## Related Aesthetics

| Aesthetic | Relationship to Superflat Pop |
|-----------|-------------------------------|
| **Superflat** | Direct parent; Murakami's fine art movement providing the visual DNA -- flat color fields, bold outlines, anime-influenced imagery. Superflat Pop is its commercially sanitized offspring |
| **Pop Art** | Foundational influence; shares bold outlines, flat color, commercial subject matter, and the blurring of high/low culture boundaries |
| **Neo-Pop** | Contemporary fine art cousin; continues Pop Art's engagement with consumer culture, overlapping in visual vocabulary |
| **Kawaii** | Core visual ingredient; the cute character design, smiley faces, and soft rounded forms that define Superflat Pop's friendliness |
| **Y2K Futurism** | Period sibling; shares the early-2000s optimism and vibrant digital palette, though Y2K leans glossy/3D where Superflat Pop stays flat |
| **McBling** | Era overlap; shares the mid-2000s commercial maximalism, bright colors, and pop culture saturation |
| **Frutiger Aero** | Contemporary counterpart; both thrived in the late 2000s, but Frutiger Aero uses glossy naturalism while Superflat Pop uses flat graphic abstraction |
| **Vectordelia** | Visual cousin; shares vector-clean outlines and vibrant palette, with Vectordelia leaning more psychedelic and pattern-heavy |
| **Avantropop** | Adjacent aesthetic blending avant-garde art with tropical pop, sharing the playful color-forward approach |
| **Colorful Pop** | Spiritual successor; takes Superflat Pop's color intensity further into maximalist, rhythm-game-influenced territory |
| **Vectorbloom** | Related floral-vector aesthetic with clean outlines and flat color, but with a more organic, botanical focus |
| **Corporate Memphis** | Later flat illustration trend; shares bold outlines and flat fills but with a more restrained, corporate-friendly palette |

---

## Notable Artists and Influences

- **Takashi Murakami** -- originator of the Superflat movement; his iconic flower motifs, Mr. DOB character, and rainbow-saturated compositions define the visual language that Superflat Pop commercializes
- **tokidoki** (Simone Legno) -- lifestyle brand embodying Superflat Pop through kawaii characters, vinyl toys, bold outlines, and rainbow palettes
- **Sanrio** -- Hello Kitty and friends represent the kawaii character design tradition that Superflat Pop absorbs
- **BAPE / A Bathing Ape** -- Japanese streetwear brand whose graphic identity (bold outlines, flat color, mascot characters) overlaps with Superflat Pop sensibility

## Media and Product References

- **Katamari Damacy** (2004, Namco) -- video game whose rainbow-colored, flat-shaded, playfully absurd visual world epitomizes Superflat Pop
- **WarioWare** series (Nintendo) -- microgame collections with bold, flat, neon-colored graphic design
- **Yo Gabba Gabba!** (2007-2015) -- children's TV show with bold outlines, flat saturated colors, vinyl-toy-inspired character design
- **Panty & Stocking with Garterbelt** (2010, Gainax) -- anime blending Superflat Pop color and flatness with UPA-revival cartoon styling
- **Summer Wars** (2009, Madhouse) -- anime film featuring digital world sequences rendered in pure Superflat Pop visual language
- **Zune** (Microsoft) -- media player whose graphic identity used bold silhouettes and flat rainbow fills in Superflat Pop style
- **UNIQLO** -- Japanese retailer whose collaborations with Murakami and other artists brought Superflat Pop directly to mass-market fashion

---

## Quick-Start Template Skeleton

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Superflat Pop Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&family=Nunito:wght@400;600;700;800;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --sfp-hot-pink: #FF4DA6;
      --sfp-yellow: #FFE500;
      --sfp-cyan: #00D4FF;
      --sfp-lime: #7FFF00;
      --sfp-orange: #FF6B2B;
      --sfp-violet: #9B30FF;
      --sfp-red: #FF1744;
      --sfp-pastel-pink: #FFB3D9;
      --sfp-pastel-yellow: #FFF59D;
      --sfp-pastel-blue: #81D4FA;
      --sfp-black: #000000;
      --sfp-soft-black: #222222;
      --sfp-white: #FFFFFF;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Nunito', sans-serif;
      background: var(--sfp-white);
      color: var(--sfp-soft-black);
      font-weight: 600;
      line-height: 1.7;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1100px;
      margin: 0 auto;
      padding: 1.5rem 2rem;
    }

    nav .logo {
      font-family: 'Fredoka One', sans-serif;
      font-size: 1.5rem;
      color: var(--sfp-hot-pink);
      -webkit-text-stroke: 1.5px var(--sfp-black);
      paint-order: stroke fill;
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 2rem;
      list-style: none;
    }

    nav ul a {
      font-weight: 700;
      color: var(--sfp-soft-black);
      text-decoration: none;
      padding: 0.3em 0.8em;
      border-radius: 100px;
      border: 2px solid transparent;
      transition: all 0.2s ease;
    }

    nav ul a:hover {
      border-color: var(--sfp-black);
      background: var(--sfp-pastel-yellow);
    }

    /* Hero */
    .hero {
      text-align: center;
      padding: 5rem 2rem;
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-family: 'Fredoka One', sans-serif;
      font-size: clamp(3rem, 7vw, 5rem);
      color: var(--sfp-hot-pink);
      -webkit-text-stroke: 3px var(--sfp-black);
      paint-order: stroke fill;
      margin-bottom: 1rem;
      position: relative;
      z-index: 1;
    }

    .hero p {
      font-size: 1.2rem;
      max-width: 550px;
      margin: 0 auto 2rem;
      position: relative;
      z-index: 1;
    }

    /* Rainbow divider */
    .rainbow-bar {
      height: 8px;
      background: linear-gradient(
        90deg,
        var(--sfp-red), var(--sfp-orange), var(--sfp-yellow),
        var(--sfp-lime), var(--sfp-cyan), var(--sfp-violet), var(--sfp-hot-pink)
      );
    }

    /* Outlined button */
    .btn {
      display: inline-block;
      background: var(--sfp-hot-pink);
      color: var(--sfp-white);
      border: 3px solid var(--sfp-black);
      border-radius: 100px;
      padding: 14px 36px;
      font-family: 'Fredoka One', sans-serif;
      font-size: 1rem;
      text-decoration: none;
      position: relative;
      transition: transform 0.15s ease;
    }

    .btn::after {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: 100px;
      border: 3px solid var(--sfp-black);
      background: var(--sfp-black);
      transform: translate(3px, 3px);
      z-index: -1;
      transition: transform 0.15s ease;
    }

    .btn:hover {
      transform: translate(-1px, -1px);
    }

    .btn:hover::after {
      transform: translate(5px, 5px);
    }

    /* Card grid */
    .cards {
      max-width: 1100px;
      margin: 0 auto;
      padding: 4rem 2rem;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
    }

    .card {
      background: var(--sfp-white);
      border: 3px solid var(--sfp-black);
      border-radius: 16px;
      padding: 2rem;
      text-align: center;
      transition: transform 0.2s ease;
    }

    .card:nth-child(1) { background: var(--sfp-pastel-pink); }
    .card:nth-child(2) { background: var(--sfp-pastel-yellow); }
    .card:nth-child(3) { background: var(--sfp-pastel-blue); }

    .card:hover {
      transform: translateY(-3px) rotate(-1deg);
    }

    .card h2 {
      font-family: 'Fredoka One', sans-serif;
      font-size: 1.4rem;
      margin-bottom: 0.75rem;
    }

    .card p {
      font-size: 0.95rem;
      line-height: 1.6;
    }

    /* CTA section */
    .cta {
      background: var(--sfp-yellow);
      border-top: 3px solid var(--sfp-black);
      border-bottom: 3px solid var(--sfp-black);
      text-align: center;
      padding: 4rem 2rem;
    }

    .cta h2 {
      font-family: 'Fredoka One', sans-serif;
      font-size: 2rem;
      margin-bottom: 1rem;
    }

    /* Footer */
    footer {
      background: var(--sfp-soft-black);
      color: var(--sfp-white);
      text-align: center;
      padding: 2.5rem;
      font-size: 0.95rem;
    }

    @media (max-width: 768px) {
      .hero { padding: 3rem 1.5rem; }
      nav { flex-direction: column; gap: 1rem; }
      nav ul { gap: 1rem; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">SuperPop</a>
    <ul>
      <li><a href="#">Features</a></li>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <div class="rainbow-bar"></div>

  <section class="hero">
    <h1>Page Title Here</h1>
    <p>A cheerful description with bold outlines, flat colors, and kawaii energy.</p>
    <a href="#" class="btn">Get Started</a>
  </section>

  <div class="rainbow-bar"></div>

  <section class="cards">
    <div class="card">
      <h2>Section One</h2>
      <p>Content goes here with flat colors and bold outlines defining every element.</p>
    </div>
    <div class="card">
      <h2>Section Two</h2>
      <p>Kawaii-inspired design with rounded shapes and vibrant rainbow palette.</p>
    </div>
    <div class="card">
      <h2>Section Three</h2>
      <p>Clean, playful, and cheerful -- the essence of Superflat Pop design.</p>
    </div>
  </section>

  <section class="cta">
    <h2>Ready to explore?</h2>
    <p>Bold, flat, colorful, and fun.</p>
    <a href="#" class="btn">Learn More</a>
  </section>

  <footer>
    <p>Built with Superflat Pop aesthetics. Flat, bold, kawaii.</p>
  </footer>
</body>
</html>
```
