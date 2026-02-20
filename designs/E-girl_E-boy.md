# E-girl / E-boy -- Design Reference

The E-girl / E-boy aesthetic is a TikTok-era digital subculture that fuses emo and scene revival, anime and manga influences, gaming culture, and kawaii Japanese fashion into a maximalist, hyper-online visual identity. Emerging around 2018-2019 on platforms like TikTok and Instagram, it is defined by bold winged eyeliner, drawn-on hearts beneath the eyes, heavy blush swept across the nose and cheeks, split-dyed or streak-colored hair, layered chains and chokers, checkered and plaid patterns, platform shoes, and mesh or fishnet underlayers. The design language mixes saccharine pastels with moody darks -- baby pink next to jet black, soft blush tones alongside chain-link metallics. It is deliberately performative, self-aware, and internet-native: a digital costume designed to be captured on camera and shared on screens. In web design, it translates to playful asymmetry, anime-inspired illustration, bold pink and black contrasts, sticker-like UI elements, and an unapologetic embrace of cute-meets-edgy maximalism.

---

## Visual Characteristics

### Core Design Traits

- **High-contrast pink and black palette**: The signature color relationship places saturated pinks, magentas, and blush tones against deep blacks and charcoals, creating the same visual tension found in e-girl makeup and fashion
- **Anime and manga-inspired illustration**: Drawn elements mimic anime art styles -- large expressive eyes, chibi characters, sparkle effects, heart stamps, and star decorations scattered across layouts
- **Checkered and plaid patterns**: Checkerboard grids, tartan plaids, and argyle patterns appear as backgrounds, section dividers, and decorative accents, referencing the plaid skirts and checkered accessories of the fashion
- **Chain and hardware motifs**: Decorative chain-link borders, padlock icons, safety pin graphics, and belt buckle ornaments bring the layered accessory culture into digital form
- **Sticker and stamp UI elements**: Interface components are styled to look like vinyl stickers, rubber stamps, or hand-drawn doodles -- slightly tilted, with visible outlines and a casual, handmade quality
- **Split and streak color blocks**: Layouts use bold color splits (half pink, half black; gradient streaks) echoing the split-dyed hair that defines the look
- **Heavy outline and stroke work**: Text, icons, and containers feature thick, visible outlines reminiscent of bold eyeliner, marker drawings, and comic book inking
- **Glitch and digital noise textures**: Subtle VHS static, pixel noise, and RGB shift effects reference the internet-native origins and screen-mediated culture
- **Layered, cluttered compositions**: Elements overlap, stack, and crowd the viewport -- stickers on top of photos, text over patterns, chains draped across cards -- reflecting the maximalist layering of the fashion
- **Emoji and kaomoji integration**: Faces like (>_<), hearts, stars, and emoji-style icons are woven into typography and navigation as functional decorative elements

### Design Principles

- Embrace the tension between cute and edgy -- every sweet element needs a sharp counterpart
- Treat the screen as a mirror: the design should feel personal, intimate, and selfie-adjacent
- Layer aggressively but maintain a visual focal point; clutter is intentional, not accidental
- Use animation sparingly but expressively -- sparkle effects, floating hearts, subtle bounces
- Color is emotional: pinks and purples convey the soft kawaii side; blacks and chains convey the alternative edge
- Typography should feel handwritten, playful, or deliberately internet-casual -- never corporate or sterile
- Interactivity should feel tactile and rewarding -- hover states that sparkle, buttons that bounce, cursors that trail hearts
- Reference internet culture directly: memes, reaction faces, chat bubbles, notification badges, and streaming overlays are all fair game
- Accessibility matters even in maximalism -- ensure text remains readable against busy backgrounds through careful contrast and backdrop treatments

---

## Color Palette

The E-girl / E-boy palette oscillates between saccharine pastels and moody darks, with hot pinks and magentas serving as the bridge. The palette is deliberately gendered in its references but fluid in application -- the same colors appear across the full spectrum of the aesthetic.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Blush Pink** | `#FF6B9D` | Primary accent, buttons, highlights, drawn-on heart stamps |
| **Hot Magenta** | `#FF2D78` | Bold CTA elements, hover states, active links |
| **E-girl Black** | `#1A1A1A` | Primary background, text color, dark panels |
| **Soft Charcoal** | `#2D2D2D` | Card backgrounds, secondary dark surfaces |
| **Baby Lavender** | `#C9A0DC` | Secondary accent, tags, soft highlight areas |
| **Neon Lilac** | `#B24BF3` | Tertiary accent, gradients, decorative glow |
| **Pastel Blue** | `#7EC8E3` | Cool accent, link text, info elements |
| **Chain Silver** | `#C0C0C0` | Metallic accents, borders, hardware motifs |
| **Bleached White** | `#F5F0F6` | Light backgrounds, text on dark, card surfaces |
| **Checkerboard Gray** | `#E8E0EB` | Pattern backgrounds, alternating grid cells |
| **Blush Cream** | `#FFE4ED` | Soft backgrounds, highlight panels, blush areas |
| **Warning Red** | `#FF4757` | Error states, destructive actions, heart break motifs |
| **Acid Green** | `#7BED9F` | Success states, gaming references, accent pops |
| **E-boy Blue** | `#546DE5` | Alternative primary accent, e-boy variant palette |
| **Deep Plum** | `#3D1F56` | Dark accent background, gradient endpoints |

### CSS Custom Properties

```css
:root {
  /* Core pinks */
  --egirl-blush: #ff6b9d;
  --egirl-magenta: #ff2d78;
  --egirl-cream: #ffe4ed;

  /* Darks */
  --egirl-black: #1a1a1a;
  --egirl-charcoal: #2d2d2d;
  --egirl-plum: #3d1f56;

  /* Purples and lilacs */
  --egirl-lavender: #c9a0dc;
  --egirl-lilac: #b24bf3;

  /* Cool tones */
  --egirl-blue: #7ec8e3;
  --egirl-eboy-blue: #546de5;

  /* Neutrals */
  --egirl-silver: #c0c0c0;
  --egirl-white: #f5f0f6;
  --egirl-gray: #e8e0eb;

  /* Utility */
  --egirl-red: #ff4757;
  --egirl-green: #7bed9f;

  /* Functional tokens */
  --egirl-bg: var(--egirl-black);
  --egirl-bg-light: var(--egirl-white);
  --egirl-text: var(--egirl-white);
  --egirl-text-dark: var(--egirl-black);
  --egirl-accent: var(--egirl-blush);
  --egirl-accent-strong: var(--egirl-magenta);
  --egirl-border: var(--egirl-silver);

  /* Glow effects */
  --egirl-glow-pink: 0 0 10px rgba(255, 107, 157, 0.4), 0 0 30px rgba(255, 107, 157, 0.15);
  --egirl-glow-lilac: 0 0 10px rgba(178, 75, 243, 0.4), 0 0 30px rgba(178, 75, 243, 0.15);
  --egirl-glow-blue: 0 0 10px rgba(126, 200, 227, 0.4), 0 0 30px rgba(126, 200, 227, 0.15);
}
```

