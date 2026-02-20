# Barbiecore Design Reference

Barbiecore is a hyper-feminine, maximalist aesthetic centered on hot pink exuberance, glossy surfaces, and unapologetic glamour inspired by the iconic Mattel fashion doll. The trend surged into the cultural mainstream alongside Greta Gerwig's 2023 Barbie film, but its roots lie in decades of Barbie branding, Y2K fashion nostalgia, and the broader rejection of quiet minimalism in favor of bold self-expression. In web and UI design, Barbiecore translates to saturated pink palettes, rounded and bubbly typography, glossy or plastic-look surfaces, playful patterns such as polka dots, hearts, and stars, and an overall feeling of confident, joyful femininity. Every element is designed to be eye-catching and fun -- from shimmering gradient buttons to candy-colored card components -- while maintaining enough structure and contrast to remain functional and accessible.

---

## Visual Characteristics

### Core Design Traits

- **Hot pink dominance** -- the signature Barbie Pink (#E0218A) anchors every composition, supported by a spectrum of magentas, fuchsias, and pastel pinks
- **Glossy, plastic-look surfaces** -- elements feel smooth and reflective, using highlights, glass effects, and subtle shine animations to evoke molded plastic
- **Rounded, bubbly shapes** -- large border-radii on cards, buttons, and containers; pill shapes, circles, and soft blobs throughout
- **Maximalist layering** -- patterns, gradients, textures, and decorative elements are layered generously; more is more
- **Retro-feminine motifs** -- hearts, stars, bows, florals, lipstick marks, high heels, and other playful feminine iconography
- **Bold glamour typography** -- display fonts range from curvy scripts to chunky rounded sans-serifs, always leaning playful and confident
- **Shimmer and sparkle effects** -- CSS animations that mimic glitter, holographic sheens, or light catching a glossy surface
- **High-contrast color blocking** -- sections alternate between vivid pinks, whites, and accent colors for strong visual rhythm
- **Polka dots, stripes, and geometric patterns** -- used as background textures or decorative overlays to add depth and personality
- **Gold and metallic accents** -- gold foil effects, metallic borders, and warm metallics add a touch of luxury to the pink foundation

### Design Principles

- Lead with pink fearlessly: hot pink is the hero color, not an accent -- build outward from it
- Embrace glamour over subtlety: every surface should feel polished, finished, and intentionally extra
- Mix retro and modern: blend Y2K and vintage Barbie nostalgia with contemporary UI patterns and techniques
- Maintain playful confidence: the aesthetic is bold and self-assured, never apologetic about its femininity
- Balance maximalism with usability: decorative elements should enhance, not obscure, the user experience
- Use texture and shine to create tactile depth: glossy buttons, matte backgrounds, shimmer overlays
- Accessibility matters: ensure text contrast meets WCAG standards even within vibrant pink palettes

---

## Color Palette

### Barbiecore Core Palette

Colors range from the iconic Barbie Pink through supporting fuchsias, pastels, and accent tones. The palette balances hot vibrancy with softer tints and strategic neutrals.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Barbie Pink** | `#E0218A` | Primary brand color, hero backgrounds, CTAs, headings |
| **Hot Fuchsia** | `#FF2D8A` | Secondary accent, hover states, gradient endpoints |
| **Magenta Dream** | `#C7166F` | Deep pink for contrast, dark overlays, footer backgrounds |
| **Raspberry Gloss** | `#ED5C9B` | Mid-tone pink, card backgrounds, borders |
| **Pastel Rose** | `#F7B9D7` | Light pink tint, section backgrounds, soft cards |
| **Blush Whisper** | `#FDE4EF` | Lightest pink, page backgrounds, hover tints |
| **Cream White** | `#FFF5F9` | Near-white with warm pink undertone, body background |
| **Pure White** | `#FFFFFF` | Text on dark pink, card surfaces, clean space |
| **Bubblegum Purple** | `#C44DFF` | Accent for variety, tags, badges, secondary buttons |
| **Sky Glam** | `#7DD3FC` | Cool accent, info states, links on dark backgrounds |
| **Sunshine Gold** | `#FFD700` | Metallic accent, stars, premium indicators, borders |
| **Coral Pop** | `#FF6B6B` | Warm accent, notifications, alerts, decorative elements |
| **Mint Fizz** | `#A7F3D0` | Success states, fresh accent against pink |
| **Deep Glamour** | `#4A0E2B` | Dark text on light backgrounds, footer, deep contrast |
| **Muted Mauve** | `#8B6B7B` | Body text alternative, captions, muted labels |

### CSS Custom Properties

```css
:root {
  /* Primary pinks */
  --barbie-pink: #E0218A;
  --barbie-hot-fuchsia: #FF2D8A;
  --barbie-magenta: #C7166F;
  --barbie-raspberry: #ED5C9B;
  --barbie-pastel-rose: #F7B9D7;
  --barbie-blush: #FDE4EF;

  /* Neutrals */
  --barbie-bg-cream: #FFF5F9;
  --barbie-white: #FFFFFF;
  --barbie-text-dark: #4A0E2B;
  --barbie-text-muted: #8B6B7B;

  /* Accents */
  --barbie-purple: #C44DFF;
  --barbie-sky: #7DD3FC;
  --barbie-gold: #FFD700;
  --barbie-coral: #FF6B6B;
  --barbie-mint: #A7F3D0;

  /* Gradients */
  --barbie-gradient-glam: linear-gradient(135deg, #E0218A, #FF2D8A, #ED5C9B);
  --barbie-gradient-sunset: linear-gradient(135deg, #E0218A, #FF6B6B, #FFD700);
  --barbie-gradient-dream: linear-gradient(135deg, #F7B9D7, #FDE4EF, #FFFFFF);
  --barbie-gradient-holographic: linear-gradient(135deg, #E0218A, #C44DFF, #7DD3FC, #A7F3D0, #FFD700);

  /* Shadows */
  --barbie-shadow-pink: 0 4px 20px rgba(224, 33, 138, 0.25);
  --barbie-shadow-soft: 0 4px 16px rgba(224, 33, 138, 0.12);
  --barbie-shadow-glow: 0 0 30px rgba(224, 33, 138, 0.35);
}
```

---

## Typography

### Typeface Characteristics

Barbiecore typography is:

- **Rounded, playful, and confident** -- letterforms feel bubbly and feminine without being childish
- **Script and display fonts for impact** -- curvy scripts and bold display faces for headings and hero text
- **Clean sans-serifs for body** -- rounded geometric sans-serifs maintain readability at smaller sizes
- **Bold weights preferred** -- 600-800 for headings to ensure pink-on-light text remains legible
- **Occasional retro flair** -- fonts that evoke 1960s Barbie packaging or Y2K magazine covers

### Recommended Google Fonts

| Font | Style | Best For |
|------|-------|----------|
| **Sacramento** | Monoline script, retro elegance | Hero headlines, accent text, branding -- closest to Barbie script feel |
| **Dancing Script** | Casual script, flowing | Decorative headings, pull quotes, feminine flair |
| **Pacifico** | Casual script, bold | Display headlines, playful hero text |
| **Fredoka** | Rounded, chunky, bubbly | Section headings, buttons, labels |
| **Quicksand** | Geometric rounded sans-serif | Body text, balanced playfulness and legibility |
| **Nunito** | Rounded terminals, versatile | Body text, all-purpose friendly font |
| **Comfortaa** | Rounded geometric, modern | Navigation, subheadings, UI elements |
| **Poppins** | Geometric, clean, versatile | Body text, form elements, fallback font |
| **Playfair Display** | Elegant high-contrast serif | Glamorous headings, editorial-style titles |
| **Lobster** | Bold script, retro | Decorative accents, nostalgic headings |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Sacramento** (400) | **Quicksand** (400-500) | Elegant script meets bubbly body, classic Barbie feel |
| **Fredoka** (600-700) | **Nunito** (400) | Chunky playful headings with clean readable body |
| **Playfair Display** (700) | **Poppins** (400) | Glamorous editorial heads with modern body text |
| **Pacifico** (400) | **Comfortaa** (400) | Retro script flair paired with rounded modern body |
| **Dancing Script** (700) | **Quicksand** (400) | Flowing feminine heads with geometric body balance |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Quicksand:wght@400;500;600;700&family=Sacramento&display=swap');

h1, h2, h3, h4, h5, h6 {
  font-family: 'Fredoka', cursive;
  font-weight: 700;
  color: var(--barbie-text-dark);
  line-height: 1.2;
  letter-spacing: -0.01em;
}

.barbie-display {
  font-family: 'Sacramento', cursive;
  font-size: clamp(3rem, 7vw, 6rem);
  font-weight: 400;
  line-height: 1.1;
  color: var(--barbie-pink);
}

body {
  font-family: 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--barbie-text-dark);
}

