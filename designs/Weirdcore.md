# Weirdcore - Design Reference

## Overview

Weirdcore is an internet-born visual aesthetic rooted in the surreal distortion of early-2000s digital imagery, evoking feelings of confusion, disorientation, nostalgia, and existential dread. It weaponizes the low-fidelity artifacts of amateur photo editing, primitive computer graphics, JPEG compression, and forgotten web pages to construct environments that feel simultaneously familiar and deeply wrong. Recurring motifs include disembodied eyes, cryptic text fragments, warped perspectives, oversaturated or washed-out color shifts, and liminal spaces rendered through corrupted digital processes. Unlike its calmer sibling Dreamcore, Weirdcore is aggressively distorted, intentionally chaotic, and leans into the uncanny valley of digital memory -- producing visuals that look like corrupted screenshots from a reality that never quite existed.

## Visual Characteristics

### Core Design Traits

- **Low-fidelity image distortion**: Heavy JPEG compression artifacts, pixel stretching, resolution degradation, and visible image corruption that mimic early internet photo quality and broken file transfers
- **Eye and face motifs**: Disembodied eyeballs, floating faces, misplaced facial features, and watchful gazes superimposed on surreal backgrounds to evoke surveillance and paranoia
- **Cryptic text overlays**: Unsettling, fragmented phrases in basic system fonts (Arial, Times New Roman, Comic Sans) placed illogically across compositions -- messages that read like half-remembered warnings or corrupted error logs
- **Color channel splitting**: RGB separation, chromatic aberration, and deliberate color channel misalignment that fracture images into ghostly overlapping layers
- **Liminal space corruption**: Familiar environments (hallways, classrooms, parking lots, pools) rendered through distortion filters, unnatural color grading, and perspective warping
- **WordArt and early web typography**: Garish gradient text, embossed effects, rainbow fills, and stretched decorative type reminiscent of Microsoft WordArt and GeoCities pages
- **Analog-digital hybrid noise**: Layered VHS tracking lines, CRT scanlines, digital glitch blocks, and film grain simultaneously applied to create temporal confusion
- **Impossible geometry**: Recursive rooms, non-Euclidean perspectives, horizon lines that bend wrong, and spaces that violate spatial logic
- **Oversaturated neon bleeding**: Harsh neon greens, magentas, and cyans that bleed beyond their boundaries as if the display cannot contain them
- **Repeating and tiling patterns**: Unsettling repetition of objects, faces, or environmental elements arranged in grids or spirals that suggest broken rendering

### Design Principles

- Distort aggressively: comfort is the enemy; every element should feel slightly to severely wrong
- Layer multiple eras of digital artifacts simultaneously -- VHS, JPEG, pixel art, and modern glitch in one composition
- Use text as a disorienting weapon rather than a communication tool; meaning should be ambiguous or absent
- Embrace anti-design: break alignment, ignore hierarchy, reject usability conventions deliberately
- Make the viewer question whether the design is intentional or a system malfunction
- Treat nostalgia as something sinister rather than warm; familiar objects become threatening in the wrong context
- Prioritize emotional unease over visual polish; roughness and imperfection are the materials

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Corrupted White | `#E8E4D8` | Yellowed, aged background like a sun-damaged photograph |
| Static Grey | `#A3A3A3` | Neutral noise, interface chrome, muted surfaces |
| Void Black | `#0A0A0F` | Deep shadows, text, pupil of the eye motif |
| Neon Bleed Green | `#39FF14` | Toxic glow, matrix-style accents, terminal text |
| Glitch Magenta | `#FF00FF` | Channel splitting, chromatic aberration highlight |
| Warning Yellow | `#E8D44D` | Grainy filter tone, aged film, cautionary accents |
| Liminal Lavender | `#B8A9C9` | Washed-out surreal haze, dreamlike midtone |
| Scan Blue | `#00BFFF` | CRT glow, hyperlink nostalgia, digital water |
| Flesh Pink | `#D4A0A0` | Uncanny skin tones, organic unease |
| Error Red | `#CC2233` | System failure, alert states, blood pixel |
| Compression Tan | `#C8B890` | JPEG artifact tone, institutional wall color |
| VHS Purple | `#6B2D8B` | Tracking distortion, analog decay accent |

### CSS Custom Properties