---

## Typography

### Typeface Characteristics

E-girl / E-boy typography is:

- **Playful and handwritten-leaning** -- rounded letterforms, casual baselines, and deliberate imperfection evoke doodles in a notebook or text messages between friends
- **Bold and chunky for display** -- headlines use thick, rounded, or bubbly fonts that demand attention and photograph well for social media
- **Mixed case and decorative** -- all-lowercase is common for body text (mimicking casual texting), while display text might mix cases or use alternating caps for emphasis
- **Sticker-like and outlined** -- text often appears with thick outlines, drop shadows, or is placed on colored label backgrounds as if applied like a sticker
- **Anime and manga influenced** -- occasional use of angular, Japanese-inspired display fonts for headings and decorative text
- **Emoji-adjacent** -- typography is frequently punctuated with symbols, kaomoji, hearts, stars, and other decorative characters integrated into the text flow

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Quicksand** | Rounded geometric sans | Body text, UI elements, casual readable content |
| **Fredoka** | Rounded, bubbly display | Headlines, buttons, sticker-like labels |
| **Comfortaa** | Rounded geometric | Navigation, subheadings, soft UI text |
| **Patrick Hand** | Handwritten, casual | Decorative text, annotations, doodle labels |
| **Bungee Shade** | Bold display with shadow | Hero text, major headlines, decorative titles |
| **Permanent Marker** | Handwritten marker | Accent text, rebellious edge, graffiti-style labels |
| **Baloo 2** | Rounded, friendly | Body text, cards, friendly UI copy |
| **Righteous** | Retro rounded display | Subheadings, bold callouts, feature labels |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Fredoka** (700) | **Quicksand** (400) | Bubbly kawaii, soft and approachable |
| **Bungee Shade** (400) | **Comfortaa** (400) | Bold and dramatic with smooth readability |
| **Permanent Marker** (400) | **Baloo 2** (400) | Edgy handwritten energy with friendly body text |
| **Righteous** (400) | **Quicksand** (500) | Retro-cool headings with clean, rounded body |
| **Fredoka** (600) | **Patrick Hand** (400) | Full notebook-doodle aesthetic, casual throughout |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&family=Quicksand:wght@400;500;600;700&family=Patrick+Hand&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Fredoka', 'Comfortaa', sans-serif;
  font-weight: 700;
  color: var(--egirl-accent);
  line-height: 1.2;
  letter-spacing: -0.01em;
}

/* Display / Hero text with outline effect */
.egirl-display {
  font-family: 'Fredoka', sans-serif;
  font-size: clamp(2.5rem, 7vw, 5rem);
  font-weight: 700;
  color: var(--egirl-cream);
  text-shadow:
    -2px -2px 0 var(--egirl-magenta),
     2px -2px 0 var(--egirl-magenta),
    -2px  2px 0 var(--egirl-magenta),
     2px  2px 0 var(--egirl-magenta);
}

/* Body text */
body {
  font-family: 'Quicksand', 'Baloo 2', sans-serif;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--egirl-text);
  font-weight: 400;
}

/* Handwritten accent text */
.egirl-handwritten {
  font-family: 'Patrick Hand', cursive;
  font-size: 1.1rem;
  color: var(--egirl-lavender);
  transform: rotate(-2deg);
  display: inline-block;
}

/* Sticker label text */
.egirl-label {
  font-family: 'Fredoka', sans-serif;
  font-weight: 600;
  font-size: 0.8rem;
  text-transform: lowercase;
  letter-spacing: 0.04em;
  background: var(--egirl-magenta);
  color: var(--egirl-white);
  padding: 4px 12px;
  border-radius: 20px;
  display: inline-block;
}

/* Kaomoji / decorative inline text */
.egirl-kaomoji {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  color: var(--egirl-blush);
  font-size: 0.9em;
}
```

---

## Layout Principles

### Grid and Structure

- **Asymmetric, collage-like layouts** -- elements are placed at slight angles, overlapping edges, and breaking out of strict grid lines to create a scrapbook or Tumblr dashboard feel
- **Dark backgrounds with pink-accented panels** -- the base canvas is typically dark (black or deep plum), with content panels in lighter pinks, creams, or translucent overlays
- **Checkered and patterned section dividers** -- instead of simple horizontal rules, sections are separated by checkerboard strips, chain graphics, or decorative doodle borders
- **Sticker-scattered compositions** -- small decorative elements (hearts, stars, chains, safety pins) are positioned around the layout as floating stickers, adding visual texture without structural purpose
- **Two-column with visual break** -- common layout splits content into a text column and an image or illustration column, with decorative elements bridging the gap
- **Full-bleed hero with overlapping elements** -- hero sections stretch edge to edge, but UI elements (navigation, titles, CTAs) break out of containers and overlap the hero image

### Section Organization

- **Navigation**: Rounded pill-style nav links with pink highlight on active state, floating slightly over the hero area; may include decorative kaomoji or heart separators between items
- **Hero**: Full-width dark or gradient background with bold display text, anime-style illustration or selfie-aesthetic imagery, floating sticker decorations, and a bouncy CTA button
- **Feature cards**: Grid of rounded cards with thick outlines, each featuring an icon or small illustration, a bold label, and short descriptive text; cards may be slightly rotated for a casual feel
- **Gallery / Lookbook**: Masonry or offset grid of images with overlay captions, heart-shaped like counters, and sticker-style tags
- **Testimonial / Quote**: Chat-bubble styled blocks with rounded corners, emoji reactions, and handwritten-style attribution
- **CTA section**: Bold gradient background (pink to purple) with large display text and a prominent bouncy button
- **Footer**: Dark background with rounded nav links, social media icons styled as stickers, and a decorative kaomoji sign-off

### Responsive Approach

- Maintain the dark-with-pink-accent color scheme at all breakpoints; never flatten to a plain white mobile layout
- Stack collage elements vertically on mobile but preserve slight rotations and overlaps for visual interest
- Reduce the number of floating sticker decorations on smaller screens to avoid clutter
- Navigation collapses into a rounded hamburger menu with an animated pink accent
- Cards shift from grid to a single-column carousel or vertical stack with swipe interaction on touch devices
- Typography scales down but retains the rounded, bubbly character -- never switch to a corporate sans-serif

---

## CSS / Design Techniques

### E-girl Card Component

A rounded, outlined card with a sticker-like quality and subtle rotation for a casual, handmade feel.

```css
.egirl-card {
  background: var(--egirl-charcoal);
  border: 3px solid var(--egirl-blush);
  border-radius: 16px;
  padding: 24px;
  position: relative;
  transform: rotate(-1deg);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  overflow: visible;
}

