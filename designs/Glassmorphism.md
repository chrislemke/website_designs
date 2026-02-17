# Glassmorphism

## Overview

Glassmorphism is a UI design aesthetic built around translucent, frosted-glass surfaces that float above vivid, colorful backgrounds. The effect creates depth and visual hierarchy through semi-transparent elements with background blur, mimicking the look of frosted or etched glass. It emerged as a dominant interface trend following Apple's macOS Big Sur (2020) and Microsoft's Fluent Design System, and has since become a staple of modern dashboard, card, and overlay design.

## Visual Characteristics

- **Frosted glass panels**: Semi-transparent surfaces with Gaussian background blur that allow underlying content to show through in a softened, diffused way
- **Depth through layering**: UI elements appear to float above the background rather than being embedded in a flat plane; multiple glass layers can stack to create parallax-like depth
- **Matte finish**: Modern glassmorphism avoids glossy reflections in favor of a clean, minimal frosted appearance
- **Light borders**: Subtle semi-transparent white strokes along element edges simulate the refraction of light at the edge of real glass
- **Soft shadows**: Minimal, diffused drop shadows reinforce the floating sensation without heavy visual weight
- **Rounded corners**: Generous border-radius values soften the geometry of glass panels
- **Vivid backgrounds**: The effect achieves maximum impact when glass elements sit over colorful gradient backgrounds, photographs, or abstract shapes that accentuate the blur

### Three Pillars (Nielsen Norman Group)

According to the Nielsen Norman Group framework, glassmorphism requires the interplay of exactly three properties:

1. **Reduced fill opacity** so the background remains partially visible
2. **Background blur** (mandatory) to maintain text readability over complex backgrounds
3. **Semi-transparent borders** to distinguish element boundaries on both dark and light surfaces

Without all three, the result is simple transparency rather than glassmorphism.

## Color Palette

### Glass Surface Colors

| Role | Value | Description |
|------|-------|-------------|
| Light glass fill | `rgba(255, 255, 255, 0.15)` | Primary glass surface (light theme) |
| Medium glass fill | `rgba(255, 255, 255, 0.25)` | Higher-contrast glass surface |
| Heavy glass fill | `rgba(255, 255, 255, 0.40)` | Dense frosted panel |
| Dark glass fill | `rgba(17, 25, 40, 0.75)` | Dark-mode glass surface |
| Dark glass fill (alt) | `rgba(0, 0, 0, 0.25)` | Subtle dark overlay |

### Border Colors

| Role | Value | Description |
|------|-------|-------------|
| Light border | `rgba(255, 255, 255, 0.20)` | Standard glass edge |
| Medium border | `rgba(255, 255, 255, 0.30)` | More visible edge |
| Strong border | `rgba(255, 255, 255, 0.50)` | High-contrast edge highlight |

### Background Gradient Swatches

Glassmorphism backgrounds are typically vivid, multi-color gradients. These hex values represent common starting points:

| Swatch | Hex | Usage |
|--------|-----|-------|
| Deep Purple | `#4A00E0` | Gradient anchor (cool) |
| Electric Blue | `#2575FC` | Gradient anchor (cool) |
| Hot Pink | `#FF0099` | Gradient accent (warm) |
| Coral | `#FF6B6B` | Gradient accent (warm) |
| Violet | `#8E2DE2` | Gradient mid-tone |
| Cyan | `#00D2FF` | Gradient highlight |
| Amber | `#FFB347` | Gradient warm accent |
| Soft Lavender | `#C471F5` | Gradient soft accent |
| Dark base | `#04060A` | Deep dark background |
| Off-white | `#F9FAFB` | Light background base |

### Example Gradient Combinations