```css
:root {
  --weird-corrupted: #E8E4D8;
  --weird-static: #A3A3A3;
  --weird-void: #0A0A0F;
  --weird-neon-green: #39FF14;
  --weird-glitch-magenta: #FF00FF;
  --weird-warning: #E8D44D;
  --weird-lavender: #B8A9C9;
  --weird-scan-blue: #00BFFF;
  --weird-flesh: #D4A0A0;
  --weird-error: #CC2233;
  --weird-compression: #C8B890;
  --weird-vhs: #6B2D8B;
}
```

## Typography

### Typeface Characteristics

Weirdcore typography deliberately abuses type. Fonts are selected for their associations with early computing, system defaults, and cheap web design. They are then distorted, misaligned, overlaid, and set at inappropriate sizes. The goal is text that feels like a message left behind in a corrupted file system -- legible enough to unsettle, broken enough to disorient. Comic Sans, Times New Roman, and Arial carry ironic weight here; pixel fonts and monospaced terminals evoke obsolete machines. WordArt-style gradients and embossing push type into the realm of garish early-web decoration.

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **VT323** | Pixel monospace | Terminal messages, error logs, system text, retro CRT displays |
| **Press Start 2P** | Pixel display | Headings with aggressive 8-bit energy, game-over screens |
| **Creepster** | Horror display | Unsettling headlines, dread-inducing labels (use sparingly) |
| **Comic Neue** | Casual handwritten | Ironic body text, naive-sinister captions (Comic Sans substitute) |
| **Special Elite** | Typewriter | Found-document text, institutional reports, degraded memos |
| **Rubik Glitch** | Glitch display | Headers with built-in distortion, corrupted titles |
| **Space Mono** | Technical monospace | Code-style body text, system interface labels |
| **Bungee Shade** | Dimensional display | WordArt-style decorative headers, retro 3D text effect |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Rubik Glitch 400 | VT323 400 | Corrupted system terminal, broken software |
| Press Start 2P 400 | Comic Neue 400 | Sinister game interface, ironic naivety |
| Creepster 400 | Special Elite 400 | Found horror document, unsettling report |
| Bungee Shade 400 | Space Mono 400 | Early web maximalism meets cold precision |
| VT323 400 | Comic Neue 300 | Old machine with childlike wrongness |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=VT323&family=Press+Start+2P&family=Creepster&family=Comic+Neue:wght@300;400;700&family=Special+Elite&family=Rubik+Glitch&family=Space+Mono:wght@400;700&family=Bungee+Shade&display=swap');

body {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--weird-void);
  -webkit-font-smoothing: none;
}

h1, h2 {
  font-family: 'Rubik Glitch', 'Impact', sans-serif;
  font-weight: 400;
  letter-spacing: 0.05em;
  color: var(--weird-neon-green);
  text-shadow:
    3px 0 var(--weird-glitch-magenta),
    -3px 0 var(--weird-scan-blue);
}

h3 {
  font-family: 'Press Start 2P', monospace;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--weird-error);
}

.system-text {
  font-family: 'VT323', monospace;
  font-size: 1.4rem;
  color: var(--weird-neon-green);
}

.found-text {
  font-family: 'Special Elite', 'Courier New', monospace;
  font-size: 0.95rem;
  color: var(--weird-static);
  transform: rotate(-0.5deg);
}

.wordart-text {
  font-family: 'Bungee Shade', cursive;
  font-size: 2.5rem;
  background: linear-gradient(180deg, var(--weird-warning), var(--weird-error), var(--weird-vhs));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
```

## Layout Principles

### Grid and Structure

- **Anti-grid chaos**: Deliberately break alignment; elements should overlap, rotate slightly, and ignore column structures
- **Layered z-index stacking**: Stack elements on top of each other with varying opacity and blend modes to create depth confusion
- **Random positioning**: Use absolute and fixed positioning to scatter elements unpredictably across the viewport
- **Broken symmetry**: Start with a recognizable layout pattern (centered hero, card grid) then corrupt it with offsets, skews, and misaligned margins
- **Mixed scale elements**: Combine extremely large elements with tiny ones in close proximity to break spatial logic

### Section Organization

- **Disorienting hero**: Full-viewport entry with distorted background, cryptic oversized text, and eye motifs
- **Corrupted content blocks**: Information presented in degraded card-like containers with visible glitch artifacts
- **System message interruptions**: Terminal-style text blocks that interrupt the flow with cryptic warnings or error messages
- **Tiling zones**: Sections where a single image or pattern repeats in an uncanny grid
- **Footer as void**: The page should feel like it dissolves into nothing or loops back on itself

### Responsive Approach

- On mobile, increase the sense of claustrophobia by letting elements overlap and crowd the viewport
- Allow horizontal overflow intentionally on some elements to break the expected containment of mobile layouts
- Scale glitch effects and text distortions proportionally; they should remain aggressive at every breakpoint
- Navigation can disappear entirely on small screens, forcing exploration and confusion
- Use viewport units aggressively to maintain the surreal sense of scale across devices

## CSS / Design Techniques

### Glitch Card

```css
.weird-card {
  background: var(--weird-corrupted);
  border: 2px solid var(--weird-static);
  padding: 32px;
  max-width: 480px;
  position: relative;
  overflow: hidden;
  transform: rotate(-0.3deg);
}

.weird-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 2px,
      rgba(57, 255, 20, 0.03) 2px,
      rgba(57, 255, 20, 0.03) 4px
    );
  pointer-events: none;
}

