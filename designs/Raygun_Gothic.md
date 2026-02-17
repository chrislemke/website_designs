# Raygun Gothic Design Reference

Raygun Gothic is a retrofuturistic aesthetic representing "a view of the future from the perspective of circa 1945 to 1970." It combines a brightly-colored art style drawn from comic books and pulp science fiction with imagery of heroism, discovery, and optimistic technological progress. The aesthetic ranges from a stylized, slightly sci-fi depiction of mid-century America to full futuristic settings with moon cities and intergalactic adventure. Shiny chrome, glowing neon, streamlined curves, rocket fins, and vibrant saturated colors define a world where the Space Age promise was fulfilled. Key values: **retrofuturism, optimism, adventure, atomic-era confidence, space exploration, pulp heroism**.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Rocket ships and fins** -- sleek, tapered rockets with stabilizer fins; aircraft-like tail fins on vehicles, buildings, and furniture
- **Chrome grilles and highlights** -- polished metal grille patterns, chrome bumper-like accents, reflective metallic trim
- **Starbursts** -- radiating spike patterns on clocks, signage, textiles, and decorative elements
- **Atom models** -- ball-and-stick atomic structures used as decorative motifs on graphics, textiles, and signage
- **Radar dishes and antennae** -- parabolic dish shapes and branching antenna structures as architectural and decorative elements
- **Robots and automatons** -- boxy or rounded humanoid robots with riveted panels, antenna ears, and glowing eyes
- **Ray guns and energy beams** -- stylized futuristic weapons emitting colorful laser/energy beams
- **Celestial bodies** -- planets with visible rings, crescent moons, spiral galaxies, and scattered stars
- **Stylized metal struts and support beams** -- exposed structural elements treated as decoration
- **Grates and grille patterns** -- geometric ventilation-like patterns used ornamentally
- **Hover vehicles** -- streamlined flying cars and saucers with smooth undersides and chrome accents
- **Neon tube forms** -- glowing tubular shapes outlining structures, signs, and decorative borders

### Design Principles

- **Streamlined aerodynamic curves** -- everything suggests speed and forward motion, even stationary objects
- **Optimistic futurism** -- designs project confidence that technology will deliver a bright, exciting future
- **Pulp drama and boldness** -- high-impact, eye-catching compositions inspired by magazine covers and movie posters
- **Chrome meets color** -- gleaming metallic surfaces paired with saturated, vibrant hues
- **Exaggerated scale** -- oversized fins, towering antennae, and dramatic rocket forms for visual impact
- **Symmetry with dynamic accents** -- broadly symmetrical compositions punctuated by angled fins and sweeping curves
- **Layered depth** -- foreground chrome elements over colorful nebula-like backgrounds, creating cinematic depth
- **Mid-century graphic style** -- clean lines, bold shapes, and limited-palette illustration techniques from 1950s commercial art

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Backgrounds** | Deep space navy, midnight black, dark teal |
| **Primary accents** | Chrome silver, polished steel |
| **Vibrant accents** | Rocket red, atomic turquoise, pulp orange, ray-gun green |
| **Glow effects** | Neon cyan, neon magenta, energy yellow |
| **Warm neutrals** | Retro cream, ivory white |

### Detailed Color Specifications

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Deep Space Navy | `#0B0E2D`, `#0D1137` | Primary dark backgrounds, deep space fields |
| Midnight Teal | `#0A2342`, `#0F3057` | Secondary dark backgrounds, panel bases |
| Chrome Silver | `#C0C0C0`, `#D6D6D6` | Metallic accents, chrome trim, borders |
| Polished Steel | `#8A9BA8`, `#7B8D9E` | Secondary metallics, structural elements |
| Rocket Red | `#E23D28`, `#D42B1E` | Call-to-action, rocket body accents, bold highlights |
| Atomic Turquoise | `#00CED1`, `#20B2AA` | Primary vibrant accent, neon glow, highlights |
| Pulp Orange | `#FF6B35`, `#E85D26` | Secondary warm accent, energy effects, hover states |
| Ray-Gun Green | `#39FF14`, `#32CD32` | Energy beams, laser effects, status indicators |
| Neon Cyan | `#00FFFF`, `#00E5FF` | Glow effects, neon outlines, interactive highlights |
| Neon Magenta | `#FF00FF`, `#E040FB` | Secondary glow, alien elements, decorative neon |
| Energy Yellow | `#FFD700`, `#FFC107` | Starburst elements, energy pulses, warm highlights |
| Retro Cream | `#FAF0DC`, `#F5EACB` | Light text on dark, retro paper feel |
| Cosmic Purple | `#4A0E78`, `#5B2C8E` | Nebula effects, deep accent, cosmic backgrounds |

