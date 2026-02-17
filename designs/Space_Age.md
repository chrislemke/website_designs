# Space Age Design Reference

Space Age is a retrofuturistic design and cultural aesthetic that emerged in the mid-1950s through the early 1970s, driven by the Cold War Space Race and a widespread fascination with space exploration and technological advancement. The visual style conveys a sense of speed, technological progress, and a clean, optimistic future. It manifests across architecture (Googie), fashion (Courrèges, Cardin, Rabanne), furniture (pod chairs, fiberglass shells), and graphic design, unified by sleek geometric forms, glossy surfaces, and an unmistakable forward-looking confidence. Unlike the closely related Atomic Age (which emphasizes nuclear science motifs), Space Age focuses specifically on **spacecraft, orbital forms, and the material culture of space exploration**. Key values: **optimism, technological progress, utopianism, scientific advancement, exploration, future orientation, modernity, convenience**.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Rockets and fins** -- sleek tapered rocket forms with stabilizer fins; tail fins on vehicles and architectural elements inspired by jet aircraft and spacecraft
- **Satellites and orbits** -- Sputnik-like spheres with radiating antennae; elliptical orbital path lines as decorative motifs
- **Flying saucers and UFOs** -- disc and elliptical pod shapes appearing in architecture (Futuro House), furniture (Ball Chair), and lighting
- **Planets and stars** -- ringed planets, crescent moons, scattered star fields, and cosmic imagery
- **Astronaut silhouettes** -- helmeted space-suited figures as iconic graphic elements
- **Geodesic domes** -- triangulated spherical structures referencing Buckminster Fuller's futuristic architecture
- **Capsules and pods** -- enclosed, egg-shaped or spherical forms suggesting space capsules and cockpits
- **Parabolas and arcs** -- sweeping curved trajectories suggesting launch paths and orbital mechanics
- **Atomic symbols** -- stylized atom models used in a playful, approachable manner (inherited from Atomic Age but with a space-exploration spin)
- **Starbursts** -- radiating spike patterns on clocks, signage, and decorative elements
- **Streamlined silhouettes** -- aerodynamic, wind-tunnel-smooth contours on every surface

### Design Principles

- **Clean, optimistic futurism** -- every element projects confidence in a bright technological future
- **Geometric precision** -- circles, ellipses, parabolas, and smooth curves dominate over irregular or organic forms
- **Sleek minimalism** -- surfaces are smooth, uncluttered, and polished; ornamentation is structural, not applied
- **Speed and trajectory** -- compositions imply motion, launch, and forward momentum
- **Pod-like enclosure** -- self-contained, cocoon-like spaces and forms suggesting spacecraft interiors
- **New material celebration** -- visible use of plastic, fiberglass, chrome, and synthetic surfaces as deliberate aesthetic choices
- **Glossy reflectivity** -- surfaces catch and reflect light, suggesting advanced materials and precision engineering
- **Modular and prefabricated feel** -- repeating units, standardized components, and snap-together aesthetics

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Dominant neutrals** | White, silver, chrome -- the clean, bright base of the Space Age |
| **Primary accents** | Bright red, vivid blue, signal orange -- bold, saturated, optimistic |
| **Secondary accents** | Yellow, turquoise, bright green -- energetic pops of color |
| **Metallics** | Chrome silver, polished aluminum, reflective steel |
| **Dark grounds** | Deep space black, midnight navy -- for cosmic/starfield contexts |

