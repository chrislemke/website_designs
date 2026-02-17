# Frutiger Eco Design Reference

Frutiger Eco is a sub-aesthetic of **Frutiger Aero** that blends **advanced technology with nature** through a strong focus on **sustainability and environmental optimism**. It inherits Frutiger Aero's glossy textures, humanism, bokeh, bubbles, and abstract flourishes, but channels them toward an **eco-friendly, green-technology narrative**. The aesthetic evokes a mid-2000s to early-2010s vision of a future where technology and nature coexist harmoniously -- solar panels on rolling green hills, futuristic architecture covered in vegetation, crystal-clear water alongside sleek devices. It is optimistic, clean, luminous, and fundamentally about the promise that technology can heal and sustain the natural world.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Solar panels and renewable energy** -- photovoltaic arrays, wind turbines, and green energy infrastructure depicted in bright, idealized settings
- **Green-tinted Earth imagery** -- the planet rendered in vivid emerald and teal tones, emphasizing environmental health
- **Nature integrated into architecture** -- buildings with living walls, rooftop gardens, trees growing through futuristic structures
- **Water elements** -- crystal-clear streams, water droplets, splashes, and reflections suggesting purity and renewal
- **Lush vegetation** -- vibrant green leaves, grass fields, seedlings, and forest canopies as recurring visual anchors
- **Glossy, translucent surfaces** -- glass-like panels and aero-glass UI elements inherited from Frutiger Aero
- **Bokeh and light effects** -- soft, diffused light circles in green and blue tones creating depth and warmth
- **Abstract organic flourishes** -- flowing curves, leaf-shaped vector swirls, and tendril-like decorative elements
- **Bubbles and spheres** -- translucent orbs suggesting water, air purity, or contained ecosystems
- **Sunlight and lens flares** -- warm golden light streaming through foliage, suggesting natural energy and vitality

### Design Principles

- **Technological optimism meets environmentalism** -- every design element communicates that technology serves nature, not the other way around
- **Bright, clean, and airy compositions** -- white space and light backgrounds evoke freshness and breathability
- **Glossy realism with organic softness** -- surfaces are polished and reflective but curves are rounded and natural, never harsh
- **Green as the dominant chromatic identity** -- green is omnipresent, from backgrounds to accents to imagery
- **Depth through layering and transparency** -- glass panels, bokeh, and translucent overlays create a rich sense of Z-axis depth
- **Humanist warmth** -- the design feels inviting and accessible, never cold or sterile despite its technological subject matter
- **Skeuomorphic tendencies** -- elements reference real-world materials (water, glass, leaves) with tactile, realistic rendering
- **Corporate sustainability messaging** -- the aesthetic was widely adopted by brands to communicate eco-friendliness and green initiatives

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | White, soft off-white, pale sky blue |
| **Primary** | Vivid green, leaf green, emerald |
| **Secondary** | Teal, cyan, sky blue |
| **Accent** | Sunlight yellow, warm gold |
| **Depth** | Dark blue, deep teal, forest green |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Pure White | `#FFFFFF`, `#F8FAFA` | Primary backgrounds, clean canvas areas |
| Cloud White | `#EEF5F0`, `#E8F0EA` | Secondary backgrounds, subtle green-tinted whites |
| Leaf Green | `#34A853`, `#3CB44B` | Primary accent, CTAs, key interactive elements |
| Vivid Emerald | `#00C853`, `#00E676` | Highlights, success states, energy indicators |
| Deep Forest | `#1B5E20`, `#2E7D32` | Dark accents, footer backgrounds, contrast text |
| Eco Teal | `#009688`, `#00897B` | Secondary accent, links, navigation elements |
| Cyan Fresh | `#00BCD4`, `#26C6DA` | Water motifs, tertiary accent, decorative elements |
| Sky Blue | `#4FC3F7`, `#81D4FA` | Sky gradients, atmospheric backgrounds |
| Deep Blue | `#0D47A1`, `#1565C0` | Earth imagery undertone, deep contrast backgrounds |
| Sunlight Gold | `#FFD54F`, `#FFC107` | Solar energy accents, warm highlights, badges |
| Warm Amber | `#FF8F00`, `#FFA000` | Energy accents, call-to-action warmth |
| Earth Brown | `#5D4037`, `#6D4C41` | Soil, wood, and organic material references |
| Petal Pink | `#F8BBD0`, `#F48FB1` | Flower accents, soft decorative touches |
| Bokeh Green | `rgba(52, 168, 83, 0.15)` | Ambient light effects, background glow |
| Bokeh Blue | `rgba(79, 195, 247, 0.12)` | Atmospheric depth, water light reflections |
| Glass White | `rgba(255, 255, 255, 0.7)` | Aero glass panel backgrounds |