.egirl-card:hover {
  transform: rotate(0deg) translateY(-4px);
  box-shadow: var(--egirl-glow-pink);
}

/* Floating heart sticker decoration */
.egirl-card::after {
  content: '\2665';
  position: absolute;
  top: -12px;
  right: -8px;
  font-size: 1.5rem;
  color: var(--egirl-magenta);
  background: var(--egirl-black);
  border: 2px solid var(--egirl-magenta);
  border-radius: 50%;
  width: 32px;
  height: 32px;
  display: flex;
  align-items: center;
  justify-content: center;
  transform: rotate(12deg);
}

.egirl-card h3 {
  font-family: 'Fredoka', sans-serif;
  color: var(--egirl-cream);
  margin-top: 0;
  font-size: 1.25rem;
}

.egirl-card p {
  font-family: 'Quicksand', sans-serif;
  color: var(--egirl-lavender);
  font-size: 0.95rem;
  line-height: 1.6;
}
```

### E-girl Button

A bouncy, pill-shaped button with a glow hover effect and optional heart icon.

```css
.egirl-button {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  font-family: 'Fredoka', sans-serif;
  font-size: 1rem;
  font-weight: 600;
  padding: 12px 28px;
  border: 2px solid var(--egirl-magenta);
  border-radius: 50px;
  background: var(--egirl-magenta);
  color: var(--egirl-white);
  cursor: pointer;
  text-decoration: none;
  transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
  text-transform: lowercase;
  letter-spacing: 0.02em;
}

.egirl-button:hover {
  transform: scale(1.05);
  box-shadow: var(--egirl-glow-pink);
  background: var(--egirl-blush);
  border-color: var(--egirl-blush);
}

.egirl-button:active {
  transform: scale(0.97);
  box-shadow: none;
}

/* Ghost / outline variant */
.egirl-button--ghost {
  background: transparent;
  color: var(--egirl-blush);
}

.egirl-button--ghost:hover {
  background: rgba(255, 107, 157, 0.1);
  color: var(--egirl-cream);
}
```

### E-girl Navigation

A floating, pill-shaped navigation bar with pink accent highlights and decorative separators.

```css
.egirl-nav {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  padding: 12px 24px;
  background: rgba(45, 45, 45, 0.85);
  backdrop-filter: blur(12px);
  border-radius: 50px;
  border: 2px solid rgba(255, 107, 157, 0.2);
  position: fixed;
  top: 20px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 100;
}

.egirl-nav a {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  color: var(--egirl-lavender);
  text-decoration: none;
  padding: 6px 16px;
  border-radius: 25px;
  transition: all 0.3s ease;
  text-transform: lowercase;
}

.egirl-nav a:hover {
  color: var(--egirl-cream);
  background: rgba(255, 107, 157, 0.15);
}

.egirl-nav a.active {
  color: var(--egirl-white);
  background: var(--egirl-magenta);
}

/* Heart separator between nav items */
.egirl-nav .separator {
  color: var(--egirl-blush);
  font-size: 0.6rem;
  opacity: 0.5;
  user-select: none;
}
```

### E-girl Hero Section

A full-viewport hero with bold display text, floating decorations, and a gradient overlay.

```css
.egirl-hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  position: relative;
  background: linear-gradient(
    135deg,
    var(--egirl-black) 0%,
    var(--egirl-plum) 50%,
    var(--egirl-black) 100%
  );
  overflow: hidden;
  padding: 40px 20px;
}

/* Checkered pattern overlay */
.egirl-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(45deg, rgba(255, 45, 120, 0.03) 25%, transparent 25%),
    linear-gradient(-45deg, rgba(255, 45, 120, 0.03) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, rgba(255, 45, 120, 0.03) 75%),
    linear-gradient(-45deg, transparent 75%, rgba(255, 45, 120, 0.03) 75%);
  background-size: 40px 40px;
  background-position: 0 0, 0 20px, 20px -20px, -20px 0px;
  pointer-events: none;
}

.egirl-hero h1 {
  font-family: 'Fredoka', sans-serif;
  font-size: clamp(3rem, 8vw, 6rem);
  font-weight: 700;
  color: var(--egirl-cream);
  text-shadow:
    -3px -3px 0 var(--egirl-magenta),
     3px -3px 0 var(--egirl-magenta),
    -3px  3px 0 var(--egirl-magenta),
     3px  3px 0 var(--egirl-magenta);
  margin-bottom: 0.5em;
  position: relative;
  z-index: 2;
}

.egirl-hero p {
  font-family: 'Quicksand', sans-serif;
  font-size: clamp(1rem, 2.5vw, 1.3rem);
  color: var(--egirl-lavender);
  max-width: 600px;
  line-height: 1.7;
  position: relative;
  z-index: 2;
}
```

### Checkerboard Background Pattern

A CSS-only checkerboard that can be applied to any section as a textural element.

```css
.egirl-checkerboard {
  background-color: var(--egirl-charcoal);
  background-image:
    linear-gradient(45deg, rgba(255, 107, 157, 0.08) 25%, transparent 25%),
    linear-gradient(-45deg, rgba(255, 107, 157, 0.08) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, rgba(255, 107, 157, 0.08) 75%),
    linear-gradient(-45deg, transparent 75%, rgba(255, 107, 157, 0.08) 75%);
  background-size: 30px 30px;
  background-position: 0 0, 0 15px, 15px -15px, -15px 0px;
}

/* Stronger variant for decorative strips */
.egirl-checkerboard--bold {
  background-image:
    linear-gradient(45deg, var(--egirl-blush) 25%, transparent 25%),
    linear-gradient(-45deg, var(--egirl-blush) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, var(--egirl-blush) 75%),
    linear-gradient(-45deg, transparent 75%, var(--egirl-blush) 75%);
  background-size: 20px 20px;
  background-position: 0 0, 0 10px, 10px -10px, -10px 0px;
}
```

### Chain Link Border

A repeating chain-link pattern created with CSS for decorative dividers.

```css
.egirl-chain-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0;
  padding: 16px 0;
  user-select: none;
  overflow: hidden;
}

