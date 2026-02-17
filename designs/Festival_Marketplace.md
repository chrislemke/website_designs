# Festival Marketplace -- Design Reference

> An architectural and graphic aesthetic associated with shopping malls of the mid-1980s
> to mid-1990s. It takes inspiration from 1800s--1900s shopping vernacular with a
> **Postmodern interpretation**, updated in a simplified, colourful, celebratory form.
> Also known as **Festival Mall Style** or **Marketplace Postmodernism**.

---

## Visual Characteristics

- **Architectural roots:** Draws from 19th-century covered market halls and arcades, reinterpreted through a bright, postmodern lens with playful exaggeration.
- **Tone:** Celebratory, festive, optimistic -- evoking the excitement of exploration and discovery within a retail environment.
- **Period peak:** Mid-1980s to mid-1990s, with the decade of origin firmly in the 1980s.
- **Key values:** "Shop till you drop," exploration, spectacle, community gathering.
- **Subject matter:** Shopping malls, indoor marketplaces, food courts, retail signage, wayfinding systems, festive commercial environments.
- **Overall feeling:** Vibrant, accessible, and welcoming consumer spaces with playful postmodern design sensibilities. A nostalgic optimism for an era of exuberant retail architecture.
- **Notable designers:** Sibley/Peteet, Steinhilber Deutsch & Gard, Michael Vanderbyl.

## Color Palette

### Primary Palette

| Role             | Colors                                                          |
|------------------|-----------------------------------------------------------------|
| Pastels / Muted  | Soft teal, muted coral, dusty rose, warm cream, pale lavender   |
| Strong Primaries | Bold red, cobalt blue, sunflower yellow, emerald green           |
| Accents          | Bright magenta, warm gold, electric teal                         |
| Neutrals         | Warm white, cool grey, terracotta, charcoal, ivory              |
| Architectural    | Marble white, brass gold, tile grey, awning stripe red           |

### CSS Custom Properties

```css
:root {
  /* Pastels / Muted Tones */
  --fest-soft-teal:      #7EC8B8;
  --fest-muted-coral:    #E8967A;
  --fest-dusty-rose:     #D4A0A0;
  --fest-warm-cream:     #FFF5E1;
  --fest-pale-lavender:  #C5B9D4;
  --fest-mint:           #A8D8C8;

  /* Strong Primaries */
  --fest-bold-red:       #CC2936;
  --fest-cobalt-blue:    #1446A0;
  --fest-sunflower:      #F5C518;
  --fest-emerald:        #2E8B57;

  /* Accents */
  --fest-magenta:        #D6336C;
  --fest-warm-gold:      #DAA520;
  --fest-electric-teal:  #00B4D8;

  /* Neutrals */
  --fest-warm-white:     #FEFCF3;
  --fest-cool-grey:      #B0B3B8;
  --fest-terracotta:     #C67A4B;
  --fest-charcoal:       #2D3436;
  --fest-ivory:          #FFFFF0;

  /* Architectural Materials */
  --fest-marble:         #F0EDE8;
  --fest-brass:          #C5A55A;
  --fest-tile-grey:      #9CA3AF;
  --fest-awning-red:     #B22234;
}
```

### Color Usage Guidelines

- **Backgrounds:** Use warm cream, ivory, or marble white as base backgrounds. Sections can alternate between pastel tones (soft teal, pale lavender) and warm white.
- **Headings and signage text:** Bold red, cobalt blue, or charcoal for maximum impact -- emulating large mall signage.
- **Navigation and wayfinding:** Cobalt blue and warm gold -- referencing compass rose motifs and directory signs.
- **Accent borders and highlights:** Sunflower yellow and magenta for badges, banners, and call-to-action elements.
- **Checkerboard patterns:** Alternate between bold red/warm white or cobalt blue/warm white for floor-tile references.
- **Ribbon and flag accents:** Bold red, cobalt blue, and sunflower yellow in combination for festive bunting effects.
- **Overall feeling:** Bright and celebratory but grounded -- not neon. The pastels provide a backdrop of sophistication while the primaries deliver visual impact reminiscent of festival banners.

## Typography

### Font Characteristics

- **Headlines / Signage:** Tall serif fonts dominate -- high-contrast, elegant serifs with a strong vertical emphasis. These reference the large-scale lettering found on mall section signs and storefronts. Decorative dots or simple shapes placed between letters add a festive, marketplace quality.
- **Body text:** Clean, legible sans-serif fonts for readability. Should feel modern but warm, not cold or industrial.
- **Accent / Decorative text:** Playful freeform or script fonts to "spice things up" -- referencing hand-painted market stall signs, carnival lettering, and festive banners.
- **Special treatment:** Lettering with dots between characters (e.g., "M A R K E T P L A C E" with interpuncts) is a signature motif.