.weird-card::after {
  content: '';
  position: absolute;
  top: -2px;
  left: 10%;
  width: 80%;
  height: 4px;
  background: var(--weird-glitch-magenta);
  opacity: 0.6;
  animation: glitch-bar 3s infinite steps(1);
}

@keyframes glitch-bar {
  0%, 90% { top: -2px; opacity: 0; }
  91% { top: 20%; opacity: 0.6; }
  93% { top: 50%; opacity: 0.4; }
  95% { top: 80%; opacity: 0.7; }
  97% { top: 10%; opacity: 0.3; }
  100% { top: -2px; opacity: 0; }
}
```

### Corrupted Button

```css
.weird-button {
  background: var(--weird-void);
  color: var(--weird-neon-green);
  border: 1px solid var(--weird-neon-green);
  padding: 10px 24px;
  font-family: 'VT323', monospace;
  font-size: 1.1rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  cursor: pointer;
  position: relative;
  transition: none;
}

.weird-button:hover {
  background: var(--weird-neon-green);
  color: var(--weird-void);
  text-shadow:
    2px 0 var(--weird-glitch-magenta),
    -2px 0 var(--weird-scan-blue);
  animation: button-corrupt 0.15s infinite steps(1);
}

@keyframes button-corrupt {
  0% { transform: translate(0, 0); }
  25% { transform: translate(-2px, 1px); }
  50% { transform: translate(2px, -1px); }
  75% { transform: translate(-1px, -2px); }
  100% { transform: translate(1px, 2px); }
}
```

### Distortion Navigation

```css
.weird-nav {
  background: var(--weird-void);
  border-bottom: 2px solid var(--weird-neon-green);
  padding: 16px 32px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
}

.weird-nav::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--weird-glitch-magenta);
  clip-path: polygon(0 0, 15% 0, 15% 100%, 30% 100%, 30% 0, 60% 0, 60% 100%, 75% 100%, 75% 0, 100% 0, 100% 100%, 0 100%);
}

.weird-nav a {
  font-family: 'VT323', monospace;
  font-size: 1rem;
  color: var(--weird-neon-green);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.2em;
}

.weird-nav a:hover {
  color: var(--weird-glitch-magenta);
  text-shadow:
    1px 0 var(--weird-scan-blue),
    -1px 0 var(--weird-error);
}
```

### Corrupted Hero

```css
.weird-hero {
  background: var(--weird-void);
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.weird-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background:
    radial-gradient(ellipse at 30% 40%, rgba(107, 45, 139, 0.15) 0%, transparent 50%),
    radial-gradient(ellipse at 70% 60%, rgba(57, 255, 20, 0.08) 0%, transparent 50%),
    radial-gradient(ellipse at 50% 50%, rgba(255, 0, 255, 0.05) 0%, transparent 70%);
  pointer-events: none;
}

.weird-hero::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent 0px,
    transparent 2px,
    rgba(57, 255, 20, 0.015) 2px,
    rgba(57, 255, 20, 0.015) 4px
  );
  pointer-events: none;
}

.weird-hero h1 {
  font-family: 'Rubik Glitch', sans-serif;
  font-size: clamp(2rem, 8vw, 5rem);
  color: var(--weird-neon-green);
  text-shadow:
    4px 0 var(--weird-glitch-magenta),
    -4px 0 var(--weird-scan-blue),
    0 0 40px rgba(57, 255, 20, 0.3);
  position: relative;
  animation: hero-glitch 4s infinite steps(1);
}