### Suggested CSS Custom Properties

```css
:root {
  /* Light base tones */
  --frutiger-eco-white: #ffffff;
  --frutiger-eco-cloud: #eef5f0;
  --frutiger-eco-mist: #e8f0ea;
  --frutiger-eco-frost: #f8fafa;

  /* Green spectrum */
  --frutiger-eco-green: #34a853;
  --frutiger-eco-green-vivid: #00c853;
  --frutiger-eco-green-bright: #00e676;
  --frutiger-eco-green-deep: #2e7d32;
  --frutiger-eco-green-forest: #1b5e20;

  /* Blue / Teal spectrum */
  --frutiger-eco-teal: #009688;
  --frutiger-eco-teal-light: #00897b;
  --frutiger-eco-cyan: #00bcd4;
  --frutiger-eco-cyan-light: #26c6da;
  --frutiger-eco-sky: #4fc3f7;
  --frutiger-eco-sky-light: #81d4fa;
  --frutiger-eco-blue-deep: #0d47a1;
  --frutiger-eco-blue: #1565c0;

  /* Warm accents */
  --frutiger-eco-gold: #ffd54f;
  --frutiger-eco-amber: #ffc107;
  --frutiger-eco-amber-deep: #ff8f00;
  --frutiger-eco-earth: #5d4037;

  /* Glow / transparency */
  --frutiger-eco-glow-green: rgba(52, 168, 83, 0.2);
  --frutiger-eco-glow-cyan: rgba(0, 188, 212, 0.15);
  --frutiger-eco-glow-gold: rgba(255, 213, 79, 0.2);
  --frutiger-eco-glass: rgba(255, 255, 255, 0.7);
  --frutiger-eco-glass-strong: rgba(255, 255, 255, 0.85);
  --frutiger-eco-glass-border: rgba(255, 255, 255, 0.5);
  --frutiger-eco-shadow: rgba(0, 80, 40, 0.08);

  /* Functional mappings */
  --frutiger-eco-bg-primary: var(--frutiger-eco-white);
  --frutiger-eco-bg-secondary: var(--frutiger-eco-cloud);
  --frutiger-eco-bg-surface: var(--frutiger-eco-glass);
  --frutiger-eco-text-primary: var(--frutiger-eco-green-forest);
  --frutiger-eco-text-secondary: #4a635a;
  --frutiger-eco-text-body: #37474f;
  --frutiger-eco-accent: var(--frutiger-eco-green);
  --frutiger-eco-accent-secondary: var(--frutiger-eco-teal);
  --frutiger-eco-border: rgba(46, 125, 50, 0.15);
}
```

### Color Approaches

- **Light, airy backgrounds dominated by white and soft greens** -- the aesthetic is bright and optimistic, never dark
- **Green as the unifying chromatic thread** -- from deep forest to vivid emerald, green appears in every context
- **Blue-to-teal as the secondary axis** -- representing water, sky, and technological clarity
- **Warm gold accents for solar energy** -- sunlight yellow/amber communicates energy, warmth, and hope
- **Gradients that mimic natural lighting** -- sky-to-earth gradients, sunlit greens, water-teal fades
- **High saturation for nature imagery, soft tones for UI** -- photographs and illustrations pop; interface elements stay gentle

---

## Typography

### Typeface Characteristics

Frutiger Eco typography is clean, humanist, and highly legible -- mirroring the aesthetic's optimistic, accessible philosophy:

