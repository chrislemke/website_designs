# Dreamcore

## Overview

Dreamcore is a surrealist internet aesthetic defined by liminal spaces, uncanny emptiness, VHS distortion, and the eerie nostalgia of places that feel familiar yet deeply wrong. It draws from half-remembered dreams, abandoned architecture, and the glitchy imperfection of degraded analog media. In digital design, Dreamcore manifests as unsettling layouts with washed-out palettes, off-kilter typography, static noise overlays, and compositions that provoke a sense of disorientation and vague unease -- as if the viewer has wandered into a space that exists between waking and sleep.

## Visual Characteristics

### Core Design Traits

- **Liminal space imagery**: Empty corridors, deserted swimming pools, abandoned malls, featureless rooms, and infinite hallways that feel transitional and unresolved
- **VHS and analog distortion**: Scanlines, chromatic aberration, tracking errors, color bleeding, and static noise that degrade the image surface
- **Washed-out, low-saturation palette**: Faded yellows, sickly greens, desaturated blues, and off-whites that feel like overexposed film or aged monitors
- **Uncanny lighting**: Fluorescent flicker, inconsistent shadow directions, overly bright rooms with no visible light source, and sunset skies that feel too vivid
- **Dreamlike scale distortion**: Elements that are slightly too large or too small, rooms that feel impossibly deep, and proportions that defy logic
- **Text as ambient element**: Words and labels that appear as signage, watermarks, or system messages rather than traditional typographic hierarchy
- **Empty negative space**: Large expanses of nothingness that create unease through absence rather than presence

### Design Principles

- Create unease through subtlety, not shock: the most effective Dreamcore feels almost normal
- Use emptiness as a compositional tool; what is missing matters more than what is present
- Degrade the design surface with noise, blur, and analog artifacts to break digital perfection
- Avoid clear narrative or logical structure; content should feel fragmented and disjointed
- Let the viewer feel like an intruder in a space not meant for them
- Balance nostalgia with wrongness: familiar elements placed in unfamiliar contexts

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Void White | `#F0EDE4` | Primary background, empty liminal space |
| Fluorescent Yellow | `#E8E4A0` | Uncanny lighting, ambient wash |
| Static Grey | `#A8A8A0` | Noise texture, muted surfaces |
| Pool Blue | `#7BA7BC` | Desaturated water, sky tones |
| Liminal Green | `#8B9E72` | Sickly institutional surfaces |
| VHS Purple | `#7B6B8A` | Chromatic aberration accent |
| Faded Pink | `#C8A8A8` | Warm distortion, skin tones |
| Monitor Black | `#1A1A1E` | Deep shadows, text |
| Hallway Beige | `#CCC4B0` | Institutional walls, carpet tones |
| Error Red | `#A04040` | Warning, glitch accent |

### CSS Custom Properties

```css
:root {
  --dream-void: #F0EDE4;
  --dream-fluorescent: #E8E4A0;
  --dream-static: #A8A8A0;
  --dream-pool: #7BA7BC;
  --dream-liminal: #8B9E72;
  --dream-vhs: #7B6B8A;
  --dream-faded-pink: #C8A8A8;
  --dream-monitor: #1A1A1E;
  --dream-hallway: #CCC4B0;
  --dream-error: #A04040;
}
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Space Mono** | 400, 700 | Primary text; monospaced, system-terminal feel | [Space Mono](https://fonts.google.com/specimen/Space+Mono) |
| **Courier Prime** | 400, 700 | Body text; typewriter-quality mono with a worn texture | [Courier Prime](https://fonts.google.com/specimen/Courier+Prime) |
| **Inter** | 300, 400, 500 | System UI text, labels, interface elements | [Inter](https://fonts.google.com/specimen/Inter) |
| **Creepster** | 400 | Decorative accent for unsettling headers (use sparingly) | [Creepster](https://fonts.google.com/specimen/Creepster) |
| **VT323** | 400 | Pixel-style monospace for retro terminal and error messages | [VT323](https://fonts.google.com/specimen/VT323) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Space Mono 700 | Courier Prime 400 | Terminal log, institutional signage |
| VT323 400 | Inter 300 | Retro CRT meets modern liminal |
| Inter 500 | Space Mono 400 | Clean but off: corporate unreality |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Courier+Prime:wght@400;700&family=VT323&display=swap');

body {
  font-family: 'Space Mono', 'Courier New', monospace;
  font-size: 0.95rem;
  line-height: 1.7;
  color: var(--dream-monitor);
  -webkit-font-smoothing: auto;
}

h1, h2, h3 {
  font-family: 'Space Mono', monospace;
  font-weight: 700;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  color: var(--dream-static);
}

.system-text {
  font-family: 'VT323', monospace;
  font-size: 1.25rem;
  color: var(--dream-liminal);
}
```

