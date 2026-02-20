# Parallax Design

## Overview

Parallax Design is a web design technique that creates the illusion of depth and spatial dimension by moving background elements at a different speed than foreground content as the user scrolls. Inspired by the multiplane camera technique pioneered in classic animation, this approach layers visual elements at varying depths along the Z-axis, producing a cinematic sense of immersion within a two-dimensional browser viewport. Parallax websites are particularly effective for narrative-driven experiences, product showcases, and brand storytelling, where the scroll itself becomes a mechanism for guiding the user through a curated visual journey. The technique rose to mainstream prominence around 2011 and has remained a durable staple of modern web design, evolving from simple background-attachment tricks to sophisticated CSS 3D transforms and scroll-driven animations. At its best, parallax design transforms passive scrolling into an engaging experience that rewards exploration with fluid motion and layered depth.

## Visual Characteristics

### Core Design Traits

- **Layered depth**: Content is organized into distinct foreground, midground, and background layers that move at different scroll speeds, creating a convincing illusion of spatial depth within the page
- **Full-viewport sections**: Each major content block typically occupies the full viewport height, creating a "scene-by-scene" progression that reinforces the storytelling structure
- **Cinematic imagery**: Large, high-quality photographic or illustrated backgrounds serve as the visual foundation, often spanning the full width and height of each section
- **Scroll-triggered reveals**: Content elements animate into view as the user scrolls, using fade-ins, slide-ups, and scale transitions tied to scroll position rather than time
- **Minimal UI chrome**: Navigation and interface elements are deliberately understated to keep focus on the immersive content, often using fixed transparent headers or hidden hamburger menus
- **Dramatic whitespace**: Generous spacing between content blocks allows each parallax scene to breathe and prevents visual overload from competing motion effects
- **Bold typographic hierarchy**: Large, high-contrast headings anchor each section, readable against moving backgrounds, with clear visual separation between headline, subhead, and body text

### Design Principles

