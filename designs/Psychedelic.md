# Psychedelic

Psychedelic design channels the **1960s acid-trip visuals: swirling lettering, vibrating complementary colors, and kaleidoscopic patterns**. Rooted in the San Francisco counterculture poster art of Wes Wilson, Victor Moscoso, and Rick Griffin, Psychedelic design deliberately overwhelms the senses with optical intensity. It distorts letterforms into organic, flowing shapes, pairs clashing colors at maximum saturation to create optical vibration, and fills every surface with undulating, repeating patterns. In digital design, the aesthetic creates immersive, hypnotic experiences that demand attention and evoke altered states of perception.

---

## Visual Characteristics

### Core Design Traits

- **Swirling, distorted letterforms** -- Typography melts, flows, and warps into organic shapes that are barely legible but visually mesmerizing
- **Vibrating complementary colors** -- Red/green, orange/blue, and purple/yellow placed adjacently at full saturation to create an optical buzzing effect
- **Kaleidoscopic patterns** -- Mandala-like radial symmetry and tessellating organic shapes fill backgrounds and borders
- **Flowing organic lines** -- Art Nouveau-influenced sinuous curves that morph into hair, smoke, flames, or paisley
- **Dense pattern fills** -- Every surface ripples with texture: paisleys, dots, concentric rings, or flowing waves
- **Radial and circular compositions** -- Designs that spiral outward from a central point, pulling the eye inward
- **High saturation, low value contrast** -- Colors are loud and pure; the intent is optical overwhelm, not readability
- **Mushroom and nature motifs** -- Organic elements (flowers, mushrooms, eyes, suns) appear as recurring symbols

### Design Principles

- **Optical intensity over readability** -- The visual impact takes precedence over easy scanning; the viewer must work to decipher content
- **Horror vacui** -- Every inch of space is filled with pattern, color, or lettering; emptiness is antithetical to the style
- **Color as sensation** -- Colors are chosen for their physiological optical effect rather than conventional harmony
- **Organic over geometric** -- All forms curve, flow, and morph; straight lines and sharp angles are avoided
- **Immersive totality** -- The design should envelope the viewer as a total sensory experience
- **Handmade authenticity** -- Imperfection, irregularity, and the evidence of human craft are valued over digital precision

---

## Color Palette

### Primary Palette

| Role | Hex | Description |
|------|-----|-------------|
| Electric Magenta | `#FF00FF` | Primary vibrating accent |
| Acid Orange | `#FF6600` | Warm vibrating accent |
| Psychedelic Purple | `#8B00FF` | Deep spectral anchor |
| Lime Green | `#33FF00` | Vibrant complementary to magenta |
| Hot Pink | `#FF1493` | Secondary warm accent |
| Electric Blue | `#0066FF` | Cool vibrating complement to orange |

### Secondary Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Sunshine Yellow | `#FFD700` | Radiant accents, sun motifs |
| Turquoise | `#00CED1` | Cool-spectrum accents |
| Crimson | `#DC143C` | Deep warm focal points |
| Violet | `#7B2FBE` | Transition and gradient tones |
| Chartreuse | `#7FFF00` | High-energy green accent |
| Deep Indigo | `#1A0033` | Dark background base |

### CSS Custom Properties

```css
:root {
  --psych-magenta: #FF00FF;
  --psych-orange: #FF6600;
  --psych-purple: #8B00FF;
  --psych-lime: #33FF00;
  --psych-pink: #FF1493;
  --psych-blue: #0066FF;
  --psych-yellow: #FFD700;
  --psych-turquoise: #00CED1;
  --psych-crimson: #DC143C;
  --psych-violet: #7B2FBE;
  --psych-chartreuse: #7FFF00;
  --psych-indigo: #1A0033;
}
```