.egirl-chain-divider::before,
.egirl-chain-divider::after {
  content: '\1F517\1F517\1F517\1F517\1F517\1F517\1F517\1F517\1F517\1F517';
  font-size: 1rem;
  letter-spacing: -2px;
  opacity: 0.4;
  filter: grayscale(100%);
}

/* CSS-only chain alternative using borders */
.egirl-chain-border {
  height: 4px;
  background: repeating-linear-gradient(
    90deg,
    var(--egirl-silver) 0px,
    var(--egirl-silver) 12px,
    transparent 12px,
    transparent 16px,
    var(--egirl-silver) 16px,
    var(--egirl-silver) 20px,
    transparent 20px,
    transparent 24px
  );
  border-radius: 2px;
  opacity: 0.5;
  margin: 24px 0;
}
```

### Sticker Badge

A small, tilted badge component for tags, categories, and decorative labels.

```css
.egirl-sticker {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  font-family: 'Fredoka', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  padding: 6px 14px;
  border-radius: 20px;
  border: 2px solid;
  transform: rotate(-3deg);
  transition: transform 0.2s ease;
  text-transform: lowercase;
  white-space: nowrap;
}

.egirl-sticker:hover {
  transform: rotate(0deg) scale(1.05);
}

.egirl-sticker--pink {
  background: var(--egirl-cream);
  color: var(--egirl-magenta);
  border-color: var(--egirl-magenta);
}

.egirl-sticker--purple {
  background: rgba(178, 75, 243, 0.15);
  color: var(--egirl-lilac);
  border-color: var(--egirl-lilac);
}

.egirl-sticker--dark {
  background: var(--egirl-black);
  color: var(--egirl-blush);
  border-color: var(--egirl-blush);
}
```

### Chat Bubble Testimonial

A testimonial component styled as a chat message with emoji reactions.

```css
.egirl-chat {
  max-width: 480px;
  padding: 20px 24px;
  background: var(--egirl-charcoal);
  border: 2px solid rgba(255, 107, 157, 0.2);
  border-radius: 20px 20px 20px 4px;
  position: relative;
  margin-bottom: 16px;
}

.egirl-chat p {
  font-family: 'Quicksand', sans-serif;
  font-size: 0.95rem;
  color: var(--egirl-white);
  line-height: 1.6;
  margin: 0;
}

.egirl-chat .sender {
  font-family: 'Fredoka', sans-serif;
  font-weight: 600;
  font-size: 0.8rem;
  color: var(--egirl-blush);
  margin-bottom: 8px;
  display: block;
}

/* Emoji reaction row */
.egirl-chat .reactions {
  display: flex;
  gap: 6px;
  margin-top: 12px;
}

.egirl-chat .reaction {
  font-size: 0.75rem;
  padding: 3px 8px;
  background: rgba(255, 107, 157, 0.1);
  border-radius: 12px;
  border: 1px solid rgba(255, 107, 157, 0.2);
  cursor: pointer;
  transition: background 0.2s ease;
}