```css
/* Cool purple-blue */
background: linear-gradient(135deg, #4A00E0 0%, #2575FC 100%);

/* Warm pink-orange */
background: linear-gradient(135deg, #FF0099 0%, #FFB347 100%);

/* Rich violet-cyan */
background: linear-gradient(135deg, #8E2DE2 0%, #00D2FF 100%);

/* Dark moody */
background: linear-gradient(135deg, #0F0C29 0%, #302B63 50%, #24243E 100%);

/* Mesh gradient (multi-stop) */
background:
  radial-gradient(at 20% 30%, #FF009966 0%, transparent 50%),
  radial-gradient(at 80% 70%, #2575FC66 0%, transparent 50%),
  radial-gradient(at 50% 50%, #8E2DE266 0%, transparent 60%),
  #0F0C29;
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Inter** | 300, 400, 500, 600 | Primary UI text; excellent legibility on translucent surfaces | [Inter](https://fonts.google.com/specimen/Inter) |
| **Poppins** | 300, 400, 500, 600 | Headings and display text; geometric, modern feel | [Poppins](https://fonts.google.com/specimen/Poppins) |
| **DM Sans** | 400, 500, 700 | Clean alternative for body text | [DM Sans](https://fonts.google.com/specimen/DM+Sans) |
| **Space Grotesk** | 400, 500, 700 | Techy, futuristic headings | [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) |
| **Outfit** | 300, 400, 600 | Soft geometric sans-serif; pairs well with glass surfaces | [Outfit](https://fonts.google.com/specimen/Outfit) |

### Typography Guidelines

- Use **white or near-white text** (`#FFFFFF` or `rgba(255, 255, 255, 0.90)`) on dark/vivid backgrounds
- Use **dark text** (`#111927` or `rgba(0, 0, 0, 0.85)`) on light glass surfaces
- Prefer **medium weight** (500) for body text on glass to maintain readability through the blur
- Keep font sizes generous; small text becomes illegible on translucent surfaces
- Avoid thin (100-200) weights on glass panels; the blur competes with delicate letterforms
- Add subtle `text-shadow: 0 1px 2px rgba(0, 0, 0, 0.1)` for improved legibility if needed

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Poppins:wght@300;400;500;600&display=swap');

body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Poppins', sans-serif;
  font-weight: 600;
  letter-spacing: -0.02em;
}
```

## Layout Principles

- **Floating card paradigm**: Glass panels hover above the background, separated by blur and shadow rather than hard edges
- **Generous spacing**: Padding and margins should be ample (24-48px internal padding, 24-32px gaps between cards) to let the frosted effect breathe
- **Layered depth**: Stack glass elements at different opacity and blur levels to create a z-axis hierarchy; background layers get heavier blur, foreground layers get lighter blur
- **Background context**: Always ensure the background behind glass panels is visually interesting (gradients, images, abstract shapes); glass over a flat white background produces no visible effect
- **Centered and symmetrical layouts**: Cards and panels are often centered on the page or arranged in balanced grid layouts
- **Limit glass surfaces**: Do not apply the glass effect to every element; reserve it for primary content cards, modals, navigation bars, and sidebars to maintain visual impact
- **Avoid stacking too many blur layers**: Each `backdrop-filter` layer triggers GPU compositing; stacking more than 2-3 layers can cause performance issues on mobile devices

## CSS Code Snippets

### Basic Glass Card

```css
.glass-card {
  background: rgba(255, 255, 255, 0.15);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.20);
  border-radius: 16px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.10);
  padding: 32px;
  color: #ffffff;
}
```

### Enhanced Glass Card with Inset Highlights

```css
.glass-card-enhanced {
  background: rgba(255, 255, 255, 0.15);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  border: 1px solid rgba(255, 255, 255, 0.30);
  border-radius: 20px;
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.10),
    inset 0 1px 0 rgba(255, 255, 255, 0.50),
    inset 0 -1px 0 rgba(255, 255, 255, 0.10);
  padding: 32px;
  color: #ffffff;
}
```

### Dark Mode Glass Card

```css
.glass-card-dark {
  background: rgba(17, 25, 40, 0.75);
  backdrop-filter: blur(14px) saturate(150%);
  -webkit-backdrop-filter: blur(14px) saturate(150%);
  border: 1px solid rgba(255, 255, 255, 0.12);
  border-radius: 16px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.37);
  padding: 32px;
  color: rgba(255, 255, 255, 0.90);
}
```

### Glass Navigation Bar

```css
.glass-nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  background: rgba(255, 255, 255, 0.10);
  backdrop-filter: blur(20px) saturate(180%);
  -webkit-backdrop-filter: blur(20px) saturate(180%);
  border-bottom: 1px solid rgba(255, 255, 255, 0.15);
  padding: 16px 32px;
}
```

### Vivid Gradient Background

```css
.glass-background {
  min-height: 100vh;
  background: linear-gradient(135deg, #4A00E0 0%, #8E2DE2 50%, #00D2FF 100%);
  /* Optional: add floating shapes for visual interest behind glass */
  position: relative;
  overflow: hidden;
}

/* Decorative blurred shapes behind glass panels */
.glass-background::before {
  content: '';
  position: absolute;
  width: 400px;
  height: 400px;
  background: rgba(255, 0, 153, 0.40);
  border-radius: 50%;
  top: -100px;
  right: -100px;
  filter: blur(80px);
}

.glass-background::after {
  content: '';
  position: absolute;
  width: 300px;
  height: 300px;
  background: rgba(0, 210, 255, 0.30);
  border-radius: 50%;
  bottom: -50px;
  left: -50px;
  filter: blur(80px);
}
```

### Glass Button

```css
.glass-button {
  background: rgba(255, 255, 255, 0.15);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.25);
  border-radius: 12px;
  padding: 12px 28px;
  color: #ffffff;
  font-weight: 500;
  cursor: pointer;
  transition: all 0.3s ease;
}

