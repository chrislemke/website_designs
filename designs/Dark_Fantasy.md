# Dark Fantasy Design Reference

## Overview

Dark Fantasy is a brooding, mythical aesthetic that fuses medieval sword-and-sorcery imagery with gothic horror sensibilities. Its roots stretch back to 18th-century Gothic literature and Romantic-era painting, but it surged into mainstream visual culture through video games like Dark Souls, Elden Ring, and The Witcher, as well as film and television adaptations such as Game of Thrones and Pan's Labyrinth. Visually, the aesthetic is defined by permanently foreboding atmospheres: mist-shrouded landscapes, crumbling stone fortresses, enchanted forests choked with shadow, and the faint glow of runes or torchlight piercing the darkness. In web and UI design, Dark Fantasy translates to deeply saturated dark backgrounds, ornate metallic accents in gold and silver, weathered textures reminiscent of parchment, stone, and hammered iron, and typography drawn from medieval manuscripts and Roman inscriptions. The goal is to immerse the viewer in a world where danger lurks in every shadow, magic carries a terrible price, and beauty is always intertwined with decay.

---

## Visual Characteristics

### Core Design Traits

- **Abyssal dark backgrounds**: Near-black surfaces with cool or neutral undertones (deep charcoal, midnight blue-black, void purple) that evoke caverns, moonless nights, and ruined halls
- **Metallic accent hierarchy**: Antique gold for primary accents, tarnished silver for secondary elements, and burnished copper or bronze for tertiary details, all rendered with subtle gradient sheen to simulate forged metal
- **Crimson and blood-red punctuation**: Deep reds used sparingly for emphasis, danger indicators, call-to-action elements, and decorative flourishes, suggesting fire, blood, and arcane power
- **Weathered and distressed textures**: Stone grain, cracked leather, hammered metal, scorched parchment, and bark overlays applied to surfaces for tactile depth and a sense of ancient age
- **Gothic architectural framing**: Pointed arches, ribbed vault patterns, ornamental tracery, and gargoyle-inspired decorative elements used to frame content sections and navigation
- **Runic and arcane ornamentation**: Decorative borders, dividers, and background patterns inspired by Norse runes, Celtic knotwork, alchemical symbols, and magical sigils
- **Atmospheric lighting effects**: Volumetric fog overlays, ember particle effects, torchlight radial gradients, and moonlight rim-lighting that create depth and a sense of environmental immersion
- **Dramatic silhouettes and negative space**: Castle spires, twisted trees, dragon wings, and mountain ridgelines used as compositional framing devices in hero sections and backgrounds
- **Desaturated, moody imagery**: Photos and illustrations processed with low saturation, raised shadows, and cool-toned color grading to maintain the somber, otherworldly atmosphere
- **Ornate border and corner details**: Intricate filigree, wrought-iron scrollwork, and hand-drawn flourishes adorning cards, panels, and section boundaries

### Design Principles

- **Darkness as foundation**: Let deep, near-black backgrounds dominate; light should feel scarce and precious, drawn from fire, moonlight, or magic
- **Restrained opulence**: Metallic and crimson accents are most powerful when used sparingly against vast dark expanses; overcrowding diminishes their impact
- **Ancient materiality**: Every surface should suggest a physical material (stone, iron, leather, parchment) through texture and shadow, grounding the digital experience in tactile reality
- **Environmental storytelling**: Layout, imagery, and decorative elements should combine to suggest a place and narrative, not merely present information
- **Earned luminance**: Light elements (gold text, glowing runes, fire effects) must feel like they emerge organically from the darkness, not simply placed atop it
- **Contrast through scarcity**: Reserve high contrast (bright gold on near-black) for the most important elements; secondary content should remain in the mid-tone muted range
- **Solemnity over spectacle**: Animations and transitions should be slow, deliberate, and atmospheric (fading mist, flickering flame) rather than flashy or playful

---

## Color Palette

| Swatch | Hex | Role / Usage |
|--------|-----|-------------|
| Void Black | `#0A0A0F` | Primary background, deepest layer |
| Dungeon Stone | `#1A1A24` | Card backgrounds, elevated surfaces |
| Fortress Grey | `#2A2A38` | Secondary surfaces, input fields |
| Smoke | `#4A4A5A` | Muted text, disabled states, borders |
| Ash | `#8A8A9A` | Secondary body text, captions |
| Bone White | `#D4D0C8` | Primary body text |
| Parchment Light | `#E8E2D6` | High-emphasis text, headings |
| Antique Gold | `#C8A84E` | Primary accent, headings, key interactive elements |
| Molten Gold | `#E8C84E` | Hover states, highlighted accents, glow effects |
| Dragon Crimson | `#8B1A1A` | Danger, emphasis, call-to-action backgrounds |
| Blood Red | `#C43030` | Active states, important alerts, decorative accents |
| Abyssal Purple | `#2E1A3E` | Atmospheric tints, magical glow undertones |
| Mystic Violet | `#6B3FA0` | Tertiary accent, arcane decorative elements |
| Enchanted Emerald | `#1A4A2E` | Success states, nature-related accents |
| Tarnished Silver | `#7A7A88` | Metallic borders, secondary decorative elements |