---

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Rubik Vinyl** | 400 | Display headings; groovy distorted letterforms | [Rubik Vinyl](https://fonts.google.com/specimen/Rubik+Vinyl) |
| **Rampart One** | 400 | Bold display titles; thick outlined psychedelic feel | [Rampart One](https://fonts.google.com/specimen/Rampart+One) |
| **Bungee Shade** | 400 | 3D shadow display type; poster-style headlines | [Bungee Shade](https://fonts.google.com/specimen/Bungee+Shade) |
| **Righteous** | 400 | Semi-display text; rounded 1960s-70s feel | [Righteous](https://fonts.google.com/specimen/Righteous) |
| **Quicksand** | 400, 500, 600, 700 | Body text; rounded sans-serif with organic warmth | [Quicksand](https://fonts.google.com/specimen/Quicksand) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Rubik Vinyl 400 | Quicksand 500 | Classic concert poster vibe |
| Bungee Shade 400 | Quicksand 400 | Bold, dimensional, groovy |
| Rampart One 400 | Righteous 400 | Maximalist psychedelic poster |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Rubik+Vinyl&family=Quicksand:wght@400;500;600;700&family=Righteous&display=swap');

body {
  font-family: 'Quicksand', 'Trebuchet MS', sans-serif;
  font-weight: 500;
  font-size: 1.0625rem;
  line-height: 1.7;
  color: #F0E6FF;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Rubik Vinyl', cursive;
  font-weight: 400;
  line-height: 1.1;
  letter-spacing: 0.02em;
}
```

---

## Layout Principles

- **Radial compositions** -- Organize content around central focal points that spiral outward; concentric rings of content mirror kaleidoscope structures
- **Dense, edge-to-edge fills** -- Backgrounds, borders, and margins are all filled with pattern and color; avoid sterile whitespace
- **Flowing, non-rigid grids** -- Content areas curve, overlap, and blend into each other rather than sitting in strict rectangular columns
- **Central vortex layouts** -- Pull the eye toward a central point using converging lines, concentric shapes, or radial gradients
- **Layered foreground elements** -- Text and imagery overlap and interweave; strict separation of elements is not required
- **Full-bleed color** -- Color extends to every edge of the viewport with no neutral borders or gutters
- **Responsive approach** -- On smaller screens, simplify pattern complexity but maintain saturated color fills and flowing type; never introduce whitespace gutters that break the immersive feel

---

## CSS / Design Techniques

### Psychedelic Gradient Background

```css
.psych-background {
  min-height: 100vh;
  background: linear-gradient(
    135deg,
    var(--psych-purple) 0%,
    var(--psych-magenta) 25%,
    var(--psych-orange) 50%,
    var(--psych-yellow) 75%,
    var(--psych-lime) 100%
  );
  background-size: 400% 400%;
  animation: psych-shift 8s ease infinite;
}

@keyframes psych-shift {
  0%, 100% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
}
```

### Vibrating Card

```css
.psych-card {
  background: var(--psych-indigo);
  border: 4px solid var(--psych-magenta);
  box-shadow:
    0 0 20px var(--psych-magenta),
    0 0 40px rgba(255, 0, 255, 0.3),
    inset 0 0 20px rgba(139, 0, 255, 0.2);
  border-radius: 24px;
  padding: 40px;
  position: relative;
  overflow: hidden;
}

.psych-card::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: conic-gradient(
    from 0deg,
    transparent,
    rgba(255, 0, 255, 0.1),
    transparent,
    rgba(51, 255, 0, 0.1),
    transparent
  );
  animation: psych-rotate 10s linear infinite;
}

@keyframes psych-rotate {
  to { transform: rotate(360deg); }
}
```

### Glowing Psychedelic Button

```css
.psych-button {
  background: linear-gradient(135deg, var(--psych-magenta), var(--psych-purple));
  color: #FFFFFF;
  border: 2px solid var(--psych-lime);
  padding: 16px 40px;
  font-family: 'Righteous', sans-serif;
  font-size: 1.1rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  border-radius: 50px;
  cursor: pointer;
  box-shadow: 0 0 15px rgba(255, 0, 255, 0.5);
  transition: all 0.3s ease;
}

.psych-button:hover {
  background: linear-gradient(135deg, var(--psych-lime), var(--psych-turquoise));
  color: var(--psych-indigo);
  border-color: var(--psych-magenta);
  box-shadow: 0 0 30px rgba(51, 255, 0, 0.6);
  transform: scale(1.05);
}
```

### Psychedelic Navigation

```css
.psych-nav {
  display: flex;
  justify-content: center;
  gap: 32px;
  padding: 20px 0;
  background: rgba(26, 0, 51, 0.8);
  border-bottom: 3px solid;
  border-image: linear-gradient(90deg, var(--psych-magenta), var(--psych-orange), var(--psych-yellow), var(--psych-lime), var(--psych-blue), var(--psych-purple)) 1;
}

.psych-nav a {
  font-family: 'Righteous', sans-serif;
  font-size: 1rem;
  color: var(--psych-yellow);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  transition: all 0.3s ease;
  text-shadow: 0 0 8px rgba(255, 215, 0, 0.5);
}

.psych-nav a:hover {
  color: var(--psych-magenta);
  text-shadow: 0 0 16px rgba(255, 0, 255, 0.7);
}
```

### Concentric Ring Pattern

```css
.psych-rings {
  position: relative;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  background: conic-gradient(
    var(--psych-magenta),
    var(--psych-orange),
    var(--psych-yellow),
    var(--psych-lime),
    var(--psych-blue),
    var(--psych-purple),
    var(--psych-magenta)
  );
  animation: psych-rotate 12s linear infinite;
}

.psych-rings::after {
  content: '';
  position: absolute;
  inset: 20px;
  border-radius: 50%;
  background: conic-gradient(
    var(--psych-purple),
    var(--psych-magenta),
    var(--psych-orange),
    var(--psych-yellow),
    var(--psych-lime),
    var(--psych-blue),
    var(--psych-purple)
  );
  animation: psych-rotate 8s linear infinite reverse;
}
```

### Hero Section

```css
.psych-hero {
  min-height: 80vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  background: radial-gradient(
    ellipse at center,
    var(--psych-violet) 0%,
    var(--psych-purple) 30%,
    var(--psych-indigo) 70%
  );
  padding: 60px 40px;
}

.psych-hero h1 {
  font-size: 5rem;
  background: linear-gradient(
    90deg,
    var(--psych-magenta),
    var(--psych-orange),
    var(--psych-yellow),
    var(--psych-lime),
    var(--psych-magenta)
  );
  background-size: 200% auto;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: psych-text-shift 4s linear infinite;
}

@keyframes psych-text-shift {
  to { background-position: 200% center; }
}
```

---

## Design Do's and Don'ts

### Do

- Use maximum-saturation complementary colors placed directly adjacent for optical vibration
- Fill every surface with pattern, gradient, or animated color
- Choose display typefaces with organic, flowing, or distorted letterforms
- Animate gradients and rotations slowly to create a hypnotic, shifting feel
- Use radial and conic gradients to create kaleidoscope and mandala effects
- Layer glowing box-shadows and text-shadows for neon luminosity
- Embrace near-illegibility in display type as part of the aesthetic

### Don't

- Use neutral grays, whites, or muted pastels; every color must be saturated and intense
- Leave empty whitespace; the background must always be active with color or pattern
- Use clean, geometric sans-serif fonts; letterforms should feel organic and handmade
- Apply minimalist layouts with generous margins; density and immersion are essential
- Use sharp corners or rigid grid structures; everything should flow and curve
- Prioritize readability over visual impact for display elements; body text can be readable but headlines should be experiential
- Apply subtle, restrained animations; if something moves, it should be bold and hypnotic

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Art Nouveau** | Primary visual ancestor; Psychedelic borrows its flowing organic lines and horror vacui directly |
| **Acid Design** | Modern digital descendant; applies psychedelic color theory to contemporary graphic design |
| **Vectordelia** | Digital vector interpretation of classic psychedelic poster art |
| **Neon Ooze** | Shares the saturated neon palette and glowing effects with a more liquid, dripping aesthetic |
| **Maximalism** | Both reject minimalism and fill every surface; Psychedelic adds optical vibration and counterculture context |
| **Gen Z Maximalism** | Contemporary revival of dense, colorful sensory overload that owes a debt to 1960s Psychedelia |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Psychedelic Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Rubik+Vinyl&family=Quicksand:wght@400;500;600;700&family=Righteous&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --psych-magenta: #FF00FF;
      --psych-orange: #FF6600;
      --psych-purple: #8B00FF;
      --psych-lime: #33FF00;
      --psych-yellow: #FFD700;
      --psych-indigo: #1A0033;
      --psych-violet: #7B2FBE;
    }

    body {
      font-family: 'Quicksand', sans-serif;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(
        135deg,
        var(--psych-purple) 0%,
        var(--psych-magenta) 25%,
        var(--psych-orange) 50%,
        var(--psych-yellow) 75%,
        var(--psych-lime) 100%
      );
      background-size: 400% 400%;
      animation: psych-shift 8s ease infinite;
      color: #F0E6FF;
    }

    @keyframes psych-shift {
      0%, 100% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
    }

    .psych-card {
      background: var(--psych-indigo);
      border: 4px solid var(--psych-magenta);
      box-shadow:
        0 0 20px var(--psych-magenta),
        0 0 40px rgba(255, 0, 255, 0.3);
      border-radius: 24px;
      padding: 48px 40px;
      max-width: 500px;
      width: 90%;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .psych-card::before {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: conic-gradient(
        from 0deg,
        transparent,
        rgba(255, 0, 255, 0.08),
        transparent,
        rgba(51, 255, 0, 0.08),
        transparent
      );
      animation: psych-rotate 10s linear infinite;
      z-index: 0;
    }

    @keyframes psych-rotate {
      to { transform: rotate(360deg); }
    }

    .psych-card > * { position: relative; z-index: 1; }

    .psych-card h1 {
      font-family: 'Rubik Vinyl', cursive;
      font-size: 3rem;
      line-height: 1.1;
      background: linear-gradient(
        90deg,
        var(--psych-magenta),
        var(--psych-orange),
        var(--psych-yellow),
        var(--psych-lime),
        var(--psych-magenta)
      );
      background-size: 200% auto;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: psych-text 4s linear infinite;
      margin-bottom: 20px;
    }

    @keyframes psych-text {
      to { background-position: 200% center; }
    }

    .psych-card p {
      font-size: 1.1rem;
      line-height: 1.7;
      font-weight: 500;
      color: rgba(240, 230, 255, 0.85);
    }

    .psych-button {
      display: inline-block;
      margin-top: 28px;
      background: linear-gradient(135deg, var(--psych-magenta), var(--psych-purple));
      color: #FFFFFF;
      border: 2px solid var(--psych-lime);
      padding: 14px 36px;
      font-family: 'Righteous', sans-serif;
      font-size: 1rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      border-radius: 50px;
      cursor: pointer;
      box-shadow: 0 0 15px rgba(255, 0, 255, 0.5);
      transition: all 0.3s ease;
    }

    .psych-button:hover {
      background: linear-gradient(135deg, var(--psych-lime), #00CED1);
      color: var(--psych-indigo);
      border-color: var(--psych-magenta);
      box-shadow: 0 0 30px rgba(51, 255, 0, 0.6);
    }
  </style>
</head>
<body>
  <div class="psych-card">
    <h1>Expand Your Mind</h1>
    <p>Colors vibrate at the edge of perception, patterns spiral
       inward toward infinity, and the boundaries of the ordinary dissolve
       into pure visual sensation.</p>
    <a href="#" class="psych-button">Turn On, Tune In</a>
  </div>
</body>
</html>
```