.glass-button:hover {
  background: rgba(255, 255, 255, 0.25);
  border-color: rgba(255, 255, 255, 0.40);
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
  transform: translateY(-1px);
}
```

### Glass Input Field

```css
.glass-input {
  background: rgba(255, 255, 255, 0.08);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 12px;
  padding: 14px 20px;
  color: #ffffff;
  font-size: 1rem;
  outline: none;
  transition: border-color 0.3s ease, background 0.3s ease;
}

.glass-input::placeholder {
  color: rgba(255, 255, 255, 0.50);
}

.glass-input:focus {
  border-color: rgba(255, 255, 255, 0.40);
  background: rgba(255, 255, 255, 0.12);
}
```

### Full Page Starter Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Glassmorphism Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Inter', sans-serif;
      min-height: 100vh;
      background: linear-gradient(135deg, #0F0C29 0%, #302B63 50%, #24243E 100%);
      color: #ffffff;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }

    /* Decorative background blobs */
    .blob {
      position: absolute;
      border-radius: 50%;
      filter: blur(80px);
      opacity: 0.6;
    }
    .blob-1 { width: 500px; height: 500px; background: #FF0099; top: -150px; left: -100px; }
    .blob-2 { width: 400px; height: 400px; background: #2575FC; bottom: -100px; right: -80px; }
    .blob-3 { width: 300px; height: 300px; background: #8E2DE2; top: 50%; left: 60%; }

    .glass-card {
      position: relative;
      z-index: 1;
      background: rgba(255, 255, 255, 0.10);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid rgba(255, 255, 255, 0.20);
      border-radius: 20px;
      box-shadow: 0 8px 32px rgba(0, 0, 0, 0.20);
      padding: 40px;
      max-width: 480px;
      width: 90%;
    }

    .glass-card h1 {
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      font-size: 1.75rem;
      margin-bottom: 12px;
    }

    .glass-card p {
      font-weight: 300;
      line-height: 1.7;
      color: rgba(255, 255, 255, 0.80);
    }
  </style>
</head>
<body>
  <div class="blob blob-1"></div>
  <div class="blob blob-2"></div>
  <div class="blob blob-3"></div>
  <div class="glass-card">
    <h1>Glass Panel</h1>
    <p>Content floats above a vivid gradient background,
       with frosted blur creating depth and hierarchy.</p>
  </div>
</body>
</html>
```

## Implementation Tips

- **Never use the CSS `opacity` property** on a glass element. It reduces the opacity of the entire element including its content and children, breaking the backdrop-filter effect. Always use `rgba()` or `hsla()` for the `background` property instead.
- **Always include the `-webkit-` prefix**: `backdrop-filter` requires `-webkit-backdrop-filter` for Safari and older WebKit browsers.
- **Add `saturate()`** to the backdrop-filter for richer color bleed-through: `backdrop-filter: blur(12px) saturate(150%)`.
- **Test on real devices**: `backdrop-filter` triggers GPU compositing which can affect performance on lower-end mobile hardware. Limit glass panels to key UI surfaces.
- **Provide fallbacks**: For browsers that do not support `backdrop-filter`, use `@supports` to fall back to a solid semi-transparent background.
- **Blur range**: 8-12px produces a subtle frost; 16-24px produces a heavy, diffused frost. Values above 30px rarely add visible improvement and cost performance.
- **Background matters**: If the background behind a glass panel is a flat solid color, the glass effect is invisible. Always pair glass surfaces with gradients, images, or colorful abstract shapes.

```css
/* Fallback for browsers without backdrop-filter support */
@supports not (backdrop-filter: blur(12px)) {
  .glass-card {
    background: rgba(30, 30, 60, 0.85);
  }
}
```

## Related Aesthetics

- **Frutiger Aero** -- Shares translucency and gloss but adds organic nature imagery and skeuomorphic textures
- **Neumorphism** -- Embossed/extruded surfaces using matching background colors and directional shadows; monochromatic rather than transparent
- **Claymorphism** -- 3D clay-like surfaces with solid pastel fills and pronounced outer shadows; opaque rather than transparent
- **Flat Design** -- Predecessor aesthetic that eliminated depth entirely; glassmorphism reintroduces depth through transparency rather than shadows
- **Skeuomorphism** -- Historical precursor with glossy reflections and realistic textures; glassmorphism retains the glass metaphor but strips away realism
- **Cyberminimalism** -- Shares the clean, minimal approach and dark backgrounds but relies on stark contrast rather than blur effects
- **Dark Aero** -- Overlaps in the use of translucent dark surfaces and saturated accent colors