- **Humanist sans-serif typefaces** -- warm, organic letterforms that feel approachable rather than mechanical
- **Named after Adrian Frutiger's typeface** -- the Frutiger font family is the canonical reference, though web alternatives are used in practice
- **Regular to medium weight for body text** -- clear and readable, never too thin or heavy
- **Semibold to bold for headlines** -- confident but not aggressive
- **Generous line-height and comfortable letter-spacing** -- airy and breathable, matching the aesthetic's open compositions
- **No serifs** -- all type is smooth, modern, sans-serif
- **Rounded variants welcome** -- subtly rounded sans-serifs reinforce the organic, nature-friendly feeling
- **Clean hierarchy** -- simple size progression, green or teal accent colors for headings

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Nunito Sans** | Humanist, slightly rounded | Body text, paragraphs -- warm and highly legible |
| **Nunito** | Rounded, friendly sans | Headlines, display text -- the organic warmth of Frutiger Eco |
| **Open Sans** | Neutral, humanist | Body text, UI labels -- clean and universally readable |
| **Poppins** | Geometric, modern | Headlines, subheadings -- contemporary with friendly geometry |
| **Lato** | Humanist, warm | Body text, paragraphs -- subtle warmth in letterforms |
| **Quicksand** | Rounded, geometric | Display text, taglines -- playful, eco-friendly feel |
| **Source Sans 3** | Humanist, technical | Body text, data displays -- clear and professional |
| **Rubik** | Slightly rounded, modern | Headlines, cards -- soft corners echo rounded UI elements |
| **Fira Sans** | Humanist, open | Body text, technical content -- close to Frutiger's proportions |
| **DM Sans** | Clean, geometric | Headlines, UI elements -- modern and balanced |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Nunito', 'Poppins', 'Rubik', sans-serif;
  font-weight: 700;
  letter-spacing: -0.01em;
  color: var(--frutiger-eco-green-forest);
  line-height: 1.2;
}

/* Display / Hero text */
.frutiger-eco-display {
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 700;
  letter-spacing: -0.02em;
  line-height: 1.1;
  color: var(--frutiger-eco-green-deep);
  text-shadow: 0 2px 20px rgba(46, 125, 50, 0.15);
}

/* Body text */
body {
  font-family: 'Nunito Sans', 'Open Sans', 'Lato', sans-serif;
  font-weight: 400;
  letter-spacing: 0.01em;
  line-height: 1.75;
  color: var(--frutiger-eco-text-body);
}

/* Tagline / subtitle */
.frutiger-eco-tagline {
  font-family: 'Quicksand', 'Poppins', sans-serif;
  font-size: 1.15rem;
  font-weight: 500;
  letter-spacing: 0.03em;
  color: var(--frutiger-eco-teal);
}

/* Label / small caps */
.frutiger-eco-label {
  font-family: 'Source Sans 3', 'Fira Sans', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--frutiger-eco-green);
}
```

---

## Layout Principles

### Grid and Structure

- **Light, expansive white backgrounds** -- generous whitespace communicates freshness and environmental purity
- **Centered, wide content areas** -- content breathes in the open space, never feeling cramped
- **Full-bleed nature imagery** -- hero sections and dividers feature edge-to-edge photographs of landscapes, greenery, or water
- **Rounded containers and cards** -- soft rounded rectangles (16-24px radius) with glossy glass effects
- **Asymmetric organic layouts** -- elements can curve, overlap, and flow rather than sitting rigidly in strict grids
- **Layered transparency** -- glass panels float over photographic or gradient backgrounds, creating depth
- **Generous padding and spacing** -- elements have room to breathe, reinforcing the open, natural feeling

### Section Organization

- Use **green gradient dividers** or **leaf/vine decorative separators** between major sections
- Apply **aero glass containers** for content cards -- semi-transparent white with backdrop blur over nature backgrounds
- Create **visual hierarchy through color intensity** -- vivid green for primary elements, soft teal for secondary, muted sage for tertiary
- Employ **rounded-rectangle cards with subtle shadows** -- the signature container shape of the Frutiger family
- Feature **full-width photographic bands** -- alternating sections of white UI and vivid nature photography
- Add **floating organic shapes** -- translucent leaf silhouettes, bubble elements, or water droplets as decorative background layers
- Include **iconography using nature symbols** -- leaves, water drops, sun rays, recycling arrows, seedlings

---

## CSS/Design Techniques

### Eco Glass Panel (Aero Glass with Green Tint)

```css
/* Frosted glass panel with green-tinted translucency -- the signature Frutiger Eco surface */
.frutiger-eco-glass {
  background: rgba(255, 255, 255, 0.72);
  backdrop-filter: blur(20px) saturate(1.4);
  -webkit-backdrop-filter: blur(20px) saturate(1.4);
  border: 1px solid rgba(255, 255, 255, 0.6);
  border-radius: 20px;
  padding: 2.5rem;
  box-shadow:
    0 8px 32px rgba(0, 80, 40, 0.08),
    0 1px 4px rgba(0, 80, 40, 0.04),
    inset 0 1px 0 rgba(255, 255, 255, 0.8);
}