### Recommended Web Fonts

| Role           | Fonts (Google Fonts)                                     |
|----------------|----------------------------------------------------------|
| Display / Sign | Playfair Display, Cormorant Garamond, Libre Baskerville  |
| Headings       | DM Serif Display, Lora (Bold), Merriweather (Black)      |
| Body           | Inter, Source Sans Pro, Nunito Sans, Open Sans            |
| Script / Fun   | Lobster, Caveat, Satisfy, Permanent Marker                |
| Monospaced     | IBM Plex Mono (for price tags, labels)                    |

### CSS Typography Example

```css
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=DM+Serif+Display&family=Inter:wght@400;600&family=Satisfy&display=swap');

h1, h2, h3 {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 900;
  letter-spacing: 0.06em;
  color: var(--fest-cobalt-blue);
}

h1 {
  font-size: 3rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
}

body {
  font-family: 'Inter', 'Helvetica Neue', sans-serif;
  font-weight: 400;
  line-height: 1.65;
  color: var(--fest-charcoal);
}

.script-accent {
  font-family: 'Satisfy', cursive;
  color: var(--fest-magenta);
  font-size: 1.3em;
}

/* Signature dotted-letter spacing */
.marketplace-lettering {
  font-family: 'Playfair Display', serif;
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.3em;
  word-spacing: 0.2em;
  color: var(--fest-bold-red);
}

/* Interpunct separator style heading */
.dotted-title::after {
  content: '';
}
.dotted-title span + span::before {
  content: '\00B7';
  margin: 0 0.15em;
  color: var(--fest-warm-gold);
}
```

## Key Design Elements and Motifs

### Recurring Visual Motifs

- **Arches** -- curved structural forms referencing covered market arcades and mall entrances; used as section frames, card tops, and decorative headers.
- **Fountains** -- circular or tiered water feature motifs as focal-point centerpieces.
- **Checkerboard patterns** -- both picnic-style gingham and large-tile floor patterns; a defining visual texture.
- **Compass rose** -- wayfinding and navigation motifs; used for directory icons and decorative elements.
- **Flags and ribbons** -- celebratory bunting, pennant strings, and ribbon accents that create a festival atmosphere.
- **Diamond shapes** -- geometric accents used in tile patterns, borders, and decorative grids.
- **Grid motifs** -- structured, repeating geometric patterns referencing tile work and architectural detailing.
- **Indoor awnings** -- striped canopy shapes over sections, referencing covered walkways and market stalls.
- **Glass roof / skylight** -- suggesting openness and natural light; translucent, bright overlays.
- **Large colorful signage** -- oversized lettering marking sections, evoking department store wayfinding.
- **Balloons and confetti** -- scattered festive elements reinforcing the celebratory theme.
- **Festival carts** -- vendor cart silhouettes as decorative motifs.
- **Circular logos** -- round badge-style graphics with serif lettering.
- **Simple colorful silhouette graphics** -- flat, bold illustrations of objects rendered as solid shapes.

### Decorative CSS Patterns

