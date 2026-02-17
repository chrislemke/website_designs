# Surrealism

Surrealism is a cultural and artistic movement that originated in the early 1920s, most famously associated with Salvador Dali, Rene Magritte, and Max Ernst. In design, Surrealism translates to **dreamlike impossible juxtapositions, melting forms, and subconscious imagery made tangible**. It favors the uncanny, the irrational, and the poetic collision of unrelated objects in hyper-real or barren landscapes. When applied to web and presentation design, Surrealism creates arresting, thought-provoking compositions that linger in memory by subverting visual expectations.

---

## Visual Characteristics

### Core Design Traits

- **Impossible juxtapositions** -- Unrelated objects placed together in dreamlike scenes that defy logic (a fish walking on land, a clock melting over a branch)
- **Hyper-real rendering** -- Photographic or painterly realism applied to impossible subjects, creating an uncanny valley of believability
- **Melting and morphing forms** -- Solid objects appear to soften, drip, warp, or transform into other objects
- **Vast empty landscapes** -- Sparse desert plains, infinite horizons, and deep perspective creating a sense of isolation and the subconscious
- **Floating and levitating objects** -- Elements defy gravity, hovering in space without visible support
- **Scale distortion** -- Ordinary objects rendered at absurd sizes or miniaturized to create disorientation
- **Shadow play** -- Long dramatic shadows that may not match their source objects, or shadows that take on independent forms
- **Eyes and body fragments** -- Disembodied eyes, hands, and lips appear as recurring motifs symbolizing perception and the subconscious

### Design Principles

- **Defamiliarization** -- Make the familiar strange by placing everyday objects in unexpected contexts
- **Dream logic** -- Compositions follow emotional rather than rational spatial relationships
- **Hyper-clarity amid absurdity** -- Crisp rendering and sharp focus on impossible content heightens the surreal effect
- **Negative space as narrative** -- Empty space suggests the vastness of the subconscious mind
- **Tension between order and chaos** -- Classical composition techniques frame irrational content
- **Symbolic layering** -- Every element carries potential symbolic or psychological meaning

---

## Color Palette

### Primary Palette

| Role | Hex | Description |
|------|-----|-------------|
| Desert Sand | `#C2A366` | Warm base tone evoking infinite landscapes |
| Twilight Blue | `#2C3E6B` | Deep evening sky, mystery and depth |
| Dali Amber | `#D4881C` | Warm golden accent, melting clocks and sunlit forms |
| Magritte Sky | `#87CEEB` | Clear impossible blue sky backdrop |
| Void Black | `#1A1A2E` | Deep shadow and negative space |
| Bone White | `#F5F0E8` | Bleached surfaces and bare canvases |

### Accent Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Blood Crimson | `#8B1A1A` | Dramatic accents, lips, organic forms |
| Absinthe Green | `#4A7C59` | Vegetation, uncanny nature elements |
| Phantom Violet | `#6B4C8A` | Dream states, transitions, ethereal elements |
| Flesh Pink | `#E8B4A2` | Human form references, warmth |
| Burnt Sienna | `#A0522D` | Earth, barren landscapes |
| Mercury Silver | `#C0C0C0` | Metallic reflections, mirrors |

### CSS Custom Properties

```css
:root {
  --surreal-sand: #C2A366;
  --surreal-twilight: #2C3E6B;
  --surreal-amber: #D4881C;
  --surreal-sky: #87CEEB;
  --surreal-void: #1A1A2E;
  --surreal-bone: #F5F0E8;
  --surreal-crimson: #8B1A1A;
  --surreal-green: #4A7C59;
  --surreal-violet: #6B4C8A;
  --surreal-flesh: #E8B4A2;
  --surreal-sienna: #A0522D;
  --surreal-silver: #C0C0C0;
}
```