/* Glass panel with top-edge shine */
.frutiger-eco-glass::before {
  content: '';
  position: absolute;
  top: 0;
  left: 8%;
  right: 8%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.9),
    transparent
  );
}
```

### Nature Hero Section with Sky-to-Earth Gradient

```css
/* Hero section evoking open sky above lush earth */
.frutiger-eco-hero {
  position: relative;
  min-height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  overflow: hidden;
  background: linear-gradient(
    180deg,
    #e3f2fd 0%,
    #e8f5e9 35%,
    #c8e6c9 65%,
    #a5d6a7 100%
  );
}

/* Sunlight rays effect */
.frutiger-eco-hero::before {
  content: '';
  position: absolute;
  top: -20%;
  left: 30%;
  width: 40%;
  height: 70%;
  background: radial-gradient(
    ellipse at center,
    rgba(255, 235, 59, 0.2) 0%,
    rgba(255, 235, 59, 0.05) 40%,
    transparent 70%
  );
  pointer-events: none;
}

/* Floating green bokeh particles */
.frutiger-eco-hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(circle 120px at 15% 30%, rgba(76, 175, 80, 0.15) 0%, transparent 100%),
    radial-gradient(circle 80px at 75% 50%, rgba(0, 188, 212, 0.1) 0%, transparent 100%),
    radial-gradient(circle 60px at 60% 20%, rgba(255, 213, 79, 0.1) 0%, transparent 100%),
    radial-gradient(circle 100px at 30% 70%, rgba(0, 150, 136, 0.08) 0%, transparent 100%);
  pointer-events: none;
}
```

### Glossy Green Button

```css
/* Glossy green button with Frutiger Aero-style shine -- the signature CTA */
.frutiger-eco-button {
  display: inline-block;
  padding: 0.85rem 2.5rem;
  border-radius: 50px;
  border: none;
  background: linear-gradient(
    180deg,
    #66bb6a 0%,
    #43a047 40%,
    #388e3c 100%
  );
  color: #ffffff;
  font-family: 'Nunito', 'Poppins', sans-serif;
  font-size: 1rem;
  font-weight: 700;
  letter-spacing: 0.03em;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 4px 16px rgba(46, 125, 50, 0.3),
    0 2px 4px rgba(46, 125, 50, 0.2),
    inset 0 1px 0 rgba(255, 255, 255, 0.35);
  transition: all 0.3s ease;
}

/* Glossy top highlight */
.frutiger-eco-button::before {
  content: '';
  position: absolute;
  top: 0;
  left: 10%;
  right: 10%;
  height: 45%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.3) 0%,
    rgba(255, 255, 255, 0.05) 100%
  );
  border-radius: 50px 50px 60% 60%;
  pointer-events: none;
}

.frutiger-eco-button:hover {
  background: linear-gradient(
    180deg,
    #81c784 0%,
    #4caf50 40%,
    #43a047 100%
  );
  box-shadow:
    0 6px 24px rgba(46, 125, 50, 0.4),
    0 2px 8px rgba(46, 125, 50, 0.25),
    inset 0 1px 0 rgba(255, 255, 255, 0.4);
  transform: translateY(-1px);
}
```

### Eco Card with Leaf Accent

```css
/* Content card with organic green accent and glossy surface */
.frutiger-eco-card {
  background: linear-gradient(
    160deg,
    rgba(255, 255, 255, 0.9) 0%,
    rgba(232, 245, 233, 0.85) 100%
  );
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(76, 175, 80, 0.15);
  border-radius: 18px;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 8px 24px rgba(0, 80, 40, 0.06),
    0 2px 6px rgba(0, 80, 40, 0.04),
    inset 0 1px 0 rgba(255, 255, 255, 0.7);
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.frutiger-eco-card:hover {
  transform: translateY(-3px);
  box-shadow:
    0 12px 36px rgba(0, 80, 40, 0.1),
    0 4px 8px rgba(0, 80, 40, 0.06),
    inset 0 1px 0 rgba(255, 255, 255, 0.8);
}

/* Green accent bar at the top */
.frutiger-eco-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(
    90deg,
    var(--frutiger-eco-green) 0%,
    var(--frutiger-eco-teal) 50%,
    var(--frutiger-eco-cyan) 100%
  );
}
```

### Green Bokeh Background

```css
/* Floating green bokeh circles for organic atmosphere */
.frutiger-eco-bokeh {
  position: absolute;
  border-radius: 50%;
  pointer-events: none;
}

