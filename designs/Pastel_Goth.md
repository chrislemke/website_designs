# Pastel Goth Design Reference

Pastel Goth is a subcultural aesthetic that fuses the soft, dreamy sweetness of pastel colors with the dark, macabre imagery of gothic subculture. Born on Tumblr around 2010-2012, it emerged from online communities that blended Japanese kawaii and Harajuku fashion sensibilities with Western goth motifs -- skulls, bats, crosses, pentagrams, coffins, crescent moons, and bones rendered in candy-soft lavenders, baby pinks, mint greens, and lilacs against a foundation of black. The aesthetic's philosophy centers on duality: the acceptance that softness and darkness, fragility and fierceness, cuteness and creepiness are not contradictions but complements. In web and UI design, Pastel Goth translates to dark backgrounds illuminated by pastel-colored elements, occult-inspired iconography used as decorative accents, dripping and melting visual effects, and typography that pairs elegant gothic serifs with bubbly rounded sans-serifs. The result is an interface that feels simultaneously inviting and unsettling -- a digital space where a sugar skull sits comfortably beside a pink bow.

---

## Visual Characteristics

### Core Design Traits

- **Pastel-on-dark contrast** -- soft lavender, baby pink, mint, and lilac tones set against deep charcoal or near-black backgrounds create an ethereal glow, as if the sweet colors are luminous objects floating in shadow
- **Gothic iconography in soft hues** -- skulls, crosses, crescent moons, bats, pentagrams, bones, coffins, and spiderwebs rendered in pastel tones rather than traditional harsh black, making them approachable and cute
- **Dripping and melting effects** -- paint drips, melting borders, and liquid edges evoking something sweet slowly dissolving into darkness; a signature visual motif of the aesthetic
- **Kawaii-goth fusion elements** -- cute characters with dark features (smiling ghosts, skulls with flower crowns, bats with heart-shaped eyes), mixing Japanese cute culture with Western macabre
- **Gradient transitions between light and dark** -- smooth gradients shifting from pastel pinks and purples into deep blacks and charcoals, embodying the core tension of the aesthetic
- **Star and sparkle accents** -- decorative stars, sparkles, and glitter effects scattered as atmospheric accents, softening gothic elements and adding a dreamy quality
- **Lace, fishnet, and texture overlays** -- semi-transparent patterns reminiscent of lace trim, fishnet fabric, or spiderweb motifs used as background textures or decorative borders
- **Sticker and badge motifs** -- design elements mimicking the look of vinyl stickers, enamel pins, and iron-on patches, referencing the physical craft culture around the aesthetic
- **Occult geometry** -- pentagrams, triple moons, alchemical symbols, and sacred geometry rendered with clean lines in pastel strokes as decorative accents
- **Soft glow and luminescence** -- pastel colors given a radiant quality through text-shadow and box-shadow effects on dark backgrounds, as if the elements emit their own light

### Design Principles

- Embrace the contradiction between soft and dark -- the tension is the aesthetic itself; neither side should dominate completely
- Black or near-black is the stage; pastels are the performers -- dark backgrounds let pastel elements glow with maximum impact
- Gothic motifs should feel approachable and playful, never genuinely threatening or disturbing
- Mix rounded, kawaii-inspired shapes with angular gothic typography for deliberate visual contrast
- Texture and imperfection add authenticity -- subtle noise, grain, or grunge overlays prevent the design from feeling too clinical
- Maintain a clear visual hierarchy even when using decorative elements generously
- Accessibility matters: ensure sufficient contrast between pastel text and dark backgrounds; pastel-on-pastel text must be avoided

---