.barbie-label {
  font-family: 'Fredoka', cursive;
  font-weight: 600;
  font-size: 0.85rem;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: var(--barbie-pink);
}

.barbie-caption {
  font-family: 'Quicksand', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--barbie-text-muted);
}

.barbie-script {
  font-family: 'Sacramento', cursive;
  font-weight: 400;
  font-size: 1.8rem;
  color: var(--barbie-pink);
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, generous layouts** -- max-width containers (1100-1200px) with ample padding create a polished, magazine-like feel
- **Rounded containers everywhere** -- border-radius of 24-40px on cards, sections, images, and buttons
- **Alternating section backgrounds** -- cycle between cream whites, soft pinks, and bold hot pink sections for rhythm
- **Pink-dominant hero areas** -- the hero section should be the most visually impactful, using large type and saturated backgrounds
- **Decorative patterns as section dividers** -- polka dot bands, wavy borders, or heart-shaped separators between sections
- **Card-heavy content organization** -- information grouped in rounded, glossy-feeling cards with soft shadows

### Section Organization

- **Navigation**: Pill-shaped or rounded nav bar with pink accent hover states; logo in script font
- **Hero**: Large script or display heading on a gradient pink background with sparkle effects and a glossy CTA button
- **Features**: Grid of rounded cards on pastel or white backgrounds, each with a pink icon or illustration
- **Showcase**: Full-width pink section with bold white text and lifestyle imagery
- **Testimonials**: Cards with heart-shaped quotation marks, pastel backgrounds, and rounded avatars
- **CTA section**: Gradient pink background with gold accents and a high-contrast button
- **Footer**: Deep magenta or dark pink background with lighter pink text and gold accent links

### Responsive Approach

- Stack sections vertically on mobile while preserving the bold pink identity
- Reduce decorative patterns and sparkle density on smaller screens
- Typography scales dramatically: hero script text shrinks gracefully with clamp()
- Buttons remain large and finger-friendly (minimum 48px touch targets) at all breakpoints
- Card grids collapse to single-column on mobile with maintained rounded corners and shadows
- Maintain glossy surface effects even on compact layouts

---

## CSS / Design Techniques

### Barbiecore Card Component

```css
.barbie-card {
  background: var(--barbie-white);
  border-radius: 28px;
  padding: 32px;
  position: relative;
  overflow: hidden;
  box-shadow: var(--barbie-shadow-soft);
  border: 2px solid var(--barbie-pastel-rose);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.barbie-card:hover {
  transform: translateY(-6px);
  box-shadow: var(--barbie-shadow-pink);
}

/* Glossy highlight overlay */
.barbie-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(180deg, rgba(255, 255, 255, 0.4) 0%, transparent 100%);
  border-radius: 28px 28px 0 0;
  pointer-events: none;
}

.barbie-card--pink {
  background: var(--barbie-blush);
  border-color: var(--barbie-raspberry);
}

.barbie-card--gradient {
  background: var(--barbie-gradient-dream);
  border-color: var(--barbie-pastel-rose);
}
```

### Barbiecore Button

```css
.barbie-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: var(--barbie-pink);
  color: #ffffff;
  border: none;
  border-radius: 50px;
  padding: 16px 40px;
  font-family: 'Fredoka', cursive;
  font-weight: 600;
  font-size: 1.05rem;
  cursor: pointer;
  text-decoration: none;
  box-shadow: var(--barbie-shadow-pink);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  position: relative;
  overflow: hidden;
}

.barbie-btn:hover {
  transform: translateY(-3px) scale(1.03);
  box-shadow: var(--barbie-shadow-glow);
}

/* Glossy shine sweep on hover */
.barbie-btn::after {
  content: '';
  position: absolute;
  top: -50%;
  left: -75%;
  width: 50%;
  height: 200%;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.3),
    transparent
  );
  transform: skewX(-25deg);
  transition: left 0.5s ease;
}

.barbie-btn:hover::after {
  left: 125%;
}

.barbie-btn--outline {
  background: transparent;
  color: var(--barbie-pink);
  border: 2px solid var(--barbie-pink);
  box-shadow: none;
}

.barbie-btn--outline:hover {
  background: var(--barbie-blush);
  box-shadow: var(--barbie-shadow-soft);
}

.barbie-btn--gold {
  background: linear-gradient(135deg, #FFD700, #FFA500);
  color: var(--barbie-text-dark);
  box-shadow: 0 4px 20px rgba(255, 215, 0, 0.3);
}
```

### Navigation Bar

```css
.barbie-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
}

.barbie-nav__logo {
  font-family: 'Sacramento', cursive;
  font-size: 2.2rem;
  color: var(--barbie-pink);
  text-decoration: none;
  transition: color 0.2s ease;
}

.barbie-nav__logo:hover {
  color: var(--barbie-hot-fuchsia);
}

.barbie-nav__links {
  display: flex;
  gap: 6px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.barbie-nav__links a {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: var(--barbie-text-dark);
  text-decoration: none;
  padding: 10px 22px;
  border-radius: 50px;
  transition: background 0.2s ease, color 0.2s ease;
}

.barbie-nav__links a:hover {
  background: var(--barbie-blush);
  color: var(--barbie-pink);
}

.barbie-nav__links a.active {
  background: var(--barbie-pink);
  color: #ffffff;
}
```

### Hero Section

```css
.barbie-hero {
  position: relative;
  text-align: center;
  padding: 100px 40px 80px;
  overflow: hidden;
  background: var(--barbie-gradient-dream);
}

.barbie-hero h1 {
  font-family: 'Sacramento', cursive;
  font-size: clamp(3.5rem, 8vw, 7rem);
  font-weight: 400;
  color: var(--barbie-pink);
  margin-bottom: 1rem;
  line-height: 1.1;
  text-shadow: 2px 2px 0px rgba(224, 33, 138, 0.1);
}

.barbie-hero p {
  font-size: 1.2rem;
  color: var(--barbie-text-muted);
  margin-bottom: 2.5rem;
  max-width: 560px;
  margin-left: auto;
  margin-right: auto;
}

/* Sparkle dots */
.barbie-hero__sparkle {
  position: absolute;
  width: 8px;
  height: 8px;
  background: var(--barbie-gold);
  border-radius: 50%;
  animation: sparkle 2s ease-in-out infinite;
}

@keyframes sparkle {
  0%, 100% { opacity: 0.2; transform: scale(0.8); }
  50% { opacity: 1; transform: scale(1.3); }
}
```

### Glossy Surface Effect

A key technique for Barbiecore is creating surfaces that feel like molded plastic or lacquered finish.

```css
.barbie-glossy {
  position: relative;
  background: var(--barbie-pink);
  border-radius: 24px;
  overflow: hidden;
}

/* Top highlight -- mimics overhead lighting on plastic */
.barbie-glossy::before {
  content: '';
  position: absolute;
  top: 0;
  left: 10%;
  right: 10%;
  height: 45%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.35) 0%,
    rgba(255, 255, 255, 0.1) 40%,
    transparent 100%
  );
  border-radius: 24px 24px 50% 50%;
  pointer-events: none;
}

/* Subtle bottom shadow for depth */
.barbie-glossy::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 5%;
  right: 5%;
  height: 20%;
  background: linear-gradient(
    0deg,
    rgba(0, 0, 0, 0.08) 0%,
    transparent 100%
  );
  pointer-events: none;
}
```

### Shimmer / Glitter Animation

Use this on headings, badges, or accent elements to create a glitter-sweep effect.

```css
.barbie-shimmer {
  position: relative;
  display: inline-block;
  overflow: hidden;
}

.barbie-shimmer::after {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    90deg,
    transparent 0%,
    rgba(255, 255, 255, 0.4) 40%,
    rgba(255, 255, 255, 0.6) 50%,
    rgba(255, 255, 255, 0.4) 60%,
    transparent 100%
  );
  animation: shimmerSweep 3s ease-in-out infinite;
}

@keyframes shimmerSweep {
  0% { left: -100%; }
  100% { left: 100%; }
}
```

### Polka Dot Background Pattern

```css
.barbie-polka {
  background-color: var(--barbie-blush);
  background-image: radial-gradient(
    circle,
    var(--barbie-pastel-rose) 8px,
    transparent 8px
  );
  background-size: 40px 40px;
}

.barbie-polka--pink {
  background-color: var(--barbie-pink);
  background-image: radial-gradient(
    circle,
    rgba(255, 255, 255, 0.15) 6px,
    transparent 6px
  );
  background-size: 32px 32px;
}
```

### Heart Divider

A decorative section divider using CSS-generated hearts.

```css
.barbie-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
  padding: 40px 0;
}

.barbie-divider__line {
  flex: 1;
  max-width: 200px;
  height: 2px;
  background: var(--barbie-gradient-glam);
  border-radius: 2px;
}

.barbie-divider__heart {
  position: relative;
  width: 24px;
  height: 22px;
  color: var(--barbie-pink);
}

.barbie-divider__heart::before,
.barbie-divider__heart::after {
  content: '';
  position: absolute;
  width: 14px;
  height: 22px;
  background: var(--barbie-pink);
  border-radius: 14px 14px 0 0;
}

.barbie-divider__heart::before {
  left: 0;
  transform: rotate(-45deg);
  transform-origin: bottom right;
}

.barbie-divider__heart::after {
  right: 0;
  transform: rotate(45deg);
  transform-origin: bottom left;
}
```

---

## Design Do's and Don'ts

### Do

- Lead every design with hot pink as the dominant color -- it should be the first thing the eye sees
- Use glossy surface effects, highlights, and subtle shine animations to create a plastic-fantastic feel
- Apply generous border-radius (24px+) on all containers, cards, images, and buttons
- Include playful decorative motifs: hearts, stars, sparkles, bows, and polka dots
- Layer pink tones from deep magenta to soft blush for depth and sophistication
- Use script or rounded display fonts for headings to maintain the feminine, playful character
- Add gold or metallic accents sparingly for a luxury feel
- Create hover interactions that feel glossy and satisfying (scale, glow, shimmer)
- Keep the overall tone confident and glamorous -- Barbiecore is bold, not shy
- Ensure text passes WCAG AA contrast requirements, especially light pink text on pink backgrounds

### Don't

- Use muted, earthy, or desaturated colors -- they contradict the vibrant energy
- Default to minimalist, sparse layouts -- Barbiecore thrives on visual richness and pattern
- Choose industrial or brutalist typography -- sharp, angular fonts clash with the bubbly spirit
- Use dark, moody color schemes as the primary palette -- darkness is only for accent contrast
- Leave large areas of plain white without any pink tint or pattern -- the warmth should be pervasive
- Overuse novelty fonts for body text -- keep body copy in clean, readable rounded sans-serifs
- Add so many decorative elements that content becomes hard to find or interact with
- Forget mobile optimization -- glossy effects and rounded layouts must scale gracefully
- Mix in clashing aesthetic signals like grunge textures, distressed type, or raw industrial elements

---

## Related Aesthetics

| Aesthetic | Relationship to Barbiecore |
|-----------|---------------------------|
| **Coquette** | Sister aesthetic; both embrace hyper-femininity, but Coquette leans softer with ribbons and pastels while Barbiecore is louder and pinker |
| **Y2K Futurism** | Shares the early-2000s nostalgia, glossy surfaces, and saturated color; Y2K adds chrome and silver tones |
| **Dopamine Design** | Both are maximalist and joy-driven; Dopamine Design uses the full rainbow while Barbiecore is pink-dominant |
| **Gen Z Maximalism** | Shares the more-is-more philosophy and internet-era visual language; Barbiecore focuses that energy through a pink, feminine lens |
| **Colorful Pop** | Both celebrate saturated color and graphic boldness; Barbiecore constrains the palette around pink |
| **Cutecore** | Shares playful, rounded shapes and joyful energy; Cutecore leans kawaii while Barbiecore leans glamour |
| **Frutiger Aero** | Both use glossy, plastic-look surfaces; Frutiger Aero applies them to nature and tech themes rather than feminine glamour |
| **Maximalism** | Parent philosophy; Barbiecore is maximalism filtered through a specific pink, feminine, pop-culture lens |
| **Hollywood Regency** | Shares the glamour and luxury emphasis; Hollywood Regency is more sophisticated and gold-heavy |
| **Danish Pastel** | Both use soft pink tones but Danish Pastel is muted and minimal where Barbiecore is saturated and maximal |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Barbiecore Design Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Quicksand:wght@400;500;600;700&family=Sacramento&display=swap" rel="stylesheet">
  <style>
    :root {
      --barbie-pink: #E0218A;
      --barbie-hot-fuchsia: #FF2D8A;
      --barbie-magenta: #C7166F;
      --barbie-raspberry: #ED5C9B;
      --barbie-pastel-rose: #F7B9D7;
      --barbie-blush: #FDE4EF;
      --barbie-bg-cream: #FFF5F9;
      --barbie-white: #FFFFFF;
      --barbie-text-dark: #4A0E2B;
      --barbie-text-muted: #8B6B7B;
      --barbie-purple: #C44DFF;
      --barbie-sky: #7DD3FC;
      --barbie-gold: #FFD700;
      --barbie-coral: #FF6B6B;
      --barbie-mint: #A7F3D0;
      --barbie-shadow-pink: 0 4px 20px rgba(224, 33, 138, 0.25);
      --barbie-shadow-soft: 0 4px 16px rgba(224, 33, 138, 0.12);
      --barbie-shadow-glow: 0 0 30px rgba(224, 33, 138, 0.35);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--barbie-bg-cream);
      color: var(--barbie-text-dark);
      font-family: 'Quicksand', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3, h4 {
      font-family: 'Fredoka', cursive;
      font-weight: 700;
      line-height: 1.2;
    }

    /* --- Navigation --- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
    }

    nav a.logo {
      font-family: 'Sacramento', cursive;
      font-size: 2.4rem;
      color: var(--barbie-pink);
      text-decoration: none;
      transition: color 0.2s;
    }

    nav a.logo:hover { color: var(--barbie-hot-fuchsia); }

    nav ul {
      display: flex;
      gap: 6px;
      list-style: none;
    }

    nav ul a {
      color: var(--barbie-text-dark);
      text-decoration: none;
      font-weight: 600;
      font-size: 0.95rem;
      padding: 10px 22px;
      border-radius: 50px;
      transition: background 0.2s, color 0.2s;
    }

    nav ul a:hover {
      background: var(--barbie-blush);
      color: var(--barbie-pink);
    }

    /* --- Hero Section --- */
    .hero {
      position: relative;
      text-align: center;
      padding: 80px 40px 90px;
      overflow: hidden;
      background: linear-gradient(180deg, var(--barbie-blush) 0%, var(--barbie-bg-cream) 100%);
      border-radius: 0 0 48px 48px;
    }

    .hero h1 {
      font-family: 'Sacramento', cursive;
      font-size: clamp(3.5rem, 8vw, 7rem);
      font-weight: 400;
      color: var(--barbie-pink);
      margin-bottom: 0.5rem;
      line-height: 1.1;
    }

    .hero .tagline {
      font-family: 'Fredoka', cursive;
      font-size: clamp(1.2rem, 3vw, 1.6rem);
      font-weight: 500;
      color: var(--barbie-raspberry);
      margin-bottom: 1.5rem;
    }

    .hero p {
      font-size: 1.15rem;
      color: var(--barbie-text-muted);
      margin-bottom: 2.5rem;
      max-width: 540px;
      margin-left: auto;
      margin-right: auto;
    }

    /* Sparkle dots in hero */
    .sparkle {
      position: absolute;
      width: 8px;
      height: 8px;
      background: var(--barbie-gold);
      border-radius: 50%;
      animation: sparkle 2s ease-in-out infinite;
    }

    @keyframes sparkle {
      0%, 100% { opacity: 0.2; transform: scale(0.8); }
      50% { opacity: 1; transform: scale(1.4); }
    }

    /* Floating hearts in hero */
    .heart-float {
      position: absolute;
      font-size: 1.5rem;
      opacity: 0.15;
      animation: floatHeart 7s ease-in-out infinite;
    }

    @keyframes floatHeart {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      33% { transform: translateY(-15px) rotate(5deg); }
      66% { transform: translateY(-8px) rotate(-3deg); }
    }

    /* Buttons */
    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      border: none;
      border-radius: 50px;
      padding: 16px 40px;
      font-family: 'Fredoka', cursive;
      font-weight: 600;
      font-size: 1.05rem;
      cursor: pointer;
      text-decoration: none;
      transition: transform 0.2s, box-shadow 0.2s;
      position: relative;
      overflow: hidden;
    }

    .btn--primary {
      background: var(--barbie-pink);
      color: #ffffff;
      box-shadow: var(--barbie-shadow-pink);
    }

    .btn--primary:hover {
      transform: translateY(-3px) scale(1.03);
      box-shadow: var(--barbie-shadow-glow);
    }

    .btn--outline {
      background: transparent;
      color: var(--barbie-pink);
      border: 2px solid var(--barbie-pink);
      box-shadow: none;
    }

    .btn--outline:hover {
      background: var(--barbie-blush);
      transform: translateY(-2px);
      box-shadow: var(--barbie-shadow-soft);
    }

    /* Shimmer sweep on primary button */
    .btn--primary::after {
      content: '';
      position: absolute;
      top: -50%;
      left: -75%;
      width: 50%;
      height: 200%;
      background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
      transform: skewX(-25deg);
      transition: left 0.5s ease;
    }

    .btn--primary:hover::after {
      left: 125%;
    }

    .btn-group {
      display: flex;
      gap: 16px;
      justify-content: center;
      flex-wrap: wrap;
    }

    /* --- Features Section --- */
    .features {
      padding: 80px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .features h2 {
      text-align: center;
      font-size: 2.2rem;
      margin-bottom: 12px;
      color: var(--barbie-pink);
    }

    .features .subtitle {
      text-align: center;
      color: var(--barbie-text-muted);
      font-size: 1.05rem;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
    }

    .feature-card {
      background: var(--barbie-white);
      border-radius: 28px;
      padding: 32px;
      border: 2px solid var(--barbie-pastel-rose);
      box-shadow: var(--barbie-shadow-soft);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      position: relative;
      overflow: hidden;
    }

    .feature-card:hover {
      transform: translateY(-6px);
      box-shadow: var(--barbie-shadow-pink);
    }

    /* Glossy top highlight */
    .feature-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 10%;
      right: 10%;
      height: 40%;
      background: linear-gradient(180deg, rgba(255,255,255,0.5) 0%, transparent 100%);
      border-radius: 28px;
      pointer-events: none;
    }

    .feature-icon {
      width: 56px;
      height: 56px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      margin-bottom: 20px;
      position: relative;
      z-index: 1;
    }

    .feature-card h3 {
      font-size: 1.25rem;
      margin-bottom: 8px;
      position: relative;
      z-index: 1;
    }

    .feature-card p {
      font-size: 0.95rem;
      color: var(--barbie-text-muted);
      line-height: 1.6;
      position: relative;
      z-index: 1;
    }

    /* --- Showcase Section (polka dot background) --- */
    .showcase {
      background-color: var(--barbie-pink);
      background-image: radial-gradient(circle, rgba(255,255,255,0.12) 6px, transparent 6px);
      background-size: 32px 32px;
      padding: 80px 40px;
      text-align: center;
      color: #ffffff;
    }

    .showcase h2 {
      font-size: 2.4rem;
      color: #ffffff;
      margin-bottom: 16px;
    }

    .showcase p {
      font-size: 1.1rem;
      opacity: 0.9;
      max-width: 600px;
      margin: 0 auto 32px;
    }

    .showcase-stats {
      display: flex;
      justify-content: center;
      gap: 48px;
      flex-wrap: wrap;
    }

    .stat {
      text-align: center;
    }

    .stat-number {
      font-family: 'Fredoka', cursive;
      font-size: 2.5rem;
      font-weight: 700;
      display: block;
      text-shadow: 2px 2px 0 rgba(0,0,0,0.1);
    }

    .stat-label {
      font-size: 0.9rem;
      opacity: 0.85;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      font-weight: 600;
    }

    /* --- Testimonial Section --- */
    .testimonials {
      padding: 80px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .testimonials h2 {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 48px;
      color: var(--barbie-pink);
    }

    .testimonial-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
    }

    .testimonial {
      background: var(--barbie-blush);
      border-radius: 24px;
      padding: 32px;
      position: relative;
    }

    .testimonial::before {
      content: '\2665';
      position: absolute;
      top: 16px;
      right: 20px;
      font-size: 2rem;
      color: var(--barbie-pastel-rose);
    }

    .testimonial p {
      font-size: 1rem;
      font-style: italic;
      margin-bottom: 16px;
      line-height: 1.6;
    }

    .testimonial-author {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .testimonial-avatar {
      width: 44px;
      height: 44px;
      border-radius: 50%;
      background: var(--barbie-pink);
      color: #fff;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Fredoka', cursive;
      font-weight: 600;
      font-size: 1rem;
    }

    .testimonial-name {
      font-weight: 700;
      font-size: 0.95rem;
    }

    .testimonial-role {
      font-size: 0.8rem;
      color: var(--barbie-text-muted);
    }

    /* --- CTA Section --- */
    .cta {
      background: linear-gradient(135deg, var(--barbie-pink), var(--barbie-hot-fuchsia), var(--barbie-raspberry));
      color: #ffffff;
      text-align: center;
      padding: 80px 40px;
      border-radius: 48px;
      max-width: 1100px;
      margin: 0 auto 40px;
      position: relative;
      overflow: hidden;
    }

    .cta::before {
      content: '';
      position: absolute;
      top: 0;
      left: 10%;
      right: 10%;
      height: 40%;
      background: linear-gradient(180deg, rgba(255,255,255,0.2) 0%, transparent 100%);
      border-radius: 48px;
      pointer-events: none;
    }

    .cta h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
      color: #ffffff;
      position: relative;
      z-index: 1;
    }

    .cta p {
      font-size: 1.1rem;
      opacity: 0.92;
      margin-bottom: 2rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
      position: relative;
      z-index: 1;
    }

    .cta .btn--primary {
      background: var(--barbie-white);
      color: var(--barbie-pink);
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
      position: relative;
      z-index: 1;
    }

    .cta .btn--primary:hover {
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
    }

    /* --- Heart Divider --- */
    .divider {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      padding: 24px 0;
    }

    .divider-line {
      width: 120px;
      height: 2px;
      background: linear-gradient(90deg, transparent, var(--barbie-pastel-rose), transparent);
      border-radius: 2px;
    }

    .divider-icon {
      color: var(--barbie-pink);
      font-size: 1.2rem;
    }

    /* --- Footer --- */
    footer {
      background: var(--barbie-magenta);
      color: var(--barbie-pastel-rose);
      text-align: center;
      padding: 48px 40px;
      font-size: 0.9rem;
    }

    footer a {
      color: var(--barbie-gold);
      text-decoration: none;
    }

    footer a:hover {
      text-decoration: underline;
    }

    footer .footer-links {
      display: flex;
      justify-content: center;
      gap: 24px;
      margin-bottom: 16px;
      flex-wrap: wrap;
    }

    footer .footer-brand {
      font-family: 'Sacramento', cursive;
      font-size: 1.8rem;
      color: #ffffff;
      margin-bottom: 12px;
    }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      nav { padding: 16px 20px; }
      nav ul { gap: 4px; }
      nav ul a { padding: 8px 14px; font-size: 0.85rem; }
      .hero { padding: 60px 24px 70px; border-radius: 0 0 32px 32px; }
      .features { padding: 60px 24px; }
      .showcase { padding: 60px 24px; }
      .showcase-stats { gap: 32px; }
      .testimonials { padding: 60px 24px; }
      .cta { border-radius: 32px; margin: 0 16px 24px; padding: 60px 24px; }
      footer { padding: 40px 24px; }
    }

    @media (max-width: 480px) {
      nav { flex-direction: column; gap: 12px; }
      .btn-group { flex-direction: column; align-items: center; }
      .btn { width: 100%; justify-content: center; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Glamour</a>
    <ul>
      <li><a href="#">Shop</a></li>
      <li><a href="#">Lookbook</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <!-- Sparkle decorations -->
    <div class="sparkle" style="top:12%; left:8%;"></div>
    <div class="sparkle" style="top:25%; right:12%; animation-delay:-0.7s; width:6px; height:6px;"></div>
    <div class="sparkle" style="bottom:20%; left:15%; animation-delay:-1.3s;"></div>
    <div class="sparkle" style="top:18%; right:25%; animation-delay:-0.4s; width:5px; height:5px;"></div>
    <div class="sparkle" style="bottom:30%; right:10%; animation-delay:-1.8s;"></div>
    <div class="sparkle" style="top:40%; left:22%; animation-delay:-1s; width:6px; height:6px;"></div>

    <!-- Floating hearts -->
    <div class="heart-float" style="top:15%; left:5%; font-size:2rem; animation-delay:-1s;">&hearts;</div>
    <div class="heart-float" style="top:30%; right:7%; font-size:1.8rem; animation-delay:-3s;">&hearts;</div>
    <div class="heart-float" style="bottom:20%; left:10%; font-size:1.4rem; animation-delay:-5s;">&hearts;</div>
    <div class="heart-float" style="bottom:35%; right:18%; font-size:1.6rem; animation-delay:-2s;">&hearts;</div>

    <h1>Life in Pink</h1>
    <div class="tagline">Bold. Glossy. Unapologetically Glamorous.</div>
    <p>A celebration of hot pink maximalism, retro femininity, and plastic-fantastic vibes. Everything you need to live your best Barbiecore life.</p>
    <div class="btn-group">
      <a href="#" class="btn btn--primary">Explore Collection</a>
      <a href="#" class="btn btn--outline">Learn More</a>
    </div>
  </section>

  <div class="divider" style="padding:40px 0;">
    <span class="divider-line"></span>
    <span class="divider-icon">&hearts;</span>
    <span class="divider-line"></span>
  </div>

  <section class="features">
    <h2>Why Barbiecore?</h2>
    <p class="subtitle">More than a trend -- it is a bold design philosophy built on joy, confidence, and pink.</p>
    <div class="features-grid">
      <div class="feature-card">
        <div class="feature-icon" style="background: var(--barbie-pink); color: #fff;">&#9733;</div>
        <h3>Maximum Glamour</h3>
        <p>Every surface shines, every element sparkles. Glossy finishes and bold pink gradients create an irresistibly polished aesthetic.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon" style="background: var(--barbie-purple); color: #fff;">&#9829;</div>
        <h3>Playful Femininity</h3>
        <p>Hearts, bows, and retro-feminine motifs celebrate a confident, unapologetic femininity that refuses to be quiet.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon" style="background: var(--barbie-coral); color: #fff;">&#10024;</div>
        <h3>Joyful Maximalism</h3>
        <p>More is more. Patterns layer on gradients, sparkles accent every corner, and color fills every pixel with energy.</p>
      </div>
    </div>
  </section>

  <section class="showcase">
    <h2>Designed to Stand Out</h2>
    <p>In a world of muted minimalism, Barbiecore dares to be loud, glossy, and unforgettable.</p>
    <div class="showcase-stats">
      <div class="stat">
        <span class="stat-number">100%</span>
        <span class="stat-label">Pink Energy</span>
      </div>
      <div class="stat">
        <span class="stat-number">24px+</span>
        <span class="stat-label">Border Radius</span>
      </div>
      <div class="stat">
        <span class="stat-number">&infin;</span>
        <span class="stat-label">Sparkle Factor</span>
      </div>
      <div class="stat">
        <span class="stat-number">0</span>
        <span class="stat-label">Dull Moments</span>
      </div>
    </div>
  </section>

  <section class="testimonials">
    <h2>What People Are Saying</h2>
    <div class="testimonial-grid">
      <div class="testimonial">
        <p>"This aesthetic transformed my entire brand. My audience engagement tripled the week I switched to a Barbiecore palette."</p>
        <div class="testimonial-author">
          <div class="testimonial-avatar">K</div>
          <div>
            <div class="testimonial-name">Kayla Reeves</div>
            <div class="testimonial-role">Brand Designer</div>
          </div>
        </div>
      </div>
      <div class="testimonial">
        <p>"I was skeptical about all the pink at first, but the glossy finishes and bold layout make everything feel so premium."</p>
        <div class="testimonial-author">
          <div class="testimonial-avatar">M</div>
          <div>
            <div class="testimonial-name">Maya Chen</div>
            <div class="testimonial-role">Product Manager</div>
          </div>
        </div>
      </div>
      <div class="testimonial">
        <p>"Finally, a design system that is not afraid to be fun. The sparkle effects and rounded cards make every page feel like a celebration."</p>
        <div class="testimonial-author">
          <div class="testimonial-avatar">R</div>
          <div>
            <div class="testimonial-name">Rosa Jimenez</div>
            <div class="testimonial-role">UX Engineer</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Ready to Go Pink?</h2>
    <p>Join the movement. Bold, glossy, and unapologetically glamorous design starts here.</p>
    <a href="#" class="btn btn--primary">Get Started</a>
  </section>

  <footer>
    <div class="footer-brand">Glamour</div>
    <div class="footer-links">
      <a href="#">Shop</a>
      <a href="#">Lookbook</a>
      <a href="#">About</a>
      <a href="#">Contact</a>
      <a href="#">Privacy</a>
    </div>
    <p>Built with Barbiecore design principles. Bold, pink, and always fabulous.</p>
  </footer>
</body>
</html>
```