---

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Playfair Display** | 400, 500, 700, 900 | Headings and display text; elegant serif with dramatic contrast | [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) |
| **Cormorant Garamond** | 300, 400, 500, 600 | Body text; refined old-style serif with classical authority | [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) |
| **EB Garamond** | 400, 500, 600, 700 | Alternative body text; scholarly, timeless | [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) |
| **Libre Baskerville** | 400, 700 | Captions and pull quotes; high readability serif | [Libre Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) |
| **Special Elite** | 400 | Accent text; typewriter feel for journal-like passages | [Special Elite](https://fonts.google.com/specimen/Special+Elite) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Playfair Display 700 | Cormorant Garamond 400 | Classic surrealist gallery catalog |
| Playfair Display 900 (italic) | EB Garamond 400 | Dramatic, literary, dreamlike |
| Special Elite 400 | Cormorant Garamond 300 | Automatic writing, subconscious journal |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,700&family=Cormorant+Garamond:wght@300;400;500;600&display=swap');

body {
  font-family: 'Cormorant Garamond', 'Georgia', serif;
  font-weight: 400;
  font-size: 1.125rem;
  line-height: 1.8;
  color: var(--surreal-void);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  letter-spacing: -0.01em;
  line-height: 1.2;
}
```

---

## Layout Principles

- **Vast negative space** -- Leave large areas of emptiness to evoke the infinite landscapes of surrealist paintings; do not fill every pixel
- **Asymmetric focal points** -- Place key elements off-center to create visual tension; use the rule of thirds as a starting point, then deliberately break it
- **Layered depth planes** -- Create distinct foreground, midground, and background layers; elements at different depths reinforce the dreamlike spatial distortion
- **Perspective distortion** -- Use exaggerated vanishing points and converging lines to pull the viewer into impossible spaces
- **Floating element placement** -- Position elements so they appear disconnected from any grid or surface, hovering in ambiguous space
- **Section breaks as horizon lines** -- Use thin horizontal dividers to suggest the endless flat landscapes common in surrealist painting
- **Responsive approach** -- On smaller screens, maintain generous vertical spacing and reduce floating element complexity; the sense of space is more important than density of content

---

## CSS / Design Techniques

### Floating Surreal Card

```css
.surreal-card {
  background: var(--surreal-bone);
  border: 1px solid var(--surreal-sand);
  padding: 48px;
  max-width: 560px;
  position: relative;
  box-shadow:
    20px 40px 60px rgba(26, 26, 46, 0.15),
    0 0 0 1px rgba(194, 163, 102, 0.2);
  transform: perspective(800px) rotateY(-2deg) rotateX(1deg);
  transition: transform 0.6s ease, box-shadow 0.6s ease;
}

.surreal-card:hover {
  transform: perspective(800px) rotateY(0deg) rotateX(0deg);
  box-shadow:
    10px 20px 40px rgba(26, 26, 46, 0.2),
    0 0 0 1px rgba(194, 163, 102, 0.3);
}
```

### Melting Element Effect

```css
.melting {
  position: relative;
  display: inline-block;
}

.melting::after {
  content: '';
  position: absolute;
  bottom: -20px;
  left: 10%;
  width: 80%;
  height: 30px;
  background: inherit;
  filter: blur(8px);
  opacity: 0.5;
  border-radius: 0 0 50% 50%;
  transform: scaleY(1.5);
}
```

### Dramatic Shadow

```css
.surreal-shadow {
  position: relative;
}

.surreal-shadow::after {
  content: '';
  position: absolute;
  bottom: -30px;
  left: 5%;
  width: 120%;
  height: 40px;
  background: radial-gradient(ellipse, rgba(26, 26, 46, 0.25) 0%, transparent 70%);
  transform: skewX(-15deg);
}
```

### Surreal Button

```css
.surreal-button {
  background: var(--surreal-twilight);
  color: var(--surreal-bone);
  border: 2px solid var(--surreal-amber);
  padding: 14px 36px;
  font-family: 'Playfair Display', serif;
  font-size: 1rem;
  font-weight: 500;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  position: relative;
  transition: all 0.4s ease;
}

.surreal-button:hover {
  background: var(--surreal-amber);
  color: var(--surreal-void);
  box-shadow: 8px 16px 32px rgba(26, 26, 46, 0.3);
  transform: translateY(-3px);
}
```

### Surreal Navigation

```css
.surreal-nav {
  display: flex;
  justify-content: center;
  gap: 48px;
  padding: 24px 0;
  border-bottom: 1px solid var(--surreal-sand);
}

.surreal-nav a {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.125rem;
  font-weight: 500;
  color: var(--surreal-twilight);
  text-decoration: none;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  position: relative;
  transition: color 0.3s ease;
}

.surreal-nav a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 50%;
  width: 0;
  height: 2px;
  background: var(--surreal-amber);
  transition: width 0.3s ease, left 0.3s ease;
}

.surreal-nav a:hover {
  color: var(--surreal-amber);
}

.surreal-nav a:hover::after {
  width: 100%;
  left: 0;
}
```

### Hero Section with Horizon

```css
.surreal-hero {
  min-height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
  padding: 80px 40px;
  background: linear-gradient(
    to bottom,
    var(--surreal-sky) 0%,
    var(--surreal-sky) 55%,
    var(--surreal-sand) 55.5%,
    var(--surreal-sand) 100%
  );
  position: relative;
}