## Color Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Void Black** | `#1A1A1A` | Primary background, deepest surface layer |
| **Coffin Gray** | `#2D2D2D` | Card backgrounds, elevated surfaces, secondary panels |
| **Tombstone** | `#4A4A4A` | Borders, dividers, muted UI elements, disabled states |
| **Spectral Lilac** | `#C8A2C8` | Primary accent, headings, interactive highlight color |
| **Ghost Lavender** | `#D8B4FE` | Secondary accent, hover states, decorative gradient endpoints |
| **Pale Orchid** | `#E9D5FF` | Light accent backgrounds, tag fills, soft highlights |
| **Crypt Pink** | `#F9A8D4` | Primary pink accent, buttons, links, call-to-action elements |
| **Baby Fang** | `#FBBDD9` | Secondary pink, notification badges, soft card accents |
| **Blush Bone** | `#FDE7F0` | Light pink backgrounds, card surfaces on light theme variants |
| **Hex Mint** | `#A7F3D0` | Tertiary accent, success states, decorative color contrast |
| **Witch Water** | `#99F6E4` | Alternate cool accent, hover effects, info badges |
| **Potion Blue** | `#BAE6FD` | Informational accents, secondary cool interactive elements |
| **Skull White** | `#F5F0F6` | Primary text on dark backgrounds, light theme surface color |
| **Bat Wing** | `#6B21A8` | Deep purple accent, active states, dark decorative elements |
| **Moon Glow** | `#FEF3C7` | Warning states, star accents, warm highlight sparkles |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --pg-bg-void: #1a1a1a;
  --pg-bg-coffin: #2d2d2d;
  --pg-bg-tombstone: #4a4a4a;

  /* Purple / Lavender family */
  --pg-lilac: #c8a2c8;
  --pg-lavender: #d8b4fe;
  --pg-orchid: #e9d5ff;
  --pg-bat-wing: #6b21a8;

  /* Pink family */
  --pg-pink: #f9a8d4;
  --pg-baby-pink: #fbbdd9;
  --pg-blush: #fde7f0;

  /* Mint / Cool family */
  --pg-mint: #a7f3d0;
  --pg-witch-water: #99f6e4;
  --pg-potion-blue: #bae6fd;

  /* Neutrals and warm accents */
  --pg-white: #f5f0f6;
  --pg-moon: #fef3c7;

  /* Glows (used for box-shadow and text-shadow) */
  --pg-glow-lilac: 0 0 12px rgba(200, 162, 200, 0.5), 0 0 40px rgba(200, 162, 200, 0.15);
  --pg-glow-pink: 0 0 12px rgba(249, 168, 212, 0.5), 0 0 40px rgba(249, 168, 212, 0.15);
  --pg-glow-mint: 0 0 12px rgba(167, 243, 208, 0.5), 0 0 40px rgba(167, 243, 208, 0.15);

  /* Borders */
  --pg-border: 1px solid rgba(200, 162, 200, 0.2);
  --pg-border-bright: 1px solid rgba(200, 162, 200, 0.5);
}
```

---

## Typography

### Recommended Google Fonts

| Font | Style | Best For |
|------|-------|----------|
| **Comfortaa** | Rounded, wide, geometric | Headlines, display text, hero sections |
| **Quicksand** | Rounded geometric sans-serif | Body text, general UI, approachable readability |
| **Fredoka** | Bubbly, bold, playful | Headings, buttons, call-to-action labels |
| **UnifrakturCook** | Blackletter / Fraktur | Gothic accent headings, decorative logo text (use sparingly) |
| **Satisfy** | Casual cursive script | Accent taglines, decorative quotes, handwritten flourishes |
| **Nunito** | Rounded sans-serif | Clean body text, navigation, alternative to Quicksand |
| **Permanent Marker** | Handwritten, bold marker | Grunge accent headings, rebellious emphasis text |
| **Bangers** | Comic-book bold | Impact headings, sticker-style labels, punk-cute elements |
| **Patrick Hand** | Casual handwriting | Personal notes, diary-style sections, annotation labels |
| **Sacramento** | Elegant flowing script | Decorative flourishes, romantic gothic accents |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Comfortaa** (700) | **Quicksand** (400) | Classic pastel goth: bubbly, rounded, approachable |
| **Fredoka** (600) | **Nunito** (400) | Playful and bold, sticker-shop aesthetic |
| **UnifrakturCook** (700) | **Quicksand** (400) | Maximum contrast: gothic blackletter meets kawaii softness |
| **Bangers** (400) | **Patrick Hand** (400) | Zine-inspired, DIY punk-cute mashup |
| **Satisfy** (400) | **Quicksand** (400) | Romantic goth, dreamy and elegant with modern body text |

### CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Comfortaa:wght@400;600;700&family=Quicksand:wght@400;500;600&family=UnifrakturCook:wght@700&family=Satisfy&display=swap');

/* Headings -- bubbly and rounded */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Comfortaa', 'Nunito', sans-serif;
  font-weight: 700;
  color: var(--pg-lavender);
  line-height: 1.3;
  letter-spacing: 0.02em;
}

/* Display / Hero text with pastel glow */
.pg-display {
  font-family: 'Comfortaa', sans-serif;
  font-size: clamp(2.5rem, 6vw, 4.5rem);
  font-weight: 700;
  color: var(--pg-pink);
  text-shadow: 0 0 20px rgba(249, 168, 212, 0.5), 0 0 60px rgba(249, 168, 212, 0.15);
}

/* Gothic accent heading -- use sparingly for decorative impact */
.pg-gothic {
  font-family: 'UnifrakturCook', cursive;
  font-weight: 700;
  font-size: 2rem;
  color: var(--pg-lilac);
  text-shadow: 0 0 15px rgba(200, 162, 200, 0.4);
}

/* Body text -- soft and rounded */
body {
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--pg-white);
  font-weight: 400;
}

/* Handwritten accent text */
.pg-handwritten {
  font-family: 'Satisfy', cursive;
  font-size: 1.4rem;
  color: var(--pg-pink);
}

/* UI labels */
.pg-label {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--pg-lilac);
}
```