```css
/* Checkerboard tile floor */
.checkerboard-tiles {
  background-image:
    linear-gradient(45deg, var(--fest-tile-grey) 25%, transparent 25%),
    linear-gradient(-45deg, var(--fest-tile-grey) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, var(--fest-tile-grey) 75%),
    linear-gradient(-45deg, transparent 75%, var(--fest-tile-grey) 75%);
  background-size: 50px 50px;
  background-position: 0 0, 0 25px, 25px -25px, -25px 0;
  background-color: var(--fest-marble);
}

/* Picnic-style gingham check */
.gingham {
  background-color: var(--fest-warm-white);
  background-image:
    linear-gradient(
      var(--fest-bold-red) 1px, transparent 1px
    ),
    linear-gradient(
      90deg, var(--fest-bold-red) 1px, transparent 1px
    );
  background-size: 20px 20px;
  background-image:
    repeating-linear-gradient(
      0deg,
      rgba(204, 41, 54, 0.15),
      rgba(204, 41, 54, 0.15) 10px,
      transparent 10px,
      transparent 20px
    ),
    repeating-linear-gradient(
      90deg,
      rgba(204, 41, 54, 0.15),
      rgba(204, 41, 54, 0.15) 10px,
      transparent 10px,
      transparent 20px
    );
}

/* Compass rose motif */
.compass-rose {
  width: 80px;
  height: 80px;
  position: relative;
  display: inline-block;
}
.compass-rose::before,
.compass-rose::after {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--fest-warm-gold);
  clip-path: polygon(50% 0%, 60% 40%, 100% 50%, 60% 60%, 50% 100%, 40% 60%, 0% 50%, 40% 40%);
}
.compass-rose::after {
  transform: rotate(45deg);
  opacity: 0.5;
}

/* Diamond pattern border */
.diamond-border {
  border: none;
  height: 20px;
  background:
    linear-gradient(45deg,  var(--fest-cobalt-blue) 25%, transparent 25%) 0 0,
    linear-gradient(-45deg, var(--fest-cobalt-blue) 25%, transparent 25%) 0 0,
    linear-gradient(45deg,  transparent 75%, var(--fest-cobalt-blue) 75%) 0 0,
    linear-gradient(-45deg, transparent 75%, var(--fest-cobalt-blue) 75%) 0 0;
  background-size: 20px 20px;
  background-color: var(--fest-sunflower);
}

/* Ribbon / pennant bunting */
.pennant-bunting {
  background-image:
    linear-gradient(135deg, var(--fest-bold-red) 33.33%,   transparent 33.33%),
    linear-gradient(225deg, var(--fest-cobalt-blue) 33.33%, transparent 33.33%);
  background-size: 40px 40px;
  height: 30px;
}

/* Flag ribbon accent */
.ribbon-flag {
  display: inline-block;
  padding: 0.4em 1.5em 0.4em 1em;
  background: var(--fest-bold-red);
  color: var(--fest-warm-white);
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  position: relative;
  clip-path: polygon(0% 0%, 90% 0%, 100% 50%, 90% 100%, 0% 100%);
}
```

## Textures and Materials

- **Patterned tile flooring** -- the primary ground texture; large-format checkerboard or diamond patterns in muted tones referencing mall floor tile.
- **Glass and light** -- transparency, brightness, and a sense of openness from skylights and glass roofs; clean, luminous quality.
- **Brass and gold accents** -- warm metallic tones for railings, trim, lettering, and decorative hardware.
- **Marble and stone** -- polished, light-colored surfaces for walls and floors; clean and upscale.
- **Painted surfaces** -- bold, flat-painted signage and structural elements in primary colors.
- **Striped canvas** -- awning fabric patterns in red/white, blue/white, or green/white stripes.
- **Neon lighting** -- subtle neon accents for sign outlines and section markers (more restrained than full neon aesthetics).

### CSS Texture Techniques

```css
/* Marble surface */
.marble-surface {
  background-color: var(--fest-marble);
  background-image:
    linear-gradient(
      135deg,
      rgba(180, 175, 168, 0.08) 0%,
      transparent 40%,
      rgba(180, 175, 168, 0.05) 60%,
      transparent 100%
    ),
    linear-gradient(
      45deg,
      rgba(160, 155, 148, 0.04) 0%,
      transparent 30%,
      rgba(160, 155, 148, 0.06) 70%,
      transparent 100%
    );
}

/* Brass / gold metallic accent */
.brass-accent {
  background: linear-gradient(
    135deg,
    #C5A55A 0%,
    #E8D48B 30%,
    #C5A55A 50%,
    #A08030 70%,
    #C5A55A 100%
  );
  color: var(--fest-charcoal);
  border: 1px solid #A08030;
  box-shadow:
    inset 0 1px 0 rgba(255, 255, 255, 0.3),
    0 2px 4px rgba(0, 0, 0, 0.15);
}

/* Awning stripe pattern */
.awning-stripes {
  background: repeating-linear-gradient(
    90deg,
    var(--fest-awning-red) 0px,
    var(--fest-awning-red) 20px,
    var(--fest-warm-white) 20px,
    var(--fest-warm-white) 40px
  );
  border-radius: 12px 12px 0 0;
  padding: 12px 20px;
}

/* Glass roof / skylight overlay */
.skylight-overlay {
  background: linear-gradient(
    180deg,
    rgba(135, 206, 235, 0.15) 0%,
    rgba(255, 255, 255, 0.05) 40%,
    transparent 100%
  );
  pointer-events: none;
}

/* Neon glow for signage */
.neon-sign {
  color: var(--fest-magenta);
  text-shadow:
    0 0 7px rgba(214, 51, 108, 0.6),
    0 0 20px rgba(214, 51, 108, 0.4),
    0 0 40px rgba(214, 51, 108, 0.2);
  font-family: 'Satisfy', cursive;
}
```

