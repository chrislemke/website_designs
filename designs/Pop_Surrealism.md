# Pop Surrealism Design Reference

Pop Surrealism, also known as Lowbrow art, is a counterculture art movement that emerged from the underground scene of late-1960s Los Angeles, rooted in hot rod culture, underground comix, punk rock, tiki art, psychedelia, and tattoo traditions. The movement was named by artist Robert Williams, who titled his 1979 book *The Lowbrow Art of Robt. Williams* as a defiant rejection of fine-art gatekeeping. Championed by artists such as Mark Ryden, Marion Peck, Todd Schorr, Camille Rose Garcia, and Robert Williams, it fuses the technical polish of Old Master painting with the imagery of pop culture, sideshow spectacle, and surrealist dream logic. The aesthetic is defined by a central paradox: beautiful yet unsettling, cute yet sinister, saccharine yet grotesque. In web and UI design, Pop Surrealism translates to richly illustrative color palettes (cotton-candy pastels against deep crimsons and blacks), ornate baroque-inspired frames and borders, carnival and sideshow typography, decorative filigree, big-eyed character motifs, and layouts that feel like stepping into a twisted storybook or a gilded cabinet of curiosities.

---

## Visual Characteristics

### Core Design Traits

- **Big-eyed characters**: Oversized, doll-like eyes dominate character illustrations, evoking innocence and vulnerability while creating an uncanny, unsettling quality reminiscent of Margaret Keane's paintings filtered through dark fairy tales
- **Ornate baroque framing**: Elaborately carved, gilded, scrollwork-heavy frames and borders surround content areas, referencing the ornate frames Mark Ryden commissions for his paintings and lending a sense of precious, museum-like presentation
- **Sweet-and-sinister duality**: Every element exists in tension between the appealing and the disturbing -- candy-colored palettes paired with macabre imagery, delicate florals intertwined with bones, plush textures alongside raw flesh
- **Carnival and sideshow motifs**: Striped tents, sideshow banners, ticket stubs, pinstripe patterns, ferris wheels, and circus typography evoke the traveling carnival -- a central visual metaphor for the movement's outsider identity
- **Psychedelic flourishes**: Swirling organic forms, paisley patterns, Art Nouveau-influenced tendrils, and vibrant color gradients that reference the movement's roots in 1960s counterculture poster art
- **Tattoo art influence**: Bold outlines, rich color fills, banner scrolls, roses, skulls, sacred hearts, and flash-sheet compositions drawn from traditional American and neo-traditional tattoo iconography
- **Kitschy Americana remix**: Vintage advertising imagery, mid-century toys, religious kitsch, fast-food mascots, and consumer products recontextualized in dreamlike or nightmarish settings
- **Hyper-detailed surfaces**: Obsessive attention to texture and detail -- wood grain, fabric weave, porcelain gloss, meat marbling -- rendered with almost photographic precision within fantastical compositions
- **Storybook and fairy-tale references**: Compositions arranged like illustrated book pages, with vignettes, decorative chapter headings, and narrative imagery that feels like a Brothers Grimm tale retold by a pop-culture-obsessed surrealist

### Design Principles

- **Tension of opposites**: Always maintain a balance between the beautiful and the grotesque, the childlike and the mature, the polished and the raw
- **Maximal detail within controlled composition**: Fill surfaces with rich detail and ornamentation, but anchor everything with strong central focal points and classical compositional structure
- **Handcrafted over algorithmic**: Favor illustrative, hand-drawn, and painterly textures over clean geometric minimalism; imperfection and organic form signal authenticity
- **Cultural collage**: Freely mix high and low culture references -- Renaissance composition with cartoon characters, religious iconography with junk-food packaging, baroque ornament with punk graphics
- **Narrative implication**: Every design element should suggest a story; viewers should feel they have stumbled into a scene mid-narrative, provoking curiosity and slight unease
- **Ornament as meaning**: Decorative elements are not mere embellishment but carry symbolic weight -- frames suggest preciousness, stripes suggest carnival, scrollwork suggests history
- **Immersive atmosphere**: The design should feel like an environment, not just a layout; the viewer should feel transported into the world of the piece

---

## Color Palette

| Swatch | Hex | Role / Usage |
|--------|-----|-------------|
| Cotton Candy | `#F4A5C0` | Primary accent, sweet-feminine highlights, character blush tones |
| Flesh Rose | `#E8B4A2` | Skin tones, warm organic surfaces, card backgrounds |
| Absinthe Green | `#7DB47A` | Nature motifs, poison/toxicity connotation, secondary accent |
| Carnival Red | `#B8242A` | Bold primary accent, striped patterns, blood/passion motifs |
| Bone White | `#F5F0E8` | Primary background, parchment feel, aged paper surfaces |
| Midnight Plum | `#2E1A3B` | Deep contrast, shadows, rich dark backgrounds |
| Gilt Gold | `#C9A84C` | Ornate frames, baroque flourishes, precious accents |
| Bruise Purple | `#6B3A6E` | Psychedelic tones, mystic/occult elements, secondary darks |
| Sideshow Teal | `#3A8A8C` | Carnival banners, cool accent, contrast to warm pinks |
| Bubblegum Hot Pink | `#E84690` | High-energy pop accent, neon signage, call-to-action |
| Caramel | `#A0632C` | Warm wood tones, antique surfaces, earthy grounding |
| Porcelain Blue | `#A0C4D8` | Delicate cool accent, sky tones, doll-like highlights |
| Tar Black | `#1A1418` | Text, outlines, deepest shadows, maximum contrast |
| Candy Apple | `#FF3333` | Warning accents, hot-rod flames, aggressive highlights |
| Buttercream | `#FFF4D6` | Soft warm background alternative, vintage paper, glow tones |

