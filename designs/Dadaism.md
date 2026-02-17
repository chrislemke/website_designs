# Dadaism

Dadaism (Dada) is a design aesthetic born from the radical anti-art movement that emerged in Zurich in 1916, spreading to Berlin, Paris, and New York. It represents **anti-art chaos: random collage, absurdist typography, cut-up text, and deliberate visual nonsense**. Dada deliberately rejects every principle of conventional design -- harmony, balance, hierarchy, and logic -- in favor of chance, contradiction, and anarchic humor. Applied to digital design, Dadaism produces compositions that are intentionally disruptive, playful, and confrontational, breaking every rule of visual communication to make the viewer question the nature of design itself.

---

## Visual Characteristics

### Core Design Traits

- **Collage and montage** -- Disparate fragments of text, photography, illustration, and found material are combined without logical relation
- **Cut-up typography** -- Letters and words clipped from different sources, mixed in varying sizes, fonts, weights, and orientations within a single word or sentence
- **Random placement** -- Elements are positioned by chance or whim rather than by grid, alignment, or compositional principle
- **Deliberate ugliness** -- Conventional beauty is rejected; awkward proportions, clashing elements, and visual discomfort are pursued
- **Overlapping and collision** -- Elements pile on top of each other without regard for legibility or spatial logic
- **Mixed media textures** -- Torn paper edges, rubber stamp marks, ticket stubs, newsprint, and handwritten scrawl coexist
- **Visual contradictions** -- Arrows point nowhere, labels describe the wrong thing, numbers count in wrong order
- **Anti-composition** -- No clear focal point, no visual hierarchy, no intended reading order; the viewer must navigate chaos

### Design Principles

- **Chance operations** -- Allow randomness, not intention, to determine placement, color, and arrangement
- **Anti-aesthetic** -- Deliberately violate principles of good design; if it looks wrong, it might be right
- **Humor and absurdity** -- Every composition should contain an element of the ridiculous, the contradictory, or the nonsensical
- **Subversion of meaning** -- Text and images are stripped of their original context and reassembled to create new, often meaningless, juxtapositions
- **Found material** -- Incorporate undesigned elements: default fonts, system UI, raw HTML, error messages, or unprocessed content
- **Ephemerality** -- Nothing is precious; the design should feel disposable, immediate, and unconcerned with permanence

---

## Color Palette

### Primary Palette

| Role | Hex | Description |
|------|-----|-------------|
| Newsprint White | `#F2EDE3` | Raw paper base, unbleached and cheap |
| Ink Black | `#1A1A1A` | Heavy text and stamp marks |
| Rubber-Stamp Red | `#CC3333` | Primary accent, bureaucratic urgency |
| Dirty Yellow | `#D4C55A` | Aged paper, caution tape, highlighter marks |
| Carbon Blue | `#2A4A7A` | Secondary accent, ink and carbon-copy tone |
| Cardboard Brown | `#8B7355` | Torn cardboard, found material surfaces |

### Accent Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Bruise Purple | `#5C3366` | Arbitrary accent, stamp ink |
| Safety Orange | `#E87020` | Warning, interruption, redirection |
| Mold Green | `#5A7A4A` | Decay, anti-beauty, organic chaos |
| Faded Pink | `#D4929A` | Remnant of destroyed elegance |
| Pencil Gray | `#999999` | Scribbled annotations, crossed-out text |
| Void Black | `#000000` | Redacted text blocks, heavy censorship |

### CSS Custom Properties

```css
:root {
  --dada-paper: #F2EDE3;
  --dada-ink: #1A1A1A;
  --dada-red: #CC3333;
  --dada-yellow: #D4C55A;
  --dada-blue: #2A4A7A;
  --dada-brown: #8B7355;
  --dada-purple: #5C3366;
  --dada-orange: #E87020;
  --dada-green: #5A7A4A;
  --dada-pink: #D4929A;
  --dada-gray: #999999;
  --dada-void: #000000;
}
```