### Detailed Color Specifications

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Space White | `#F7F7F7`, `#FAFAFA` | Primary background, clean surfaces, dominant base color |
| Chrome Silver | `#C0C0C0`, `#D4D4D4` | Metallic accents, borders, structural elements, dividers |
| Polished Aluminum | `#E8E8E8`, `#EBEBEB` | Light metallic surfaces, secondary panels |
| Rocket Red | `#E53935`, `#D32F2F` | Primary accent, call-to-action, bold highlights |
| Orbital Blue | `#1E88E5`, `#1976D2` | Primary cool accent, links, interactive elements |
| Signal Orange | `#FF8F00`, `#F57C00` | Warm accent, energy, optimism, hover states |
| Satellite Yellow | `#FFD600`, `#FFC107` | Highlight, starburst elements, attention-drawing |
| Capsule Turquoise | `#00BCD4`, `#0097A7` | Secondary cool accent, retro-futuristic flair |
| Launchpad Green | `#43A047`, `#2E7D32` | Status indicators, secondary accent |
| Deep Space Black | `#0A0A1A`, `#0D0D24` | Dark backgrounds, cosmic starfield base |
| Midnight Navy | `#0D1B3E`, `#0F2044` | Dark panel backgrounds, deep space gradients |
| Astronaut Gray | `#78909C`, `#607D8B` | Muted text, secondary elements, space suit tone |
| Retro Cream | `#FFF8E7`, `#FFFDE7` | Warm light background variant, vintage paper feel |

### Suggested CSS Custom Properties

```css
:root {
  /* Clean neutrals */
  --space-white: #f7f7f7;
  --space-cream: #fff8e7;
  --space-silver: #c0c0c0;
  --space-silver-light: #e8e8e8;
  --space-silver-dark: #9e9e9e;
  --space-gray: #78909c;

  /* Bold accents */
  --space-red: #e53935;
  --space-blue: #1e88e5;
  --space-orange: #ff8f00;
  --space-yellow: #ffd600;
  --space-turquoise: #00bcd4;
  --space-green: #43a047;

  /* Dark grounds */
  --space-black: #0a0a1a;
  --space-navy: #0d1b3e;
  --space-dark: #0f2044;

  /* Functional */
  --space-bg-primary: var(--space-white);
  --space-bg-dark: var(--space-black);
  --space-bg-panel: var(--space-silver-light);
  --space-text-primary: #1a1a2e;
  --space-text-light: var(--space-white);
  --space-text-muted: var(--space-gray);
  --space-accent: var(--space-blue);
  --space-accent-warm: var(--space-red);
  --space-border: var(--space-silver);
}
```

### Approaches

- **Clean white with chrome and color pops** -- bright white/silver base with bold red, blue, and orange accents (the signature Space Age look; think TWA Terminal interior)
- **Deep space cosmic** -- dark navy/black backgrounds with chrome elements and neon-bright accent colors against starfield
- **Warm retro-futurism** -- cream/off-white backgrounds with chrome borders and saturated primary accents (vintage poster feel)
- **Monochrome chrome** -- predominantly silver/white/gray palette with a single vivid accent color for maximum futuristic impact
- **Pod interior** -- enclosed feeling with curved white panels, soft ambient lighting effects, and turquoise/blue accents

---

## Typography

### Typeface Characteristics

Space Age typography is geometric, clean, and forward-looking:

- **Geometric sans-serifs** with precise, engineered letterforms suggesting technical precision
- **Wide, extended proportions** -- letterforms stretched horizontally to evoke expansiveness and the vastness of space
- **Uniform stroke weights** -- monoline or near-monoline construction for a clean, machine-made feel
- **Uppercase-dominant headlines** evoking mission control displays, spacecraft labeling, and technical stencils
- **Wide letter-spacing** for headlines, referencing aerospace signage and retro-futuristic movie titles
- **Rounded terminals** on body text for an approachable, optimistic quality
- **No ornament or flourish** -- letterforms are purely functional, befitting the modernist futurism of the era

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Orbitron** | Geometric, futuristic, space-age | Headlines, display text, hero titles |
| **Audiowide** | Wide, technical, retro-futuristic | Headlines, navigation labels |
| **Russo One** | Bold, wide, geometric | Section headings, strong emphasis |
| **Rajdhani** | Geometric, technical, semi-condensed | Subheadings, data labels, UI elements |
| **Exo 2** | Modern geometric, clean | Versatile: headings and body |
| **Jost** | Geometric sans, Futura-inspired | Body text, all-purpose |
| **Space Grotesk** | Modern geometric, technical | Body text, code, data displays |
| **Michroma** | Wide, technical, minimal | Display text, labels |
| **Electrolize** | Digital, technical, monospace feel | Captions, technical labels |
| **Saira** | Extended geometric family | Flexible across weights for entire layouts |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Orbitron', 'Audiowide', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.10em;
  color: var(--space-text-primary);
  font-weight: 700;
}