@keyframes hero-glitch {
  0%, 85% { text-shadow: 4px 0 var(--weird-glitch-magenta), -4px 0 var(--weird-scan-blue), 0 0 40px rgba(57,255,20,0.3); transform: translate(0,0) skewX(0deg); }
  86% { text-shadow: -6px 0 var(--weird-error), 6px 0 var(--weird-scan-blue); transform: translate(3px,-1px) skewX(-2deg); }
  88% { text-shadow: 8px 2px var(--weird-glitch-magenta), -4px -2px var(--weird-neon-green); transform: translate(-2px,2px) skewX(1deg); }
  90% { text-shadow: 4px 0 var(--weird-glitch-magenta), -4px 0 var(--weird-scan-blue), 0 0 40px rgba(57,255,20,0.3); transform: translate(0,0) skewX(0deg); }
}

.weird-hero .subtitle {
  font-family: 'VT323', monospace;
  font-size: 1.2rem;
  color: var(--weird-static);
  margin-top: 24px;
  position: relative;
}
```

### Eye Motif Element

```css
.weird-eye {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  border: 3px solid var(--weird-neon-green);
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 0 30px rgba(57, 255, 20, 0.2);
  animation: eye-pulse 3s ease-in-out infinite;
}

.weird-eye::before {
  content: '';
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: var(--weird-neon-green);
}

.weird-eye::after {
  content: '';
  position: absolute;
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background: var(--weird-void);
}

@keyframes eye-pulse {
  0%, 100% { box-shadow: 0 0 30px rgba(57, 255, 20, 0.2); }
  50% { box-shadow: 0 0 60px rgba(57, 255, 20, 0.4), 0 0 100px rgba(255, 0, 255, 0.15); }
}
```

### System Warning Message

```css
.weird-system {
  font-family: 'VT323', monospace;
  font-size: 1.3rem;
  color: var(--weird-neon-green);
  background: rgba(10, 10, 15, 0.9);
  border-left: 3px solid var(--weird-error);
  padding: 16px 24px;
  margin: 32px 0;
  position: relative;
}

.weird-system::before {
  content: 'WARNING://';
  display: block;
  font-size: 0.9rem;
  color: var(--weird-error);
  margin-bottom: 8px;
  letter-spacing: 0.2em;
}

.weird-system::after {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 60%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255, 0, 255, 0.03));
  pointer-events: none;
}
```

### Scanline Overlay

```css
.weird-scanlines {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  pointer-events: none;
  z-index: 9999;
  background:
    repeating-linear-gradient(
      0deg,
      rgba(0, 0, 0, 0.03) 0px,
      rgba(0, 0, 0, 0.03) 1px,
      transparent 1px,
      transparent 3px
    );
  mix-blend-mode: multiply;
}

.weird-scanlines::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: radial-gradient(
    ellipse at center,
    transparent 50%,
    rgba(10, 10, 15, 0.15) 100%
  );
}
```

### Corrupted Image Container

```css
.weird-image {
  position: relative;
  overflow: hidden;
  filter: contrast(1.2) saturate(0.7) hue-rotate(10deg);
}

.weird-image::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background:
    linear-gradient(
      transparent 0%,
      rgba(255, 0, 255, 0.05) 30%,
      transparent 31%,
      transparent 60%,
      rgba(57, 255, 20, 0.05) 61%,
      transparent 62%
    );
  pointer-events: none;
  animation: image-corrupt 5s linear infinite;
}

@keyframes image-corrupt {
  0% { transform: translateY(-100%); }
  100% { transform: translateY(100%); }
}