### CSS Custom Properties

```css
:root {
  --df-void: #0A0A0F;
  --df-stone: #1A1A24;
  --df-fortress: #2A2A38;
  --df-smoke: #4A4A5A;
  --df-ash: #8A8A9A;
  --df-bone: #D4D0C8;
  --df-parchment: #E8E2D6;
  --df-gold: #C8A84E;
  --df-gold-bright: #E8C84E;
  --df-crimson: #8B1A1A;
  --df-blood: #C43030;
  --df-purple: #2E1A3E;
  --df-violet: #6B3FA0;
  --df-emerald: #1A4A2E;
  --df-silver: #7A7A88;

  /* Semantic tokens */
  --df-bg-primary: var(--df-void);
  --df-bg-surface: var(--df-stone);
  --df-bg-elevated: var(--df-fortress);
  --df-text-primary: var(--df-bone);
  --df-text-heading: var(--df-parchment);
  --df-text-muted: var(--df-ash);
  --df-accent-primary: var(--df-gold);
  --df-accent-danger: var(--df-crimson);
  --df-border: rgba(200, 168, 78, 0.15);
}
```

---

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **MedievalSharp** | 400 | Display titles; spiky, engraved forms evoking swords and sorcery | [MedievalSharp](https://fonts.google.com/specimen/MedievalSharp) |
| **Cinzel Decorative** | 400, 700, 900 | Hero titles; grand Roman-inscribed capitals with ornate flourishes | [Cinzel Decorative](https://fonts.google.com/specimen/Cinzel+Decorative) |
| **Cinzel** | 400, 500, 600, 700 | Section headings and nav links; stately Roman inscription letterforms | [Cinzel](https://fonts.google.com/specimen/Cinzel) |
| **Uncial Antiqua** | 400 | Decorative accents and labels; monastic uncial script evoking ancient manuscripts | [Uncial Antiqua](https://fonts.google.com/specimen/Uncial+Antiqua) |
| **Cormorant** | 300, 400, 500, 600, 700 | Subheadings and pull quotes; elegant, high-contrast serif with a literary quality | [Cormorant](https://fonts.google.com/specimen/Cormorant) |
| **EB Garamond** | 400, 500, 600, 700 | Body text; classical old-style Garamond for extended reading | [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) |
| **Spectral** | 300, 400, 500, 600, 700 | Long-form body text; designed for screen legibility in serif contexts | [Spectral](https://fonts.google.com/specimen/Spectral) |
| **Playfair Display** | 400, 500, 600, 700, 900 | Alternate headings; high-contrast transitional serif with dramatic weight | [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Cinzel Decorative 700 | EB Garamond 400 | Regal inscription titles over classical literary prose; formal and commanding |
| MedievalSharp 400 | Spectral 400 | Raw sword-and-sorcery headers with clean, readable body text; adventurous and grounded |
| Cinzel 600 | Cormorant 400 | Stately Roman capitals paired with elegant serif body; refined dark court atmosphere |
| Playfair Display 700 | EB Garamond 400 | Dramatic editorial headings with old-style body; sophisticated and brooding |
| Uncial Antiqua 400 | Spectral 400 | Ancient manuscript accent titles with modern-readable body; mystical and accessible |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@400;700;900&family=Cinzel:wght@400;600;700&family=EB+Garamond:wght@400;500;600&family=MedievalSharp&family=Cormorant:wght@400;500;600&display=swap');

body {
  font-family: 'EB Garamond', 'Georgia', serif;
  font-size: 1.1rem;
  line-height: 1.8;
  color: var(--df-bone);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Cinzel', 'Times New Roman', serif;
  font-weight: 600;
  letter-spacing: 0.04em;
  color: var(--df-parchment);
}

.display-title {
  font-family: 'Cinzel Decorative', serif;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--df-gold);
  text-shadow: 0 0 40px rgba(200, 168, 78, 0.2);
}

.rune-label {
  font-family: 'MedievalSharp', cursive;
  font-size: 0.9rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--df-gold);
}

.quote-text {
  font-family: 'Cormorant', serif;
  font-weight: 500;
  font-size: 1.3rem;
  font-style: italic;
  color: var(--df-ash);
  line-height: 1.7;
}
```

---

## Layout Principles

- **Full-bleed dark canvas**: The background should stretch edge-to-edge with no white margins; the entire viewport is the dark world
- **Centered content column with atmospheric margins**: Primary content sits in a 700-850px column, while the margins host atmospheric textures, fog gradients, or faint decorative rune patterns
- **Layered depth through elevation**: Use progressively lighter dark tones (void -> stone -> fortress) to establish a clear sense of surfaces stacking upward from the abyss
- **Gothic vertical rhythm**: Generous vertical spacing (48-80px between major sections) creates a sense of solemn pacing, as though moving through the halls of a cathedral
- **Architectural section framing**: Use ornamental borders, pointed-arch header shapes, or subtle stone-column sidebars to give sections the feeling of physical spaces
- **Hero sections as landscapes**: Full-viewport hero areas should suggest vast environments through layered gradients, silhouettes, and atmospheric depth
- **Asymmetric grid for narrative layouts**: Two-column layouts where one column is dominant (60-70%) allow for storytelling structures with supporting imagery or sidebar lore
- **Responsive degradation of ornament**: On mobile, reduce decorative borders and filigree to maintain performance and readability; keep the atmospheric background and gold accents intact
- **Scroll-driven atmosphere**: Use subtle parallax or opacity shifts on background elements to create a sense of moving through a physical space as the user scrolls

---

## CSS / Design Techniques

### Dark Fantasy Card

```css
.df-card {
  background: var(--df-stone);
  border: 1px solid rgba(200, 168, 78, 0.15);
  border-radius: 2px;
  padding: 32px;
  position: relative;
  box-shadow:
    0 4px 24px rgba(0, 0, 0, 0.6),
    inset 0 1px 0 rgba(200, 168, 78, 0.08);
  transition: border-color 0.4s ease, box-shadow 0.4s ease;
}

.df-card:hover {
  border-color: rgba(200, 168, 78, 0.3);
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.7),
    0 0 60px rgba(200, 168, 78, 0.05),
    inset 0 1px 0 rgba(200, 168, 78, 0.12);
}

/* Inner decorative frame */
.df-card::before {
  content: '';
  position: absolute;
  top: 6px;
  left: 6px;
  right: 6px;
  bottom: 6px;
  border: 1px solid rgba(200, 168, 78, 0.08);
  pointer-events: none;
}

/* Corner ornament accents */
.df-card::after {
  content: '';
  position: absolute;
  top: 3px;
  left: 3px;
  width: 16px;
  height: 16px;
  border-top: 2px solid rgba(200, 168, 78, 0.3);
  border-left: 2px solid rgba(200, 168, 78, 0.3);
  pointer-events: none;
}
```

### Forged Button

```css
.df-button {
  display: inline-block;
  background: linear-gradient(180deg, rgba(200, 168, 78, 0.12) 0%, rgba(200, 168, 78, 0.04) 100%);
  color: var(--df-gold);
  border: 1px solid rgba(200, 168, 78, 0.4);
  border-radius: 2px;
  padding: 14px 36px;
  font-family: 'Cinzel', serif;
  font-size: 0.8rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.14em;
  text-decoration: none;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: all 0.4s ease;
}

.df-button:hover {
  background: linear-gradient(180deg, var(--df-gold) 0%, #A8883E 100%);
  color: var(--df-void);
  border-color: var(--df-gold);
  box-shadow:
    0 0 24px rgba(200, 168, 78, 0.3),
    0 0 60px rgba(200, 168, 78, 0.1);
  text-shadow: none;
}

/* Metallic sheen sweep on hover */
.df-button::after {
  content: '';
  position: absolute;
  top: -50%;
  left: -60%;
  width: 40%;
  height: 200%;
  background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.12), transparent);
  transform: skewX(-20deg);
  transition: left 0.6s ease;
}

.df-button:hover::after {
  left: 120%;
}

/* Crimson danger variant */
.df-button--danger {
  border-color: rgba(196, 48, 48, 0.5);
  color: var(--df-blood);
  background: linear-gradient(180deg, rgba(139, 26, 26, 0.15) 0%, rgba(139, 26, 26, 0.05) 100%);
}

.df-button--danger:hover {
  background: linear-gradient(180deg, var(--df-blood) 0%, var(--df-crimson) 100%);
  color: var(--df-parchment);
  border-color: var(--df-blood);
  box-shadow: 0 0 24px rgba(196, 48, 48, 0.3);
}
```

### Navigation Bar

```css
.df-nav {
  background: rgba(10, 10, 15, 0.95);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(200, 168, 78, 0.12);
  padding: 0 40px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 64px;
  position: sticky;
  top: 0;
  z-index: 100;
}

.df-nav__brand {
  font-family: 'Cinzel Decorative', serif;
  font-size: 1.1rem;
  font-weight: 700;
  color: var(--df-gold);
  text-decoration: none;
  letter-spacing: 0.06em;
}

.df-nav__links {
  display: flex;
  gap: 8px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.df-nav__links a {
  font-family: 'Cinzel', serif;
  font-size: 0.75rem;
  color: var(--df-ash);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  padding: 8px 16px;
  border-radius: 2px;
  transition: color 0.3s ease, background 0.3s ease;
}

.df-nav__links a:hover,
.df-nav__links a.active {
  color: var(--df-gold);
  background: rgba(200, 168, 78, 0.08);
}

/* Decorative separator between nav items */
.df-nav__links li + li::before {
  content: '\2022';
  color: rgba(200, 168, 78, 0.2);
  margin-right: 8px;
  font-size: 0.5rem;
  vertical-align: middle;
}
```

### Hero Section

```css
.df-hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 120px 40px 80px;
  position: relative;
  overflow: hidden;
  background: var(--df-void);
}

/* Atmospheric fog layer */
.df-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(ellipse at 50% 80%, rgba(46, 26, 62, 0.2) 0%, transparent 60%),
    radial-gradient(ellipse at 20% 20%, rgba(139, 26, 26, 0.06) 0%, transparent 40%),
    radial-gradient(ellipse at 80% 30%, rgba(200, 168, 78, 0.04) 0%, transparent 40%);
  pointer-events: none;
}

/* Bottom fade to content */
.df-hero::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 200px;
  background: linear-gradient(to top, var(--df-void) 0%, transparent 100%);
  pointer-events: none;
}

.df-hero__label {
  font-family: 'MedievalSharp', cursive;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.25em;
  color: var(--df-gold);
  margin-bottom: 24px;
  position: relative;
  z-index: 1;
}

.df-hero__title {
  font-family: 'Cinzel Decorative', serif;
  font-size: clamp(2.4rem, 6vw, 4.5rem);
  font-weight: 700;
  color: var(--df-parchment);
  text-shadow: 0 0 80px rgba(200, 168, 78, 0.15);
  margin-bottom: 24px;
  position: relative;
  z-index: 1;
  max-width: 800px;
}

.df-hero__subtitle {
  font-family: 'Cormorant', serif;
  font-size: 1.25rem;
  font-style: italic;
  color: var(--df-ash);
  max-width: 560px;
  line-height: 1.8;
  margin-bottom: 40px;
  position: relative;
  z-index: 1;
}
```

### Rune Border

```css
.df-rune-border {
  position: relative;
  padding: 40px;
  border: 1px solid rgba(200, 168, 78, 0.2);
}

/* Rune symbols along the top edge */
.df-rune-border::before {
  content: '\16A0 \00a0 \16A2 \00a0 \16A6 \00a0 \16B1 \00a0 \16B7 \00a0 \16C1 \00a0 \16C7 \00a0 \16D2';
  position: absolute;
  top: -10px;
  left: 50%;
  transform: translateX(-50%);
  background: var(--df-void);
  padding: 0 20px;
  font-size: 0.85rem;
  letter-spacing: 0.3em;
  color: rgba(200, 168, 78, 0.4);
}

/* Corner embellishments */
.df-rune-border::after {
  content: '';
  position: absolute;
  inset: 4px;
  border: 1px solid rgba(200, 168, 78, 0.06);
  pointer-events: none;
}

/* Apply to all four corners with extra elements if needed */
.df-rune-border .corner-tl,
.df-rune-border .corner-tr,
.df-rune-border .corner-bl,
.df-rune-border .corner-br {
  position: absolute;
  width: 20px;
  height: 20px;
  border-color: rgba(200, 168, 78, 0.35);
  border-style: solid;
  border-width: 0;
}

.df-rune-border .corner-tl { top: 2px; left: 2px; border-top-width: 2px; border-left-width: 2px; }
.df-rune-border .corner-tr { top: 2px; right: 2px; border-top-width: 2px; border-right-width: 2px; }
.df-rune-border .corner-bl { bottom: 2px; left: 2px; border-bottom-width: 2px; border-left-width: 2px; }
.df-rune-border .corner-br { bottom: 2px; right: 2px; border-bottom-width: 2px; border-right-width: 2px; }
```

### Parchment Texture Panel

```css
.df-parchment {
  background:
    linear-gradient(135deg, rgba(200, 168, 78, 0.03) 0%, transparent 50%),
    linear-gradient(225deg, rgba(139, 26, 26, 0.02) 0%, transparent 50%),
    var(--df-stone);
  border: 1px solid rgba(200, 168, 78, 0.12);
  border-radius: 2px;
  padding: 40px;
  position: relative;
  overflow: hidden;
}

/* Subtle noise texture overlay */
.df-parchment::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
  background-size: 200px 200px;
  opacity: 0.5;
  pointer-events: none;
}