/* Display / Hero text */
.space-display {
  font-family: 'Orbitron', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  letter-spacing: 0.15em;
  line-height: 1.1;
  font-weight: 900;
  color: var(--space-text-primary);
}

/* Body text */
body {
  font-family: 'Jost', 'Space Grotesk', sans-serif;
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--space-text-primary);
}

/* Technical / label text */
.space-label {
  font-family: 'Rajdhani', 'Electrolize', sans-serif;
  font-size: 0.8em;
  text-transform: uppercase;
  letter-spacing: 0.20em;
  color: var(--space-gray);
  font-weight: 600;
}

/* Accent numeral / data display */
.space-data {
  font-family: 'Space Grotesk', monospace;
  font-size: 2em;
  font-weight: 700;
  color: var(--space-accent);
  letter-spacing: 0.05em;
}
```

---

## Layout Principles

### Grid and Structure

- **Clean, open compositions** -- generous whitespace evoking the vast emptiness of space; content floats in open fields
- **Circular and elliptical containers** -- pod-shaped content areas, circular image masks, and orbital arrangement of elements
- **Strong horizontal bands** -- wide, landscape-oriented sections referencing control panels and spacecraft instrument layouts
- **Centered symmetry with dynamic accents** -- primary content centered (spacecraft cockpit perspective) with asymmetric decorative elements
- **Modular grid** -- repeating, standardized content units suggesting prefabricated space-station modules
- **Layered depth** -- foreground chrome UI elements over cosmic gradient or clean white backgrounds

### Section Organization

- Use **thin chrome dividers** or **orbital arc separators** between sections
- Apply **circular or elliptical frames** around key content (referencing portholes and capsule windows)
- Create **hierarchy through scale and weight** -- oversized bold headlines, moderate subheadings, light body text
- Employ **curved panel edges** -- rounded rectangles and pill-shaped containers rather than sharp corners
- Feature **floating satellite decorations** -- small circular or starburst elements as visual punctuation
- Use **alternating light/dark sections** -- white panels alternating with deep space dark panels for dramatic contrast

---

## CSS/Design Techniques

### Chrome Metallic Surface

```css
/* Polished chrome gradient */
.space-chrome-surface {
  background: linear-gradient(
    180deg,
    #f0f0f0 0%,
    #d4d4d4 20%,
    #a0a0a0 45%,
    #c0c0c0 55%,
    #e8e8e8 80%,
    #f5f5f5 100%
  );
}