- **Progressive disclosure**: Information is revealed gradually through the scroll journey, maintaining curiosity and encouraging users to continue exploring deeper into the page
- **Purposeful motion**: Every parallax movement serves a narrative or functional goal; motion is never decorative but always guides attention or reinforces the content hierarchy
- **Performance-first layering**: Layers are constructed with GPU-accelerated transforms (translate3d, will-change) to ensure smooth 60fps scrolling even with multiple moving elements
- **Accessible degradation**: The design remains fully functional and readable when parallax effects are disabled or unsupported, ensuring content is never locked behind scroll animations
- **Rhythm and pacing**: The speed differential between layers creates a visual rhythm that mirrors the content's narrative pacing, with faster sections for excitement and slower sections for contemplation

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Deep Space | `#0B0E17` | Primary dark background for hero and immersive sections |
| Midnight Navy | `#141B2D` | Secondary dark background for alternating sections |
| Charcoal Depth | `#1E2538` | Card and panel surface color on dark backgrounds |
| Slate Mist | `#2A3247` | Elevated surface, navbar backgrounds |
| Steel Gray | `#8892A8` | Secondary text, muted labels, and borders |
| Silver Fog | `#C5CDD9` | Body text on dark backgrounds |
| Cloud White | `#F0F2F5` | Primary text on dark backgrounds, light section base |
| Electric Blue | `#3B82F6` | Primary accent for CTAs, links, and active states |
| Cyan Glow | `#06B6D4` | Secondary accent for highlights and gradients |
| Warm Amber | `#F59E0B` | Tertiary accent for emphasis and warnings |
| Soft Violet | `#8B5CF6` | Gradient accent for decorative depth layers |
| Coral Pulse | `#EF4444` | Alert accent and hover state contrast |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --color-deep-space: #0B0E17;
  --color-midnight-navy: #141B2D;
  --color-charcoal-depth: #1E2538;
  --color-slate-mist: #2A3247;

  /* Text & Neutrals */
  --color-steel-gray: #8892A8;
  --color-silver-fog: #C5CDD9;
  --color-cloud-white: #F0F2F5;

  /* Accents */
  --color-electric-blue: #3B82F6;
  --color-cyan-glow: #06B6D4;
  --color-warm-amber: #F59E0B;
  --color-soft-violet: #8B5CF6;
  --color-coral-pulse: #EF4444;

  /* Functional Aliases */
  --bg-primary: var(--color-deep-space);
  --bg-secondary: var(--color-midnight-navy);
  --bg-surface: var(--color-charcoal-depth);
  --text-primary: var(--color-cloud-white);
  --text-secondary: var(--color-silver-fog);
  --text-muted: var(--color-steel-gray);
  --accent-primary: var(--color-electric-blue);
  --accent-secondary: var(--color-cyan-glow);
}
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| Inter | 400, 500, 600, 700 | Primary body text and UI elements | [fonts.google.com/specimen/Inter](https://fonts.google.com/specimen/Inter) |
| Space Grotesk | 500, 700 | Display headings and hero text | [fonts.google.com/specimen/Space+Grotesk](https://fonts.google.com/specimen/Space+Grotesk) |
| Sora | 400, 600, 700 | Alternative heading font with geometric clarity | [fonts.google.com/specimen/Sora](https://fonts.google.com/specimen/Sora) |
| JetBrains Mono | 400, 500 | Code snippets and technical labels | [fonts.google.com/specimen/JetBrains+Mono](https://fonts.google.com/specimen/JetBrains+Mono) |
| Playfair Display | 600, 700 | Elegant editorial headings for storytelling sections | [fonts.google.com/specimen/Playfair+Display](https://fonts.google.com/specimen/Playfair+Display) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Space Grotesk 700 | Inter 400 | Modern tech-forward, clean and authoritative |
| Playfair Display 700 | Inter 400 | Editorial elegance meets functional readability |
| Sora 700 | Inter 400 | Geometric precision with approachable warmth |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Inter:wght@400;500;600;700&display=swap');

body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--text-primary);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3, h4 {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  line-height: 1.15;
  letter-spacing: -0.02em;
}

h1 { font-size: clamp(2.5rem, 6vw, 5rem); }
h2 { font-size: clamp(1.8rem, 4vw, 3rem); }
h3 { font-size: clamp(1.25rem, 2.5vw, 1.75rem); }

p {
  font-size: clamp(1rem, 1.25vw, 1.125rem);
  max-width: 65ch;
  color: var(--text-secondary);
}

.label {
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--accent-primary);
}
```

## Layout Principles

- **Full-viewport sections**: Each parallax scene should fill the entire viewport (`min-height: 100vh`) to create immersive, self-contained visual stages that the user scrolls through one at a time
- **CSS perspective container**: The outermost scrolling container sets `perspective` on a parent element, allowing child layers translated along the Z-axis to move at naturally different scroll speeds without JavaScript
- **Layer stacking with translateZ**: Background layers use negative `translateZ` values (move them farther away so they scroll slower) and are scaled back up to compensate for the perspective size reduction
- **Sticky and fixed positioning**: Use `position: sticky` for elements that should pin in place during a scroll range, and `position: fixed` sparingly for persistent navigation overlays
- **Content containment**: Text and interactive elements should always be placed on the foreground layer (translateZ 0) to maintain crisp rendering, accessibility, and pointer-event reliability
- **Responsive breakpoints**: Reduce or disable parallax depth on screens below 768px to prevent disorienting motion on touch devices and improve mobile performance
- **Vertical rhythm grid**: Maintain consistent vertical spacing multiples (e.g., 4rem / 6rem / 8rem) between sections to create predictable scroll pacing across the entire page

## CSS / Design Techniques

### Parallax Layer

The foundation of CSS-only parallax: a perspective container with child layers at different Z-depths.

```css
.parallax-container {
  height: 100vh;
  overflow-x: hidden;
  overflow-y: auto;
  perspective: 8px;
  perspective-origin: 50% 50%;
}

.parallax-group {
  position: relative;
  height: 100vh;
  transform-style: preserve-3d;
}

.parallax-layer--back {
  position: absolute;
  inset: 0;
  transform: translateZ(-4px) scale(1.5);
  z-index: -1;
}

.parallax-layer--base {
  position: relative;
  transform: translateZ(0);
  z-index: 1;
}

.parallax-layer--deep {
  position: absolute;
  inset: 0;
  transform: translateZ(-8px) scale(2);
  z-index: -2;
}
```

### Scroll-Triggered Section

Sections that animate into view as the user scrolls, using Intersection Observer fallback classes and modern scroll-driven animations.

```css
.scroll-reveal {
  opacity: 0;
  transform: translateY(60px);
  transition: opacity 0.8s cubic-bezier(0.16, 1, 0.3, 1),
              transform 0.8s cubic-bezier(0.16, 1, 0.3, 1);
}

.scroll-reveal.is-visible {
  opacity: 1;
  transform: translateY(0);
}

.scroll-reveal--delay-1 { transition-delay: 0.1s; }
.scroll-reveal--delay-2 { transition-delay: 0.2s; }
.scroll-reveal--delay-3 { transition-delay: 0.3s; }

/* Modern: scroll-driven animation (Chrome 115+) */
@supports (animation-timeline: scroll()) {
  .scroll-reveal-native {
    animation: reveal-up linear both;
    animation-timeline: view();
    animation-range: entry 0% entry 40%;
  }
  @keyframes reveal-up {
    from { opacity: 0; transform: translateY(60px); }
    to   { opacity: 1; transform: translateY(0); }
  }
}
```

### Card

Dark, layered cards with subtle borders and hover lift effects that reinforce the depth theme.

```css
.parallax-card {
  background: var(--bg-surface);
  border: 1px solid rgba(255, 255, 255, 0.06);
  border-radius: 16px;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1),
              box-shadow 0.4s cubic-bezier(0.16, 1, 0.3, 1);
}

.parallax-card::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(59, 130, 246, 0.3), transparent);
}