## Layout Principles

- **Centered void**: Large areas of empty background surrounding sparse, isolated content elements create the signature liminal emptiness
- **Off-grid placement**: Elements positioned slightly off-center or at unexpected coordinates, breaking comfortable alignment expectations
- **Single-column isolation**: Content presented one element at a time with excessive vertical spacing, forcing the viewer to scroll through emptiness
- **No visible navigation**: Navigation elements are hidden, minimal, or disguised as ambient text; the viewer should feel lost
- **Oversized containers, undersized content**: Cards and sections that feel too big for their content, creating an unsettling sense of empty rooms
- **Responsive approach**: On mobile, the sense of emptiness intensifies with even more vertical space; avoid filling the viewport with content

## CSS / Design Techniques

### Liminal Card

```css
.dream-card {
  background: var(--dream-void);
  border: 1px solid var(--dream-static);
  padding: 48px;
  max-width: 500px;
  position: relative;
  box-shadow: 0 0 40px rgba(26, 26, 30, 0.04);
}

.dream-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 2px,
    rgba(168, 168, 160, 0.03) 2px,
    rgba(168, 168, 160, 0.03) 4px
  );
  pointer-events: none;
}
```

### VHS Distortion Overlay

```css
.dream-vhs-overlay {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  pointer-events: none;
  z-index: 1000;
  background: repeating-linear-gradient(
    0deg,
    rgba(0, 0, 0, 0.02) 0px,
    rgba(0, 0, 0, 0.02) 1px,
    transparent 1px,
    transparent 3px
  );
}

.dream-vhs-overlay::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: radial-gradient(
    ellipse at center,
    transparent 60%,
    rgba(26, 26, 30, 0.08) 100%
  );
}
```

### Glitch Button

```css
.dream-button {
  background: transparent;
  color: var(--dream-monitor);
  border: 1px solid var(--dream-static);
  padding: 12px 32px;
  font-family: 'Space Mono', monospace;
  font-size: 0.85rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  position: relative;
  transition: all 0.3s ease;
}

.dream-button:hover {
  background: var(--dream-fluorescent);
  border-color: var(--dream-monitor);
  color: var(--dream-monitor);
  text-shadow:
    2px 0 var(--dream-error),
    -2px 0 var(--dream-pool);
}
```

### Empty Hero Section

```css
.dream-hero {
  background: var(--dream-hallway);
  min-height: 80vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.dream-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background:
    linear-gradient(180deg, rgba(240,237,228,0.3) 0%, transparent 30%, transparent 70%, rgba(240,237,228,0.3) 100%);
  pointer-events: none;
}

.dream-hero h1 {
  font-family: 'Space Mono', monospace;
  font-size: 1.5rem;
  font-weight: 400;
  text-transform: uppercase;
  letter-spacing: 0.3em;
  color: var(--dream-static);
  position: relative;
}

.dream-hero .subtitle {
  font-family: 'VT323', monospace;
  font-size: 1rem;
  color: var(--dream-liminal);
  margin-top: 24px;
  position: relative;
}
```

### System Message

```css
.dream-system {
  font-family: 'VT323', monospace;
  font-size: 1.1rem;
  color: var(--dream-liminal);
  background: rgba(26, 26, 30, 0.03);
  border-left: 2px solid var(--dream-static);
  padding: 12px 20px;
  margin: 32px 0;
}

.dream-system::before {
  content: '> ';
  color: var(--dream-error);
}
```

### Fluorescent Navigation

```css
.dream-nav {
  background: var(--dream-void);
  border-bottom: 1px solid rgba(168, 168, 160, 0.3);
  padding: 24px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.dream-nav a {
  font-family: 'Space Mono', monospace;
  font-size: 0.75rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--dream-static);
  text-decoration: none;
  transition: color 0.3s ease;
}

.dream-nav a:hover {
  color: var(--dream-monitor);
  text-shadow:
    1px 0 var(--dream-error),
    -1px 0 var(--dream-pool);
}
```

## Design Do's and Don'ts

### Do

- Use excessive empty space to create unease and isolation
- Apply subtle analog distortions: scanlines, chromatic aberration, static noise
- Choose washed-out, desaturated colors that feel like faded film or old monitors
- Place text in unexpected positions as if it were ambient signage
- Create compositions where something feels slightly wrong but hard to identify
- Use monospaced and system fonts to evoke institutional or terminal environments
- Let the viewer feel disoriented and uncertain about where to look or click

### Don't