### Suggested CSS Custom Properties

```css
:root {
  /* Deep backgrounds */
  --raygun-space: #0b0e2d;
  --raygun-navy: #0d1137;
  --raygun-teal-dark: #0a2342;
  --raygun-midnight: #0f3057;

  /* Metallics */
  --raygun-chrome: #c0c0c0;
  --raygun-chrome-light: #e0e0e0;
  --raygun-chrome-dark: #8a9ba8;
  --raygun-steel: #7b8d9e;

  /* Vibrant accents */
  --raygun-red: #e23d28;
  --raygun-turquoise: #00ced1;
  --raygun-orange: #ff6b35;
  --raygun-green: #39ff14;
  --raygun-yellow: #ffd700;
  --raygun-purple: #5b2c8e;

  /* Neon / glow */
  --raygun-neon-cyan: #00ffff;
  --raygun-neon-magenta: #ff00ff;
  --raygun-neon-green: #39ff14;

  /* Warm neutrals */
  --raygun-cream: #faf0dc;
  --raygun-ivory: #f5f5f0;

  /* Functional */
  --raygun-bg-primary: var(--raygun-space);
  --raygun-bg-secondary: var(--raygun-teal-dark);
  --raygun-bg-panel: var(--raygun-midnight);
  --raygun-text-primary: var(--raygun-cream);
  --raygun-text-heading: var(--raygun-neon-cyan);
  --raygun-accent: var(--raygun-turquoise);
  --raygun-accent-warm: var(--raygun-orange);
  --raygun-border: var(--raygun-chrome);
}
```

### Approaches

- **Deep space with neon accents** -- dark navy/black base with glowing cyan, magenta, and green neon outlines and accents
- **Chrome and color pop** -- silver metallic surfaces and borders paired with saturated red, orange, and turquoise
- **Pulp magazine palette** -- limited bold primaries (red, turquoise, yellow) against deep dark backgrounds, evoking vintage sci-fi cover art
- **Retro-optimist light theme** -- cream/ivory backgrounds with chrome accents and bright saturated spot colors (diner/Googie variant)
- **Cosmic gradient fields** -- deep purple-to-teal gradient backgrounds suggesting nebulae and deep space, with chrome foreground elements

---

## Typography

### Typeface Characteristics

Raygun Gothic typography blends mid-century commercial lettering with space-age futurism:

- **Bold, geometric sans-serifs** with a retro-futuristic character
- **Extended or wide letterforms** suggesting expansiveness and the vastness of space
- **Uppercase-dominant headlines** evoking rocket nosecone stencils and mission patches
- **Inline and dimensional effects** -- letters with internal lines, shadows, or bevels suggesting chrome engraving
- **Wide letter-spacing** for headlines, mimicking retro signage and pulp magazine mastheads
- **Rounded terminals** on body text for a friendly, optimistic mid-century feel
- **Occasional script or brush styles** for diner-influenced or nostalgic accents

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Orbitron** | Geometric, futuristic, space-age | Headlines, display text |
| **Audiowide** | Wide, technical, retro-futuristic | Headlines, titles |
| **Bungee** | Bold, playful, display | Feature headings, banners |
| **Bungee Shade** | Dimensional retro display | Large hero text, poster-style |
| **Monoton** | Retro outline display | Decorative neon-style titles |
| **Righteous** | Rounded retro, 1960s feel | Subheadings, labels |
| **Russo One** | Bold, wide, geometric | Section headings, navigation |
| **Jost** | Geometric sans, Futura-inspired | Body text, clean all-purpose |
| **Space Grotesk** | Modern geometric, technical | Body text, data displays |
| **Pacifico** | 1950s brush script | Decorative diner-style accents |
| **Bangers** | Comic book / pulp style | Callouts, exclamatory text |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Orbitron', 'Audiowide', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--raygun-neon-cyan);
  font-weight: 700;
}