---

## Layout Principles

- **Dark canvas, pastel illumination** -- use near-black backgrounds (`#1A1A1A` or `#2D2D2D`) as the primary canvas; pastel-colored cards, text, and accents float above like luminous objects in shadow
- **Centered, medium-width layouts** -- keep content at 800-1000px max-width to maintain an intimate, curated feel befitting the subcultural origin
- **Generous vertical spacing** -- sections should breathe with 60-100px of vertical padding; the mood is dreamy and unhurried, not cramped or dense
- **Rounded containers with tinted shadows** -- use border-radius of 12-20px on cards and containers; shadows should be tinted with purple or pink (`rgba(200, 162, 200, 0.15)`) rather than pure black
- **Card-based content grids** -- rounded cards arranged in 2-3 column grids for features, products, or portfolio items, each with a pastel accent gradient top-border
- **Decorative dividers** -- use gothic-themed section breaks: drip effects, crescent moons, skull symbols, or lace-pattern borders between major content areas
- **Sticker-scatter compositions** -- decorative elements positioned semi-randomly to mimic stickers placed on a notebook or laptop, adding personality
- **Responsive stacking** -- on mobile, stack cards vertically, preserve rounded corners and generous padding, and scale down decorative elements while keeping the dark-to-pastel contrast intact

---

## CSS / Design Techniques

### Pastel Goth Card Component

```css
.pg-card {
  background: rgba(45, 45, 45, 0.8);
  border: 2px solid rgba(200, 162, 200, 0.2);
  border-radius: 16px;
  padding: 28px;
  position: relative;
  backdrop-filter: blur(8px);
  transition: border-color 0.3s ease, box-shadow 0.3s ease, transform 0.3s ease;
}

.pg-card:hover {
  border-color: rgba(249, 168, 212, 0.5);
  box-shadow: var(--pg-glow-pink);
  transform: translateY(-4px);
}

/* Decorative skull accent in corner */
.pg-card::before {
  content: '\2620';
  position: absolute;
  top: -12px;
  right: 20px;
  font-size: 1.4rem;
  background: var(--pg-bg-void);
  padding: 0 8px;
  color: var(--pg-lavender);
}

/* Card grid layout */
.pg-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
}
```

### Pastel Goth Button

```css
.pg-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: linear-gradient(135deg, var(--pg-pink), var(--pg-lavender));
  color: var(--pg-bg-void);
  border: none;
  border-radius: 50px;
  padding: 14px 36px;
  font-family: 'Comfortaa', sans-serif;
  font-weight: 700;
  font-size: 0.9rem;
  letter-spacing: 0.04em;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(249, 168, 212, 0.3);
}

.pg-button:hover {
  box-shadow: var(--pg-glow-pink);
  transform: translateY(-2px);
  filter: brightness(1.1);
}

/* Ghost / outline variant */
.pg-button--ghost {
  background: transparent;
  color: var(--pg-pink);
  border: 2px solid var(--pg-pink);
  box-shadow: none;
}

.pg-button--ghost:hover {
  background: rgba(249, 168, 212, 0.1);
  box-shadow: var(--pg-glow-pink);
}

/* Mint variant */
.pg-button--mint {
  background: linear-gradient(135deg, var(--pg-mint), var(--pg-witch-water));
}

.pg-button--mint:hover {
  box-shadow: var(--pg-glow-mint);
}
```

### Navigation Bar

```css
.pg-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 16px 32px;
  background: rgba(26, 26, 26, 0.9);
  backdrop-filter: blur(12px);
  border-bottom: 2px solid rgba(200, 162, 200, 0.15);
}

.pg-nav__logo {
  font-family: 'UnifrakturCook', cursive;
  font-weight: 700;
  font-size: 1.4rem;
  color: var(--pg-lavender);
  text-decoration: none;
  text-shadow: 0 0 10px rgba(216, 180, 254, 0.4);
}

.pg-nav__links {
  display: flex;
  gap: 8px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.pg-nav__links a {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.85rem;
  color: var(--pg-white);
  text-decoration: none;
  padding: 8px 18px;
  border-radius: 50px;
  transition: all 0.2s ease;
}

.pg-nav__links a:hover,
.pg-nav__links a.active {
  background: rgba(249, 168, 212, 0.15);
  color: var(--pg-pink);
}
```

### Hero Section