- Use bright, saturated colors or cheerful palettes that feel inviting
- Apply glossy effects, glass textures, or polished modern UI patterns
- Create logical, well-labeled navigation that makes the experience comfortable
- Fill the layout with dense content; emptiness is the primary material
- Use decorative script fonts or ornamental flourishes; the aesthetic is cold and plain
- Make things explicitly scary or horror-themed; Dreamcore is unsettling, not frightening
- Overdo the VHS/glitch effects to the point of unreadability; subtlety is key

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Weirdcore** | Close sibling; both use surreal, unsettling imagery but Weirdcore is more aggressively distorted and chaotic |
| **Vaporwave** | Shares VHS nostalgia and surreal digital spaces; Vaporwave is more colorful, ironic, and consumer-culture-focused |
| **Liminal Space** | Overlapping category; liminal spaces are the primary subject matter of Dreamcore photography |
| **Y2K** | Both reference late-90s/early-2000s digital aesthetics; Y2K is optimistic and glossy while Dreamcore is eerie and degraded |
| **Dark Academia** | Both mine nostalgia for old institutional spaces; Dark Academia is scholarly and warm while Dreamcore is cold and empty |
| **Brutalism (web)** | Shares raw, uncomfortable design choices and rejection of UX conventions; Brutalism is aggressive while Dreamcore is passively unsettling |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dreamcore Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=VT323&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Space Mono', 'Courier New', monospace;
      font-size: 0.95rem;
      line-height: 1.7;
      color: #1A1A1E;
      background: #F0EDE4;
      min-height: 100vh;
      position: relative;
    }

    /* Scanline overlay */
    body::after {
      content: '';
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      pointer-events: none;
      z-index: 1000;
      background: repeating-linear-gradient(
        0deg,
        rgba(0,0,0,0.015) 0px,
        rgba(0,0,0,0.015) 1px,
        transparent 1px,
        transparent 3px
      );
    }

    .nav {
      background: #F0EDE4;
      border-bottom: 1px solid rgba(168,168,160,0.3);
      padding: 24px 40px;
      display: flex;
      justify-content: space-between;
    }

    .nav a {
      font-size: 0.75rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: #A8A8A0;
      text-decoration: none;
    }

    .hero {
      background: #CCC4B0;
      min-height: 70vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      position: relative;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: linear-gradient(180deg,
        rgba(240,237,228,0.3) 0%, transparent 30%,
        transparent 70%, rgba(240,237,228,0.3) 100%);
    }

    .hero h1 {
      font-size: 1.4rem;
      font-weight: 400;
      text-transform: uppercase;
      letter-spacing: 0.3em;
      color: #A8A8A0;
      position: relative;
    }

    .hero .sub {
      font-family: 'VT323', monospace;
      font-size: 1rem;
      color: #8B9E72;
      margin-top: 24px;
      position: relative;
    }

    .content {
      max-width: 600px;
      margin: 100px auto;
      padding: 0 40px;
    }

    .card {
      background: #F0EDE4;
      border: 1px solid #A8A8A0;
      padding: 48px;
      margin-bottom: 60px;
      position: relative;
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: repeating-linear-gradient(
        0deg, transparent, transparent 2px,
        rgba(168,168,160,0.03) 2px,
        rgba(168,168,160,0.03) 4px
      );
      pointer-events: none;
    }

    .card h2 {
      font-size: 0.85rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: #A8A8A0;
      margin-bottom: 16px;
    }

    .card p {
      color: rgba(26,26,30,0.6);
      font-size: 0.9rem;
    }

    .system {
      font-family: 'VT323', monospace;
      font-size: 1.1rem;
      color: #8B9E72;
      border-left: 2px solid #A8A8A0;
      padding: 12px 20px;
      margin: 40px 0;
    }

    .system::before {
      content: '> ';
      color: #A04040;
    }

    .button {
      display: inline-block;
      margin-top: 20px;
      background: transparent;
      color: #1A1A1E;
      border: 1px solid #A8A8A0;
      padding: 10px 28px;
      font-family: 'Space Mono', monospace;
      font-size: 0.8rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <nav class="nav">
    <a href="#">room_0x00</a>
    <div>
      <a href="#">corridor</a>
      <a href="#" style="margin-left:24px;">exit</a>
    </div>
  </nav>
  <header class="hero">
    <h1>You are here</h1>
    <div class="sub">location unknown . . . do you remember this place?</div>
  </header>
  <main class="content">
    <div class="system">this room should not exist</div>
    <div class="card">
      <h2>Room 14</h2>
      <p>The fluorescent lights hum at a frequency you cannot name.
         The carpet smells like 1997. No one else is here.</p>
      <a href="#" class="button">enter</a>
    </div>
    <div class="card">
      <h2>The Pool</h2>
      <p>Still water reflects a ceiling that should not be this high.
         The clock on the wall reads a time that has not happened yet.</p>
      <a href="#" class="button">enter</a>
    </div>
  </main>
</body>
</html>
```