/* Burnt-edge vignette */
.df-parchment::after {
  content: '';
  position: absolute;
  inset: 0;
  box-shadow: inset 0 0 60px rgba(0, 0, 0, 0.4);
  pointer-events: none;
}

.df-parchment__text {
  position: relative;
  z-index: 1;
  font-family: 'EB Garamond', serif;
  color: var(--df-bone);
  line-height: 1.9;
}
```

### Ornate Divider

```css
.df-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 56px 0;
  gap: 16px;
}

.df-divider::before,
.df-divider::after {
  content: '';
  flex: 1;
  max-width: 200px;
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(200, 168, 78, 0.35), transparent);
}

.df-divider__symbol {
  color: var(--df-gold);
  font-size: 1.4rem;
  line-height: 1;
  opacity: 0.7;
}

/* Variant: Sword divider using CSS shapes */
.df-divider--sword::before,
.df-divider--sword::after {
  max-width: 160px;
}

.df-divider--sword .df-divider__symbol {
  display: inline-block;
  width: 24px;
  height: 2px;
  background: var(--df-gold);
  position: relative;
  opacity: 0.5;
}

.df-divider--sword .df-divider__symbol::before {
  content: '';
  position: absolute;
  top: -3px;
  left: 50%;
  transform: translateX(-50%);
  width: 8px;
  height: 8px;
  border: 1px solid var(--df-gold);
  transform: translateX(-50%) rotate(45deg);
}
```

### Ember Glow Text Effect

```css
.df-ember-text {
  font-family: 'Cinzel Decorative', serif;
  font-weight: 700;
  font-size: 3rem;
  color: var(--df-gold);
  text-shadow:
    0 0 10px rgba(200, 168, 78, 0.4),
    0 0 40px rgba(200, 168, 78, 0.15),
    0 0 80px rgba(139, 26, 26, 0.1);
  animation: ember-flicker 4s ease-in-out infinite alternate;
}