.weird-image img {
  display: block;
  width: 100%;
  image-rendering: pixelated;
}
```

## Design Do's and Don'ts

### Do

- Layer multiple types of digital distortion (JPEG, VHS, pixel, glitch) simultaneously for temporal confusion
- Use cryptic, fragmented text that reads like corrupted error messages or half-remembered thoughts
- Include eye motifs and watchful imagery to create a sense of paranoid surveillance
- Embrace anti-design: break grids, ignore hierarchy, misalign elements, and reject conventional UX
- Start with familiar environments and corrupt them until they become uncanny and threatening
- Use neon green, magenta, and cyan as aggressive accent colors that bleed and glow unnaturally
- Apply chromatic aberration and RGB channel splitting to text and images for a broken-display feel
- Make the viewer uncertain whether the design is intentional or a genuine malfunction
- Reference early internet aesthetics (WordArt, GeoCities, Windows XP) through a sinister lens
- Use animation sparingly but with jarring, stepped timing functions rather than smooth easing

### Don't

- Create polished, clean, or visually comfortable layouts; Weirdcore must feel wrong
- Use warm, inviting color palettes or harmonious color relationships
- Apply smooth, predictable animations with gentle easing curves
- Build logical navigation systems that help the user feel oriented and safe
- Use professional, well-kerned typography with proper hierarchy; text should feel broken or misused
- Confuse Weirdcore with generic horror; it is surreal unease, not jump scares or gore
- Overdo effects to the point of complete illegibility; there should be enough clarity to draw the viewer in
- Use modern, trendy UI patterns (glassmorphism, neumorphism, bento grids) without corrupting them first
- Apply consistent branding rules; Weirdcore thrives on visual inconsistency
- Make the aesthetic feel ironic or humorous; the tone should be genuinely unsettling, not comedic

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Dreamcore** | Closest sibling; shares liminal spaces and surreal nostalgia but Dreamcore is subtler, quieter, and more passively unsettling where Weirdcore is aggressive and chaotic |
| **Vaporwave** | Both mine early internet and digital nostalgia; Vaporwave is ironic, consumer-culture-focused, and visually lush where Weirdcore is sinister and degraded |
| **Liminal Spaces** | Overlapping subject matter (empty hallways, pools, malls); Liminal Spaces is photographic documentation while Weirdcore actively distorts and corrupts these images |
| **Y2K Futurism** | Shares the late-90s/early-2000s digital source material; Y2K is optimistic, glossy, and forward-looking while Weirdcore treats the same era as a corrupted nightmare |
| **Glitchcore** | Near-synonym in some contexts; Glitchcore emphasizes the technical process of digital corruption while Weirdcore focuses on the emotional and psychological effect |
| **Backrooms** | Shares liminal space imagery and existential dread; Backrooms is more narrative and worldbuilding-focused while Weirdcore is purely visual and atmospheric |
| **Cyberpunk** | Both feature neon-on-dark palettes and digital dystopia; Cyberpunk is narrative and worldbuilt while Weirdcore is abstract and ambiguous |
| **Early Cyber** | Shares early internet visual DNA; Early Cyber celebrates the era with genuine enthusiasm while Weirdcore makes it feel haunted and corrupted |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>WEIRDCORE // LAYOUT_0x3F</title>
  <link href="https://fonts.googleapis.com/css2?family=VT323&family=Rubik+Glitch&family=Press+Start+2P&family=Comic+Neue:wght@300;400;700&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --weird-corrupted: #E8E4D8;
      --weird-static: #A3A3A3;
      --weird-void: #0A0A0F;
      --weird-neon-green: #39FF14;
      --weird-glitch-magenta: #FF00FF;
      --weird-warning: #E8D44D;
      --weird-lavender: #B8A9C9;
      --weird-scan-blue: #00BFFF;
      --weird-flesh: #D4A0A0;
      --weird-error: #CC2233;
      --weird-compression: #C8B890;
      --weird-vhs: #6B2D8B;
    }

    body {
      font-family: 'Comic Neue', 'Comic Sans MS', cursive;
      font-size: 1rem;
      line-height: 1.6;
      color: var(--weird-corrupted);
      background: var(--weird-void);
      min-height: 100vh;
      overflow-x: hidden;
      -webkit-font-smoothing: none;
    }

    /* Scanline overlay */
    body::after {
      content: '';
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      pointer-events: none;
      z-index: 9999;
      background:
        repeating-linear-gradient(
          0deg,
          rgba(57, 255, 20, 0.015) 0px,
          rgba(57, 255, 20, 0.015) 1px,
          transparent 1px,
          transparent 3px
        );
    }

    /* CRT vignette */
    body::before {
      content: '';
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      pointer-events: none;
      z-index: 9998;
      background: radial-gradient(ellipse at center, transparent 50%, rgba(10,10,15,0.4) 100%);
    }

    /* --- Navigation --- */
    .nav {
      background: var(--weird-void);
      border-bottom: 2px solid var(--weird-neon-green);
      padding: 14px 32px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: relative;
      z-index: 100;
    }

    .nav::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      right: 0;
      height: 2px;
      background: var(--weird-glitch-magenta);
      clip-path: polygon(0 0, 20% 0, 20% 100%, 35% 100%, 35% 0, 55% 0, 55% 100%, 70% 100%, 70% 0, 100% 0, 100% 100%, 0 100%);
    }

    .nav-logo {
      font-family: 'VT323', monospace;
      font-size: 1.2rem;
      color: var(--weird-neon-green);
      text-decoration: none;
      letter-spacing: 0.15em;
    }

    .nav-links a {
      font-family: 'VT323', monospace;
      font-size: 0.95rem;
      color: var(--weird-neon-green);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      margin-left: 28px;
    }

    .nav-links a:hover {
      color: var(--weird-glitch-magenta);
      text-shadow: 1px 0 var(--weird-scan-blue), -1px 0 var(--weird-error);
    }

    /* --- Hero --- */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background:
        radial-gradient(ellipse at 25% 35%, rgba(107,45,139,0.12) 0%, transparent 50%),
        radial-gradient(ellipse at 75% 65%, rgba(57,255,20,0.06) 0%, transparent 50%),
        radial-gradient(ellipse at 50% 50%, rgba(255,0,255,0.04) 0%, transparent 70%);
      pointer-events: none;
    }

    .hero-title {
      font-family: 'Rubik Glitch', sans-serif;
      font-size: clamp(2.5rem, 10vw, 6rem);
      font-weight: 400;
      color: var(--weird-neon-green);
      text-shadow:
        5px 0 var(--weird-glitch-magenta),
        -5px 0 var(--weird-scan-blue),
        0 0 60px rgba(57,255,20,0.25);
      position: relative;
      z-index: 10;
      animation: title-glitch 5s infinite steps(1);
    }

    @keyframes title-glitch {
      0%, 88% { text-shadow: 5px 0 var(--weird-glitch-magenta), -5px 0 var(--weird-scan-blue), 0 0 60px rgba(57,255,20,0.25); transform: translate(0,0) skewX(0deg); }
      89% { text-shadow: -8px 2px var(--weird-error), 6px -2px var(--weird-scan-blue); transform: translate(4px,-2px) skewX(-3deg); }
      91% { text-shadow: 10px 3px var(--weird-glitch-magenta), -5px -1px var(--weird-neon-green); transform: translate(-3px,3px) skewX(2deg); }
      93% { text-shadow: 5px 0 var(--weird-glitch-magenta), -5px 0 var(--weird-scan-blue), 0 0 60px rgba(57,255,20,0.25); transform: translate(0,0) skewX(0deg); }
    }

    .hero-sub {
      font-family: 'VT323', monospace;
      font-size: 1.3rem;
      color: var(--weird-static);
      margin-top: 28px;
      letter-spacing: 0.3em;
      position: relative;
      z-index: 10;
    }

    /* Floating Eye */
    .eye {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      border: 3px solid var(--weird-neon-green);
      position: absolute;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 0 30px rgba(57,255,20,0.15);
      animation: eye-float 6s ease-in-out infinite;
      z-index: 5;
    }

    .eye.eye-1 { top: 15%; left: 10%; animation-delay: 0s; }
    .eye.eye-2 { bottom: 20%; right: 8%; animation-delay: -2s; width: 70px; height: 70px; border-color: var(--weird-glitch-magenta); box-shadow: 0 0 30px rgba(255,0,255,0.15); }
    .eye.eye-3 { top: 60%; left: 75%; animation-delay: -4s; width: 50px; height: 50px; border-color: var(--weird-error); box-shadow: 0 0 20px rgba(204,34,51,0.15); }

    .eye::before {
      content: '';
      width: 40%;
      height: 40%;
      border-radius: 50%;
      background: currentColor;
    }

    .eye::after {
      content: '';
      position: absolute;
      width: 15%;
      height: 15%;
      border-radius: 50%;
      background: var(--weird-void);
    }

    .eye.eye-1 { color: var(--weird-neon-green); }
    .eye.eye-2 { color: var(--weird-glitch-magenta); }
    .eye.eye-3 { color: var(--weird-error); }

    @keyframes eye-float {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      33% { transform: translateY(-15px) rotate(3deg); }
      66% { transform: translateY(10px) rotate(-2deg); }
    }

    /* --- System Warning --- */
    .warning {
      font-family: 'VT323', monospace;
      font-size: 1.2rem;
      color: var(--weird-neon-green);
      background: rgba(10,10,15,0.85);
      border-left: 3px solid var(--weird-error);
      padding: 16px 24px;
      margin: 60px auto;
      max-width: 600px;
      position: relative;
    }

    .warning::before {
      content: 'WARNING://';
      display: block;
      font-size: 0.85rem;
      color: var(--weird-error);
      margin-bottom: 6px;
      letter-spacing: 0.2em;
    }

    /* --- Content Grid --- */
    .content {
      max-width: 800px;
      margin: 0 auto;
      padding: 60px 32px;
    }

    .section-label {
      font-family: 'Press Start 2P', monospace;
      font-size: 0.65rem;
      color: var(--weird-error);
      text-transform: uppercase;
      letter-spacing: 0.15em;
      margin-bottom: 32px;
    }

    .cards {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 24px;
    }

    .card {
      background: rgba(232,228,216,0.04);
      border: 1px solid rgba(163,163,163,0.2);
      padding: 28px;
      position: relative;
      overflow: hidden;
      transform: rotate(-0.3deg);
    }

    .card:nth-child(2) { transform: rotate(0.4deg); }
    .card:nth-child(3) { transform: rotate(0.2deg); }
    .card:nth-child(4) { transform: rotate(-0.5deg); }

    .card::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: repeating-linear-gradient(
        0deg, transparent, transparent 2px,
        rgba(57,255,20,0.02) 2px,
        rgba(57,255,20,0.02) 4px
      );
      pointer-events: none;
    }

    .card::after {
      content: '';
      position: absolute;
      top: -2px;
      left: 15%;
      width: 70%;
      height: 3px;
      background: var(--weird-glitch-magenta);
      opacity: 0;
      animation: card-glitch-bar 6s infinite steps(1);
    }

    .card:nth-child(2)::after { animation-delay: -1.5s; background: var(--weird-scan-blue); }
    .card:nth-child(3)::after { animation-delay: -3s; background: var(--weird-error); }
    .card:nth-child(4)::after { animation-delay: -4.5s; }

    @keyframes card-glitch-bar {
      0%, 92% { top: -2px; opacity: 0; }
      93% { top: 25%; opacity: 0.5; }
      95% { top: 60%; opacity: 0.3; }
      97% { top: 10%; opacity: 0.6; }
      100% { top: -2px; opacity: 0; }
    }

    .card h3 {
      font-family: 'Rubik Glitch', sans-serif;
      font-size: 1.1rem;
      font-weight: 400;
      color: var(--weird-neon-green);
      margin-bottom: 12px;
      text-shadow: 2px 0 var(--weird-glitch-magenta), -2px 0 var(--weird-scan-blue);
    }

    .card p {
      font-family: 'Comic Neue', cursive;
      font-size: 0.9rem;
      color: var(--weird-static);
      line-height: 1.5;
    }

    .card .tag {
      font-family: 'VT323', monospace;
      font-size: 0.85rem;
      color: var(--weird-warning);
      margin-top: 16px;
      display: inline-block;
    }

    /* --- Buttons --- */
    .button {
      display: inline-block;
      background: var(--weird-void);
      color: var(--weird-neon-green);
      border: 1px solid var(--weird-neon-green);
      padding: 10px 24px;
      font-family: 'VT323', monospace;
      font-size: 1.05rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      margin-top: 16px;
    }

    .button:hover {
      background: var(--weird-neon-green);
      color: var(--weird-void);
      text-shadow: 2px 0 var(--weird-glitch-magenta), -2px 0 var(--weird-scan-blue);
      animation: button-shake 0.15s infinite steps(1);
    }

    @keyframes button-shake {
      0% { transform: translate(0,0); }
      25% { transform: translate(-2px,1px); }
      50% { transform: translate(2px,-1px); }
      75% { transform: translate(-1px,-2px); }
      100% { transform: translate(1px,2px); }
    }

    /* --- Marquee Banner --- */
    .marquee-wrap {
      overflow: hidden;
      border-top: 1px solid rgba(57,255,20,0.2);
      border-bottom: 1px solid rgba(57,255,20,0.2);
      padding: 12px 0;
      margin: 60px 0;
    }

    .marquee {
      font-family: 'Press Start 2P', monospace;
      font-size: 0.55rem;
      color: var(--weird-error);
      letter-spacing: 0.3em;
      text-transform: uppercase;
      white-space: nowrap;
      animation: scroll-left 20s linear infinite;
    }

    @keyframes scroll-left {
      0% { transform: translateX(100%); }
      100% { transform: translateX(-100%); }
    }

    /* --- Footer --- */
    .footer {
      text-align: center;
      padding: 60px 32px;
      border-top: 1px solid rgba(163,163,163,0.1);
    }

    .footer p {
      font-family: 'VT323', monospace;
      font-size: 0.95rem;
      color: rgba(163,163,163,0.4);
      letter-spacing: 0.2em;
    }

    .footer .blink {
      animation: blink 1.5s steps(1) infinite;
      color: var(--weird-neon-green);
    }

    @keyframes blink {
      0%, 50% { opacity: 1; }
      51%, 100% { opacity: 0; }
    }

    /* --- Responsive --- */
    @media (max-width: 640px) {
      .cards { grid-template-columns: 1fr; }
      .nav { padding: 12px 16px; }
      .nav-links a { margin-left: 16px; font-size: 0.8rem; }
      .content { padding: 40px 16px; }
      .warning { margin: 40px 16px; }
      .eye.eye-2, .eye.eye-3 { display: none; }
    }
  </style>
</head>
<body>
  <nav class="nav">
    <a href="#" class="nav-logo">SYS://WEIRD_0x3F</a>
    <div class="nav-links">
      <a href="#">VOID</a>
      <a href="#">MEMORY</a>
      <a href="#">EXIT?</a>
    </div>
  </nav>

  <header class="hero">
    <div class="eye eye-1"></div>
    <div class="eye eye-2"></div>
    <div class="eye eye-3"></div>
    <h1 class="hero-title">WEIRDCORE</h1>
    <div class="hero-sub">do you remember this place . . . you were never here</div>
  </header>

  <div class="warning">you are not supposed to be reading this. the file was marked for deletion on a date that has not occurred yet.</div>

  <main class="content">
    <div class="section-label">// RECOVERED_FILES</div>
    <div class="cards">
      <div class="card">
        <h3>Room 404</h3>
        <p>The hallway extends further than the building allows. The lights flicker at a frequency your eyes cannot track. You have been here before.</p>
        <span class="tag">[LOCATION: UNKNOWN]</span>
        <br>
        <a href="#" class="button">ENTER</a>
      </div>
      <div class="card">
        <h3>The Signal</h3>
        <p>A television displays static in a room with no power outlets. The static forms patterns if you watch long enough. Do not watch long enough.</p>
        <span class="tag">[STATUS: ACTIVE]</span>
        <br>
        <a href="#" class="button">RECEIVE</a>
      </div>
      <div class="card">
        <h3>Memory_03.jpg</h3>
        <p>This photograph was taken on a camera that does not exist, in a location that was demolished in 1998. The timestamp reads tomorrow.</p>
        <span class="tag">[CORRUPTION: 78%]</span>
        <br>
        <a href="#" class="button">RECOVER</a>
      </div>
      <div class="card">
        <h3>The Pool</h3>
        <p>Still water. No reflections. The depth gauge reads a negative number. Someone left a towel on a chair that is bolted to the ceiling.</p>
        <span class="tag">[DEPTH: -12m]</span>
        <br>
        <a href="#" class="button">DESCEND</a>
      </div>
    </div>

    <div class="marquee-wrap">
      <div class="marquee">/// THIS CONTENT HAS BEEN FLAGGED FOR REVIEW /// FILE ORIGIN: UNRESOLVED /// TIMESTAMP: ERR_OVERFLOW /// DO NOT DISTRIBUTE /// THIS CONTENT HAS BEEN FLAGGED FOR REVIEW ///</div>
    </div>

    <div class="warning">process terminated unexpectedly. 3 files were modified by an unknown user at 03:33:33. no login records exist for this session.</div>
  </main>

  <footer class="footer">
    <p>LAST MODIFIED: NEVER <span class="blink">_</span></p>
    <p style="margin-top: 12px; font-size: 0.8rem;">connection_status: unstable // user_count: 1 (unverified)</p>
  </footer>
</body>
</html>
```