## Layout Principles

### Structure

- **Arcade / corridor composition** -- layouts that guide the eye along a path, like walking through a covered market arcade. Vertical navigation or sidebar structures emulating a walkway with storefronts.
- **Arched section headers** -- content sections framed with arch-shaped tops, referencing architectural arches found in festival marketplaces.
- **Symmetrical and balanced** -- centered alignments, equal-weight columns, and bilateral symmetry reflecting classical marketplace architecture.
- **Clear wayfinding hierarchy** -- large, bold signage-style headings for section identification, smaller serif text for descriptions, with compass or directional motifs for navigation.
- **Card-based "storefront" layouts** -- individual content blocks styled as shop fronts or market stalls, each with its own awning header and bordered frame.
- **Central fountain focal point** -- a prominent hero or centerpiece element that draws the eye, referencing the indoor fountain as the heart of the mall.

### Grid and Spacing

```css
.fest-layout {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 2.5rem;
  max-width: 1280px;
  margin: 0 auto;
  padding: 3rem 2rem;
}

/* Storefront card */
.fest-card {
  background: var(--fest-warm-white);
  border: 3px solid var(--fest-cobalt-blue);
  border-radius: 0 0 12px 12px;
  overflow: hidden;
  box-shadow:
    0 4px 12px rgba(0, 0, 0, 0.08),
    0 1px 3px rgba(0, 0, 0, 0.06);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.fest-card:hover {
  transform: translateY(-4px);
  box-shadow:
    0 8px 24px rgba(0, 0, 0, 0.12),
    0 2px 6px rgba(0, 0, 0, 0.08);
}

/* Awning-style card header */
.fest-card-header {
  background: repeating-linear-gradient(
    90deg,
    var(--fest-bold-red) 0px,
    var(--fest-bold-red) 18px,
    var(--fest-warm-white) 18px,
    var(--fest-warm-white) 36px
  );
  padding: 1rem 1.5rem;
  border-bottom: 3px solid var(--fest-bold-red);
}

.fest-card-header h3 {
  font-family: 'Playfair Display', serif;
  font-weight: 900;
  color: var(--fest-warm-white);
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.4);
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.fest-card-body {
  padding: 1.5rem;
}

/* Section divider with diamond motif */
.fest-divider {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin: 3rem 0;
}

.fest-divider::before,
.fest-divider::after {
  content: '';
  flex: 1;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--fest-brass),
    transparent
  );
}

.fest-divider::before {
  background: linear-gradient(
    90deg,
    transparent,
    var(--fest-brass)
  );
}

.fest-divider::after {
  background: linear-gradient(
    90deg,
    var(--fest-brass),
    transparent
  );
}

/* Arch-topped section */
.arch-section {
  position: relative;
  padding: 3rem 2rem 2rem;
  margin-top: 3rem;
}

.arch-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 10%;
  right: 10%;
  height: 60px;
  background: var(--fest-cobalt-blue);
  border-radius: 100px 100px 0 0;
}

.arch-section h2 {
  position: relative;
  z-index: 1;
  text-align: center;
  color: var(--fest-warm-white);
  margin-top: -1.5rem;
}
```

### Header / Hero Section

```css
.fest-hero {
  background: var(--fest-warm-cream);
  text-align: center;
  padding: 5rem 2rem 4rem;
  position: relative;
  overflow: hidden;
  border-bottom: 4px solid var(--fest-brass);
}

/* Subtle skylight glow from above */
.fest-hero::before {
  content: '';
  position: absolute;
  top: -50%;
  left: 25%;
  right: 25%;
  height: 100%;
  background: radial-gradient(
    ellipse,
    rgba(135, 206, 235, 0.12) 0%,
    transparent 70%
  );
  pointer-events: none;
}

.fest-hero h1 {
  font-family: 'Playfair Display', serif;
  font-size: 3.5rem;
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--fest-cobalt-blue);
  margin-bottom: 0.5rem;
  text-shadow: 2px 2px 0 rgba(197, 165, 90, 0.3);
}

.fest-hero .tagline {
  font-family: 'Satisfy', cursive;
  font-size: 1.6rem;
  color: var(--fest-magenta);
  margin-top: 0.5rem;
}

/* Pennant bunting below hero */
.fest-hero::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 24px;
  background-image:
    linear-gradient(135deg, var(--fest-bold-red) 33%, transparent 33%),
    linear-gradient(225deg, var(--fest-sunflower) 33%, transparent 33%);
  background-size: 36px 24px;
}

/* Navigation styled as mall directory */
.fest-nav {
  display: flex;
  justify-content: center;
  gap: 0;
  background: var(--fest-cobalt-blue);
  padding: 0;
}

.fest-nav a {
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--fest-warm-white);
  padding: 1rem 2rem;
  text-decoration: none;
  border-right: 1px solid rgba(255, 255, 255, 0.2);
  transition: background 0.2s ease;
}

.fest-nav a:hover {
  background: var(--fest-bold-red);
}

.fest-nav a:last-child {
  border-right: none;
}
```