```css
.pg-hero {
  position: relative;
  min-height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 32px;
  background: var(--pg-bg-void);
  overflow: hidden;
}

/* Gradient orb background glow */
.pg-hero::before {
  content: '';
  position: absolute;
  top: 20%;
  left: 50%;
  transform: translateX(-50%);
  width: 600px;
  height: 600px;
  background: radial-gradient(
    circle,
    rgba(200, 162, 200, 0.15) 0%,
    rgba(249, 168, 212, 0.08) 40%,
    transparent 70%
  );
  border-radius: 50%;
  pointer-events: none;
  filter: blur(60px);
}

/* Subtle starfield overlay */
.pg-hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    radial-gradient(1px 1px at 15% 25%, rgba(216, 180, 254, 0.4) 0%, transparent 100%),
    radial-gradient(1px 1px at 45% 65%, rgba(249, 168, 212, 0.3) 0%, transparent 100%),
    radial-gradient(1px 1px at 75% 15%, rgba(167, 243, 208, 0.3) 0%, transparent 100%),
    radial-gradient(1.5px 1.5px at 85% 75%, rgba(216, 180, 254, 0.3) 0%, transparent 100%),
    radial-gradient(1px 1px at 25% 85%, rgba(249, 168, 212, 0.3) 0%, transparent 100%);
  pointer-events: none;
  z-index: 1;
}

.pg-hero__content {
  position: relative;
  z-index: 2;
  max-width: 700px;
}

.pg-hero__content h1 {
  font-size: clamp(2.5rem, 6vw, 4.5rem);
  color: var(--pg-lavender);
  text-shadow: 0 0 30px rgba(216, 180, 254, 0.4), 0 0 80px rgba(216, 180, 254, 0.1);
  margin-bottom: 1rem;
}

.pg-hero__content p {
  font-size: 1.1rem;
  color: rgba(245, 240, 246, 0.7);
  max-width: 550px;
  margin: 0 auto 2.5rem;
  line-height: 1.8;
}

@media (max-width: 768px) {
  .pg-hero {
    min-height: auto;
    padding: 60px 20px;
  }
}
```

### Drip Divider

```css
.pg-drip-divider {
  position: relative;
  height: 40px;
  overflow: hidden;
}

.pg-drip-divider::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(90deg, var(--pg-lavender), var(--pg-pink), var(--pg-mint), var(--pg-lavender));
}

.pg-drip-divider::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 40px;
  background:
    radial-gradient(ellipse 12px 20px at 10% 0%, var(--pg-lavender) 50%, transparent 50%),
    radial-gradient(ellipse 8px 28px at 25% 0%, var(--pg-pink) 50%, transparent 50%),
    radial-gradient(ellipse 10px 16px at 42% 0%, var(--pg-mint) 50%, transparent 50%),
    radial-gradient(ellipse 14px 24px at 60% 0%, var(--pg-lavender) 50%, transparent 50%),
    radial-gradient(ellipse 8px 32px at 78% 0%, var(--pg-pink) 50%, transparent 50%),
    radial-gradient(ellipse 10px 18px at 92% 0%, var(--pg-mint) 50%, transparent 50%);
  pointer-events: none;
}
```

### Gothic Badge / Tag Component

```css
.pg-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  background: rgba(200, 162, 200, 0.12);
  color: var(--pg-lavender);
  padding: 6px 14px;
  border-radius: 50px;
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  letter-spacing: 0.04em;
  border: 1px solid rgba(200, 162, 200, 0.2);
}

.pg-badge--pink {
  background: rgba(249, 168, 212, 0.12);
  color: var(--pg-pink);
  border-color: rgba(249, 168, 212, 0.2);
}

.pg-badge--mint {
  background: rgba(167, 243, 208, 0.12);
  color: var(--pg-mint);
  border-color: rgba(167, 243, 208, 0.2);
}

/* Sticker variant with slight rotation and dashed border */
.pg-badge--sticker {
  transform: rotate(-3deg);
  box-shadow: 2px 3px 6px rgba(0, 0, 0, 0.3);
  border: 2px dashed rgba(200, 162, 200, 0.3);
}
```

### Testimonial / Quote Block

```css
.pg-quote {
  background: rgba(45, 45, 45, 0.6);
  border: 2px solid rgba(200, 162, 200, 0.15);
  border-radius: 20px;
  padding: 36px 32px;
  position: relative;
  text-align: center;
}

/* Decorative opening quotation mark */
.pg-quote::before {
  content: '\201C';
  position: absolute;
  top: 12px;
  left: 20px;
  font-size: 3rem;
  color: var(--pg-lavender);
  opacity: 0.4;
  line-height: 1;
  font-family: Georgia, serif;
}

.pg-quote blockquote {
  font-family: 'Satisfy', cursive;
  font-size: 1.3rem;
  color: var(--pg-pink);
  line-height: 1.6;
  margin: 0 0 16px;
  padding: 0;
  border: none;
}

.pg-quote cite {
  font-family: 'Quicksand', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--pg-lilac);
  font-style: normal;
  letter-spacing: 0.06em;
}

/* Skull icon before citation */
.pg-quote cite::before {
  content: '\2620 ';
}
```