/* Display / Hero text */
.raygun-display {
  font-family: 'Bungee Shade', 'Bungee', sans-serif;
  font-size: clamp(3rem, 8vw, 8rem);
  letter-spacing: 0.08em;
  line-height: 1.1;
  color: var(--raygun-neon-cyan);
  text-shadow:
    0 0 10px var(--raygun-neon-cyan),
    0 0 30px rgba(0, 255, 255, 0.4),
    3px 3px 0 var(--raygun-red);
}

/* Body text */
body {
  font-family: 'Jost', 'Space Grotesk', sans-serif;
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--raygun-cream);
}

/* Retro script accent */
.raygun-script {
  font-family: 'Pacifico', cursive;
  font-size: 1.4em;
  color: var(--raygun-orange);
  transform: rotate(-3deg);
}

/* Pulp / comic callout */
.raygun-pulp {
  font-family: 'Bangers', 'Bungee', sans-serif;
  font-size: 1.6em;
  color: var(--raygun-yellow);
  text-transform: uppercase;
  letter-spacing: 0.06em;
  text-shadow: 2px 2px 0 var(--raygun-red);
}
```

---

## Layout Principles

### Grid and Structure

- **Dramatic, cinematic compositions** -- large hero areas with deep-space backgrounds and chrome-framed content
- **Sweeping curves and arcs** -- section boundaries follow parabolic or fin-shaped curves rather than straight horizontal lines
- **Central vertical axis with flanking fins** -- content centered with decorative fin or antenna elements on the sides
- **Layered foreground/background** -- chrome UI elements float over starfield or gradient cosmic backgrounds
- **Generous vertical spacing** -- sections breathe with the vastness of space between them
- **Angled and tapered containers** -- panels narrow toward the top or bottom like rocket fuselages

### Section Organization

- Use **chrome-bordered panels** with rounded corners and metallic gradient edges as content containers
- Apply **neon-glow dividers** between sections -- thin lines with cyan or magenta glow effects
- Create **hierarchy through glow intensity** -- brighter neon glow = higher importance
- Employ **fin-shaped decorative elements** as section separators or side accents
- Feature **starburst or atom decorations** as visual punctuation between content blocks
- Place **radar-dish or antenna ornaments** in header/navigation areas
- Use **cosmic gradient backgrounds** that shift hue between sections (navy to teal to purple)

---

## CSS/Design Techniques

### Neon Glow Text Effect

```css
.raygun-neon {
  color: var(--raygun-neon-cyan);
  text-shadow:
    0 0 7px var(--raygun-neon-cyan),
    0 0 10px var(--raygun-neon-cyan),
    0 0 21px var(--raygun-neon-cyan),
    0 0 42px var(--raygun-turquoise),
    0 0 82px var(--raygun-turquoise);
}

/* Magenta neon variant */
.raygun-neon-magenta {
  color: var(--raygun-neon-magenta);
  text-shadow:
    0 0 7px var(--raygun-neon-magenta),
    0 0 10px var(--raygun-neon-magenta),
    0 0 21px var(--raygun-neon-magenta),
    0 0 42px #b000b0,
    0 0 82px #b000b0;
}
```

### Chrome Metallic Surface

```css
/* Polished chrome gradient (vertical reflection) */
.raygun-chrome-surface {
  background: linear-gradient(
    180deg,
    #e8e8e8 0%,
    #c0c0c0 20%,
    #808080 45%,
    #a0a0a0 55%,
    #d4d4d4 80%,
    #f0f0f0 100%
  );
}