.surreal-hero h1 {
  font-size: 4rem;
  color: var(--surreal-void);
  text-align: center;
  margin-bottom: 24px;
  text-shadow: 2px 4px 8px rgba(26, 26, 46, 0.1);
}
```

---

## Design Do's and Don'ts

### Do

- Use vast negative space to evoke the infinite subconscious landscape
- Juxtapose hyper-realistic imagery with impossible scenarios
- Employ dramatic, elongated shadows for theatrical depth
- Use classical serif typography to ground the irrational content in visual authority
- Create a sense of stillness and quiet tension in compositions
- Let single powerful images speak rather than cluttering with many elements
- Use subtle perspective distortion to unsettle the viewer

### Don't

- Fill every area with content; emptiness is essential to the surrealist mood
- Use cartoonish or playful rendering; surrealism requires convincing realism applied to impossible subjects
- Apply bright, saturated candy colors; favor muted earth tones, twilight blues, and aged warm tones
- Use rounded, bubbly UI elements; prefer sharp edges and classical geometry
- Add excessive animation; surrealism is about frozen impossible moments, not motion graphics
- Confuse surrealism with fantasy or psychedelic art; surrealism is rooted in the uncanny, not the spectacular
- Use generic stock photography; every image should feel deliberate and symbolically charged

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Art Deco** | Shares the 1920s-30s origin period; Art Deco celebrates rational geometry while Surrealism subverts it |
| **Art Nouveau** | Both draw on organic forms, but Art Nouveau celebrates natural beauty while Surrealism distorts it |
| **Whimsigothic** | Shares dreamlike and mysterious qualities with a darker, more fantastical approach |
| **Maximalism** | Surrealism can be maximalist in concept but typically uses sparse compositions |
| **Dark Aero** | Both create atmospheric depth through layering and dramatic lighting |
| **Ligne Claire** | Clean rendering style that can serve surreal content, as seen in Moebius comics |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Surrealism Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,700&family=Cormorant+Garamond:wght@300;400;500;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --surreal-sand: #C2A366;
      --surreal-twilight: #2C3E6B;
      --surreal-amber: #D4881C;
      --surreal-sky: #87CEEB;
      --surreal-void: #1A1A2E;
      --surreal-bone: #F5F0E8;
    }

    body {
      font-family: 'Cormorant Garamond', Georgia, serif;
      background: linear-gradient(
        to bottom,
        var(--surreal-sky) 0%,
        var(--surreal-sky) 50%,
        var(--surreal-sand) 50.5%,
        #D2B896 100%
      );
      color: var(--surreal-void);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }

    .surreal-card {
      background: var(--surreal-bone);
      border: 1px solid var(--surreal-sand);
      padding: 56px 48px;
      max-width: 520px;
      width: 90%;
      text-align: center;
      position: relative;
      box-shadow: 20px 40px 80px rgba(26, 26, 46, 0.15);
      transform: perspective(800px) rotateY(-1deg);
    }

    /* Dramatic elongated shadow beneath the card */
    .surreal-card::after {
      content: '';
      position: absolute;
      bottom: -40px;
      left: 5%;
      width: 120%;
      height: 50px;
      background: radial-gradient(ellipse, rgba(26, 26, 46, 0.18) 0%, transparent 70%);
      transform: skewX(-10deg);
      z-index: -1;
    }

    .surreal-card h1 {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      font-size: 2.5rem;
      line-height: 1.15;
      margin-bottom: 20px;
      color: var(--surreal-void);
    }

    .surreal-card p {
      font-size: 1.2rem;
      line-height: 1.8;
      color: #3A3A50;
      font-weight: 400;
    }

    .surreal-card .accent-line {
      width: 60px;
      height: 2px;
      background: var(--surreal-amber);
      margin: 24px auto;
    }

    .surreal-button {
      display: inline-block;
      margin-top: 24px;
      background: var(--surreal-twilight);
      color: var(--surreal-bone);
      border: 2px solid var(--surreal-amber);
      padding: 12px 32px;
      font-family: 'Playfair Display', serif;
      font-size: 0.95rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .surreal-button:hover {
      background: var(--surreal-amber);
      color: var(--surreal-void);
    }
  </style>
</head>
<body>
  <div class="surreal-card">
    <h1>The Persistence of Design</h1>
    <div class="accent-line"></div>
    <p>Objects hover in impossible stillness above an endless plain,
       their shadows stretching toward a horizon that never arrives.</p>
    <a href="#" class="surreal-button">Enter the Dream</a>
  </div>
</body>
</html>
```