## Design Techniques Summary

| Technique                 | Implementation                                                        |
|---------------------------|-----------------------------------------------------------------------|
| Arched section headers    | `border-radius: 100px 100px 0 0;` on pseudo-elements or containers   |
| Awning stripe headers     | `repeating-linear-gradient(90deg, ...)` in red/white or blue/white    |
| Checkerboard floor        | Four `linear-gradient(45deg, ...)` layers with offset positions       |
| Diamond pattern borders   | Rotated square gradients in contrasting primary colors                |
| Pennant bunting            | Triangular gradients at `135deg / 225deg` in alternating colors       |
| Brass / gold accents      | Multi-stop `linear-gradient(135deg, ...)` with warm gold tones        |
| Compass rose motif        | `clip-path: polygon(...)` with 8-point star shape                     |
| Dotted interpunct titles  | `letter-spacing: 0.3em` with `::before` interpunct pseudo-elements   |
| Tall serif signage        | Playfair Display or DM Serif Display at large sizes, uppercase       |
| Skylight glow             | Radial gradient overlay with soft blue tint, `pointer-events: none`  |
| Neon sign accents         | Layered `text-shadow` with decreasing opacity at increasing blur     |
| Storefront cards          | Bordered cards with awning-striped header bar and hover lift          |
| Mall directory nav        | Horizontal nav bar with tall serif links, divider borders            |
| Ribbon flag labels        | `clip-path: polygon(...)` with pointed right edge                     |
| Marble texture            | Layered angled gradients with very low opacity grey tones            |

## Related Aesthetics

These aesthetics share visual DNA with Festival Marketplace and can be blended or referenced:

| Aesthetic              | Relationship                                                              |
|------------------------|---------------------------------------------------------------------------|
| **American Kitsch**    | Shares the celebratory, colorful, consumer-culture DNA; checkerboard patterns and retro signage overlap |
| **Memphis Design**     | Core postmodern sibling; bold geometric patterns, primary colors, playful irreverence |
| **Memphis Lite**       | Softer, more commercial version of Memphis; pastel geometrics in retail settings |
| **Mallsoft**           | Sonic/visual cousin; the vaporwave nostalgia for 1990s mall atmospheres and liminal retail spaces |
| **Liminal Space**      | The eerie, empty counterpart; vacant versions of the same architectural spaces become uncanny |
| **Factory Pomo**       | Industrial postmodernism sharing the same era; bold forms and color in commercial architecture |
| **Fanfare**            | Direct overlap in celebratory motifs: flags, ribbons, confetti, bright primary colors |
| **Neoclassical PoMo**  | Shares the historical-reference approach; classical columns and arches in postmodern context |
| **Vintage Americana**  | The aged, nostalgic predecessor; Festival Marketplace modernizes its market-town sensibilities |
| **Whimsicraft**        | Shares playful, handmade quality; craft-fair and market-stall visual language |
| **Monochrome Luxe**    | Contrasting aesthetic; the upscale, minimal version of retail design vs. Festival Marketplace's maximalism |
| **Utopian Scholastic** | Shares the bright, optimistic, institutional design language of the same era |