---

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Special Elite** | 400 | Primary typewriter text; rough mechanical feel | [Special Elite](https://fonts.google.com/specimen/Special+Elite) |
| **Courier Prime** | 400, 700 | Body text; raw monospace typewriter | [Courier Prime](https://fonts.google.com/specimen/Courier+Prime) |
| **Libre Baskerville** | 400, 700 | Ironic formal serif fragments amid chaos | [Libre Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) |
| **Anton** | 400 | Loud, confrontational display headlines | [Anton](https://fonts.google.com/specimen/Anton) |
| **Permanent Marker** | 400 | Handwritten scrawl for annotations and graffiti | [Permanent Marker](https://fonts.google.com/specimen/Permanent+Marker) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Anton 400 + Permanent Marker 400 (mixed) | Special Elite 400 | Chaotic broadside, ransom note |
| Libre Baskerville 700 (rotated) | Courier Prime 400 | Formal text destroyed by random arrangement |
| Permanent Marker 400 | Courier Prime 400 | Scrawled manifesto, zine aesthetic |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Special+Elite&family=Courier+Prime:ital,wght@0,400;0,700;1,400&family=Anton&family=Permanent+Marker&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&display=swap');

body {
  font-family: 'Courier Prime', 'Courier New', monospace;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--dada-ink);
  -webkit-font-smoothing: auto; /* Deliberately rough */
}

h1, h2, h3 {
  font-family: 'Anton', sans-serif;
  font-weight: 400;
  text-transform: uppercase;
  line-height: 1.0;
  /* Each heading rotated a different amount */
}

h1 { transform: rotate(-3deg); }
h2 { transform: rotate(2deg); }
h3 { transform: rotate(-1deg); font-family: 'Permanent Marker', cursive; }
```

---

## Layout Principles

- **No grid** -- Elements are positioned with arbitrary coordinates; alignment is actively avoided
- **Overlapping and obstruction** -- Content deliberately overlaps and partially obscures other content; the viewer must work to read
- **Random rotation** -- Every element is rotated by a small random amount (1-8 degrees in either direction); nothing is perfectly level
- **Mixed scales** -- Combine extremely large and extremely small elements without conventional hierarchy; a footnote might be larger than a headline
- **Edge bleeding** -- Elements are clipped by the viewport edges, suggesting the chaos extends beyond the visible frame
- **Stacking disorder** -- Z-index values are arbitrary; important content may be partially hidden behind less important content
- **Responsive approach** -- On smaller screens, the chaos becomes denser rather than reorganizing into a clean mobile layout; elements stack more aggressively and rotations increase

---

## CSS / Design Techniques

### Collage Card

```css
.dada-card {
  background: var(--dada-paper);
  border: 2px solid var(--dada-ink);
  padding: 32px 28px;
  max-width: 500px;
  position: relative;
  transform: rotate(-2deg);
  box-shadow: 3px 3px 0 var(--dada-ink);
}

/* Torn paper edge effect */
.dada-card::before {
  content: '';
  position: absolute;
  top: -4px;
  left: 10%;
  right: 20%;
  height: 8px;
  background: var(--dada-paper);
  clip-path: polygon(
    0 100%, 5% 30%, 10% 80%, 15% 20%, 20% 90%, 25% 10%,
    30% 70%, 35% 40%, 40% 100%, 45% 30%, 50% 80%, 55% 20%,
    60% 90%, 65% 40%, 70% 70%, 75% 10%, 80% 60%, 85% 30%,
    90% 80%, 95% 50%, 100% 100%
  );
}
```

### Ransom-Note Text

```css
.dada-ransom {
  display: inline;
  line-height: 2.5;
}

.dada-ransom span {
  display: inline-block;
  padding: 2px 6px;
  margin: 2px;
  font-size: inherit;
}

.dada-ransom span:nth-child(odd) {
  font-family: 'Anton', sans-serif;
  background: var(--dada-red);
  color: var(--dada-paper);
  transform: rotate(-2deg);
}

.dada-ransom span:nth-child(even) {
  font-family: 'Libre Baskerville', serif;
  border: 1px solid var(--dada-ink);
  transform: rotate(1deg);
}

.dada-ransom span:nth-child(3n) {
  font-family: 'Permanent Marker', cursive;
  background: var(--dada-yellow);
  transform: rotate(3deg);
}
```

### Rubber Stamp Effect

```css
.dada-stamp {
  display: inline-block;
  font-family: 'Anton', sans-serif;
  font-size: 1.5rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--dada-red);
  border: 4px solid var(--dada-red);
  padding: 8px 20px;
  transform: rotate(-8deg);
  opacity: 0.85;
  position: relative;
}

.dada-stamp::after {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 3px,
    rgba(242, 237, 227, 0.4) 3px,
    rgba(242, 237, 227, 0.4) 5px
  );
  pointer-events: none;
}
```

### Dada Button (Anti-Button)

```css
.dada-button {
  background: var(--dada-ink);
  color: var(--dada-paper);
  border: 3px solid var(--dada-red);
  padding: 12px 28px;
  font-family: 'Special Elite', monospace;
  font-size: 1rem;
  cursor: pointer;
  transform: rotate(2deg);
  position: relative;
  transition: transform 0.15s ease;
}

.dada-button:hover {
  transform: rotate(-3deg) scale(1.05);
  background: var(--dada-red);
}

/* Deliberately misaligned label */
.dada-button::after {
  content: '\2190'; /* left arrow */
  position: absolute;
  top: -12px;
  right: -16px;
  font-size: 1.2rem;
  color: var(--dada-blue);
  transform: rotate(45deg);
}
```

### Dada Navigation (Anti-Navigation)

```css
.dada-nav {
  display: flex;
  flex-wrap: wrap;
  gap: 4px;
  padding: 16px;
  background: var(--dada-paper);
  border-bottom: 3px dashed var(--dada-ink);
}

.dada-nav a {
  font-family: 'Special Elite', monospace;
  font-size: 0.95rem;
  color: var(--dada-ink);
  text-decoration: line-through;
  padding: 6px 14px;
  border: 1px solid var(--dada-ink);
  transition: all 0.15s ease;
}

.dada-nav a:nth-child(1) { transform: rotate(-2deg); }
.dada-nav a:nth-child(2) { transform: rotate(3deg); background: var(--dada-yellow); }
.dada-nav a:nth-child(3) { transform: rotate(-1deg); }
.dada-nav a:nth-child(4) { transform: rotate(4deg); background: var(--dada-pink); }

.dada-nav a:hover {
  background: var(--dada-red);
  color: var(--dada-paper);
  text-decoration: none;
  transform: rotate(0deg);
}
```

### Hero Section (Anti-Hero)

```css
.dada-hero {
  min-height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 40px;
  background: var(--dada-paper);
  position: relative;
  overflow: hidden;
}

.dada-hero h1 {
  font-size: 5rem;
  transform: rotate(-5deg);
  position: relative;
}

.dada-hero h1::before {
  content: 'NO.';
  position: absolute;
  top: -20px;
  right: -30px;
  font-family: 'Permanent Marker', cursive;
  font-size: 1.5rem;
  color: var(--dada-red);
  transform: rotate(15deg);
}

/* Random scattered background fragments */
.dada-hero .fragment {
  position: absolute;
  font-family: 'Courier Prime', monospace;
  font-size: 0.75rem;
  color: var(--dada-gray);
  pointer-events: none;
}
```

### Redacted / Censored Text

```css
.dada-redacted {
  background: var(--dada-void);
  color: var(--dada-void);
  padding: 0 4px;
  user-select: none;
}

.dada-redacted:hover {
  color: var(--dada-red);
}
```

---

## Design Do's and Don'ts

### Do

- Rotate elements randomly; nothing should be perfectly horizontal or vertical
- Mix multiple typefaces within a single line or word for ransom-note effect
- Use torn edges, dashed borders, rubber-stamp textures, and collage overlaps
- Break conventional hierarchy; the least important text can be the largest
- Include deliberate contradictions: crossed-out text, mismatched labels, arrows pointing at nothing
- Embrace the ugly, the awkward, and the uncomfortable; beauty is not the goal
- Leave evidence of process: visible borders, construction marks, placeholder-like elements

### Don't

- Create clean, aligned, balanced compositions; order is the enemy
- Use a consistent, harmonious color palette; colors should clash and feel arbitrary
- Apply smooth gradients or polished effects; the finish should be raw and rough
- Respect conventional reading order; the viewer navigates the chaos at will
- Use a single typeface consistently; font diversity is essential to the collage feel
- Over-design or over-polish; Dadaism must feel spontaneous, not crafted
- Take the design too seriously; humor and absurdity are core to Dada

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Neubrutalism** | Digital descendant of Dada's raw, anti-aesthetic approach with bold typography and stark contrast |
| **DIY Punk** | Shares the cut-and-paste collage method, hand-made roughness, and anti-establishment attitude |
| **Corporate Grunge** | Applies deliberate ugliness and destruction to corporate design language; a Dada-influenced hybrid |
| **Cluttercore** | Shares the horror vacui and anti-minimalist density, though Cluttercore celebrates rather than subverts |
| **New Wave** | Post-punk graphic design that inherited Dada's deconstructed typography and rule-breaking |
| **Surrealism** | Direct historical successor; Surrealism retained Dada's absurdity but replaced nihilism with dream logic |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dadaism Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Special+Elite&family=Courier+Prime:wght@400;700&family=Anton&family=Permanent+Marker&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --dada-paper: #F2EDE3;
      --dada-ink: #1A1A1A;
      --dada-red: #CC3333;
      --dada-yellow: #D4C55A;
      --dada-blue: #2A4A7A;
      --dada-brown: #8B7355;
      --dada-gray: #999999;
    }

    body {
      font-family: 'Courier Prime', monospace;
      background: var(--dada-paper);
      color: var(--dada-ink);
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 40px 20px;
      position: relative;
      overflow: hidden;
    }

    /* Scattered background fragments */
    body::before {
      content: 'ART? ART? ART? ART?';
      position: absolute;
      top: 10%;
      left: 5%;
      font-family: 'Permanent Marker', cursive;
      font-size: 1.5rem;
      color: var(--dada-gray);
      opacity: 0.15;
      transform: rotate(12deg);
      pointer-events: none;
    }

    body::after {
      content: 'EVERYTHING IS NOTHING';
      position: absolute;
      bottom: 8%;
      right: 3%;
      font-family: 'Anton', sans-serif;
      font-size: 1rem;
      color: var(--dada-red);
      opacity: 0.12;
      transform: rotate(-8deg);
      letter-spacing: 0.2em;
      pointer-events: none;
    }

    .dada-card {
      background: var(--dada-paper);
      border: 2px solid var(--dada-ink);
      padding: 40px 32px;
      max-width: 480px;
      width: 100%;
      transform: rotate(-2deg);
      box-shadow: 4px 4px 0 var(--dada-ink);
      position: relative;
    }

    .dada-stamp {
      display: inline-block;
      font-family: 'Anton', sans-serif;
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--dada-red);
      border: 3px solid var(--dada-red);
      padding: 4px 12px;
      transform: rotate(-8deg);
      opacity: 0.8;
      margin-bottom: 20px;
    }

    .dada-card h1 {
      font-family: 'Anton', sans-serif;
      font-size: 2.75rem;
      text-transform: uppercase;
      line-height: 1.0;
      transform: rotate(1deg);
      margin-bottom: 16px;
    }

    .dada-card h1 .alt {
      font-family: 'Permanent Marker', cursive;
      font-size: 2rem;
      display: inline-block;
      background: var(--dada-yellow);
      padding: 2px 8px;
      transform: rotate(-4deg);
    }

    .dada-card p {
      font-size: 0.95rem;
      line-height: 1.7;
      transform: rotate(0.5deg);
    }

    .dada-card p .struck {
      text-decoration: line-through;
      color: var(--dada-gray);
    }

    .dada-card p .highlight {
      background: var(--dada-yellow);
      padding: 0 4px;
    }

    .dada-button {
      display: inline-block;
      margin-top: 24px;
      background: var(--dada-ink);
      color: var(--dada-paper);
      border: 3px solid var(--dada-red);
      padding: 10px 24px;
      font-family: 'Special Elite', monospace;
      font-size: 0.95rem;
      text-decoration: none;
      cursor: pointer;
      transform: rotate(2deg);
      transition: transform 0.15s ease;
    }

    .dada-button:hover {
      transform: rotate(-3deg) scale(1.05);
      background: var(--dada-red);
    }

    .annotation {
      position: absolute;
      top: -16px;
      right: 20px;
      font-family: 'Permanent Marker', cursive;
      font-size: 0.85rem;
      color: var(--dada-blue);
      transform: rotate(6deg);
    }
  </style>
</head>
<body>
  <div class="dada-card">
    <div class="annotation">&larr; is this art?</div>
    <div class="dada-stamp">Rejected</div>
    <h1>The Art of <span class="alt">Nothing</span></h1>
    <p>We declare that <span class="struck">beauty</span> meaning
       has been <span class="highlight">abolished</span> by committee vote.
       All that remains is the glorious nonsense of
       pure contradiction.</p>
    <a href="#" class="dada-button">Click Here (or Don't)</a>
  </div>
</body>
</html>
```