.frutiger-eco-bokeh--green {
  background: radial-gradient(
    circle,
    rgba(76, 175, 80, 0.25) 0%,
    rgba(76, 175, 80, 0.05) 60%,
    transparent 100%
  );
  filter: blur(30px);
}

.frutiger-eco-bokeh--cyan {
  background: radial-gradient(
    circle,
    rgba(0, 188, 212, 0.2) 0%,
    rgba(0, 188, 212, 0.04) 60%,
    transparent 100%
  );
  filter: blur(25px);
}

.frutiger-eco-bokeh--gold {
  background: radial-gradient(
    circle,
    rgba(255, 213, 79, 0.2) 0%,
    rgba(255, 213, 79, 0.04) 60%,
    transparent 100%
  );
  filter: blur(35px);
}

/* Animated floating motion */
@keyframes eco-float {
  0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.7; }
  25% { transform: translate(15px, -25px) scale(1.05); opacity: 0.9; }
  50% { transform: translate(-10px, -40px) scale(1.1); opacity: 0.8; }
  75% { transform: translate(20px, -15px) scale(0.95); opacity: 1; }
}

.frutiger-eco-bokeh--animated {
  animation: eco-float 15s ease-in-out infinite;
}
```

### Water Drop / Bubble Effect

```css
/* Translucent water droplet / bubble -- iconic Frutiger element */
.frutiger-eco-bubble {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background: radial-gradient(
    circle at 35% 30%,
    rgba(255, 255, 255, 0.6) 0%,
    rgba(255, 255, 255, 0.1) 30%,
    rgba(0, 188, 212, 0.05) 60%,
    rgba(0, 150, 136, 0.08) 100%
  );
  border: 1px solid rgba(255, 255, 255, 0.4);
  box-shadow:
    0 4px 20px rgba(0, 150, 136, 0.1),
    inset 0 -4px 12px rgba(0, 188, 212, 0.08),
    inset 0 2px 4px rgba(255, 255, 255, 0.5);
  position: relative;
}

/* Inner highlight / light reflection */
.frutiger-eco-bubble::before {
  content: '';
  position: absolute;
  top: 12%;
  left: 20%;
  width: 35%;
  height: 25%;
  background: radial-gradient(
    ellipse,
    rgba(255, 255, 255, 0.7) 0%,
    transparent 100%
  );
  border-radius: 50%;
  transform: rotate(-20deg);
}
```

### Leaf Decorative Divider

```css
/* Green gradient divider with organic feel */
.frutiger-eco-divider {
  border: none;
  height: 3px;
  max-width: 200px;
  margin: 3rem auto;
  background: linear-gradient(
    90deg,
    transparent,
    var(--frutiger-eco-green) 20%,
    var(--frutiger-eco-teal) 50%,
    var(--frutiger-eco-cyan-light) 80%,
    transparent
  );
  border-radius: 3px;
  box-shadow: 0 0 10px var(--frutiger-eco-glow-green);
}
```

### Organic Wave Section Separator

```css
/* Wavy section divider using SVG-based clip-path */
.frutiger-eco-wave {
  position: relative;
  margin-top: -60px;
  height: 120px;
  overflow: hidden;
}

.frutiger-eco-wave svg {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 120px;
}