## Quick-Start Template Skeleton

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Festival Marketplace Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=DM+Serif+Display&family=Inter:wght@400;600&family=Satisfy&display=swap" rel="stylesheet">
  <style>
    :root {
      --fest-soft-teal:     #7EC8B8;
      --fest-muted-coral:   #E8967A;
      --fest-dusty-rose:    #D4A0A0;
      --fest-warm-cream:    #FFF5E1;
      --fest-pale-lavender: #C5B9D4;
      --fest-mint:          #A8D8C8;
      --fest-bold-red:      #CC2936;
      --fest-cobalt-blue:   #1446A0;
      --fest-sunflower:     #F5C518;
      --fest-emerald:       #2E8B57;
      --fest-magenta:       #D6336C;
      --fest-warm-gold:     #DAA520;
      --fest-electric-teal: #00B4D8;
      --fest-warm-white:    #FEFCF3;
      --fest-cool-grey:     #B0B3B8;
      --fest-terracotta:    #C67A4B;
      --fest-charcoal:      #2D3436;
      --fest-ivory:         #FFFFF0;
      --fest-marble:        #F0EDE8;
      --fest-brass:         #C5A55A;
      --fest-tile-grey:     #9CA3AF;
      --fest-awning-red:    #B22234;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Inter', 'Helvetica Neue', sans-serif;
      background: var(--fest-warm-cream);
      color: var(--fest-charcoal);
      line-height: 1.65;
    }

    /* Hero with skylight glow and pennant bunting */
    header {
      background: var(--fest-warm-cream);
      text-align: center;
      padding: 5rem 2rem 3.5rem;
      position: relative;
      border-bottom: 4px solid var(--fest-brass);
      overflow: hidden;
    }

    header::before {
      content: '';
      position: absolute;
      top: -40%;
      left: 20%;
      right: 20%;
      height: 80%;
      background: radial-gradient(ellipse, rgba(135,206,235,0.12) 0%, transparent 70%);
      pointer-events: none;
    }

    header::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 20px;
      background-image:
        linear-gradient(135deg, var(--fest-bold-red) 33%, transparent 33%),
        linear-gradient(225deg, var(--fest-sunflower) 33%, transparent 33%);
      background-size: 32px 20px;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      font-size: 3.2rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--fest-cobalt-blue);
      text-shadow: 2px 2px 0 rgba(197,165,90,0.3);
    }

    header p {
      font-family: 'Satisfy', cursive;
      font-size: 1.5rem;
      color: var(--fest-magenta);
      margin-top: 0.5rem;
    }

    /* Mall directory navigation */
    nav {
      display: flex;
      justify-content: center;
      background: var(--fest-cobalt-blue);
    }

    nav a {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--fest-warm-white);
      padding: 1rem 2rem;
      text-decoration: none;
      border-right: 1px solid rgba(255,255,255,0.2);
      transition: background 0.2s;
    }

    nav a:hover { background: var(--fest-bold-red); }
    nav a:last-child { border-right: none; }

    /* Main content grid */
    main {
      max-width: 1200px;
      margin: 0 auto;
      padding: 3rem 2rem;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 2.5rem;
    }

    /* Storefront card with awning */
    .card {
      background: var(--fest-warm-white);
      border: 3px solid var(--fest-cobalt-blue);
      border-radius: 0 0 12px 12px;
      overflow: hidden;
      box-shadow: 0 4px 12px rgba(0,0,0,0.08);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.12);
    }

    .card-header {
      background: repeating-linear-gradient(
        90deg,
        var(--fest-bold-red) 0px, var(--fest-bold-red) 18px,
        var(--fest-warm-white) 18px, var(--fest-warm-white) 36px
      );
      padding: 0.8rem 1.5rem;
      border-bottom: 3px solid var(--fest-bold-red);
    }

    .card-header h2 {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      font-size: 1.2rem;
      color: var(--fest-warm-white);
      text-shadow: 1px 1px 2px rgba(0,0,0,0.4);
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    .card-body {
      padding: 1.5rem;
    }

    /* Footer */
    footer {
      background: var(--fest-charcoal);
      color: var(--fest-warm-cream);
      text-align: center;
      padding: 2.5rem;
      font-family: 'Satisfy', cursive;
      font-size: 1.2rem;
      border-top: 4px solid var(--fest-brass);
    }
  </style>
</head>
<body>
  <header>
    <h1>Page Title Here</h1>
    <p>A festive tagline in script font</p>
  </header>
  <nav>
    <a href="#section1">Directory</a>
    <a href="#section2">Market</a>
    <a href="#section3">Pavilion</a>
  </nav>
  <main>
    <div class="card">
      <div class="card-header"><h2>Section One</h2></div>
      <div class="card-body"><p>Content goes here.</p></div>
    </div>
    <div class="card">
      <div class="card-header"><h2>Section Two</h2></div>
      <div class="card-body"><p>Content goes here.</p></div>
    </div>
    <div class="card">
      <div class="card-header"><h2>Section Three</h2></div>
      <div class="card-body"><p>Content goes here.</p></div>
    </div>
  </main>
  <footer>
    <p>Welcome to the Marketplace</p>
  </footer>
</body>
</html>
```