### Pastel Goth Form Input

```css
.pg-input {
  width: 100%;
  background: rgba(45, 45, 45, 0.6);
  border: 2px solid rgba(200, 162, 200, 0.2);
  border-radius: 50px;
  padding: 14px 24px;
  font-family: 'Quicksand', sans-serif;
  font-size: 0.95rem;
  color: var(--pg-white);
  outline: none;
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

.pg-input::placeholder {
  color: rgba(200, 162, 200, 0.4);
}

.pg-input:focus {
  border-color: var(--pg-pink);
  box-shadow: var(--pg-glow-pink);
}

/* Textarea variant with reduced border-radius */
.pg-input--textarea {
  border-radius: 16px;
  resize: vertical;
  min-height: 120px;
}
```

---

## Design Do's and Don'ts

### Do's

- Use a black or near-black foundation and layer pastel colors on top for maximum ethereal contrast
- Render gothic motifs (skulls, bats, crosses, moons) in pastel colors to keep them approachable and creepy-cute
- Apply generous border-radius (12-20px on cards, 50px on buttons and badges) for the soft, bubbly feel
- Mix rounded sans-serif body fonts (Quicksand, Nunito) with occasional blackletter display fonts (UnifrakturCook) for tonal contrast
- Use subtle pastel glow effects via `box-shadow` and `text-shadow` on dark backgrounds for luminescence
- Add grunge textures, noise overlays, or distressed edges for a soft-grunge layer of authenticity
- Include decorative elements like stickers, badges, and scattered gothic icons to inject personality
- Use pastel gradients (lavender-to-pink, pink-to-mint) on buttons and accent borders for depth
- Tint all shadows with purple or pink (`rgba(200, 162, 200, 0.15)`) rather than pure black

### Don'ts

- Use a plain white background -- it strips away the gothic darkness that is half of the aesthetic
- Make gothic symbols look genuinely scary or disturbing -- the mood should be cute, not horrifying
- Overuse blackletter fonts -- they become unreadable quickly; reserve them for short display text and logos
- Apply too many saturated or neon colors -- pastels should feel soft and muted, not electric or cyberpunk
- Mix pastels with warm earth tones or browns -- stick to cool-toned and pink-family pastels with black
- Create overly clean, corporate-feeling layouts -- the aesthetic thrives on personality, craft, and imperfection
- Use harsh, angular shapes exclusively -- the kawaii side of the aesthetic demands roundness and softness
- Ignore accessibility -- low-contrast pastel-on-pastel text is difficult to read; ensure WCAG compliance for body text
- Combine too many pastel colors at once without a dominant anchor -- pick 2-3 core pastels and use black as the unifying canvas

---

## Related Aesthetics