@keyframes ember-flicker {
  0% {
    text-shadow:
      0 0 10px rgba(200, 168, 78, 0.4),
      0 0 40px rgba(200, 168, 78, 0.15),
      0 0 80px rgba(139, 26, 26, 0.1);
  }
  50% {
    text-shadow:
      0 0 14px rgba(200, 168, 78, 0.5),
      0 0 50px rgba(200, 168, 78, 0.2),
      0 0 100px rgba(139, 26, 26, 0.15);
  }
  100% {
    text-shadow:
      0 0 8px rgba(200, 168, 78, 0.35),
      0 0 35px rgba(200, 168, 78, 0.12),
      0 0 70px rgba(139, 26, 26, 0.08);
  }
}
```

### Tooltip / Lore Popup

```css
.df-tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted rgba(200, 168, 78, 0.3);
  cursor: help;
}

.df-tooltip__content {
  visibility: hidden;
  opacity: 0;
  position: absolute;
  bottom: calc(100% + 12px);
  left: 50%;
  transform: translateX(-50%) translateY(4px);
  background: var(--df-fortress);
  border: 1px solid rgba(200, 168, 78, 0.25);
  border-radius: 2px;
  padding: 16px 20px;
  min-width: 240px;
  max-width: 320px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.6);
  transition: all 0.3s ease;
  z-index: 50;
}