.parallax-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4), 0 0 60px rgba(59, 130, 246, 0.08);
}
```

### Button

Buttons with gradient fills and a glow effect on hover, fitting the depth-forward aesthetic.

```css
.btn-parallax {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.875rem 2rem;
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: #fff;
  background: linear-gradient(135deg, var(--color-electric-blue), var(--color-cyan-glow));
  border: none;
  border-radius: 12px;
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.btn-parallax:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(59, 130, 246, 0.35), 0 0 60px rgba(6, 182, 212, 0.15);
}

.btn-parallax--outline {
  background: transparent;
  border: 2px solid var(--color-electric-blue);
  color: var(--color-electric-blue);
}

.btn-parallax--outline:hover {
  background: rgba(59, 130, 246, 0.1);
  box-shadow: 0 0 30px rgba(59, 130, 246, 0.15);
}
```

### Navigation

A fixed transparent navbar that gains a solid backdrop on scroll, staying unobtrusive over parallax content.

```css
.parallax-nav {
  position: fixed;
  top: 0; left: 0; right: 0;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
  background: transparent;
  transition: background 0.4s ease, backdrop-filter 0.4s ease;
}

.parallax-nav.is-scrolled {
  background: rgba(11, 14, 23, 0.85);
  backdrop-filter: blur(16px);
  -webkit-backdrop-filter: blur(16px);
  border-bottom: 1px solid rgba(255, 255, 255, 0.06);
}

.parallax-nav__link {
  color: var(--text-secondary);
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: 500;
  transition: color 0.3s ease;
  position: relative;
}

.parallax-nav__link::after {
  content: '';
  position: absolute;
  bottom: -4px; left: 0;
  width: 0; height: 2px;
  background: var(--accent-primary);
  transition: width 0.3s ease;
}