| Aesthetic | Relationship to Pastel Goth |
|-----------|----------------------------|
| **Cutecore** | Shares the kawaii influence, rounded shapes, and playful iconography; Cutecore lacks the gothic darkness and macabre motifs entirely |
| **Coquette** | Overlaps in pastel pinks, bows, and feminine softness; Coquette is romantic and flirty where Pastel Goth is morbid and subcultural |
| **Danish Pastel** | Both use soft pastel palettes, but Danish Pastel is minimalist Scandinavian while Pastel Goth embraces maximalist gothic decoration |
| **Dark Academia** | Shares appreciation for dark, moody atmospheres; Dark Academia is intellectual and classical where Pastel Goth is playful and internet-native |
| **Cyberpunk** | Both use glowing elements on dark backgrounds; Cyberpunk is neon, angular, and dystopian while Pastel Goth is soft, rounded, and subcultural |
| **Dreamcore** | Overlaps in ethereal, surreal quality and pastel tones; Dreamcore leans into uncanny liminal spaces rather than gothic iconography |
| **Whimsigothic** | Shares occult and mystical symbols; Whimsigothic leans more toward witchcraft, celestial themes, and warmer jewel tones |
| **Goblincore** | Both subvert conventional beauty and embrace the macabre; Goblincore is earthy and natural while Pastel Goth is sugary and digital |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pastel Goth Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Comfortaa:wght@400;600;700&family=Quicksand:wght@400;500;600&family=UnifrakturCook:wght@700&family=Satisfy&display=swap" rel="stylesheet">
  <style>
    :root {
      --pg-bg-void: #1a1a1a;
      --pg-bg-coffin: #2d2d2d;
      --pg-bg-tombstone: #4a4a4a;
      --pg-lilac: #c8a2c8;
      --pg-lavender: #d8b4fe;
      --pg-orchid: #e9d5ff;
      --pg-bat-wing: #6b21a8;
      --pg-pink: #f9a8d4;
      --pg-baby-pink: #fbbdd9;
      --pg-blush: #fde7f0;
      --pg-mint: #a7f3d0;
      --pg-witch-water: #99f6e4;
      --pg-potion-blue: #bae6fd;
      --pg-white: #f5f0f6;
      --pg-moon: #fef3c7;
      --pg-glow-lilac: 0 0 12px rgba(200, 162, 200, 0.5), 0 0 40px rgba(200, 162, 200, 0.15);
      --pg-glow-pink: 0 0 12px rgba(249, 168, 212, 0.5), 0 0 40px rgba(249, 168, 212, 0.15);
      --pg-glow-mint: 0 0 12px rgba(167, 243, 208, 0.5), 0 0 40px rgba(167, 243, 208, 0.15);
    }

    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--pg-bg-void);
      color: var(--pg-white);
      font-family: 'Quicksand', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Comfortaa', sans-serif;
      font-weight: 700;
      line-height: 1.3;
    }

    /* -- Navigation -- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 16px 32px;
      border-bottom: 2px solid rgba(200, 162, 200, 0.12);
    }

    nav a.logo {
      font-family: 'UnifrakturCook', cursive;
      font-weight: 700;
      font-size: 1.5rem;
      color: var(--pg-lavender);
      text-decoration: none;
      text-shadow: 0 0 10px rgba(216, 180, 254, 0.4);
    }

    nav ul {
      display: flex;
      gap: 6px;
      list-style: none;
    }

    nav ul a {
      font-family: 'Quicksand', sans-serif;
      font-weight: 600;
      color: var(--pg-white);
      text-decoration: none;
      font-size: 0.85rem;
      padding: 8px 18px;
      border-radius: 50px;
      transition: all 0.2s ease;
    }

    nav ul a:hover {
      background: rgba(249, 168, 212, 0.12);
      color: var(--pg-pink);
    }

    /* -- Hero Section -- */
    .hero {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 85vh;
      padding: 80px 32px;
      overflow: hidden;
    }

    /* Gradient orb glow */
    .hero::before {
      content: '';
      position: absolute;
      top: 15%;
      left: 50%;
      transform: translateX(-50%);
      width: 500px;
      height: 500px;
      background: radial-gradient(circle, rgba(200, 162, 200, 0.12) 0%, rgba(249, 168, 212, 0.06) 40%, transparent 70%);
      border-radius: 50%;
      pointer-events: none;
      filter: blur(60px);
    }

    /* Starfield sparkles */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background-image:
        radial-gradient(1.5px 1.5px at 10% 20%, rgba(216, 180, 254, 0.3) 0%, transparent 100%),
        radial-gradient(1px 1px at 30% 70%, rgba(249, 168, 212, 0.25) 0%, transparent 100%),
        radial-gradient(1px 1px at 55% 10%, rgba(167, 243, 208, 0.25) 0%, transparent 100%),
        radial-gradient(1.5px 1.5px at 80% 60%, rgba(216, 180, 254, 0.3) 0%, transparent 100%),
        radial-gradient(1px 1px at 90% 30%, rgba(249, 168, 212, 0.2) 0%, transparent 100%),
        radial-gradient(1px 1px at 20% 90%, rgba(167, 243, 208, 0.2) 0%, transparent 100%);
      pointer-events: none;
      z-index: 1;
    }

    .hero-content {
      position: relative;
      z-index: 2;
      max-width: 650px;
    }

    .hero-motif {
      font-size: 3rem;
      margin-bottom: 1rem;
      display: block;
    }

    .hero h1 {
      font-size: clamp(2.2rem, 5.5vw, 4rem);
      color: var(--pg-lavender);
      text-shadow: 0 0 25px rgba(216, 180, 254, 0.4), 0 0 70px rgba(216, 180, 254, 0.1);
      margin-bottom: 1rem;
    }

    .hero .subtitle {
      font-family: 'Satisfy', cursive;
      font-size: 1.4rem;
      color: var(--pg-pink);
      margin-bottom: 1rem;
    }

    .hero p {
      color: rgba(245, 240, 246, 0.65);
      font-size: 1.05rem;
      margin-bottom: 2.5rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: linear-gradient(135deg, var(--pg-pink), var(--pg-lavender));
      color: var(--pg-bg-void);
      border: none;
      border-radius: 50px;
      padding: 14px 36px;
      font-family: 'Comfortaa', sans-serif;
      font-weight: 700;
      font-size: 0.9rem;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 4px 20px rgba(249, 168, 212, 0.3);
    }

    .btn:hover {
      box-shadow: 0 0 12px rgba(249, 168, 212, 0.5), 0 0 40px rgba(249, 168, 212, 0.15);
      transform: translateY(-2px);
    }

    .btn--ghost {
      background: transparent;
      color: var(--pg-pink);
      border: 2px solid var(--pg-pink);
      box-shadow: none;
      margin-left: 12px;
    }

    .btn--ghost:hover {
      background: rgba(249, 168, 212, 0.1);
      box-shadow: 0 0 12px rgba(249, 168, 212, 0.3);
    }

    /* -- Drip Divider -- */
    .drip {
      position: relative;
      height: 40px;
      overflow: hidden;
    }

    .drip::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 3px;
      background: linear-gradient(90deg, var(--pg-lavender), var(--pg-pink), var(--pg-mint), var(--pg-lavender));
    }

    .drip::after {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 40px;
      background:
        radial-gradient(ellipse 10px 18px at 8% 0%, var(--pg-lavender) 50%, transparent 50%),
        radial-gradient(ellipse 6px 26px at 22% 0%, var(--pg-pink) 50%, transparent 50%),
        radial-gradient(ellipse 8px 14px at 40% 0%, var(--pg-mint) 50%, transparent 50%),
        radial-gradient(ellipse 12px 22px at 58% 0%, var(--pg-lavender) 50%, transparent 50%),
        radial-gradient(ellipse 6px 30px at 74% 0%, var(--pg-pink) 50%, transparent 50%),
        radial-gradient(ellipse 8px 16px at 90% 0%, var(--pg-mint) 50%, transparent 50%);
      pointer-events: none;
    }

    /* -- Features Section -- */
    .features {
      padding: 60px 32px 80px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--pg-pink);
      margin-bottom: 8px;
    }

    .features .section-sub {
      text-align: center;
      font-family: 'Satisfy', cursive;
      color: var(--pg-lilac);
      font-size: 1.1rem;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
    }

    .feature {
      background: rgba(45, 45, 45, 0.7);
      border: 2px solid rgba(200, 162, 200, 0.15);
      border-radius: 16px;
      padding: 28px;
      position: relative;
      transition: border-color 0.3s, box-shadow 0.3s, transform 0.3s;
    }

    .feature:hover {
      border-color: rgba(249, 168, 212, 0.4);
      box-shadow: var(--pg-glow-pink);
      transform: translateY(-3px);
    }

    .feature-icon {
      font-size: 2rem;
      margin-bottom: 12px;
      display: block;
    }

    .feature-badge {
      display: inline-block;
      background: rgba(200, 162, 200, 0.12);
      color: var(--pg-lavender);
      padding: 4px 12px;
      border-radius: 50px;
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 0.06em;
      margin-bottom: 12px;
      border: 1px solid rgba(200, 162, 200, 0.2);
    }

    .feature h3 {
      font-size: 1.15rem;
      color: var(--pg-lavender);
      margin-bottom: 8px;
    }

    .feature p {
      color: rgba(245, 240, 246, 0.6);
      font-size: 0.9rem;
      line-height: 1.6;
    }

    /* -- Testimonial Section -- */
    .testimonial {
      padding: 60px 32px 80px;
      max-width: 700px;
      margin: 0 auto;
      text-align: center;
    }

    .testimonial-card {
      background: rgba(45, 45, 45, 0.5);
      border: 2px solid rgba(200, 162, 200, 0.12);
      border-radius: 20px;
      padding: 40px 36px;
      position: relative;
    }

    .testimonial-card::before {
      content: '\201C';
      position: absolute;
      top: 12px;
      left: 24px;
      font-size: 3.5rem;
      color: var(--pg-lavender);
      opacity: 0.3;
      line-height: 1;
      font-family: Georgia, serif;
    }

    .testimonial-card blockquote {
      font-family: 'Satisfy', cursive;
      font-size: 1.3rem;
      color: var(--pg-pink);
      line-height: 1.7;
      margin-bottom: 20px;
    }

    .testimonial-card cite {
      font-family: 'Quicksand', sans-serif;
      font-size: 0.85rem;
      font-weight: 600;
      color: var(--pg-lilac);
      font-style: normal;
    }

    .testimonial-card cite::before {
      content: '\2620 ';
    }

    /* -- CTA / Newsletter Section -- */
    .cta {
      text-align: center;
      padding: 60px 32px 80px;
      max-width: 600px;
      margin: 0 auto;
    }

    .cta h2 {
      font-size: 1.8rem;
      color: var(--pg-mint);
      text-shadow: 0 0 15px rgba(167, 243, 208, 0.3);
      margin-bottom: 8px;
    }

    .cta p {
      color: rgba(245, 240, 246, 0.6);
      margin-bottom: 2rem;
    }

    .cta-form {
      display: flex;
      gap: 12px;
      max-width: 460px;
      margin: 0 auto;
    }

    .cta-form input {
      flex: 1;
      background: rgba(45, 45, 45, 0.6);
      border: 2px solid rgba(200, 162, 200, 0.2);
      border-radius: 50px;
      padding: 14px 24px;
      font-family: 'Quicksand', sans-serif;
      font-size: 0.9rem;
      color: var(--pg-white);
      outline: none;
      transition: border-color 0.3s, box-shadow 0.3s;
    }

    .cta-form input::placeholder {
      color: rgba(200, 162, 200, 0.35);
    }

    .cta-form input:focus {
      border-color: var(--pg-pink);
      box-shadow: var(--pg-glow-pink);
    }

    .cta-form .btn { white-space: nowrap; }

    /* -- Footer -- */
    footer {
      border-top: 2px solid rgba(200, 162, 200, 0.1);
      text-align: center;
      padding: 32px;
    }

    footer .footer-icons {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-bottom: 16px;
      font-size: 1.2rem;
    }

    footer .footer-icons a {
      color: var(--pg-lilac);
      text-decoration: none;
      transition: color 0.2s, text-shadow 0.2s;
    }

    footer .footer-icons a:hover {
      color: var(--pg-pink);
      text-shadow: 0 0 8px rgba(249, 168, 212, 0.4);
    }

    footer .gothic-text {
      font-family: 'UnifrakturCook', cursive;
      color: var(--pg-lilac);
      font-size: 1rem;
      margin-bottom: 4px;
    }

    footer p {
      color: rgba(245, 240, 246, 0.4);
      font-size: 0.8rem;
    }

    /* -- Responsive -- */
    @media (max-width: 768px) {
      nav { padding: 12px 20px; }
      nav ul { gap: 4px; }
      nav ul a { padding: 6px 12px; font-size: 0.8rem; }
      .hero { min-height: auto; padding: 60px 20px; }
      .features { padding: 40px 20px 60px; }
      .testimonial { padding: 40px 20px 60px; }
      .cta { padding: 40px 20px 60px; }
      .cta-form { flex-direction: column; }
      .btn--ghost { margin-left: 0; margin-top: 8px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Nocturne</a>
    <ul>
      <li><a href="#">Shop</a></li>
      <li><a href="#">Lookbook</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <span class="hero-motif">&#9760;</span>
      <h1>Soft Darkness, Sweet Decay</h1>
      <p class="subtitle">where sugar skulls meet lavender dreams</p>
      <p>Handcrafted accessories where kawaii meets the crypt. Enamel pins, chokers, and charms for the pastel-hearted creature of the night.</p>
      <div>
        <a href="#" class="btn">Browse Collection</a>
        <a href="#" class="btn btn--ghost">Our Story</a>
      </div>
    </div>
  </section>

  <div class="drip"></div>

  <section class="features">
    <h2>New Arrivals</h2>
    <p class="section-sub">freshly risen from the grave</p>
    <div class="features-grid">
      <div class="feature">
        <span class="feature-icon">&#128128;</span>
        <span class="feature-badge">Limited Edition</span>
        <h3>Sugar Skull Pin Set</h3>
        <p>A collection of five enamel pins featuring candy-colored skulls adorned with flower crowns, bows, and tiny bat wings. Soft enamel on black nickel.</p>
      </div>
      <div class="feature">
        <span class="feature-icon">&#127768;</span>
        <span class="feature-badge">Bestseller</span>
        <h3>Crescent Moon Choker</h3>
        <p>Lavender velvet choker with a dangling crescent moon pendant in iridescent finish. Adjustable chain with a tiny coffin clasp detail.</p>
      </div>
      <div class="feature">
        <span class="feature-icon">&#128420;</span>
        <span class="feature-badge">Pre-Order</span>
        <h3>Bat Wing Earrings</h3>
        <p>Translucent resin bat wings in gradient pink-to-purple with embedded glitter. Hypoallergenic surgical steel hooks for sensitive ears.</p>
      </div>
    </div>
  </section>

  <div class="drip"></div>

  <section class="testimonial">
    <div class="testimonial-card">
      <blockquote>I wear the skull pin set every single day. People always stop me to ask where I got them. The quality is absolutely beautiful and perfectly creepy-cute.</blockquote>
      <cite>Lilith M. -- Verified Customer</cite>
    </div>
  </section>

  <div class="drip"></div>

  <section class="cta">
    <h2>Join the Coven</h2>
    <p>Subscribe to our newsletter for early access to new drops, exclusive discount spells, and behind-the-scenes peeks into our haunted workshop.</p>
    <div class="cta-form">
      <input type="email" placeholder="your@email.hex">
      <a href="#" class="btn">Subscribe</a>
    </div>
  </section>

  <footer>
    <div class="footer-icons">
      <a href="#">&#9760;</a>
      <a href="#">&#128420;</a>
      <a href="#">&#127768;</a>
      <a href="#">&#10013;</a>
    </div>
    <p class="gothic-text">Nocturne</p>
    <p>Handcrafted with love and a little darkness &middot; Est. 2019</p>
  </footer>
</body>
</html>
```