/* Chrome text effect */
.space-chrome-text {
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #c0c0c0 30%,
    #808080 50%,
    #c0c0c0 70%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

### Porthole / Capsule Window Frame

```css
.space-porthole {
  width: 280px;
  height: 280px;
  border-radius: 50%;
  border: 12px solid var(--space-silver);
  box-shadow:
    inset 0 0 30px rgba(0, 0, 0, 0.15),
    0 0 0 4px var(--space-silver-dark),
    0 0 0 8px var(--space-silver-light),
    0 8px 24px rgba(0, 0, 0, 0.2);
  overflow: hidden;
  background: var(--space-navy);
}

/* Porthole rivet accents */
.space-porthole::before {
  content: '';
  position: absolute;
  inset: -16px;
  border-radius: 50%;
  background:
    radial-gradient(circle at 50% 2%, var(--space-silver-dark) 3px, transparent 3px),
    radial-gradient(circle at 50% 98%, var(--space-silver-dark) 3px, transparent 3px),
    radial-gradient(circle at 2% 50%, var(--space-silver-dark) 3px, transparent 3px),
    radial-gradient(circle at 98% 50%, var(--space-silver-dark) 3px, transparent 3px);
}
```

### Orbital Ring Decoration

```css
.space-orbit {
  position: relative;
  width: 300px;
  height: 300px;
}

.space-orbit::before,
.space-orbit::after {
  content: '';
  position: absolute;
  inset: 5%;
  border: 2px solid var(--space-silver);
  border-radius: 50%;
  opacity: 0.4;
}

.space-orbit::before {
  transform: rotateX(70deg);
  animation: orbit-rotate 8s linear infinite;
}

.space-orbit::after {
  transform: rotateX(70deg) rotateZ(60deg);
  animation: orbit-rotate 8s linear infinite reverse;
}

/* Satellite dot on orbit */
.space-satellite {
  width: 10px;
  height: 10px;
  background: var(--space-red);
  border-radius: 50%;
  box-shadow: 0 0 8px var(--space-red), 0 0 16px var(--space-red);
  animation: orbit-rotate 4s linear infinite;
}

@keyframes orbit-rotate {
  to { transform: rotateX(70deg) rotateZ(360deg); }
}
```

### Geodesic Dome Pattern

```css
/* Triangulated dome-like pattern overlay */
.space-geodesic {
  background-image:
    linear-gradient(60deg, var(--space-silver) 1px, transparent 1px),
    linear-gradient(-60deg, var(--space-silver) 1px, transparent 1px),
    linear-gradient(0deg, var(--space-silver) 1px, transparent 1px);
  background-size: 40px 70px;
  opacity: 0.08;
}
```

### Starburst Accent

```css
.space-starburst {
  position: relative;
  width: 160px;
  height: 160px;
}

.space-starburst::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-conic-gradient(
    var(--space-yellow) 0deg 4deg,
    transparent 4deg 12deg
  );
  border-radius: 50%;
  opacity: 0.15;
  animation: starburst-pulse 4s ease-in-out infinite alternate;
}

@keyframes starburst-pulse {
  from { transform: scale(0.95); opacity: 0.1; }
  to { transform: scale(1.05); opacity: 0.2; }
}
```

### Rocket Fin Section Divider

```css
.space-fin-divider {
  height: 60px;
  position: relative;
  overflow: hidden;
}

.space-fin-divider::before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 40px solid transparent;
  border-right: 40px solid transparent;
  border-bottom: 60px solid var(--space-silver);
  opacity: 0.25;
}

/* Chrome line through center */
.space-fin-divider::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--space-silver) 20%,
    var(--space-silver) 80%,
    transparent
  );
}
```

### Space Age Card / Panel

```css
.space-card {
  background: var(--space-white);
  border: 1px solid var(--space-silver);
  border-radius: 16px;
  padding: 2.5rem;
  position: relative;
  overflow: hidden;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.06);
}

/* Colored top accent bar */
.space-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(
    90deg,
    var(--space-red),
    var(--space-blue),
    var(--space-turquoise)
  );
}

/* Dark variant for cosmic sections */
.space-card--dark {
  background: var(--space-navy);
  border-color: rgba(192, 192, 192, 0.2);
  color: var(--space-white);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
}
```

### Pill / Capsule-Shaped Container

```css
.space-capsule {
  border-radius: 999px;
  padding: 1rem 2.5rem;
  background: var(--space-silver-light);
  border: 2px solid var(--space-silver);
  display: inline-flex;
  align-items: center;
  gap: 0.75rem;
}

.space-capsule--accent {
  background: var(--space-blue);
  border-color: var(--space-blue);
  color: white;
}
```

### Cosmic Starfield Background

```css
/* Deep space with scattered stars */
.space-starfield {
  background-color: var(--space-black);
  background-image:
    radial-gradient(1px 1px at 15% 25%, rgba(255, 255, 255, 0.8), transparent),
    radial-gradient(1px 1px at 45% 65%, rgba(255, 255, 255, 0.6), transparent),
    radial-gradient(1.5px 1.5px at 75% 20%, rgba(255, 255, 255, 0.9), transparent),
    radial-gradient(1px 1px at 80% 80%, rgba(255, 255, 255, 0.5), transparent),
    radial-gradient(1px 1px at 30% 90%, rgba(255, 255, 255, 0.7), transparent),
    radial-gradient(1.5px 1.5px at 60% 45%, rgba(255, 255, 255, 0.4), transparent);
  background-size: 200px 200px;
}

/* Gradient variant with nebula feel */
.space-cosmic-bg {
  background: linear-gradient(
    160deg,
    #0a0a1a 0%,
    #0d1b3e 40%,
    #0f2044 70%,
    #0a0a1a 100%
  );
}
```

### Glossy Surface / Plastic Sheen

```css
/* Glossy fiberglass-like surface */
.space-glossy {
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.25) 0%,
    rgba(255, 255, 255, 0.05) 40%,
    rgba(255, 255, 255, 0) 60%,
    rgba(255, 255, 255, 0.1) 100%
  );
  position: relative;
}

/* Reflection highlight strip */
.space-glossy::after {
  content: '';
  position: absolute;
  top: 8%;
  left: 15%;
  right: 40%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.6),
    transparent
  );
  border-radius: 50%;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Space Age materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Polished chrome / steel | Multi-stop silver linear gradients with bright highlight bands |
| Fiberglass (molded furniture) | Smooth solid-color panels with generous border-radius and subtle gradient sheen overlay |
| Glossy white plastic | Clean white backgrounds with faint diagonal highlight gradient |
| PVC / vinyl | Smooth surfaces with subtle sheen; semi-gloss solid colors |
| Metallic fabric | Fine repeating-linear-gradient shimmer texture over solid color |
| Glass (architectural) | Semi-transparent panels with subtle backdrop-filter blur |
| Concrete (brutalist elements) | Light gray backgrounds with minimal texture; flat and clean |
| Anodized aluminum | Tinted metallic gradients (blue-chrome, turquoise-chrome) |
| Plexiglass / Lucite | Semi-transparent overlays with border and subtle inner shadow |
| Prefabricated panels | Modular grid layouts with consistent spacing and uniform card containers |
| Neon tube signage | CSS text-shadow and box-shadow glow effects in vivid colors |
| Space suit material | Matte white/silver surfaces with subtle quilted or segmented pattern |

---

## Key Designers and Influences

| Designer/Reference | Contribution |
|-------------------|-------------|
| **Eero Saarinen** | TWA Flight Center at JFK -- sweeping concrete curves, pod-like interiors; Tulip Table and Chair |
| **Eero Aarnio** | Ball Chair (1963) -- iconic spherical pod seat embodying Space Age enclosure and futurism |
| **Verner Panton** | Panton Chair -- revolutionary single-piece S-curved plastic chair |
| **Andre Courreges** | "Moon Girl" fashion line -- go-go boots, A-line silhouettes, white/silver dominance, geometric cutouts |
| **Pierre Cardin** | "Cosmos" collection (1967) -- geometric cutout dresses with matching helmets, theatrical futurism |
| **Paco Rabanne** | Metal-disc chain-mail dresses and metallic ensembles; radical synthetic material fashion |
| **Matti Suuronen** | Futuro House (1968) -- elliptical, UFO-shaped prefabricated plastic dwelling |
| **Buckminster Fuller** | Geodesic dome structures -- lightweight triangulated spheres as futuristic architecture |
| **Googie architects** | Upswept roofs, parabolas, and starbursts in commercial architecture (Theme Building at LAX) |
| **Cadillac (1959)** | Coupe de Ville with dramatic tailfins and chrome details inspired by rocket and jet aircraft imagery |

---

## Related Aesthetics

| Aesthetic | Relationship to Space Age |
|-----------|--------------------------|
| **Atomic Age** | Predecessor and sibling; shares optimistic futurism but emphasizes nuclear/atomic motifs rather than space exploration |
| **Raygun Gothic** | Retro-futuristic cousin; combines Art Deco with rocket-era imagery in a more fantastical, pulp-fiction direction |
| **Mid-Century Modern** | Broader contemporary movement; Space Age is a more futuristic, technology-obsessed branch of MCM |
| **Googie** | Architectural sub-style; exuberant commercial expression with upswept roofs, starbursts, and boomerang shapes |
| **Retrofuturism** | Parent category; Space Age is one of the defining retrofuturistic styles |
| **Atompunk** | Speculative fiction aesthetic that amplifies Space Age and Atomic Age visual language to extremes |
| **Rocketpunk** | Science fiction sub-genre focused specifically on rocket technology and early space travel aesthetics |
| **Mod** | Contemporary fashion/cultural movement sharing Space Age's clean geometric forms and youth-culture optimism |
| **Pop Art** | Contemporary art movement sharing bold colors, graphic simplicity, and celebration of modern consumer culture |
| **Cassette Futurism** | Successor retrofuturism; represents the next generation (1970s-1980s) with analog tech replacing chrome rockets |
| **Y2K Futurism** | Later descendant; translates Space Age optimism into digital-era chrome, silver, and iridescent surfaces |
| **Streamline Moderne** | Direct predecessor; aerodynamic curves and chrome surfaces that Space Age launched into orbit |

---

## Quick-Start: Minimal Space Age Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Space Age Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Jost:wght@300;400;500&family=Rajdhani:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --space-white: #f7f7f7;
      --space-silver: #c0c0c0;
      --space-silver-light: #e8e8e8;
      --space-red: #e53935;
      --space-blue: #1e88e5;
      --space-orange: #ff8f00;
      --space-yellow: #ffd600;
      --space-turquoise: #00bcd4;
      --space-black: #0a0a1a;
      --space-navy: #0d1b3e;
      --space-gray: #78909c;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--space-white);
      color: #1a1a2e;
      font-family: 'Jost', sans-serif;
      font-weight: 400;
      letter-spacing: 0.02em;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.10em;
      font-weight: 700;
    }

    .hero {
      text-align: center;
      padding: 6rem 2rem;
      position: relative;
      overflow: hidden;
      background: var(--space-white);
    }

    .hero h1 {
      font-size: clamp(3rem, 8vw, 7rem);
      letter-spacing: 0.15em;
      font-weight: 900;
      color: #1a1a2e;
    }

    /* Orbital ring behind hero */
    .hero::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%) rotateX(70deg);
      width: 500px;
      height: 500px;
      border: 2px solid var(--space-silver);
      border-radius: 50%;
      opacity: 0.15;
      pointer-events: none;
    }

    .space-divider {
      width: 50%;
      margin: 2rem auto;
      border: none;
      height: 1px;
      background: linear-gradient(
        90deg,
        transparent,
        var(--space-silver) 20%,
        var(--space-silver) 80%,
        transparent
      );
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
    }

    .space-card {
      background: white;
      border: 1px solid var(--space-silver);
      border-radius: 16px;
      padding: 2.5rem;
      position: relative;
      overflow: hidden;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.06);
    }

    .space-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 4px;
      background: linear-gradient(
        90deg,
        var(--space-red),
        var(--space-blue),
        var(--space-turquoise)
      );
    }

    .space-label {
      font-family: 'Rajdhani', sans-serif;
      font-size: 0.8em;
      text-transform: uppercase;
      letter-spacing: 0.20em;
      color: var(--space-gray);
      font-weight: 600;
    }

    a {
      color: var(--space-blue);
      text-decoration: none;
      border-bottom: 1px solid var(--space-silver);
    }

    a:hover {
      color: var(--space-red);
      border-bottom-color: var(--space-red);
    }
  </style>
</head>
<body>
  <div class="hero">
    <p class="space-label">Mission Control</p>
    <h1>Title Here</h1>
    <hr class="space-divider">
    <p>A clean, futuristic subtitle in Jost</p>
  </div>
  <section>
    <div class="space-card">
      <h2>Section Heading</h2>
      <p>Content with Space Age styling applied.</p>
    </div>
  </section>
</body>
</html>
```