.parallax-nav__link:hover::after { width: 100%; }
```

### Hero Section

A full-viewport hero with layered background elements and centered content.

```css
.parallax-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  overflow: hidden;
  background: var(--bg-primary);
}

.parallax-hero__bg {
  position: absolute;
  inset: -20%;
  background:
    radial-gradient(ellipse at 30% 50%, rgba(59, 130, 246, 0.12) 0%, transparent 60%),
    radial-gradient(ellipse at 70% 50%, rgba(139, 92, 246, 0.1) 0%, transparent 60%);
  pointer-events: none;
}

.parallax-hero__title {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(3rem, 7vw, 5.5rem);
  font-weight: 700;
  line-height: 1.05;
  background: linear-gradient(135deg, var(--text-primary), var(--text-secondary));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.parallax-hero__scroll-indicator {
  position: absolute;
  bottom: 2rem; left: 50%;
  transform: translateX(-50%);
  color: var(--text-muted);
  font-size: 0.75rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  animation: float 2.5s ease-in-out infinite;
}

@keyframes float {
  0%, 100% { transform: translateX(-50%) translateY(0); }
  50% { transform: translateX(-50%) translateY(-10px); }
}
```

## Design Do's and Don'ts

### Do's

- **Do use GPU-accelerated transforms** (`translate3d`, `will-change: transform`) to keep parallax scrolling smooth at 60 frames per second
- **Do provide a static fallback** for browsers that lack 3D transform support and for users who prefer reduced motion (`prefers-reduced-motion: reduce`)
- **Do keep text on the foreground layer** (translateZ 0) so it stays crisp, accessible, and clickable without pointer-event interference
- **Do optimize background images** aggressively with modern formats (WebP, AVIF) and responsive `srcset` to prevent scroll jank from oversized assets
- **Do limit the number of parallax layers** to 2-3 per section; excessive layers introduce rendering overhead and visual noise that detracts from the content
- **Do maintain strong color contrast** between text and background layers to meet WCAG AA standards even as backgrounds shift during scrolling
- **Do test on real devices** across iOS, Android, and low-powered laptops, since parallax performance varies dramatically by hardware and browser

### Don'ts

- **Don't hijack the scroll** by overriding native scroll behavior with custom scroll speeds or snapping that disorients users and breaks accessibility expectations
- **Don't use `background-attachment: fixed`** as your only parallax method, since it is unsupported on iOS Safari and forces full-page repaints that destroy performance
- **Don't apply parallax to every section** of the page; strategic restraint is more impactful than constant motion, and overuse causes motion fatigue
- **Don't nest parallax containers** inside each other, as compounding perspective values create unpredictable layer behavior and severe rendering issues
- **Don't forget `overflow: hidden`** on parallax groups, or translated background layers will bleed outside their intended section boundaries
- **Don't rely solely on scroll position for critical content** since users on assistive technologies or keyboard navigation may not trigger scroll-based reveals
- **Don't ignore mobile entirely**; either implement a simplified parallax experience for touch devices or gracefully disable it below your responsive breakpoint

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| Glassmorphism | Shares the use of backdrop blur, layered depth, and translucent surfaces to create dimensional UI elements |
| Dark Mode Neon | Complements parallax with dark backgrounds and vibrant accent glows that enhance the cinematic, immersive mood |
| Minimalism | Parallax design benefits from minimalist content strategy, letting generous whitespace and restrained layouts amplify the depth effect |
| Aurora Gradient | Gradient-heavy backgrounds pair naturally with parallax layering, creating atmospheric color shifts as layers move |
| Cyberpunk | Shares the dark, high-contrast color palette and tech-forward visual language common in immersive parallax storytelling sites |
| Flat Design | Serves as a historical counterpoint; parallax design deliberately rejects flatness in favor of dimensional depth and spatial illusion |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Parallax Design Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --deep-space: #0B0E17; --midnight: #141B2D; --charcoal: #1E2538;
      --slate: #2A3247; --steel: #8892A8; --silver: #C5CDD9;
      --cloud: #F0F2F5; --blue: #3B82F6; --cyan: #06B6D4;
      --amber: #F59E0B; --violet: #8B5CF6;
    }
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      color: var(--cloud); background: var(--deep-space);
      line-height: 1.7; -webkit-font-smoothing: antialiased;
    }
    h1, h2, h3 { font-family: 'Space Grotesk', sans-serif; font-weight: 700; line-height: 1.15; letter-spacing: -0.02em; }
    a { color: var(--blue); text-decoration: none; }

    /* -- Nav -- */
    .nav {
      position: fixed; top: 0; left: 0; right: 0; z-index: 1000;
      display: flex; align-items: center; justify-content: space-between;
      padding: 1.25rem 2.5rem; background: transparent;
      transition: background 0.4s, backdrop-filter 0.4s;
    }
    .nav.scrolled {
      background: rgba(11,14,23,0.88); backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      border-bottom: 1px solid rgba(255,255,255,0.06);
    }
    .nav-logo { font-family: 'Space Grotesk', sans-serif; font-weight: 700; font-size: 1.3rem; color: var(--cloud); text-decoration: none; }
    .nav-logo span { color: var(--blue); }
    .nav-links { display: flex; gap: 2rem; list-style: none; }
    .nav-links a {
      color: var(--silver); font-size: 0.9rem; font-weight: 500;
      text-decoration: none; transition: color 0.3s; position: relative;
    }
    .nav-links a:hover { color: var(--cloud); }
    .nav-links a::after {
      content: ''; position: absolute; bottom: -4px; left: 0;
      width: 0; height: 2px; background: var(--blue); transition: width 0.3s;
    }
    .nav-links a:hover::after { width: 100%; }

    /* -- Buttons -- */
    .btn {
      display: inline-flex; align-items: center; padding: 0.875rem 2rem;
      font-family: 'Inter', sans-serif; font-weight: 600; font-size: 0.95rem;
      color: #fff; background: linear-gradient(135deg, var(--blue), var(--cyan));
      border: none; border-radius: 12px; cursor: pointer;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .btn:hover { transform: translateY(-2px); box-shadow: 0 8px 30px rgba(59,130,246,0.35); }
    .btn-outline {
      background: transparent; border: 2px solid var(--blue); color: var(--blue);
    }
    .btn-outline:hover { background: rgba(59,130,246,0.08); box-shadow: 0 0 30px rgba(59,130,246,0.15); }

    /* -- Hero -- */
    .hero {
      position: relative; min-height: 100vh; display: flex;
      align-items: center; justify-content: center; text-align: center; overflow: hidden;
    }
    .hero-bg {
      position: absolute; inset: -20%; pointer-events: none;
      background:
        radial-gradient(ellipse at 20% 50%, rgba(139,92,246,0.15), transparent 50%),
        radial-gradient(ellipse at 80% 50%, rgba(59,130,246,0.12), transparent 50%);
      animation: drift 20s ease-in-out infinite alternate;
    }
    .hero-bg-2 {
      position: absolute; inset: -20%; pointer-events: none;
      background:
        radial-gradient(ellipse at 60% 30%, rgba(6,182,212,0.1), transparent 40%),
        radial-gradient(ellipse at 40% 70%, rgba(245,158,11,0.06), transparent 40%);
      animation: drift 15s ease-in-out infinite alternate-reverse;
    }
    @keyframes drift {
      0% { transform: translate(0,0) scale(1); }
      100% { transform: translate(30px,-20px) scale(1.05); }
    }
    .hero-content { position: relative; z-index: 2; max-width: 800px; padding: 2rem; }
    .hero-label { font-weight: 600; font-size: 0.8rem; letter-spacing: 0.15em; text-transform: uppercase; color: var(--blue); margin-bottom: 1.5rem; }
    .hero h1 {
      font-size: clamp(2.8rem, 7vw, 5.5rem); margin-bottom: 1.5rem;
      background: linear-gradient(135deg, var(--cloud), var(--silver));
      -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
    }
    .hero p { font-size: clamp(1.05rem, 1.8vw, 1.25rem); color: var(--silver); max-width: 560px; margin: 0 auto 2.5rem; }
    .hero-actions { display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap; }
    .scroll-hint {
      position: absolute; bottom: 2.5rem; left: 50%; transform: translateX(-50%);
      color: var(--steel); font-size: 0.7rem; letter-spacing: 0.12em;
      text-transform: uppercase; animation: float 2.5s ease-in-out infinite;
    }
    @keyframes float {
      0%, 100% { transform: translateX(-50%) translateY(0); }
      50% { transform: translateX(-50%) translateY(-8px); }
    }
    .fade-bottom {
      position: absolute; bottom: 0; left: 0; right: 0; height: 180px;
      background: linear-gradient(to top, var(--midnight), transparent);
      pointer-events: none; z-index: 3;
    }
    .fade-top {
      position: absolute; top: 0; left: 0; right: 0; height: 180px;
      background: linear-gradient(to bottom, var(--deep-space), transparent);
      pointer-events: none; z-index: 3;
    }

    /* -- Sections -- */
    .section {
      position: relative; min-height: 100vh; display: flex;
      align-items: center; overflow: hidden;
    }
    .section-dark { background: var(--deep-space); }
    .section-navy { background: var(--midnight); }
    .section-inner { position: relative; z-index: 2; width: 100%; max-width: 1200px; margin: 0 auto; padding: 6rem 2rem; }
    .section-header { text-align: center; margin-bottom: 4rem; }
    .section-label { font-weight: 600; font-size: 0.8rem; letter-spacing: 0.15em; text-transform: uppercase; color: var(--cyan); margin-bottom: 1rem; display: block; }
    .section-header h2 { font-size: clamp(2rem, 4vw, 3rem); margin-bottom: 1rem; }
    .section-header p { font-size: 1.05rem; color: var(--silver); max-width: 600px; margin: 0 auto; }

    /* -- Cards -- */
    .card-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 2rem; }
    .card {
      background: var(--charcoal); border: 1px solid rgba(255,255,255,0.06);
      border-radius: 16px; padding: 2rem; position: relative; overflow: hidden;
      transition: transform 0.4s cubic-bezier(0.16,1,0.3,1), box-shadow 0.4s cubic-bezier(0.16,1,0.3,1);
    }
    .card::before {
      content: ''; position: absolute; top: 0; left: 0; right: 0; height: 1px;
      background: linear-gradient(90deg, transparent, rgba(59,130,246,0.3), transparent);
    }
    .card:hover { transform: translateY(-6px); box-shadow: 0 20px 40px rgba(0,0,0,0.3); }
    .card-icon {
      width: 48px; height: 48px; border-radius: 12px; display: flex;
      align-items: center; justify-content: center; font-size: 1.4rem;
      margin-bottom: 1.25rem; background: rgba(59,130,246,0.1); color: var(--blue);
    }
    .card-icon.cyan { background: rgba(6,182,212,0.1); color: var(--cyan); }
    .card-icon.violet { background: rgba(139,92,246,0.1); color: var(--violet); }
    .card-icon.amber { background: rgba(245,158,11,0.1); color: var(--amber); }
    .card h3 { font-family: 'Space Grotesk', sans-serif; font-size: 1.2rem; margin-bottom: 0.75rem; }
    .card p { font-size: 0.95rem; color: var(--silver); line-height: 1.7; }

    /* -- Stats -- */
    .stats { display: grid; grid-template-columns: repeat(4, 1fr); gap: 2rem; text-align: center; padding: 4rem 0; }
    .stat-num { font-family: 'Space Grotesk', sans-serif; font-size: clamp(2rem, 4vw, 3rem); font-weight: 700; color: var(--blue); }
    .stat-label { font-size: 0.85rem; color: var(--steel); text-transform: uppercase; letter-spacing: 0.08em; margin-top: 0.5rem; }

    /* -- Footer -- */
    .footer {
      background: var(--midnight); border-top: 1px solid rgba(255,255,255,0.06);
      padding: 3rem 2rem; text-align: center; color: var(--steel); font-size: 0.9rem;
    }

    /* -- Scroll Reveal -- */
    .reveal { opacity: 0; transform: translateY(40px); transition: opacity 0.7s cubic-bezier(0.16,1,0.3,1), transform 0.7s cubic-bezier(0.16,1,0.3,1); }
    .reveal.visible { opacity: 1; transform: translateY(0); }
    .reveal.d1 { transition-delay: 0.1s; }
    .reveal.d2 { transition-delay: 0.2s; }
    .reveal.d3 { transition-delay: 0.3s; }

    /* -- Reduced Motion -- */
    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after { animation-duration: 0.01ms !important; transition-duration: 0.01ms !important; }
      .reveal { opacity: 1; transform: none; }
    }

    /* -- Responsive -- */
    @media (max-width: 768px) {
      .nav-links { display: none; }
      .stats { grid-template-columns: repeat(2, 1fr); }
      .card-grid { grid-template-columns: 1fr; }
      .section-inner { padding: 4rem 1.5rem; }
    }
  </style>
</head>
<body>
  <!-- Navigation -->
  <nav class="nav" id="nav">
    <a href="#" class="nav-logo">Parallax<span>.</span></a>
    <ul class="nav-links">
      <li><a href="#features">Features</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#stats">Stats</a></li>
      <li><a href="#techniques">Techniques</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="hero-bg"></div>
    <div class="hero-bg-2"></div>
    <div class="hero-content">
      <p class="hero-label">Immersive Web Experiences</p>
      <h1>Design with Depth</h1>
      <p>Create layered, scroll-driven experiences that guide users through your story with cinematic motion and spatial depth.</p>
      <div class="hero-actions">
        <button class="btn">Get Started</button>
        <button class="btn btn-outline">Learn More</button>
      </div>
    </div>
    <div class="scroll-hint">Scroll &#8595;</div>
    <div class="fade-bottom"></div>
  </section>

  <!-- Features -->
  <section class="section section-navy" id="features">
    <div class="fade-top"></div>
    <div class="section-inner">
      <div class="section-header reveal">
        <span class="section-label">Features</span>
        <h2>Layered by Design</h2>
        <p>Every element exists at a purposeful depth, creating visual hierarchy through spatial relationships.</p>
      </div>
      <div class="card-grid">
        <div class="card reveal d1">
          <div class="card-icon">&#9670;</div>
          <h3>Depth Layering</h3>
          <p>Background, midground, and foreground elements move at independent scroll speeds, producing natural three-dimensional space.</p>
        </div>
        <div class="card reveal d2">
          <div class="card-icon cyan">&#9674;</div>
          <h3>Scroll Reveals</h3>
          <p>Content animates into view as users scroll, using eased transitions tied to viewport intersection for progressive disclosure.</p>
        </div>
        <div class="card reveal d3">
          <div class="card-icon violet">&#10023;</div>
          <h3>Cinematic Pacing</h3>
          <p>Full-viewport sections create a scene-by-scene rhythm, giving each content block room to breathe and make its impact.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- About -->
  <section class="section section-dark" id="about">
    <div class="section-inner">
      <div class="section-header reveal">
        <span class="section-label" style="color: var(--amber);">About the Technique</span>
        <h2>Motion with Meaning</h2>
        <p>Parallax design transforms the humble scroll into a storytelling device. By assigning different movement rates to layered elements, designers create depth that mirrors how we perceive the real world.</p>
      </div>
    </div>
  </section>

  <!-- Stats -->
  <section class="section section-navy" id="stats">
    <div class="section-inner">
      <div class="section-header reveal">
        <span class="section-label">By the Numbers</span>
        <h2>Performance Matters</h2>
      </div>
      <div class="stats reveal">
        <div><div class="stat-num">60</div><div class="stat-label">FPS Target</div></div>
        <div><div class="stat-num">3</div><div class="stat-label">Max Layers</div></div>
        <div><div class="stat-num">8px</div><div class="stat-label">Perspective</div></div>
        <div><div class="stat-num">0ms</div><div class="stat-label">JS Required</div></div>
      </div>
    </div>
  </section>

  <!-- Techniques -->
  <section class="section section-dark" id="techniques">
    <div class="section-inner">
      <div class="section-header reveal">
        <span class="section-label">Techniques</span>
        <h2>Build with Confidence</h2>
        <p>Core CSS techniques that power smooth, accessible parallax experiences without JavaScript dependencies.</p>
      </div>
      <div class="card-grid">
        <div class="card reveal d1">
          <div class="card-icon amber">&#9632;</div>
          <h3>CSS Perspective</h3>
          <p>Set perspective on the scroll container and translateZ on child layers. Elements farther away scroll slower -- pure CSS.</p>
        </div>
        <div class="card reveal d2">
          <div class="card-icon">&#9650;</div>
          <h3>GPU Acceleration</h3>
          <p>Use translate3d and will-change to promote layers to the GPU compositor, eliminating paint bottlenecks during scroll.</p>
        </div>
        <div class="card reveal d3">
          <div class="card-icon cyan">&#9679;</div>
          <h3>Scroll Timelines</h3>
          <p>The animation-timeline: scroll() API ties CSS animations directly to scroll progress for declarative parallax.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <p>Parallax Design Template &mdash; Built with CSS layers, depth, and purpose.</p>
  </footer>

  <script>
    // Scroll reveal via Intersection Observer
    const obs = new IntersectionObserver((entries) => {
      entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('visible'); });
    }, { threshold: 0.15, rootMargin: '0px 0px -60px 0px' });
    document.querySelectorAll('.reveal').forEach(el => obs.observe(el));

    // Nav background on scroll
    const nav = document.getElementById('nav');
    window.addEventListener('scroll', () => {
      nav.classList.toggle('scrolled', window.scrollY > 80);
    }, { passive: true });
  </script>
</body>
</html>
```

## Implementation Tips

- **Use `perspective` on the scroll container, not individual layers**: Setting `perspective: 8px` on the parent and `transform: translateZ(-Npx) scale(1 + N/perspective)` on children is the most reliable pure-CSS parallax pattern, avoiding the inconsistencies of `background-attachment: fixed`
- **Always pair `translateZ` with a compensating `scale`**: When you move a layer back with `translateZ(-4px)`, perspective makes it appear smaller; multiply its scale by `(perspective + offset) / perspective` (e.g., `scale(1.5)` for -4px at 8px perspective) to restore its intended visual size
- **Use `will-change: transform` sparingly and purposefully**: Apply it only to actively animating parallax layers to promote them to GPU compositing; overusing it on static elements wastes memory and can degrade performance
- **Wrap parallax disabling in a `prefers-reduced-motion` media query**: Users who experience motion sickness should receive a static version of the layout with all content visible and no scroll-triggered animations
- **Optimize images for parallax backgrounds**: Since background layers are often scaled up 1.5-2x to fill the viewport at depth, source images need higher resolution than their visible size; use `srcset` with 2x variants and serve WebP/AVIF formats
- **Test scroll performance with browser DevTools paint profiling**: Open the Performance panel, record a scroll interaction, and look for long paint or composite tasks that drop below 60fps; these indicate layers that are not properly GPU-accelerated