.df-tooltip__content::after {
  content: '';
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translateX(-50%);
  border: 6px solid transparent;
  border-top-color: rgba(200, 168, 78, 0.25);
}

.df-tooltip:hover .df-tooltip__content {
  visibility: visible;
  opacity: 1;
  transform: translateX(-50%) translateY(0);
}

.df-tooltip__content h4 {
  font-family: 'Cinzel', serif;
  font-size: 0.8rem;
  color: var(--df-gold);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-bottom: 8px;
}

.df-tooltip__content p {
  font-family: 'EB Garamond', serif;
  font-size: 0.9rem;
  color: var(--df-ash);
  line-height: 1.6;
}
```

---

## Design Do's and Don'ts

### Do's

- Use deep, cool-toned dark backgrounds (charcoal, midnight, void) as the dominant canvas
- Apply antique gold and tarnished silver accents with restraint for maximum dramatic impact
- Choose serif and medieval-inspired typefaces for headings; pair with readable serifs for body text
- Add subtle atmospheric effects: radial fog gradients, faint ember glows, vignette shadows
- Use weathered textures (stone, leather, metal, parchment) to ground surfaces in physicality
- Employ ornamental borders, runic patterns, and gothic architectural framing for section divisions
- Keep animations slow and atmospheric (flickering, fading, drifting) to match the solemn mood
- Maintain strong contrast between gold accent text and dark backgrounds for accessibility
- Use crimson and blood-red sparingly as punctuation for danger, urgency, or call-to-action
- Layer multiple translucent shadows and inset glows to create a convincing sense of depth

### Don'ts

- Avoid bright, saturated colors (neon, pastel, electric blue) that break the somber atmosphere
- Do not use rounded, bubbly shapes or playful border-radius values; keep corners sharp (0-4px)
- Avoid sans-serif fonts for primary text; they feel too modern and clinical for the medieval tone
- Do not use pure white (`#FFFFFF`) text; prefer warm off-whites and bone tones for a candlelit feel
- Avoid flat design: every surface should have texture, shadow, or gradient to suggest materiality
- Do not overload with ornamental elements; the darkness and negative space are essential to the mood
- Avoid fast, bouncy, or playful animations (spring physics, elastic easing, confetti)
- Do not use stock photography of modern settings; all imagery should feel timeless or fantastical
- Avoid uniform spacing and grid rigidity; allow for organic, asymmetric compositions when appropriate
- Do not use light or white backgrounds for any major section; even modals should be dark-surfaced

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Dark Academia** | Shares the dark palette, classical typography, and love of aged textures, but Dark Academia is scholarly and earthly while Dark Fantasy is mythical and supernatural |
| **Gothic** | Close sibling; both draw from medieval architecture and somber moods, but Gothic leans toward horror and religious iconography while Dark Fantasy emphasizes sword-and-sorcery and magic |
| **Medievalcore** | Overlapping interest in medieval imagery, armor, and castles, but Medievalcore is more historically grounded while Dark Fantasy embraces the supernatural |
| **Cyberpunk** | Both use dark backgrounds with vivid accents, but Cyberpunk is neon-lit and technological while Dark Fantasy is fire-lit and arcane |
| **Baroque** | Shared love of ornate detail and dramatic contrast, but Baroque is opulent and gilded while Dark Fantasy is weathered and foreboding |
| **Industrial Gothic** | Both feature dark, heavy aesthetics with metal textures, but Industrial Gothic is mechanical and urban while Dark Fantasy is organic and ancient |
| **Goblincore** | Overlapping interest in forest settings, moss, and earthy materials, but Goblincore is whimsical and cozy while Dark Fantasy is threatening and grand |
| **Whimsigothic** | Both blend gothic and fantastical elements, but Whimsigothic is playful and eclectic while Dark Fantasy is serious and immersive |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dark Fantasy Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@400;700;900&family=Cinzel:wght@400;600;700&family=EB+Garamond:wght@400;500;600&family=MedievalSharp&family=Cormorant:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --df-void: #0A0A0F;
      --df-stone: #1A1A24;
      --df-fortress: #2A2A38;
      --df-smoke: #4A4A5A;
      --df-ash: #8A8A9A;
      --df-bone: #D4D0C8;
      --df-parchment: #E8E2D6;
      --df-gold: #C8A84E;
      --df-gold-bright: #E8C84E;
      --df-crimson: #8B1A1A;
      --df-blood: #C43030;
      --df-purple: #2E1A3E;
      --df-violet: #6B3FA0;
      --df-silver: #7A7A88;
    }

    body {
      font-family: 'EB Garamond', Georgia, serif;
      font-size: 1.1rem;
      line-height: 1.8;
      color: var(--df-bone);
      background: var(--df-void);
      min-height: 100vh;
      -webkit-font-smoothing: antialiased;
    }

    /* ---- Navigation ---- */
    nav {
      background: rgba(10, 10, 15, 0.95);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(200, 168, 78, 0.12);
      padding: 0 40px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 60px;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    nav .brand {
      font-family: 'Cinzel Decorative', serif;
      font-size: 1rem;
      font-weight: 700;
      color: var(--df-gold);
      text-decoration: none;
      letter-spacing: 0.06em;
    }

    nav .links {
      display: flex;
      gap: 4px;
      list-style: none;
    }

    nav .links a {
      font-family: 'Cinzel', serif;
      font-size: 0.7rem;
      color: var(--df-ash);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      padding: 8px 14px;
      border-radius: 2px;
      transition: color 0.3s, background 0.3s;
    }

    nav .links a:hover { color: var(--df-gold); background: rgba(200,168,78,0.08); }

    /* ---- Hero ---- */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 120px 24px 100px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse at 50% 85%, rgba(46, 26, 62, 0.25) 0%, transparent 55%),
        radial-gradient(ellipse at 20% 20%, rgba(139, 26, 26, 0.07) 0%, transparent 40%),
        radial-gradient(ellipse at 80% 30%, rgba(200, 168, 78, 0.05) 0%, transparent 40%);
      pointer-events: none;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 200px;
      background: linear-gradient(to top, var(--df-void), transparent);
      pointer-events: none;
    }

    .hero .label {
      font-family: 'MedievalSharp', cursive;
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.25em;
      color: var(--df-gold);
      margin-bottom: 20px;
      position: relative;
      z-index: 1;
    }

    .hero h1 {
      font-family: 'Cinzel Decorative', serif;
      font-size: clamp(2.2rem, 5.5vw, 4rem);
      font-weight: 700;
      color: var(--df-parchment);
      text-shadow: 0 0 80px rgba(200, 168, 78, 0.15);
      margin-bottom: 20px;
      position: relative;
      z-index: 1;
      max-width: 750px;
    }

    .hero .tagline {
      font-family: 'Cormorant', serif;
      font-size: 1.2rem;
      font-style: italic;
      color: var(--df-ash);
      max-width: 500px;
      line-height: 1.7;
      margin-bottom: 36px;
      position: relative;
      z-index: 1;
    }

    /* ---- Buttons ---- */
    .btn {
      display: inline-block;
      background: linear-gradient(180deg, rgba(200,168,78,0.12), rgba(200,168,78,0.04));
      color: var(--df-gold);
      border: 1px solid rgba(200, 168, 78, 0.4);
      border-radius: 2px;
      padding: 14px 36px;
      font-family: 'Cinzel', serif;
      font-size: 0.78rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.14em;
      text-decoration: none;
      cursor: pointer;
      position: relative;
      z-index: 1;
      overflow: hidden;
      transition: all 0.4s ease;
    }

    .btn:hover {
      background: linear-gradient(180deg, var(--df-gold), #A8883E);
      color: var(--df-void);
      border-color: var(--df-gold);
      box-shadow: 0 0 24px rgba(200,168,78,0.3), 0 0 60px rgba(200,168,78,0.1);
    }

    .btn--crimson {
      border-color: rgba(196, 48, 48, 0.5);
      color: var(--df-blood);
      background: linear-gradient(180deg, rgba(139,26,26,0.15), rgba(139,26,26,0.05));
    }

    .btn--crimson:hover {
      background: linear-gradient(180deg, var(--df-blood), var(--df-crimson));
      color: var(--df-parchment);
      border-color: var(--df-blood);
      box-shadow: 0 0 24px rgba(196,48,48,0.3);
    }

    /* ---- Divider ---- */
    .divider {
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 56px auto;
      max-width: 500px;
      gap: 16px;
    }

    .divider::before, .divider::after {
      content: '';
      flex: 1;
      height: 1px;
      background: linear-gradient(90deg, transparent, rgba(200,168,78,0.3), transparent);
    }

    .divider span {
      color: var(--df-gold);
      font-size: 1.3rem;
      opacity: 0.7;
      line-height: 1;
    }

    /* ---- Content Container ---- */
    .container {
      max-width: 820px;
      margin: 0 auto;
      padding: 0 24px 80px;
    }

    /* ---- Section Title ---- */
    .section-title {
      font-family: 'Cinzel', serif;
      font-size: 0.75rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--df-gold);
      margin-bottom: 32px;
      text-align: center;
    }

    /* ---- Cards Grid ---- */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
      margin-bottom: 48px;
    }

    .card {
      background: var(--df-stone);
      border: 1px solid rgba(200, 168, 78, 0.15);
      border-radius: 2px;
      padding: 32px;
      position: relative;
      box-shadow: 0 4px 24px rgba(0,0,0,0.5), inset 0 1px 0 rgba(200,168,78,0.08);
      transition: border-color 0.4s, box-shadow 0.4s;
    }

    .card:hover {
      border-color: rgba(200,168,78,0.3);
      box-shadow: 0 8px 32px rgba(0,0,0,0.6), 0 0 60px rgba(200,168,78,0.04);
    }

    .card::before {
      content: '';
      position: absolute;
      top: 6px; left: 6px; right: 6px; bottom: 6px;
      border: 1px solid rgba(200,168,78,0.06);
      pointer-events: none;
    }

    .card h3 {
      font-family: 'Cinzel', serif;
      font-size: 1.15rem;
      font-weight: 600;
      color: var(--df-parchment);
      margin-bottom: 12px;
    }

    .card .card-label {
      font-family: 'MedievalSharp', cursive;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.18em;
      color: var(--df-gold);
      opacity: 0.7;
      margin-bottom: 8px;
    }

    .card p {
      color: var(--df-ash);
      font-size: 1rem;
      line-height: 1.75;
    }

    /* ---- Rune Border Section ---- */
    .rune-section {
      position: relative;
      border: 1px solid rgba(200, 168, 78, 0.18);
      padding: 48px 36px;
      margin-bottom: 48px;
    }

    .rune-section::before {
      content: '\16A0 \00a0 \16A2 \00a0 \16A6 \00a0 \16B1 \00a0 \16B7 \00a0 \16C1';
      position: absolute;
      top: -10px;
      left: 50%;
      transform: translateX(-50%);
      background: var(--df-void);
      padding: 0 16px;
      font-size: 0.8rem;
      letter-spacing: 0.3em;
      color: rgba(200, 168, 78, 0.35);
    }

    .rune-section .corner {
      position: absolute;
      width: 18px;
      height: 18px;
    }

    .rune-section .corner--tl { top: 2px; left: 2px; border-top: 2px solid rgba(200,168,78,0.35); border-left: 2px solid rgba(200,168,78,0.35); }
    .rune-section .corner--tr { top: 2px; right: 2px; border-top: 2px solid rgba(200,168,78,0.35); border-right: 2px solid rgba(200,168,78,0.35); }
    .rune-section .corner--bl { bottom: 2px; left: 2px; border-bottom: 2px solid rgba(200,168,78,0.35); border-left: 2px solid rgba(200,168,78,0.35); }
    .rune-section .corner--br { bottom: 2px; right: 2px; border-bottom: 2px solid rgba(200,168,78,0.35); border-right: 2px solid rgba(200,168,78,0.35); }

    .rune-section h2 {
      font-family: 'Cinzel Decorative', serif;
      font-size: 1.6rem;
      font-weight: 700;
      color: var(--df-parchment);
      text-align: center;
      margin-bottom: 16px;
    }

    .rune-section p {
      text-align: center;
      max-width: 560px;
      margin: 0 auto;
      color: var(--df-ash);
      line-height: 1.85;
    }

    /* ---- Parchment Panel ---- */
    .parchment {
      background:
        linear-gradient(135deg, rgba(200,168,78,0.03), transparent 50%),
        linear-gradient(225deg, rgba(139,26,26,0.02), transparent 50%),
        var(--df-stone);
      border: 1px solid rgba(200, 168, 78, 0.12);
      border-radius: 2px;
      padding: 40px;
      position: relative;
      overflow: hidden;
      margin-bottom: 48px;
    }

    .parchment::after {
      content: '';
      position: absolute;
      inset: 0;
      box-shadow: inset 0 0 60px rgba(0,0,0,0.35);
      pointer-events: none;
    }

    .parchment blockquote {
      font-family: 'Cormorant', serif;
      font-size: 1.25rem;
      font-style: italic;
      color: var(--df-bone);
      line-height: 1.8;
      text-align: center;
      position: relative;
      z-index: 1;
    }

    .parchment .attribution {
      font-family: 'Cinzel', serif;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--df-smoke);
      text-align: center;
      margin-top: 16px;
      position: relative;
      z-index: 1;
    }

    /* ---- Ember Glow Title ---- */
    .ember-glow {
      font-family: 'Cinzel Decorative', serif;
      font-weight: 700;
      color: var(--df-gold);
      text-align: center;
      text-shadow:
        0 0 10px rgba(200,168,78,0.4),
        0 0 40px rgba(200,168,78,0.15),
        0 0 80px rgba(139,26,26,0.1);
      animation: ember 4s ease-in-out infinite alternate;
    }

    @keyframes ember {
      0%   { text-shadow: 0 0 10px rgba(200,168,78,0.4), 0 0 40px rgba(200,168,78,0.15), 0 0 80px rgba(139,26,26,0.1); }
      50%  { text-shadow: 0 0 14px rgba(200,168,78,0.5), 0 0 50px rgba(200,168,78,0.2), 0 0 100px rgba(139,26,26,0.15); }
      100% { text-shadow: 0 0 8px rgba(200,168,78,0.35), 0 0 35px rgba(200,168,78,0.12), 0 0 70px rgba(139,26,26,0.08); }
    }

    /* ---- Footer ---- */
    footer {
      border-top: 1px solid rgba(200, 168, 78, 0.1);
      padding: 40px 24px;
      text-align: center;
    }

    footer p {
      font-family: 'Cinzel', serif;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--df-smoke);
    }

    /* ---- Responsive ---- */
    @media (max-width: 640px) {
      nav { padding: 0 16px; }
      nav .links { gap: 0; }
      nav .links a { padding: 8px 8px; font-size: 0.65rem; }
      .hero { padding: 80px 16px 60px; }
      .hero h1 { font-size: 2rem; }
      .cards { grid-template-columns: 1fr; }
      .rune-section { padding: 32px 20px; }
      .rune-section::before { font-size: 0.65rem; }
      .parchment { padding: 28px 20px; }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <a href="#" class="brand">Shadowkeep</a>
    <ul class="links">
      <li><a href="#">Realms</a></li>
      <li><a href="#">Bestiary</a></li>
      <li><a href="#">Grimoire</a></li>
      <li><a href="#">Chronicles</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <p class="label">From the Ashen Throne</p>
    <h1>Where Darkness Reigns and Legends Are Forged</h1>
    <p class="tagline">Beyond the mist-shrouded mountains, ancient evils stir in crumbling keeps,
      and only those who dare the abyss may claim the crown of fire.</p>
    <div style="display: flex; gap: 16px; flex-wrap: wrap; justify-content: center;">
      <a href="#" class="btn">Begin the Quest</a>
      <a href="#" class="btn btn--crimson">Enter the Abyss</a>
    </div>
  </section>

  <!-- Divider -->
  <div class="divider"><span>&#10038;</span></div>

  <!-- Content -->
  <div class="container">
    <p class="section-title">Tales from the Ruined Kingdoms</p>

    <!-- Card Grid -->
    <div class="cards">
      <div class="card">
        <p class="card-label">Chapter I</p>
        <h3>The Hollow Knight</h3>
        <p>In the depths of the Undercrypt, a knight clad in corroded armor stands vigil over a throne no king has claimed in a thousand years. His sword hums with a forgotten enchantment.</p>
      </div>
      <div class="card">
        <p class="card-label">Chapter II</p>
        <h3>The Witch of Thornveil</h3>
        <p>Deep in the Thornveil Forest, where the canopy swallows all light, an ancient sorceress weaves spells from moonlight and memory. Her price is always more than coin.</p>
      </div>
      <div class="card">
        <p class="card-label">Chapter III</p>
        <h3>The Dragon's Tithe</h3>
        <p>Each harvest moon, the village of Ashenmere sends tribute to the peak of Mount Dreadfire. What dwells there has not been seen in living memory, only felt in tremors and flame.</p>
      </div>
      <div class="card">
        <p class="card-label">Chapter IV</p>
        <h3>The Shattered Covenant</h3>
        <p>Once, five orders stood united against the encroaching void. Now their towers lie broken, their banners torn, and the seals they forged grow weaker with each passing eclipse.</p>
      </div>
    </div>

    <!-- Divider -->
    <div class="divider"><span>&#9876;</span></div>

    <!-- Rune Border Section -->
    <div class="rune-section">
      <span class="corner corner--tl"></span>
      <span class="corner corner--tr"></span>
      <span class="corner corner--bl"></span>
      <span class="corner corner--br"></span>
      <h2>The Grimoire</h2>
      <p>Herein lie the collected incantations, sigils, and forbidden knowledge gathered by the Order of the Obsidian Quill across ten centuries of arcane study. Read at your own peril.</p>
    </div>

    <!-- Parchment Quote -->
    <div class="parchment">
      <blockquote>
        "The flame does not ask permission to consume. It simply burns, and in its wake, leaves only ash and the terrible clarity of what remains."
      </blockquote>
      <p class="attribution">Inscription on the Wall of the First Pyre</p>
    </div>

    <!-- Ember Glow Title -->
    <p class="ember-glow" style="font-size: 2rem; margin-bottom: 48px;">Finis Coronat Opus</p>

    <!-- Final CTA -->
    <div style="text-align: center;">
      <a href="#" class="btn">Claim Your Destiny</a>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <p>Forged in shadow &bull; Anno Tenebris MMXXVI</p>
  </footer>

</body>
</html>
```