/* Chrome text effect */
.raygun-chrome-text {
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #c0c0c0 35%,
    #707070 50%,
    #c0c0c0 65%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

### Starburst Decoration

```css
.raygun-starburst {
  position: relative;
  width: 200px;
  height: 200px;
}

.raygun-starburst::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-conic-gradient(
    var(--raygun-yellow) 0deg 4deg,
    transparent 4deg 12deg
  );
  border-radius: 50%;
  opacity: 0.15;
  animation: starburst-spin 25s linear infinite;
}

@keyframes starburst-spin {
  to { transform: rotate(360deg); }
}
```

### Rocket Fin Section Divider

```css
.raygun-fin-divider {
  height: 80px;
  position: relative;
  background: var(--raygun-bg-primary);
}

.raygun-fin-divider::before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 60px solid transparent;
  border-right: 60px solid transparent;
  border-bottom: 80px solid var(--raygun-chrome);
  opacity: 0.3;
}

/* Alternate: sweeping fin curve */
.raygun-sweep-divider {
  height: 60px;
  background: var(--raygun-bg-secondary);
  clip-path: polygon(0 100%, 0 60%, 40% 0, 60% 0, 100% 60%, 100% 100%);
  border-top: 2px solid var(--raygun-chrome);
}
```

### Neon Border / Glow Box

```css
.raygun-neon-box {
  border: 1px solid var(--raygun-neon-cyan);
  border-radius: 12px;
  box-shadow:
    0 0 8px rgba(0, 255, 255, 0.3),
    0 0 20px rgba(0, 255, 255, 0.1),
    inset 0 0 8px rgba(0, 255, 255, 0.05);
  padding: 2rem;
  background: rgba(10, 35, 66, 0.8);
}

/* Warm neon variant */
.raygun-neon-box-warm {
  border-color: var(--raygun-orange);
  box-shadow:
    0 0 8px rgba(255, 107, 53, 0.3),
    0 0 20px rgba(255, 107, 53, 0.1),
    inset 0 0 8px rgba(255, 107, 53, 0.05);
}
```

### Cosmic Gradient Background

```css
/* Deep space nebula background */
.raygun-cosmic-bg {
  background: linear-gradient(
    160deg,
    #0b0e2d 0%,
    #0a2342 30%,
    #1a0a3e 60%,
    #0f3057 100%
  );
}

/* Animated starfield overlay */
.raygun-starfield {
  background-image:
    radial-gradient(1px 1px at 10% 20%, rgba(255, 255, 255, 0.8), transparent),
    radial-gradient(1px 1px at 40% 60%, rgba(255, 255, 255, 0.6), transparent),
    radial-gradient(1.5px 1.5px at 70% 30%, rgba(255, 255, 255, 0.9), transparent),
    radial-gradient(1px 1px at 85% 75%, rgba(255, 255, 255, 0.5), transparent),
    radial-gradient(1px 1px at 25% 85%, rgba(255, 255, 255, 0.7), transparent),
    radial-gradient(1.5px 1.5px at 55% 10%, rgba(255, 255, 255, 0.6), transparent);
  background-size: 250px 250px;
}
```

### Chrome-Framed Card / Panel

```css
.raygun-card {
  background: linear-gradient(
    160deg,
    rgba(15, 48, 87, 0.9) 0%,
    rgba(10, 35, 66, 0.95) 100%
  );
  border: 1px solid var(--raygun-chrome-dark);
  border-radius: 12px;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 4px 20px rgba(0, 0, 0, 0.5),
    inset 0 1px 0 rgba(192, 192, 192, 0.1);
}

/* Chrome top edge highlight */
.raygun-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 5%;
  right: 5%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--raygun-chrome-light) 30%,
    var(--raygun-chrome-light) 70%,
    transparent
  );
}

/* Subtle starburst corner decoration */
.raygun-card::after {
  content: '';
  position: absolute;
  top: -40px;
  right: -40px;
  width: 100px;
  height: 100px;
  background: repeating-conic-gradient(
    var(--raygun-yellow) 0deg 3deg,
    transparent 3deg 15deg
  );
  border-radius: 50%;
  opacity: 0.06;
}
```

### Atom Orbit Decoration

```css
.raygun-atom {
  position: relative;
  width: 120px;
  height: 120px;
}

/* Nucleus */
.raygun-atom-nucleus {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 16px;
  height: 16px;
  background: var(--raygun-neon-cyan);
  border-radius: 50%;
  box-shadow: 0 0 10px var(--raygun-neon-cyan), 0 0 20px var(--raygun-neon-cyan);
}

/* Orbital rings */
.raygun-atom::before,
.raygun-atom::after {
  content: '';
  position: absolute;
  inset: 10%;
  border: 1.5px solid var(--raygun-turquoise);
  border-radius: 50%;
  opacity: 0.5;
}

.raygun-atom::before {
  transform: rotateX(65deg);
  animation: orbit-spin 4s linear infinite;
}

.raygun-atom::after {
  transform: rotateX(65deg) rotateZ(60deg);
  animation: orbit-spin 4s linear infinite reverse;
}

@keyframes orbit-spin {
  to { transform: rotateX(65deg) rotateZ(360deg); }
}
```

### Ray Gun Energy Beam Accent

```css
/* Horizontal energy beam divider */
.raygun-beam {
  height: 3px;
  margin: 2rem auto;
  width: 60%;
  background: linear-gradient(
    90deg,
    transparent,
    var(--raygun-neon-green) 15%,
    var(--raygun-neon-cyan) 50%,
    var(--raygun-neon-green) 85%,
    transparent
  );
  box-shadow:
    0 0 8px rgba(57, 255, 20, 0.4),
    0 0 20px rgba(0, 206, 209, 0.2);
  border-radius: 2px;
}
```

### Grille / Vent Pattern

```css
/* Horizontal chrome grille pattern */
.raygun-grille {
  background: repeating-linear-gradient(
    0deg,
    var(--raygun-chrome) 0px,
    var(--raygun-chrome) 2px,
    var(--raygun-teal-dark) 2px,
    var(--raygun-teal-dark) 8px
  );
  border-radius: 8px;
  padding: 1rem;
  border: 2px solid var(--raygun-chrome);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Raygun Gothic materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Polished chrome / steel | Multi-stop silver linear gradients with bright center highlights |
| Neon tube lighting | CSS `text-shadow` and `box-shadow` glow effects in cyan, magenta, green |
| Brushed aluminum | Directional gradient with fine repeating-linear-gradient texture overlay |
| Colored anodized metal | Tinted metallic gradients (turquoise-chrome, red-chrome) |
| Riveted metal panels | Subtle dot-pattern backgrounds with chrome borders |
| Bakelite / early plastics | Smooth, deep solid colors (dark teal, burgundy) with slight sheen gradient |
| Rocket fuselage skin | Smooth silver gradient with subtle rivet dot pattern overlay |
| Neon signage glass | Semi-transparent colored borders with outer glow effects |
| Starfield / deep space | Dark gradient backgrounds with scattered radial-gradient star dots |
| Ray gun energy beam | Bright gradient lines with saturated glow box-shadows |
| Pulp magazine paper | Warm cream/ivory backgrounds with slight texture noise |
| Comic book ink | High-contrast flat color blocks with bold dark outlines |

---

## Key Influences and References

| Reference | Contribution |
|-----------|-------------|
| **Flash Gordon** (1934) | Archetypal rocket ships, alien worlds, heroic pulp adventure visual language |
| **Buck Rogers** (1929) | Ray guns, space suits, chrome cityscapes, retro-futuristic technology |
| **The Jetsons** (1962) | Domestic retrofuturism, hover cars, automated homes, pastel space-age palette |
| **Forbidden Planet** (1956) | Chrome interiors, energy weapons, alien architecture, Robby the Robot |
| **Googie architecture** | Upswept roofs, boomerang shapes, starbursts, space-age commercial design |
| **1950s pulp sci-fi covers** | Saturated color palettes, dramatic compositions, chrome rockets, alien vistas |
| **Tomorrowland** (Disneyland, 1955) | Immersive retrofuturistic environments, monorails, space-themed architecture |
| **Meet the Robinsons** (2007) | Fully realized Raygun Gothic cityscapes, chrome bubble architecture |
| **My Life as a Teenage Robot** (2002) | Animated Raygun Gothic world with 1950s-meets-future visual design |

---

## Related Aesthetics

| Aesthetic | Relationship to Raygun Gothic |
|-----------|-------------------------------|
| **Art Deco** | Predecessor; shares geometric ornamentation and metallic glamour, which Raygun Gothic projects into space-age contexts |
| **Atompunk** | Sibling; Atompunk amplifies the nuclear anxiety side while Raygun Gothic emphasizes the optimistic adventure side |
| **Googie** | Architectural cousin; shares fins, starbursts, and boomerang shapes in commercial building design |
| **Streamline Moderne** | Direct ancestor; aerodynamic curves and chrome surfaces that Raygun Gothic launches into outer space |
| **Space Age** | Later evolution; focuses specifically on the 1960s space exploration era with sleeker, more minimal forms |
| **Retrofuturism** | Parent category; Raygun Gothic is one of the most recognizable retrofuturistic sub-styles |
| **Dieselpunk** | Period neighbor; shares early-mid 20th century machine aesthetics but with darker, grittier industrial tone |
| **Mid-Century Modern** | Contemporary; shares era and some forms but Mid-Century Modern is more restrained and domestic |
| **Cassette Futurism** | Successor; represents the next generation of retrofuturism (1970s-1980s) with analog tech instead of chrome rockets |
| **Diner** | Overlapping; shares chrome, neon, and bright colors in a terrestrial, food-service context |

---

## Quick-Start: Minimal Raygun Gothic Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Raygun Gothic Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Jost:wght@300;400;500&family=Bungee+Shade&family=Bangers&display=swap" rel="stylesheet">
  <style>
    :root {
      --raygun-space: #0b0e2d;
      --raygun-teal-dark: #0a2342;
      --raygun-midnight: #0f3057;
      --raygun-chrome: #c0c0c0;
      --raygun-chrome-light: #e0e0e0;
      --raygun-red: #e23d28;
      --raygun-turquoise: #00ced1;
      --raygun-orange: #ff6b35;
      --raygun-neon-cyan: #00ffff;
      --raygun-yellow: #ffd700;
      --raygun-cream: #faf0dc;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: linear-gradient(160deg, #0b0e2d 0%, #0a2342 50%, #0f3057 100%);
      color: var(--raygun-cream);
      font-family: 'Jost', sans-serif;
      font-weight: 400;
      letter-spacing: 0.02em;
      line-height: 1.7;
      min-height: 100vh;
    }

    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      color: var(--raygun-neon-cyan);
      text-shadow: 0 0 10px rgba(0, 255, 255, 0.4);
    }

    .hero {
      text-align: center;
      padding: 6rem 2rem;
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-family: 'Bungee Shade', sans-serif;
      font-size: clamp(3rem, 8vw, 7rem);
      letter-spacing: 0.08em;
      color: var(--raygun-neon-cyan);
      text-shadow:
        0 0 10px var(--raygun-neon-cyan),
        0 0 30px rgba(0, 255, 255, 0.3),
        3px 3px 0 var(--raygun-red);
    }

    /* Starburst background decoration */
    .hero::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 600px;
      height: 600px;
      background: repeating-conic-gradient(
        var(--raygun-yellow) 0deg 3deg,
        transparent 3deg 12deg
      );
      border-radius: 50%;
      opacity: 0.04;
      pointer-events: none;
    }

    .raygun-divider {
      width: 60%;
      margin: 2rem auto;
      border: none;
      height: 2px;
      background: linear-gradient(
        90deg,
        transparent,
        var(--raygun-neon-cyan) 20%,
        var(--raygun-neon-cyan) 80%,
        transparent
      );
      box-shadow: 0 0 8px rgba(0, 255, 255, 0.3);
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
    }

    .raygun-card {
      background: rgba(15, 48, 87, 0.8);
      border: 1px solid rgba(192, 192, 192, 0.3);
      border-radius: 12px;
      padding: 2rem;
      box-shadow:
        0 4px 20px rgba(0, 0, 0, 0.5),
        inset 0 1px 0 rgba(192, 192, 192, 0.1);
    }

    a {
      color: var(--raygun-neon-cyan);
      text-decoration: none;
      border-bottom: 1px dashed var(--raygun-turquoise);
    }

    a:hover {
      color: var(--raygun-orange);
      border-bottom-color: var(--raygun-orange);
      text-shadow: 0 0 8px var(--raygun-orange);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <hr class="raygun-divider">
    <p>A retrofuturistic subtitle in clean Jost</p>
  </div>
  <section>
    <div class="raygun-card">
      <h2>Section Heading</h2>
      <p>Content with Raygun Gothic styling applied.</p>
    </div>
  </section>
</body>
</html>
```