### CSS Custom Properties

```css
:root {
  /* Sweet tones */
  --pop-cotton-candy:    #F4A5C0;
  --pop-flesh-rose:      #E8B4A2;
  --pop-buttercream:     #FFF4D6;
  --pop-porcelain-blue:  #A0C4D8;

  /* Bold accents */
  --pop-carnival-red:    #B8242A;
  --pop-candy-apple:     #FF3333;
  --pop-bubblegum:       #E84690;
  --pop-gilt-gold:       #C9A84C;

  /* Nature and mystic */
  --pop-absinthe:        #7DB47A;
  --pop-sideshow-teal:   #3A8A8C;
  --pop-bruise-purple:   #6B3A6E;

  /* Darks and neutrals */
  --pop-midnight-plum:   #2E1A3B;
  --pop-tar-black:       #1A1418;
  --pop-caramel:         #A0632C;
  --pop-bone-white:      #F5F0E8;
}
```

---

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Playfair Display** | 400, 700, 900 | Primary headings; high-contrast serif with baroque elegance | [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) |
| **UnifrakturCook** | 700 | Decorative blackletter for carnival banners and sideshow headings | [UnifrakturCook](https://fonts.google.com/specimen/UnifrakturCook) |
| **Creepster** | 400 | Halloween/horror accent text, spooky subheadings | [Creepster](https://fonts.google.com/specimen/Creepster) |
| **Lora** | 400, 500, 700 | Body text; elegant readable serif with organic curves | [Lora](https://fonts.google.com/specimen/Lora) |
| **Cinzel Decorative** | 400, 700, 900 | Ornate display headings, gilded frame titles | [Cinzel Decorative](https://fonts.google.com/specimen/Cinzel+Decorative) |
| **Rye** | 400 | Western/sideshow carnival display type | [Rye](https://fonts.google.com/specimen/Rye) |
| **IM Fell English** | 400 | Antiquarian body text with a slightly worn, historical feel | [IM Fell English](https://fonts.google.com/specimen/IM+Fell+English) |
| **Stint Ultra Expanded** | 400 | Wide display font for banner and marquee text | [Stint Ultra Expanded](https://fonts.google.com/specimen/Stint+Ultra+Expanded) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Cinzel Decorative 700 | Lora 400 | Gilded gallery exhibition, baroque refinement |
| Creepster 400 | IM Fell English 400 | Dark fairy tale, haunted storybook |
| Rye 400 | Lora 500 | Carnival sideshow, vintage spectacle |
| Playfair Display 900 | Lora 400 | Elegant surrealism, fine art meets pop |
| UnifrakturCook 700 | IM Fell English 400 | Gothic circus, medieval carnival |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=Lora:wght@400;500;700&family=Cinzel+Decorative:wght@400;700;900&family=Creepster&family=Rye&display=swap');

body {
  font-family: 'Lora', 'Georgia', serif;
  font-size: 1rem;
  line-height: 1.75;
  color: var(--pop-tar-black);
  -webkit-font-smoothing: antialiased;
}

h1, h2 {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 900;
  letter-spacing: 0.02em;
  color: var(--pop-carnival-red);
}

h3, h4 {
  font-family: 'Cinzel Decorative', 'Playfair Display', serif;
  font-weight: 700;
  letter-spacing: 0.05em;
  color: var(--pop-midnight-plum);
}

.carnival-title {
  font-family: 'Rye', 'Playfair Display', serif;
  font-size: 2.5rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--pop-gilt-gold);
  text-shadow: 2px 2px 0 var(--pop-tar-black);
}

.spooky-accent {
  font-family: 'Creepster', cursive;
  color: var(--pop-bubblegum);
  letter-spacing: 0.03em;
}
```

---

## Layout Principles

- **Symmetrical and centered compositions**: Mirror the classical, altar-like compositions of Mark Ryden and religious icon painting; center key content with symmetrical flanking elements
- **Ornate frames as structural containers**: Use CSS borders, box-shadows, and pseudo-elements to create elaborate frame-like containers around content sections, evoking gallery presentation
- **Layered depth with overlapping elements**: Stack content layers to create a collage-like depth -- images overlapping frames, text overlaying illustration, decorative elements breaking container boundaries
- **Generous ornamented margins**: Instead of stark whitespace, fill margins with subtle repeating patterns (stripes, filigree, damask) to maintain the maximalist, storybook atmosphere
- **Vertical scroll as narrative journey**: Design the page as a sequential narrative experience; each scroll reveals a new scene or chapter in the visual story
- **Vignette and focal-point lighting**: Use radial gradients and shadow overlays to create a spotlight effect, drawing the eye inward like a stage or diorama
- **Responsive adaptation**: On smaller screens, simplify ornate frames to single borders with corner flourishes; maintain color palette and typographic hierarchy; stack symmetrical layouts vertically while preserving center alignment

---

## CSS / Design Techniques

### Pop Surrealist Card

```css
.pop-card {
  background: var(--pop-bone-white);
  border: 3px solid var(--pop-gilt-gold);
  border-radius: 4px;
  padding: 2rem;
  position: relative;
  box-shadow:
    0 0 0 1px var(--pop-tar-black),
    0 0 0 5px var(--pop-carnival-red),
    0 0 0 6px var(--pop-tar-black),
    8px 8px 0 var(--pop-tar-black);
  max-width: 420px;
}

.pop-card::before {
  content: '';
  position: absolute;
  top: 8px;
  left: 8px;
  right: 8px;
  bottom: 8px;
  border: 1px solid var(--pop-gilt-gold);
  border-radius: 2px;
  pointer-events: none;
  opacity: 0.5;
}

.pop-card h3 {
  font-family: 'Cinzel Decorative', serif;
  font-weight: 700;
  text-align: center;
  color: var(--pop-carnival-red);
  margin-bottom: 1rem;
  font-size: 1.3rem;
}

.pop-card p {
  font-family: 'Lora', serif;
  color: var(--pop-tar-black);
  line-height: 1.7;
  text-align: center;
}
```

### Sideshow Button

```css
.pop-button {
  display: inline-block;
  font-family: 'Rye', 'Playfair Display', serif;
  font-size: 1rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--pop-buttercream);
  background: linear-gradient(
    180deg,
    var(--pop-carnival-red) 0%,
    #8B1A1F 100%
  );
  border: 3px solid var(--pop-gilt-gold);
  padding: 14px 36px;
  cursor: pointer;
  position: relative;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
  box-shadow:
    0 0 0 1px var(--pop-tar-black),
    4px 4px 0 var(--pop-tar-black);
  transition: all 0.2s ease;
}

.pop-button:hover {
  background: linear-gradient(
    180deg,
    var(--pop-bubblegum) 0%,
    var(--pop-carnival-red) 100%
  );
  box-shadow:
    0 0 0 1px var(--pop-tar-black),
    2px 2px 0 var(--pop-tar-black);
  transform: translate(2px, 2px);
}

.pop-button:active {
  transform: translate(4px, 4px);
  box-shadow: 0 0 0 1px var(--pop-tar-black);
}
```

### Carnival Navigation Bar

```css
.pop-nav {
  background: var(--pop-midnight-plum);
  border-bottom: 4px solid var(--pop-gilt-gold);
  padding: 0 2rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
}

.pop-nav::after {
  content: '';
  position: absolute;
  bottom: -12px;
  left: 0;
  right: 0;
  height: 8px;
  background: repeating-linear-gradient(
    90deg,
    var(--pop-carnival-red) 0px,
    var(--pop-carnival-red) 12px,
    var(--pop-bone-white) 12px,
    var(--pop-bone-white) 24px
  );
}

.pop-nav-logo {
  font-family: 'Cinzel Decorative', serif;
  font-weight: 900;
  font-size: 1.5rem;
  color: var(--pop-gilt-gold);
  text-shadow: 1px 1px 0 var(--pop-tar-black);
  padding: 1rem 0;
}

.pop-nav-links {
  list-style: none;
  display: flex;
  gap: 0;
  margin: 0;
  padding: 0;
}

.pop-nav-links a {
  display: block;
  font-family: 'Rye', serif;
  font-size: 0.85rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--pop-bone-white);
  text-decoration: none;
  padding: 1.2rem 1.5rem;
  transition: background 0.2s ease, color 0.2s ease;
  border-left: 1px solid rgba(201, 168, 76, 0.2);
}

.pop-nav-links a:hover {
  background: var(--pop-carnival-red);
  color: var(--pop-buttercream);
}
```

### Hero Section

```css
.pop-hero {
  background:
    radial-gradient(
      ellipse at center,
      rgba(244, 165, 192, 0.15) 0%,
      transparent 70%
    ),
    var(--pop-midnight-plum);
  text-align: center;
  padding: 6rem 2rem;
  position: relative;
  overflow: hidden;
  border-bottom: 6px solid var(--pop-gilt-gold);
}

.pop-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent 0px,
    transparent 3px,
    rgba(201, 168, 76, 0.03) 3px,
    rgba(201, 168, 76, 0.03) 4px
  );
  pointer-events: none;
}

.pop-hero h1 {
  font-family: 'Playfair Display', serif;
  font-weight: 900;
  font-size: 4rem;
  color: var(--pop-bone-white);
  text-shadow:
    0 0 20px rgba(244, 165, 192, 0.4),
    3px 3px 0 var(--pop-carnival-red);
  margin-bottom: 1rem;
  position: relative;
}

.pop-hero .subtitle {
  font-family: 'Cinzel Decorative', serif;
  font-size: 1.2rem;
  color: var(--pop-gilt-gold);
  letter-spacing: 0.15em;
  text-transform: uppercase;
}

.pop-hero .tagline {
  font-family: 'Lora', serif;
  font-style: italic;
  font-size: 1.1rem;
  color: var(--pop-cotton-candy);
  margin-top: 1.5rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}
```

### Ornate Frame Container

```css
.pop-ornate-frame {
  position: relative;
  background: var(--pop-bone-white);
  border: 2px solid var(--pop-gilt-gold);
  padding: 3rem;
  margin: 2rem auto;
  max-width: 700px;
}

/* Inner border line */
.pop-ornate-frame::before {
  content: '';
  position: absolute;
  top: 10px;
  left: 10px;
  right: 10px;
  bottom: 10px;
  border: 1px solid var(--pop-gilt-gold);
  pointer-events: none;
}

/* Corner flourishes using box-shadow */
.pop-ornate-frame::after {
  content: '\2766'; /* floral heart */
  position: absolute;
  top: -14px;
  left: 50%;
  transform: translateX(-50%);
  font-size: 1.6rem;
  color: var(--pop-gilt-gold);
  background: var(--pop-bone-white);
  padding: 0 12px;
}

.pop-corner-tl,
.pop-corner-tr,
.pop-corner-bl,
.pop-corner-br {
  position: absolute;
  width: 30px;
  height: 30px;
  border-color: var(--pop-gilt-gold);
  border-style: solid;
}

.pop-corner-tl { top: 4px; left: 4px; border-width: 3px 0 0 3px; }
.pop-corner-tr { top: 4px; right: 4px; border-width: 3px 3px 0 0; }
.pop-corner-bl { bottom: 4px; left: 4px; border-width: 0 0 3px 3px; }
.pop-corner-br { bottom: 4px; right: 4px; border-width: 0 3px 3px 0; }
```

### Carnival Banner

```css
.pop-banner {
  position: relative;
  display: inline-block;
  background: var(--pop-carnival-red);
  color: var(--pop-buttercream);
  font-family: 'Rye', serif;
  font-size: 1.4rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  text-align: center;
  padding: 1rem 3rem;
  text-shadow: 1px 1px 0 var(--pop-tar-black);
}

/* Left ribbon tail */
.pop-banner::before {
  content: '';
  position: absolute;
  top: 0;
  left: -20px;
  width: 0;
  height: 0;
  border-top: 28px solid var(--pop-carnival-red);
  border-bottom: 28px solid var(--pop-carnival-red);
  border-left: 20px solid transparent;
}

/* Right ribbon tail */
.pop-banner::after {
  content: '';
  position: absolute;
  top: 0;
  right: -20px;
  width: 0;
  height: 0;
  border-top: 28px solid var(--pop-carnival-red);
  border-bottom: 28px solid var(--pop-carnival-red);
  border-right: 20px solid transparent;
}
```

### Eyeball Motif Decoration

```css
.pop-eye {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background: radial-gradient(
    circle at 50% 50%,
    var(--pop-tar-black) 18%,
    var(--pop-bruise-purple) 18%,
    var(--pop-bruise-purple) 35%,
    var(--pop-bone-white) 35%,
    var(--pop-bone-white) 100%
  );
  box-shadow:
    0 0 0 4px var(--pop-tar-black),
    0 0 0 8px var(--pop-cotton-candy),
    0 0 0 10px var(--pop-tar-black);
  position: relative;
  display: inline-block;
}

/* Highlight reflection */
.pop-eye::after {
  content: '';
  position: absolute;
  top: 20%;
  left: 55%;
  width: 12px;
  height: 12px;
  background: white;
  border-radius: 50%;
}

/* Veins / bloodshot lines via a wrapper class */
.pop-eye-bloodshot {
  background:
    radial-gradient(
      circle at 50% 50%,
      var(--pop-tar-black) 18%,
      var(--pop-bruise-purple) 18%,
      var(--pop-bruise-purple) 35%,
      var(--pop-bone-white) 35%,
      var(--pop-bone-white) 100%
    ),
    repeating-conic-gradient(
      from 0deg,
      transparent 0deg 15deg,
      rgba(184, 36, 42, 0.15) 15deg 17deg,
      transparent 17deg 30deg
    );
}
```

### Dripping Text Effect

```css
.pop-drip-text {
  font-family: 'Creepster', cursive;
  font-size: 3rem;
  color: var(--pop-bubblegum);
  position: relative;
  display: inline-block;
  text-shadow:
    2px 2px 0 var(--pop-tar-black),
    -1px -1px 0 var(--pop-tar-black),
    1px -1px 0 var(--pop-tar-black),
    -1px 1px 0 var(--pop-tar-black);
}

/* Drip drops */
.pop-drip-text::after {
  content: '';
  position: absolute;
  bottom: -18px;
  left: 15%;
  width: 8px;
  height: 18px;
  background: var(--pop-bubblegum);
  border-radius: 0 0 50% 50%;
  box-shadow:
    30px 6px 0 0 var(--pop-bubblegum),
    68px -2px 0 0 var(--pop-bubblegum),
    110px 8px 0 0 var(--pop-bubblegum);
  animation: drip 2s ease-in-out infinite;
}

@keyframes drip {
  0%, 100% { transform: translateY(0); opacity: 1; }
  50% { transform: translateY(8px); opacity: 0.7; }
}
```

### Striped Carnival Background

```css
.pop-carnival-stripes {
  background: repeating-linear-gradient(
    90deg,
    var(--pop-carnival-red) 0px,
    var(--pop-carnival-red) 40px,
    var(--pop-bone-white) 40px,
    var(--pop-bone-white) 80px
  );
}

/* Radial sunburst variant */
.pop-sunburst {
  background: repeating-conic-gradient(
    from 0deg,
    var(--pop-carnival-red) 0deg 10deg,
    var(--pop-midnight-plum) 10deg 20deg
  );
}

/* Damask-like repeating pattern using pseudo-elements */
.pop-damask-bg {
  background-color: var(--pop-bone-white);
  background-image:
    radial-gradient(
      ellipse at 50% 50%,
      rgba(201, 168, 76, 0.08) 0%,
      transparent 70%
    );
  background-size: 60px 60px;
}
```

---

## Design Do's and Don'ts

### Do

- Use rich, layered color schemes that balance saccharine pastels with deep, moody darks
- Incorporate ornate decorative borders and frames that reference baroque and Victorian craftsmanship
- Mix serif typefaces with decorative carnival display fonts for authentic visual tension
- Include hand-drawn or illustrative elements wherever possible -- even as CSS-rendered decorations
- Let content breathe within ornate containers; the frame is part of the message
- Create deliberate contrast between cute/innocent and dark/unsettling elements
- Use gold accents sparingly to convey preciousness and gallery-quality presentation
- Add subtle texture (paper grain, canvas weave) to backgrounds to avoid flat digital sterility
- Reference specific cultural artifacts: sideshow banners, Victorian ephemera, tattoo flash sheets, vintage toy packaging

### Don't

- Fall into pure minimalism -- Pop Surrealism is inherently maximalist and decorative; stripped-down layouts lose the aesthetic entirely
- Use only bright, happy colors without darker counterpoints; the sinister undertone is essential to the movement's identity
- Overuse horror or gore elements -- the aesthetic is unsettling, not gratuitously violent; subtlety is key
- Apply carnival fonts to all text -- reserve decorative typefaces for headings and accents; body text must remain readable
- Ignore the fine-art heritage -- Pop Surrealism is not simply "weird art"; it descends from Dali, Bosch, and Dutch Golden Age painting
- Use flat, unadorned containers when ornate frames would establish the proper atmosphere
- Rely solely on stock photography -- the aesthetic demands illustration, painting, or heavily stylized imagery
- Treat the palette as purely pastel or purely dark; the interplay between sweet and sinister tones defines the look
- Neglect responsive considerations -- ornate frames and complex layouts must degrade gracefully on smaller screens

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Dreamcore** | Shares surreal, unsettling imagery and dreamlike compositions; Dreamcore is more vacant and liminal where Pop Surrealism is richly populated |
| **Fleischer Style** | Shares rubber-hose cartoon influence, dark whimsy, and the fusion of cute with sinister; Fleischer is animation-specific, Pop Surrealism is painterly |
| **American Kitsch** | Pop Surrealism directly appropriates and subverts kitschy Americana -- vintage ads, suburban idealism, consumer culture |
| **Art Nouveau** | Shared love of organic, flowing ornamental forms, decorative frames, and the integration of art with design |
| **Baroque** | Ornate gilded framing, dramatic lighting, and maximalist detail are borrowed directly from the Baroque tradition |
| **Catholic Kitsch** | Religious iconography, sacred hearts, saints, and devotional imagery are frequently remixed in Pop Surrealist work |
| **Goblincore** | Shares a fascination with the strange, grotesque, and overlooked; Goblincore is earthy and naturalistic where Pop Surrealism is painterly |
| **Maximalism** | Both reject minimalist restraint in favor of dense, layered, richly detailed compositions |
| **DIY Punk** | Shares countercultural outsider identity and roots in underground zine/poster culture |
| **Psychedelic / Acid Design** | Shared roots in 1960s counterculture poster art, vibrant colors, and mind-bending visual distortions |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pop Surrealism &mdash; Cabinet of Curiosities</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=Lora:wght@400;500;700&family=Cinzel+Decorative:wght@400;700;900&family=Creepster&family=Rye&display=swap" rel="stylesheet">
  <style>
    /* ===========================
       CSS Custom Properties
       =========================== */
    :root {
      --pop-cotton-candy:    #F4A5C0;
      --pop-flesh-rose:      #E8B4A2;
      --pop-buttercream:     #FFF4D6;
      --pop-porcelain-blue:  #A0C4D8;
      --pop-carnival-red:    #B8242A;
      --pop-candy-apple:     #FF3333;
      --pop-bubblegum:       #E84690;
      --pop-gilt-gold:       #C9A84C;
      --pop-absinthe:        #7DB47A;
      --pop-sideshow-teal:   #3A8A8C;
      --pop-bruise-purple:   #6B3A6E;
      --pop-midnight-plum:   #2E1A3B;
      --pop-tar-black:       #1A1418;
      --pop-caramel:         #A0632C;
      --pop-bone-white:      #F5F0E8;
    }

    /* ===========================
       Reset & Base
       =========================== */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Lora', 'Georgia', serif;
      font-size: 1rem;
      line-height: 1.75;
      color: var(--pop-tar-black);
      background: var(--pop-bone-white);
      -webkit-font-smoothing: antialiased;
    }

    img { max-width: 100%; display: block; }
    a { color: var(--pop-carnival-red); text-decoration: none; }
    a:hover { color: var(--pop-bubblegum); }

    /* ===========================
       Background Texture
       =========================== */
    body::before {
      content: '';
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      pointer-events: none;
      z-index: 0;
      background:
        radial-gradient(ellipse at 20% 50%, rgba(244,165,192,0.06) 0%, transparent 50%),
        radial-gradient(ellipse at 80% 50%, rgba(107,58,110,0.04) 0%, transparent 50%);
    }

    /* ===========================
       Navigation
       =========================== */
    .nav {
      background: var(--pop-midnight-plum);
      border-bottom: 4px solid var(--pop-gilt-gold);
      padding: 0 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: relative;
      z-index: 10;
    }

    .nav::after {
      content: '';
      position: absolute;
      bottom: -12px;
      left: 0; right: 0;
      height: 8px;
      background: repeating-linear-gradient(
        90deg,
        var(--pop-carnival-red) 0px, var(--pop-carnival-red) 12px,
        var(--pop-bone-white) 12px, var(--pop-bone-white) 24px
      );
    }

    .nav-logo {
      font-family: 'Cinzel Decorative', serif;
      font-weight: 900;
      font-size: 1.4rem;
      color: var(--pop-gilt-gold);
      text-shadow: 1px 1px 0 var(--pop-tar-black);
      padding: 1rem 0;
    }

    .nav-links {
      list-style: none;
      display: flex;
      gap: 0;
    }

    .nav-links a {
      display: block;
      font-family: 'Rye', serif;
      font-size: 0.8rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      color: var(--pop-bone-white);
      padding: 1.2rem 1.4rem;
      transition: background 0.2s ease;
      border-left: 1px solid rgba(201,168,76,0.2);
    }

    .nav-links a:hover {
      background: var(--pop-carnival-red);
      color: var(--pop-buttercream);
    }

    /* ===========================
       Hero Section
       =========================== */
    .hero {
      background:
        radial-gradient(ellipse at center, rgba(244,165,192,0.15) 0%, transparent 70%),
        var(--pop-midnight-plum);
      text-align: center;
      padding: 7rem 2rem 6rem;
      position: relative;
      overflow: hidden;
      border-bottom: 6px solid var(--pop-gilt-gold);
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: repeating-conic-gradient(
        from 0deg at 50% 120%,
        rgba(201,168,76,0.03) 0deg 5deg,
        transparent 5deg 10deg
      );
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      color: var(--pop-bone-white);
      text-shadow:
        0 0 30px rgba(244,165,192,0.35),
        3px 3px 0 var(--pop-carnival-red);
      margin-bottom: 0.75rem;
      position: relative;
    }

    .hero .subtitle {
      font-family: 'Cinzel Decorative', serif;
      font-size: clamp(0.8rem, 2vw, 1.2rem);
      color: var(--pop-gilt-gold);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      margin-bottom: 1.5rem;
    }

    .hero .tagline {
      font-family: 'Lora', serif;
      font-style: italic;
      font-size: 1.1rem;
      color: var(--pop-cotton-candy);
      max-width: 550px;
      margin: 0 auto 2.5rem;
    }

    /* ===========================
       Button
       =========================== */
    .btn {
      display: inline-block;
      font-family: 'Rye', serif;
      font-size: 0.95rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--pop-buttercream);
      background: linear-gradient(180deg, var(--pop-carnival-red) 0%, #8B1A1F 100%);
      border: 3px solid var(--pop-gilt-gold);
      padding: 14px 36px;
      cursor: pointer;
      text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
      box-shadow:
        0 0 0 1px var(--pop-tar-black),
        4px 4px 0 var(--pop-tar-black);
      transition: all 0.2s ease;
    }

    .btn:hover {
      background: linear-gradient(180deg, var(--pop-bubblegum) 0%, var(--pop-carnival-red) 100%);
      color: var(--pop-buttercream);
      box-shadow: 0 0 0 1px var(--pop-tar-black), 2px 2px 0 var(--pop-tar-black);
      transform: translate(2px, 2px);
    }

    /* ===========================
       Section Divider
       =========================== */
    .divider {
      text-align: center;
      padding: 2rem 0;
      position: relative;
    }

    .divider::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 10%;
      right: 10%;
      height: 1px;
      background: linear-gradient(
        90deg,
        transparent 0%,
        var(--pop-gilt-gold) 20%,
        var(--pop-gilt-gold) 80%,
        transparent 100%
      );
    }

    .divider-icon {
      position: relative;
      display: inline-block;
      background: var(--pop-bone-white);
      padding: 0 1rem;
      font-size: 1.5rem;
      color: var(--pop-gilt-gold);
    }

    /* ===========================
       Ornate Frame Section
       =========================== */
    .ornate-frame {
      position: relative;
      background: var(--pop-bone-white);
      border: 2px solid var(--pop-gilt-gold);
      padding: 3rem 2.5rem;
      margin: 0 auto;
      max-width: 800px;
    }

    .ornate-frame::before {
      content: '';
      position: absolute;
      top: 10px; left: 10px; right: 10px; bottom: 10px;
      border: 1px solid var(--pop-gilt-gold);
      pointer-events: none;
    }

    .ornate-frame::after {
      content: '\2766';
      position: absolute;
      top: -14px;
      left: 50%;
      transform: translateX(-50%);
      font-size: 1.5rem;
      color: var(--pop-gilt-gold);
      background: var(--pop-bone-white);
      padding: 0 14px;
    }

    .ornate-frame h2 {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      text-align: center;
      color: var(--pop-carnival-red);
      font-size: 2rem;
      margin-bottom: 1.5rem;
    }

    .ornate-frame p {
      text-align: center;
      color: var(--pop-tar-black);
      max-width: 600px;
      margin: 0 auto;
    }

    /* ===========================
       Card Grid
       =========================== */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2.5rem;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 2rem;
    }

    .card {
      background: var(--pop-bone-white);
      border: 3px solid var(--pop-gilt-gold);
      border-radius: 4px;
      padding: 2rem;
      position: relative;
      box-shadow:
        0 0 0 1px var(--pop-tar-black),
        0 0 0 5px var(--pop-carnival-red),
        0 0 0 6px var(--pop-tar-black),
        6px 6px 0 var(--pop-tar-black);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow:
        0 0 0 1px var(--pop-tar-black),
        0 0 0 5px var(--pop-bubblegum),
        0 0 0 6px var(--pop-tar-black),
        8px 10px 0 var(--pop-tar-black);
    }

    .card::before {
      content: '';
      position: absolute;
      top: 8px; left: 8px; right: 8px; bottom: 8px;
      border: 1px solid rgba(201,168,76,0.4);
      pointer-events: none;
    }

    .card-icon {
      font-size: 2.5rem;
      text-align: center;
      margin-bottom: 1rem;
    }

    .card h3 {
      font-family: 'Cinzel Decorative', serif;
      font-weight: 700;
      text-align: center;
      color: var(--pop-carnival-red);
      margin-bottom: 0.75rem;
      font-size: 1.15rem;
    }

    .card p {
      text-align: center;
      font-size: 0.95rem;
      line-height: 1.7;
      color: var(--pop-tar-black);
    }

    /* ===========================
       Eyeball Decoration
       =========================== */
    .eye {
      width: 60px;
      height: 60px;
      border-radius: 50%;
      background: radial-gradient(
        circle at 50% 50%,
        var(--pop-tar-black) 20%,
        var(--pop-bruise-purple) 20%,
        var(--pop-bruise-purple) 38%,
        var(--pop-bone-white) 38%
      );
      box-shadow:
        0 0 0 3px var(--pop-tar-black),
        0 0 0 6px var(--pop-cotton-candy),
        0 0 0 8px var(--pop-tar-black);
      position: relative;
      display: inline-block;
      margin: 0 8px;
    }

    .eye::after {
      content: '';
      position: absolute;
      top: 18%;
      left: 55%;
      width: 10px;
      height: 10px;
      background: white;
      border-radius: 50%;
    }

    /* ===========================
       Dripping Text
       =========================== */
    .drip-text {
      font-family: 'Creepster', cursive;
      font-size: clamp(2rem, 5vw, 3.5rem);
      color: var(--pop-bubblegum);
      display: inline-block;
      position: relative;
      text-shadow:
        2px 2px 0 var(--pop-tar-black),
        -1px -1px 0 var(--pop-tar-black),
        1px -1px 0 var(--pop-tar-black),
        -1px 1px 0 var(--pop-tar-black);
    }

    .drip-text::after {
      content: '';
      position: absolute;
      bottom: -14px;
      left: 12%;
      width: 7px;
      height: 16px;
      background: var(--pop-bubblegum);
      border-radius: 0 0 50% 50%;
      box-shadow:
        28px 5px 0 0 var(--pop-bubblegum),
        62px -3px 0 0 var(--pop-bubblegum),
        100px 7px 0 0 var(--pop-bubblegum);
      animation: drip 2.5s ease-in-out infinite;
    }

    @keyframes drip {
      0%, 100% { transform: translateY(0); opacity: 1; }
      60% { transform: translateY(10px); opacity: 0.6; }
    }

    /* ===========================
       Carnival Banner
       =========================== */
    .banner {
      position: relative;
      display: inline-block;
      background: var(--pop-carnival-red);
      color: var(--pop-buttercream);
      font-family: 'Rye', serif;
      font-size: 1.2rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-align: center;
      padding: 0.8rem 2.5rem;
      text-shadow: 1px 1px 0 var(--pop-tar-black);
    }

    .banner::before {
      content: '';
      position: absolute;
      top: 0; left: -18px;
      border-top: 23px solid var(--pop-carnival-red);
      border-bottom: 23px solid var(--pop-carnival-red);
      border-left: 18px solid transparent;
    }

    .banner::after {
      content: '';
      position: absolute;
      top: 0; right: -18px;
      border-top: 23px solid var(--pop-carnival-red);
      border-bottom: 23px solid var(--pop-carnival-red);
      border-right: 18px solid transparent;
    }

    /* ===========================
       Sideshow Stripe Background
       =========================== */
    .stripe-section {
      background: repeating-linear-gradient(
        90deg,
        var(--pop-midnight-plum) 0px, var(--pop-midnight-plum) 50px,
        #3A2050 50px, #3A2050 100px
      );
      padding: 4rem 2rem;
      text-align: center;
    }

    .stripe-section h2 {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      color: var(--pop-gilt-gold);
      font-size: 2.2rem;
      text-shadow: 2px 2px 0 var(--pop-tar-black);
      margin-bottom: 1.5rem;
    }

    .stripe-section p {
      color: var(--pop-cotton-candy);
      max-width: 600px;
      margin: 0 auto;
    }

    /* ===========================
       Footer
       =========================== */
    .footer {
      background: var(--pop-tar-black);
      color: var(--pop-flesh-rose);
      text-align: center;
      padding: 3rem 2rem;
      border-top: 4px solid var(--pop-gilt-gold);
      position: relative;
    }

    .footer::before {
      content: '';
      position: absolute;
      top: -12px;
      left: 0; right: 0;
      height: 8px;
      background: repeating-linear-gradient(
        90deg,
        var(--pop-carnival-red) 0px, var(--pop-carnival-red) 12px,
        var(--pop-tar-black) 12px, var(--pop-tar-black) 24px
      );
    }

    .footer-title {
      font-family: 'Cinzel Decorative', serif;
      font-weight: 700;
      font-size: 1.1rem;
      color: var(--pop-gilt-gold);
      letter-spacing: 0.1em;
      margin-bottom: 0.5rem;
    }

    .footer p {
      font-size: 0.9rem;
      opacity: 0.7;
    }

    /* ===========================
       Utility / Spacing
       =========================== */
    .section-pad { padding: 4rem 2rem; }
    .text-center { text-align: center; }
    .mt-2 { margin-top: 2rem; }
    .mb-3 { margin-bottom: 3rem; }

    /* ===========================
       Responsive
       =========================== */
    @media (max-width: 768px) {
      .nav { flex-direction: column; padding: 1rem; }
      .nav-links { flex-wrap: wrap; justify-content: center; }
      .nav-links a { padding: 0.8rem 1rem; font-size: 0.75rem; border-left: none; }
      .hero { padding: 5rem 1.5rem 4rem; }
      .card-grid { grid-template-columns: 1fr; padding: 0 1.5rem; }
      .ornate-frame { margin: 0 1rem; padding: 2rem 1.5rem; }
      .banner { font-size: 1rem; padding: 0.7rem 2rem; }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav class="nav">
    <div class="nav-logo">Cabinet of Curiosities</div>
    <ul class="nav-links">
      <li><a href="#gallery">Gallery</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#oddities">Oddities</a></li>
      <li><a href="#visit">Visit</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <header class="hero">
    <p class="subtitle">Welcome to the</p>
    <h1>Cabinet of Curiosities</h1>
    <p class="tagline">Where the beautiful and the grotesque hold hands and dance beneath cotton-candy skies.</p>
    <a href="#gallery" class="btn">Enter the Gallery</a>
  </header>

  <!-- Divider -->
  <div class="divider">
    <span class="divider-icon">&#10048;</span>
  </div>

  <!-- Ornate Frame Section -->
  <section id="about" class="section-pad">
    <div class="ornate-frame">
      <h2>The Art of Dark Whimsy</h2>
      <p>
        Step inside a world where wide-eyed porcelain dolls preside over banquets of raw meat,
        where butterflies emerge from cracked skulls, and where the carousel never stops spinning.
        Pop Surrealism invites you to look closer at the beautiful things that unsettle you
        and find beauty in the things that make you look away.
      </p>
    </div>
  </section>

  <!-- Carnival Banner -->
  <div class="text-center section-pad">
    <span class="banner">Now Exhibiting</span>
  </div>

  <!-- Card Grid -->
  <section id="gallery" class="mb-3">
    <div class="card-grid">
      <div class="card">
        <div class="card-icon">&#128065;</div>
        <h3>The Watchers</h3>
        <p>Big-eyed figures peer from ornate frames, their gaze following you through the gallery. Innocence rendered with unsettling precision.</p>
      </div>
      <div class="card">
        <div class="card-icon">&#127922;</div>
        <h3>Carnival Nocturne</h3>
        <p>Sideshow banners flutter in a wind that smells of caramel and formaldehyde. Step right up to see the wonders within.</p>
      </div>
      <div class="card">
        <div class="card-icon">&#127800;</div>
        <h3>Flora Macabra</h3>
        <p>Roses bloom from ribcages. Mushrooms sprout from the pages of forgotten fairy tales. Nature, beautiful and indifferent.</p>
      </div>
    </div>
  </section>

  <!-- Drip Text + Eyes Section -->
  <section class="stripe-section">
    <div class="mb-3">
      <span class="eye"></span>
      <span class="eye"></span>
      <span class="eye"></span>
    </div>
    <h2>Dare to Look</h2>
    <p>
      The lowbrow tradition has always been about what the galleries refused to show.
      Underground comix, hot-rod pinstriping, tattoo flash, psychedelic posters --
      art made for the people, by the people, with no permission asked.
    </p>
    <div class="mt-2">
      <span class="drip-text">Sweet Dreams</span>
    </div>
  </section>

  <!-- Divider -->
  <div class="divider">
    <span class="divider-icon">&#9883;</span>
  </div>

  <!-- Second Ornate Frame -->
  <section id="oddities" class="section-pad">
    <div class="ornate-frame">
      <h2>Oddities &amp; Ephemera</h2>
      <p>
        Every artifact in this collection tells a story that polite society would rather forget.
        Vintage tin toys with sinister grins. Anatomical models in velvet-lined cases.
        Hand-painted sideshow banners promising impossible wonders.
        Collect them all -- if you dare.
      </p>
      <div class="text-center mt-2">
        <a href="#" class="btn">Browse Collection</a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="footer-title">Cabinet of Curiosities</div>
    <p>A Pop Surrealism design template. Beautiful yet unsettling, sweet yet sinister.</p>
  </footer>

</body>
</html>
```