.egirl-chat .reaction:hover {
  background: rgba(255, 107, 157, 0.25);
}
```

---

## Design Do's and Don'ts

### Do

- Use the pink-and-black contrast as the foundation of every layout -- it is the most recognizable signal of the aesthetic
- Layer decorative stickers, hearts, and stars as floating elements to create visual texture and personality
- Apply thick outlines and visible borders to cards, buttons, and containers for that hand-drawn, sticker-peel quality
- Use rounded, bubbly fonts for headlines and playful handwritten fonts for accent text
- Include anime-inspired illustrations, chibi characters, or kawaii icons as decorative and functional elements
- Add checkered or plaid patterns as subtle background textures or bold decorative strips
- Implement bouncy, spring-like micro-animations on interactive elements (buttons, cards, toggles)
- Integrate kaomoji and emoji into UI text naturally -- in navigation, headings, and labels
- Use gradient overlays (pink to purple, pink to black) for section backgrounds and hero areas
- Keep body text readable with sufficient contrast -- use lighter lavenders and creams on dark backgrounds
- Make the design feel personal and camera-ready -- as if it could be a screenshot shared on social media

### Don't

- Use a cold, corporate sans-serif font -- this immediately kills the playful, internet-native energy
- Default to plain white backgrounds -- the aesthetic requires either dark (black/charcoal) or tinted (blush/cream) surfaces
- Overuse neon or overly saturated colors uniformly -- the palette needs the soft-to-bold range (baby pink to hot magenta) to breathe
- Create rigid, symmetrical, grid-perfect layouts -- the charm is in the slight rotations, overlaps, and casual placement
- Forget the edgy counterpoint -- an all-pastel, all-soft design becomes generic kawaii rather than e-girl/e-boy
- Use realistic photography without stylization -- images should be filtered, tinted, or paired with illustrated overlays
- Neglect mobile responsiveness -- this aesthetic is born on phones and must look native to small screens
- Add too many competing animations -- sparkles and bounces should accent the experience, not overwhelm it
- Ignore accessibility -- ensure readable text contrast ratios even when using pink-on-dark or patterned backgrounds
- Strip out all personality for "clean" design -- the maximalism and clutter are features, not bugs

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Kawaii / Positivity Kawaii** | Shares the cute, rounded, pastel-pink visual language, but Kawaii is uniformly sweet while E-girl / E-boy adds an edgy, alternative underbelly |
| **Vaporwave** | Both are internet-native aesthetics with strong pink and purple palettes; Vaporwave is nostalgic and ironic while E-girl is contemporary and performative |
| **Gen Z Maximalism** | Shares the cluttered, sticker-laden, anti-minimalist approach; E-girl is a specific flavor within the broader maximalist movement |
| **Cyberpunk** | The dark-background-with-neon-accents structure is shared, but Cyberpunk is dystopian and mechanical while E-girl is playful and personal |
| **RGB Gamer** | Overlaps in the gaming culture references and neon-on-dark palette; RGB Gamer is hardware-focused while E-girl is fashion-and-identity-focused |
| **Kidcore** | Both use bold colors and playful motifs; Kidcore draws from childhood nostalgia while E-girl draws from anime and internet subculture |
| **Dark Mode Neon** | Shares the dark canvas with bright accent colors; Dark Mode Neon is utilitarian while E-girl is decorative and emotional |
| **Whimsigothic** | Both blend darkness with feminine softness; Whimsigothic uses mystical and Victorian references while E-girl uses anime and internet culture |
| **Dopamine Design** | Shares the bright, bold, feel-good maximalism; Dopamine Design is broader and less subcultural in its references |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>pixelheartz -- streaming & gaming collective</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&family=Quicksand:wght@400;500;600;700&family=Patrick+Hand&display=swap" rel="stylesheet">
  <style>
    /* === CSS Custom Properties === */
    :root {
      --egirl-blush: #ff6b9d;
      --egirl-magenta: #ff2d78;
      --egirl-cream: #ffe4ed;
      --egirl-black: #1a1a1a;
      --egirl-charcoal: #2d2d2d;
      --egirl-plum: #3d1f56;
      --egirl-lavender: #c9a0dc;
      --egirl-lilac: #b24bf3;
      --egirl-blue: #7ec8e3;
      --egirl-silver: #c0c0c0;
      --egirl-white: #f5f0f6;
      --egirl-gray: #e8e0eb;
      --egirl-red: #ff4757;
      --egirl-green: #7bed9f;
      --egirl-glow-pink: 0 0 10px rgba(255, 107, 157, 0.4), 0 0 30px rgba(255, 107, 157, 0.15);
      --egirl-glow-lilac: 0 0 10px rgba(178, 75, 243, 0.4), 0 0 30px rgba(178, 75, 243, 0.15);
    }

    /* === Reset & Base === */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Quicksand', sans-serif;
      background: var(--egirl-black);
      color: var(--egirl-white);
      line-height: 1.7;
      overflow-x: hidden;
    }

    a {
      color: var(--egirl-blush);
      text-decoration: none;
      transition: color 0.3s ease;
    }

    a:hover {
      color: var(--egirl-cream);
    }

    img {
      max-width: 100%;
      display: block;
    }

    /* === Navigation === */
    .nav {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 6px;
      padding: 10px 20px;
      background: rgba(45, 45, 45, 0.9);
      backdrop-filter: blur(12px);
      border-radius: 50px;
      border: 2px solid rgba(255, 107, 157, 0.2);
      position: fixed;
      top: 16px;
      left: 50%;
      transform: translateX(-50%);
      z-index: 100;
    }

    .nav a {
      font-family: 'Quicksand', sans-serif;
      font-weight: 600;
      font-size: 0.85rem;
      color: var(--egirl-lavender);
      padding: 6px 14px;
      border-radius: 25px;
      transition: all 0.3s ease;
      text-transform: lowercase;
    }

    .nav a:hover {
      color: var(--egirl-cream);
      background: rgba(255, 107, 157, 0.15);
    }

    .nav a.active {
      color: var(--egirl-white);
      background: var(--egirl-magenta);
    }

    .nav .sep {
      color: var(--egirl-blush);
      font-size: 0.5rem;
      opacity: 0.4;
      user-select: none;
    }

    /* === Hero === */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      position: relative;
      background: linear-gradient(135deg, var(--egirl-black) 0%, var(--egirl-plum) 50%, var(--egirl-black) 100%);
      padding: 100px 20px 60px;
      overflow: hidden;
    }

    /* Checkerboard overlay */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image:
        linear-gradient(45deg, rgba(255, 45, 120, 0.04) 25%, transparent 25%),
        linear-gradient(-45deg, rgba(255, 45, 120, 0.04) 25%, transparent 25%),
        linear-gradient(45deg, transparent 75%, rgba(255, 45, 120, 0.04) 75%),
        linear-gradient(-45deg, transparent 75%, rgba(255, 45, 120, 0.04) 75%);
      background-size: 40px 40px;
      background-position: 0 0, 0 20px, 20px -20px, -20px 0px;
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Fredoka', sans-serif;
      font-size: clamp(2.8rem, 8vw, 5.5rem);
      font-weight: 700;
      color: var(--egirl-cream);
      text-shadow:
        -3px -3px 0 var(--egirl-magenta),
         3px -3px 0 var(--egirl-magenta),
        -3px  3px 0 var(--egirl-magenta),
         3px  3px 0 var(--egirl-magenta);
      margin-bottom: 16px;
      position: relative;
      z-index: 2;
    }

    .hero .subtitle {
      font-family: 'Patrick Hand', cursive;
      font-size: clamp(1.1rem, 3vw, 1.5rem);
      color: var(--egirl-lavender);
      transform: rotate(-2deg);
      margin-bottom: 24px;
      position: relative;
      z-index: 2;
    }

    .hero p {
      font-size: clamp(0.95rem, 2vw, 1.1rem);
      color: var(--egirl-lavender);
      max-width: 560px;
      margin-bottom: 32px;
      position: relative;
      z-index: 2;
    }

    /* Floating decorations */
    .hero .deco {
      position: absolute;
      font-size: 2rem;
      opacity: 0.3;
      pointer-events: none;
      z-index: 1;
      animation: float 4s ease-in-out infinite;
    }

    .hero .deco:nth-child(1) { top: 15%; left: 10%; animation-delay: 0s; }
    .hero .deco:nth-child(2) { top: 25%; right: 12%; animation-delay: 1s; font-size: 1.5rem; }
    .hero .deco:nth-child(3) { bottom: 20%; left: 15%; animation-delay: 2s; font-size: 1.8rem; }
    .hero .deco:nth-child(4) { bottom: 30%; right: 8%; animation-delay: 0.5s; }
    .hero .deco:nth-child(5) { top: 40%; left: 5%; animation-delay: 1.5s; font-size: 1.2rem; }

    @keyframes float {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      50% { transform: translateY(-12px) rotate(5deg); }
    }

    /* Buttons */
    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      font-family: 'Fredoka', sans-serif;
      font-size: 1rem;
      font-weight: 600;
      padding: 12px 28px;
      border: 2px solid var(--egirl-magenta);
      border-radius: 50px;
      background: var(--egirl-magenta);
      color: var(--egirl-white);
      cursor: pointer;
      text-decoration: none;
      transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
      text-transform: lowercase;
      position: relative;
      z-index: 2;
    }

    .btn:hover {
      transform: scale(1.05);
      box-shadow: var(--egirl-glow-pink);
      background: var(--egirl-blush);
      border-color: var(--egirl-blush);
      color: var(--egirl-white);
    }

    .btn:active {
      transform: scale(0.97);
    }

    .btn--ghost {
      background: transparent;
      color: var(--egirl-blush);
    }

    .btn--ghost:hover {
      background: rgba(255, 107, 157, 0.1);
      color: var(--egirl-cream);
    }

    /* === Chain Divider === */
    .chain-divider {
      height: 4px;
      background: repeating-linear-gradient(
        90deg,
        var(--egirl-silver) 0px,
        var(--egirl-silver) 12px,
        transparent 12px,
        transparent 16px,
        var(--egirl-silver) 16px,
        var(--egirl-silver) 20px,
        transparent 20px,
        transparent 24px
      );
      border-radius: 2px;
      opacity: 0.3;
      margin: 0;
    }

    /* === Section Base === */
    section {
      padding: 80px 20px;
    }

    .container {
      max-width: 1100px;
      margin: 0 auto;
    }

    .section-title {
      font-family: 'Fredoka', sans-serif;
      font-size: clamp(1.8rem, 4vw, 2.5rem);
      font-weight: 700;
      color: var(--egirl-cream);
      text-align: center;
      margin-bottom: 8px;
    }

    .section-subtitle {
      font-family: 'Patrick Hand', cursive;
      font-size: 1.1rem;
      color: var(--egirl-blush);
      text-align: center;
      margin-bottom: 48px;
      transform: rotate(-1deg);
    }

    /* === Features Section === */
    .features {
      background: var(--egirl-charcoal);
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
    }

    .feature-card {
      background: var(--egirl-black);
      border: 3px solid var(--egirl-blush);
      border-radius: 16px;
      padding: 28px 24px;
      position: relative;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .feature-card:nth-child(odd) {
      transform: rotate(-1deg);
    }

    .feature-card:nth-child(even) {
      transform: rotate(1deg);
    }

    .feature-card:hover {
      transform: rotate(0deg) translateY(-6px);
      box-shadow: var(--egirl-glow-pink);
    }

    .feature-card .icon {
      font-size: 2rem;
      margin-bottom: 12px;
      display: block;
    }

    .feature-card h3 {
      font-family: 'Fredoka', sans-serif;
      font-size: 1.15rem;
      font-weight: 700;
      color: var(--egirl-cream);
      margin-bottom: 8px;
    }

    .feature-card p {
      font-size: 0.9rem;
      color: var(--egirl-lavender);
      line-height: 1.6;
    }

    /* Sticker tag on cards */
    .sticker {
      display: inline-flex;
      align-items: center;
      gap: 4px;
      font-family: 'Fredoka', sans-serif;
      font-weight: 600;
      font-size: 0.7rem;
      padding: 4px 12px;
      border-radius: 20px;
      border: 2px solid var(--egirl-magenta);
      background: var(--egirl-cream);
      color: var(--egirl-magenta);
      transform: rotate(-3deg);
      text-transform: lowercase;
      margin-bottom: 12px;
    }

    /* === Streamers / Team Section === */
    .team {
      background: var(--egirl-black);
    }

    .team-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 28px;
    }

    .team-card {
      text-align: center;
      padding: 32px 20px 24px;
      background: var(--egirl-charcoal);
      border-radius: 20px;
      border: 2px solid rgba(255, 107, 157, 0.15);
      transition: border-color 0.3s ease, box-shadow 0.3s ease;
    }

    .team-card:hover {
      border-color: var(--egirl-blush);
      box-shadow: var(--egirl-glow-pink);
    }

    .team-card .avatar {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--egirl-magenta), var(--egirl-lilac));
      margin: 0 auto 16px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      border: 3px solid var(--egirl-blush);
    }

    .team-card h3 {
      font-family: 'Fredoka', sans-serif;
      font-size: 1.05rem;
      font-weight: 700;
      color: var(--egirl-cream);
      margin-bottom: 4px;
    }

    .team-card .role {
      font-family: 'Patrick Hand', cursive;
      font-size: 0.9rem;
      color: var(--egirl-blush);
      margin-bottom: 12px;
    }

    .team-card .socials {
      display: flex;
      gap: 8px;
      justify-content: center;
    }

    .team-card .social-link {
      width: 32px;
      height: 32px;
      border-radius: 50%;
      background: rgba(255, 107, 157, 0.1);
      border: 1px solid rgba(255, 107, 157, 0.2);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.8rem;
      color: var(--egirl-lavender);
      transition: all 0.3s ease;
    }

    .team-card .social-link:hover {
      background: var(--egirl-magenta);
      color: var(--egirl-white);
      border-color: var(--egirl-magenta);
    }

    /* === Chat Testimonials === */
    .testimonials {
      background: var(--egirl-charcoal);
    }

    .chat-list {
      max-width: 600px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 16px;
    }

    .chat-bubble {
      padding: 20px 24px;
      background: var(--egirl-black);
      border: 2px solid rgba(255, 107, 157, 0.15);
      border-radius: 20px 20px 20px 4px;
      position: relative;
    }

    .chat-bubble:nth-child(even) {
      border-radius: 20px 20px 4px 20px;
      margin-left: 40px;
    }

    .chat-bubble:nth-child(odd) {
      margin-right: 40px;
    }

    .chat-bubble .sender {
      font-family: 'Fredoka', sans-serif;
      font-weight: 600;
      font-size: 0.8rem;
      color: var(--egirl-blush);
      margin-bottom: 6px;
      display: block;
    }

    .chat-bubble p {
      font-size: 0.92rem;
      color: var(--egirl-white);
      line-height: 1.6;
    }

    .chat-bubble .reactions {
      display: flex;
      gap: 6px;
      margin-top: 10px;
    }

    .chat-bubble .reaction {
      font-size: 0.7rem;
      padding: 2px 8px;
      background: rgba(255, 107, 157, 0.08);
      border-radius: 12px;
      border: 1px solid rgba(255, 107, 157, 0.15);
    }

    /* === Schedule Section === */
    .schedule {
      background: var(--egirl-black);
    }

    .schedule-table {
      width: 100%;
      border-collapse: separate;
      border-spacing: 0 8px;
      max-width: 700px;
      margin: 0 auto;
    }

    .schedule-table th {
      font-family: 'Fredoka', sans-serif;
      font-weight: 600;
      font-size: 0.8rem;
      color: var(--egirl-blush);
      text-align: left;
      padding: 8px 16px;
      text-transform: lowercase;
      letter-spacing: 0.04em;
    }

    .schedule-table td {
      padding: 14px 16px;
      background: var(--egirl-charcoal);
      color: var(--egirl-white);
      font-size: 0.9rem;
    }

    .schedule-table tr td:first-child {
      border-radius: 12px 0 0 12px;
      font-weight: 600;
    }

    .schedule-table tr td:last-child {
      border-radius: 0 12px 12px 0;
    }

    .schedule-table .live-badge {
      font-family: 'Fredoka', sans-serif;
      font-weight: 600;
      font-size: 0.65rem;
      padding: 3px 10px;
      background: var(--egirl-magenta);
      color: var(--egirl-white);
      border-radius: 20px;
      text-transform: lowercase;
      letter-spacing: 0.03em;
    }

    /* === CTA Section === */
    .cta {
      background: linear-gradient(135deg, var(--egirl-plum) 0%, var(--egirl-magenta) 100%);
      text-align: center;
      padding: 80px 20px;
      position: relative;
      overflow: hidden;
    }

    .cta::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image:
        linear-gradient(45deg, rgba(255, 255, 255, 0.03) 25%, transparent 25%),
        linear-gradient(-45deg, rgba(255, 255, 255, 0.03) 25%, transparent 25%),
        linear-gradient(45deg, transparent 75%, rgba(255, 255, 255, 0.03) 75%),
        linear-gradient(-45deg, transparent 75%, rgba(255, 255, 255, 0.03) 75%);
      background-size: 30px 30px;
      background-position: 0 0, 0 15px, 15px -15px, -15px 0px;
      pointer-events: none;
    }

    .cta h2 {
      font-family: 'Fredoka', sans-serif;
      font-size: clamp(2rem, 5vw, 3rem);
      font-weight: 700;
      color: var(--egirl-white);
      margin-bottom: 12px;
      position: relative;
      z-index: 2;
    }

    .cta p {
      font-size: 1.1rem;
      color: var(--egirl-cream);
      margin-bottom: 28px;
      position: relative;
      z-index: 2;
    }

    .cta .btn {
      background: var(--egirl-white);
      color: var(--egirl-magenta);
      border-color: var(--egirl-white);
      position: relative;
      z-index: 2;
    }

    .cta .btn:hover {
      background: var(--egirl-cream);
      transform: scale(1.05);
      box-shadow: 0 0 20px rgba(255, 255, 255, 0.3);
      color: var(--egirl-magenta);
    }

    /* === Footer === */
    .footer {
      background: var(--egirl-charcoal);
      padding: 40px 20px;
      text-align: center;
      border-top: 3px solid rgba(255, 107, 157, 0.15);
    }

    .footer-links {
      display: flex;
      gap: 20px;
      justify-content: center;
      margin-bottom: 16px;
      flex-wrap: wrap;
    }

    .footer-links a {
      font-family: 'Quicksand', sans-serif;
      font-weight: 600;
      font-size: 0.85rem;
      color: var(--egirl-lavender);
      text-transform: lowercase;
    }

    .footer-links a:hover {
      color: var(--egirl-blush);
    }

    .footer .kaomoji {
      font-size: 1.2rem;
      color: var(--egirl-blush);
      margin-bottom: 8px;
      display: block;
    }

    .footer .copyright {
      font-size: 0.8rem;
      color: var(--egirl-silver);
      opacity: 0.6;
    }

    /* === Responsive === */
    @media (max-width: 768px) {
      .nav {
        gap: 4px;
        padding: 8px 14px;
      }

      .nav a {
        font-size: 0.75rem;
        padding: 5px 10px;
      }

      .nav .sep {
        display: none;
      }

      .features-grid,
      .team-grid {
        grid-template-columns: 1fr;
        max-width: 400px;
        margin-left: auto;
        margin-right: auto;
      }

      .feature-card:nth-child(odd),
      .feature-card:nth-child(even) {
        transform: rotate(0deg);
      }

      .chat-bubble:nth-child(even) {
        margin-left: 0;
      }

      .chat-bubble:nth-child(odd) {
        margin-right: 0;
      }

      .schedule-table {
        font-size: 0.85rem;
      }

      section {
        padding: 60px 16px;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav class="nav">
    <a href="#home" class="active">home</a>
    <span class="sep">&hearts;</span>
    <a href="#about">about</a>
    <span class="sep">&hearts;</span>
    <a href="#team">streamers</a>
    <span class="sep">&hearts;</span>
    <a href="#schedule">schedule</a>
    <span class="sep">&hearts;</span>
    <a href="#join">join us</a>
  </nav>

  <!-- Hero Section -->
  <section class="hero" id="home">
    <span class="deco">&hearts;</span>
    <span class="deco">&starf;</span>
    <span class="deco">&#9832;</span>
    <span class="deco">&hearts;</span>
    <span class="deco">&starf;</span>
    <h1>pixelheartz</h1>
    <p class="subtitle">~ a streaming &amp; gaming collective for the chronically online ~</p>
    <p>we are a crew of streamers, artists, and gamers building a cozy corner of the internet. late night raids, anime watch parties, fan art drops, and zero gatekeeping. welcome home.</p>
    <div style="display: flex; gap: 12px; flex-wrap: wrap; justify-content: center; position: relative; z-index: 2;">
      <a href="#join" class="btn">&hearts; join the collective</a>
      <a href="#schedule" class="btn btn--ghost">see who's live</a>
    </div>
  </section>

  <div class="chain-divider"></div>

  <!-- Features Section -->
  <section class="features" id="about">
    <div class="container">
      <h2 class="section-title">what we do &hearts;</h2>
      <p class="section-subtitle">( more than just gaming, promise )</p>
      <div class="features-grid">
        <div class="feature-card">
          <span class="sticker">new!</span>
          <span class="icon">&#127918;</span>
          <h3>co-op streams</h3>
          <p>multiplayer chaos every thursday night. we rotate games weekly -- from cozy farm sims to competitive fps rounds. everyone is welcome regardless of skill level.</p>
        </div>
        <div class="feature-card">
          <span class="sticker">&hearts; fave</span>
          <span class="icon">&#127912;</span>
          <h3>art drops</h3>
          <p>monthly digital art showcases where our members share fan art, original characters, and design experiments. we feature everything from pixel art to full illustrations.</p>
        </div>
        <div class="feature-card">
          <span class="sticker">weekly</span>
          <span class="icon">&#127909;</span>
          <h3>anime nights</h3>
          <p>synchronized watch parties every sunday. we pick a series together, watch two episodes, and then spend an hour yelling about it in voice chat. tissues optional.</p>
        </div>
        <div class="feature-card">
          <span class="sticker">24/7</span>
          <span class="icon">&#128172;</span>
          <h3>community discord</h3>
          <p>our server is always active. dedicated channels for gaming, art feedback, music sharing, vent sessions, and extremely niche meme categories. lurkers are loved too.</p>
        </div>
        <div class="feature-card">
          <span class="sticker">monthly</span>
          <span class="icon">&#127925;</span>
          <h3>playlist drops</h3>
          <p>curated playlists assembled by our members each month. hyperpop, bedroom pop, emo rap, j-pop deep cuts, and lofi study beats. collaborative vibes only.</p>
        </div>
        <div class="feature-card">
          <span class="sticker">collab</span>
          <span class="icon">&#10024;</span>
          <h3>merch collabs</h3>
          <p>limited edition sticker packs, enamel pins, and apparel designed by our artists. every drop sells out so make sure you have notifications on.</p>
        </div>
      </div>
    </div>
  </section>

  <div class="chain-divider"></div>

  <!-- Team Section -->
  <section class="team" id="team">
    <div class="container">
      <h2 class="section-title">meet the streamers</h2>
      <p class="section-subtitle">( the people behind the pixels )</p>
      <div class="team-grid">
        <div class="team-card">
          <div class="avatar">&#128049;</div>
          <h3>kittyxglitch</h3>
          <p class="role">variety streamer</p>
          <p style="font-size: 0.82rem; color: var(--egirl-lavender); margin-bottom: 14px;">cozy horror games and late night chat. known for the cat ear headset and the unhinged commentary.</p>
          <div class="socials">
            <span class="social-link">tw</span>
            <span class="social-link">tt</span>
            <span class="social-link">yt</span>
          </div>
        </div>
        <div class="team-card">
          <div class="avatar">&#9876;</div>
          <h3>dxrkprince</h3>
          <p class="role">competitive fps</p>
          <p style="font-size: 0.82rem; color: var(--egirl-lavender); margin-bottom: 14px;">ranked grind content with a side of existential crisis. chain necklace always on. always.</p>
          <div class="socials">
            <span class="social-link">tw</span>
            <span class="social-link">tt</span>
            <span class="social-link">ig</span>
          </div>
        </div>
        <div class="team-card">
          <div class="avatar">&#127800;</div>
          <h3>blushpxl</h3>
          <p class="role">art + just chatting</p>
          <p style="font-size: 0.82rem; color: var(--egirl-lavender); margin-bottom: 14px;">live digital art sessions, character design, and emotionally devastating anime discussions.</p>
          <div class="socials">
            <span class="social-link">tw</span>
            <span class="social-link">ig</span>
            <span class="social-link">yt</span>
          </div>
        </div>
        <div class="team-card">
          <div class="avatar">&#128126;</div>
          <h3>voidbxby</h3>
          <p class="role">rhythm games + music</p>
          <p style="font-size: 0.82rem; color: var(--egirl-lavender); margin-bottom: 14px;">osu! grind streams, music production sessions, and occasional karaoke that goes way too hard.</p>
          <div class="socials">
            <span class="social-link">tw</span>
            <span class="social-link">sc</span>
            <span class="social-link">tt</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <div class="chain-divider"></div>

  <!-- Testimonials Section -->
  <section class="testimonials">
    <div class="container">
      <h2 class="section-title">community love</h2>
      <p class="section-subtitle">( actual messages from our discord )</p>
      <div class="chat-list">
        <div class="chat-bubble">
          <span class="sender">moonpetal_99</span>
          <p>i joined like three weeks ago and this is genuinely the first online community where i feel like i can just be myself. the anime nights are everything to me.</p>
          <div class="reactions">
            <span class="reaction">&hearts; 24</span>
            <span class="reaction">&#128557; 8</span>
          </div>
        </div>
        <div class="chat-bubble">
          <span class="sender">chainz_boi</span>
          <p>the co-op streams are so chaotic but in the best way possible. last week we spent 40 minutes trying to name a chicken in stardew valley. peak content.</p>
          <div class="reactions">
            <span class="reaction">&#128514; 31</span>
            <span class="reaction">&hearts; 12</span>
          </div>
        </div>
        <div class="chat-bubble">
          <span class="sender">glitchberry</span>
          <p>the art drop last month literally motivated me to start drawing again after two years of creative block. this community is magic and i will fight anyone who disagrees.</p>
          <div class="reactions">
            <span class="reaction">&hearts; 47</span>
            <span class="reaction">&#10024; 19</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <div class="chain-divider"></div>

  <!-- Schedule Section -->
  <section class="schedule" id="schedule">
    <div class="container">
      <h2 class="section-title">stream schedule &starf;</h2>
      <p class="section-subtitle">( all times in your local timezone... jk it's EST )</p>
      <table class="schedule-table">
        <thead>
          <tr>
            <th>day</th>
            <th>streamer</th>
            <th>content</th>
            <th>time</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>monday</td>
            <td>blushpxl</td>
            <td>art stream -- character design</td>
            <td>7pm</td>
          </tr>
          <tr>
            <td>tuesday</td>
            <td>dxrkprince</td>
            <td>ranked valorant grind</td>
            <td>9pm</td>
          </tr>
          <tr>
            <td>wednesday</td>
            <td>voidbxby</td>
            <td>music production + osu!</td>
            <td>8pm</td>
          </tr>
          <tr>
            <td>thursday</td>
            <td>everyone</td>
            <td>co-op game night <span class="live-badge">live now</span></td>
            <td>8pm</td>
          </tr>
          <tr>
            <td>friday</td>
            <td>kittyxglitch</td>
            <td>horror game friday</td>
            <td>10pm</td>
          </tr>
          <tr>
            <td>sunday</td>
            <td>everyone</td>
            <td>anime watch party</td>
            <td>6pm</td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>

  <div class="chain-divider"></div>

  <!-- CTA Section -->
  <section class="cta" id="join">
    <h2>wanna be a pixelheart? &hearts;</h2>
    <p>no applications, no tryouts, just vibes. drop into the discord and say hi.</p>
    <a href="#" class="btn">join the discord &rarr;</a>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="footer-links">
      <a href="#">home</a>
      <a href="#">about</a>
      <a href="#">streamers</a>
      <a href="#">schedule</a>
      <a href="#">merch</a>
      <a href="#">discord</a>
    </div>
    <span class="kaomoji">(&gt;_&lt;) &hearts;</span>
    <span class="copyright">pixelheartz collective 2026 -- made with too much caffeine and not enough sleep</span>
  </footer>

</body>
</html>
```