/* Alternative: pure CSS wave using clip-path */
.frutiger-eco-wave-css {
  height: 80px;
  background: var(--frutiger-eco-cloud);
  clip-path: polygon(
    0% 60%, 5% 55%, 10% 48%, 15% 44%, 20% 42%,
    25% 44%, 30% 50%, 35% 55%, 40% 56%, 45% 52%,
    50% 45%, 55% 40%, 60% 38%, 65% 42%, 70% 48%,
    75% 52%, 80% 50%, 85% 45%, 90% 42%, 95% 48%,
    100% 55%, 100% 100%, 0% 100%
  );
}
```

### Eco Stat / Feature Box with Icon

```css
/* Feature highlight box with nature icon styling */
.frutiger-eco-feature {
  text-align: center;
  padding: 2rem 1.5rem;
}

.frutiger-eco-feature-icon {
  width: 72px;
  height: 72px;
  margin: 0 auto 1.2rem;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.8rem;
  background: linear-gradient(
    135deg,
    rgba(76, 175, 80, 0.12) 0%,
    rgba(0, 150, 136, 0.08) 100%
  );
  border: 1px solid rgba(76, 175, 80, 0.2);
  color: var(--frutiger-eco-green);
  box-shadow:
    0 4px 16px rgba(76, 175, 80, 0.1),
    inset 0 1px 0 rgba(255, 255, 255, 0.6);
}

.frutiger-eco-feature h3 {
  font-family: 'Nunito', sans-serif;
  font-weight: 700;
  color: var(--frutiger-eco-green-deep);
  margin-bottom: 0.5rem;
}

.frutiger-eco-feature p {
  color: var(--frutiger-eco-text-body);
  line-height: 1.6;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Frutiger Eco materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Frosted glass / window pane | Semi-transparent white background + `backdrop-filter: blur(20px)` + white border |
| Dew on a leaf | Translucent bubble/sphere with radial gradient highlights and soft shadow |
| Sunlit green foliage | Vivid green gradient background with warm gold radial-gradient overlay |
| Clear water | Cyan-to-transparent gradient with glossy reflections |
| Solar panel glass | Dark teal surface with subtle grid pattern overlay and bright reflection strip |
| Living green wall | Rich photographic background with green-tinted glass overlay |
| Polished white plastic | Clean white background with subtle `linear-gradient` shine and soft shadow |
| Morning sky | Pale blue-to-white vertical gradient with soft warm glow at horizon |
| Bamboo / natural wood | Warm tan gradient with fine `repeating-linear-gradient` grain texture |
| Water droplets on glass | Multiple small `radial-gradient` circles with highlight and soft shadow |

---

## Associated Brands and Visual References

The following products, brands, and interfaces exemplify the Frutiger Eco aesthetic:

- **Cleaning product branding** -- brands like Seventh Generation, Method, and Ecover use Frutiger Eco visual language extensively (green tones, leaf imagery, glossy surfaces, eco-messaging)
- **Windows Vista / 7 default wallpapers** -- lush green hills, blue skies, and Aero glass combine the parent Frutiger Aero with nature motifs
- **Samsung and LG eco-product marketing** -- green-tinted technology imagery with nature integration
- **Toyota Prius and hybrid vehicle advertising** -- futuristic eco-architecture, green city scapes, solar imagery
- **Green energy company websites** -- solar panel fields under blue skies, wind turbines on green hills
- **Corporate sustainability reports** -- the dominant visual language for ESG and CSR communications in the late 2000s and 2010s
- **Eco-certification labels** -- Energy Star, LEED, FSC logos and associated branding materials
- **Smart home / green building visualizations** -- futuristic architecture with integrated renewable energy and vegetation

---

## Related Aesthetics

| Aesthetic | Relationship to Frutiger Eco |
|-----------|------------------------------|
| **Frutiger Aero** | Parent aesthetic; Frutiger Eco is the environmentally-focused sub-variant, retaining the glossy depth and humanist warmth while centering nature and sustainability |
| **Solarpunk** | Closest philosophical sibling; shares the optimistic vision of technology harmonizing with nature, but Solarpunk trends more illustrative / Art Nouveau while Frutiger Eco is more corporate and photographic |
| **Cleancore** | Shares the emphasis on purity, freshness, and white/green palettes; Cleancore is broader and less technology-focused |
| **Cyberprep** | Shares technological optimism but Cyberprep is more urban/luxury while Frutiger Eco is more nature/sustainability oriented |
| **Naturecore** | Overlaps in nature imagery and green palette; Naturecore is more rustic and analog, lacking Frutiger Eco's technological futurism |
| **Vectorflourish** | Shares decorative organic vector curves and abstract botanical flourishes as design elements |
| **Y2K Futurism** | Broader umbrella; Frutiger Eco is a nature-focused expression of the same era's techno-optimism |
| **Abstract Tech** | Related; shares clean, futuristic visual language but Abstract Tech is less nature-focused |
| **Dark Aero** | Sibling under Frutiger Aero; Dark Aero takes the parent aesthetic toward dark, sleek, tech-heavy palettes -- the polar opposite of Frutiger Eco's bright, nature-forward direction |
| **Corporate Memphis** | Successor era aesthetic for corporate illustration; replaced Frutiger Eco's photorealistic glossy style with flat, abstract figures |
| **Flat Design** | Eventual successor; stripped away Frutiger Eco's depth, gloss, and skeuomorphic elements in favor of minimal, flat surfaces |

---

## Quick-Start: Minimal Frutiger Eco Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Frutiger Eco Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Nunito+Sans:wght@400;500;600&family=Quicksand:wght@500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --frutiger-eco-white: #ffffff;
      --frutiger-eco-cloud: #eef5f0;
      --frutiger-eco-green: #34a853;
      --frutiger-eco-green-vivid: #00c853;
      --frutiger-eco-green-deep: #2e7d32;
      --frutiger-eco-green-forest: #1b5e20;
      --frutiger-eco-teal: #009688;
      --frutiger-eco-cyan: #00bcd4;
      --frutiger-eco-sky: #4fc3f7;
      --frutiger-eco-gold: #ffd54f;
      --frutiger-eco-glass: rgba(255, 255, 255, 0.72);
      --frutiger-eco-glass-border: rgba(255, 255, 255, 0.6);
      --frutiger-eco-glow-green: rgba(52, 168, 83, 0.2);
      --frutiger-eco-shadow: rgba(0, 80, 40, 0.08);
      --frutiger-eco-text-body: #37474f;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--frutiger-eco-white);
      color: var(--frutiger-eco-text-body);
      font-family: 'Nunito Sans', sans-serif;
      font-weight: 400;
      letter-spacing: 0.01em;
      line-height: 1.75;
      min-height: 100vh;
      overflow-x: hidden;
    }

    h1, h2, h3 {
      font-family: 'Nunito', sans-serif;
      font-weight: 700;
      color: var(--frutiger-eco-green-forest);
    }

    /* Hero with sky-to-earth gradient and bokeh */
    .hero {
      text-align: center;
      padding: 8rem 2rem 6rem;
      position: relative;
      overflow: hidden;
      background: linear-gradient(
        180deg,
        #e3f2fd 0%,
        #e8f5e9 35%,
        #c8e6c9 65%,
        #a5d6a7 100%
      );
    }

    /* Sunlight glow */
    .hero::before {
      content: '';
      position: absolute;
      top: -10%;
      left: 25%;
      width: 50%;
      height: 60%;
      background: radial-gradient(
        ellipse at center,
        rgba(255, 235, 59, 0.15) 0%,
        transparent 70%
      );
      pointer-events: none;
    }

    /* Green bokeh particles */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(circle 100px at 12% 35%, rgba(76, 175, 80, 0.15) 0%, transparent 100%),
        radial-gradient(circle 70px at 80% 45%, rgba(0, 188, 212, 0.1) 0%, transparent 100%),
        radial-gradient(circle 50px at 55% 15%, rgba(255, 213, 79, 0.08) 0%, transparent 100%);
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Quicksand', 'Nunito', sans-serif;
      font-size: clamp(2.5rem, 5vw, 4.5rem);
      font-weight: 700;
      color: var(--frutiger-eco-green-forest);
      text-shadow: 0 2px 20px rgba(46, 125, 50, 0.1);
      position: relative;
      z-index: 1;
    }

    .hero p {
      margin-top: 1.2rem;
      font-size: 1.15rem;
      font-weight: 500;
      color: var(--frutiger-eco-teal);
      position: relative;
      z-index: 1;
    }

    /* Eco divider */
    .eco-divider {
      border: none;
      height: 3px;
      width: 120px;
      margin: 1.5rem auto;
      background: linear-gradient(
        90deg,
        var(--frutiger-eco-green),
        var(--frutiger-eco-teal),
        var(--frutiger-eco-cyan)
      );
      border-radius: 3px;
      box-shadow: 0 0 8px var(--frutiger-eco-glow-green);
      position: relative;
      z-index: 1;
    }

    section {
      max-width: 960px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    /* Aero glass card */
    .glass-card {
      background: var(--frutiger-eco-glass);
      backdrop-filter: blur(20px) saturate(1.4);
      -webkit-backdrop-filter: blur(20px) saturate(1.4);
      border: 1px solid var(--frutiger-eco-glass-border);
      border-radius: 20px;
      padding: 2.5rem;
      position: relative;
      overflow: hidden;
      box-shadow:
        0 8px 32px var(--frutiger-eco-shadow),
        inset 0 1px 0 rgba(255, 255, 255, 0.8);
    }

    /* Green accent top bar */
    .glass-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 4px;
      background: linear-gradient(
        90deg,
        var(--frutiger-eco-green) 0%,
        var(--frutiger-eco-teal) 50%,
        var(--frutiger-eco-cyan) 100%
      );
    }

    .glass-card h2 {
      margin-top: 0.5rem;
    }

    .glass-card p {
      margin-top: 1rem;
      line-height: 1.8;
    }

    /* Glossy CTA button */
    .eco-button {
      display: inline-block;
      margin-top: 1.5rem;
      padding: 0.85rem 2.5rem;
      border-radius: 50px;
      border: none;
      background: linear-gradient(180deg, #66bb6a 0%, #43a047 40%, #388e3c 100%);
      color: #fff;
      font-family: 'Nunito', sans-serif;
      font-size: 1rem;
      font-weight: 700;
      cursor: pointer;
      position: relative;
      overflow: hidden;
      box-shadow:
        0 4px 16px rgba(46, 125, 50, 0.3),
        inset 0 1px 0 rgba(255, 255, 255, 0.35);
      transition: all 0.3s ease;
      text-decoration: none;
    }

    /* Button gloss */
    .eco-button::before {
      content: '';
      position: absolute;
      top: 0;
      left: 10%;
      right: 10%;
      height: 45%;
      background: linear-gradient(180deg, rgba(255,255,255,0.3) 0%, rgba(255,255,255,0.05) 100%);
      border-radius: 50px 50px 60% 60%;
      pointer-events: none;
    }

    .eco-button:hover {
      transform: translateY(-2px);
      box-shadow:
        0 6px 24px rgba(46, 125, 50, 0.4),
        inset 0 1px 0 rgba(255, 255, 255, 0.4);
    }

    /* Ambient bokeh elements */
    .bokeh {
      position: fixed;
      border-radius: 50%;
      pointer-events: none;
      z-index: 0;
    }

    .bokeh--1 {
      width: 350px;
      height: 350px;
      background: radial-gradient(circle, rgba(76,175,80,0.12) 0%, transparent 70%);
      filter: blur(40px);
      top: 60%;
      left: -5%;
    }

    .bokeh--2 {
      width: 250px;
      height: 250px;
      background: radial-gradient(circle, rgba(0,188,212,0.08) 0%, transparent 70%);
      filter: blur(30px);
      top: 30%;
      right: -3%;
    }

    .bokeh--3 {
      width: 180px;
      height: 180px;
      background: radial-gradient(circle, rgba(255,213,79,0.1) 0%, transparent 70%);
      filter: blur(35px);
      bottom: 10%;
      right: 20%;
    }
  </style>
</head>
<body>
  <!-- Ambient bokeh -->
  <div class="bokeh bokeh--1"></div>
  <div class="bokeh bokeh--2"></div>
  <div class="bokeh bokeh--3"></div>

  <div class="hero">
    <h1>Title Here</h1>
    <hr class="eco-divider">
    <p>Subtitle celebrating technology in harmony with nature</p>
  </div>

  <section>
    <div class="glass-card">
      <h2>Section Heading</h2>
      <p>Content rendered on a frosted glass panel with green eco accents, soft bokeh atmosphere, and the optimistic warmth of the Frutiger Eco aesthetic.</p>
      <a href="#" class="eco-button">Learn More</a>
    </div>
  </section>
</body>
</html>
```
