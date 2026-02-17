# Light Skeuomorphism -- Design Reference

Light Skeuomorphism is a 2026 revival of skeuomorphic design philosophy with a lighter, more refined touch. Where the original skeuomorphism of the early 2010s relied on heavy leather, wood, and felt textures to mimic physical objects, Light Skeuomorphism distills the approach to its essence: subtle real-world object mimicry through lightly embossed surfaces, soft pressed and raised effects, and delicate gradients that suggest physicality without overt material imitation. Think of Apple's modern app icons -- gently rounded, softly lit from a consistent top-left source, with just enough shadow and gradient to feel tangible -- but applied to full web layouts. The result is a warm, tactile interface language that bridges the gap between flat design's clarity and skeuomorphism's intuitive physicality, creating surfaces that feel like they could be touched, pressed, and lifted.

---

## Visual Characteristics

- **Subtle inset and outset shadows** -- soft box-shadows create the illusion of surfaces that are gently raised above or pressed into the background, rather than floating or flat
- **Delicate linear gradients** -- surfaces carry faint top-to-bottom gradients (lighter at the top, slightly darker at the bottom) that simulate curvature and light falling across a physical surface
- **Consistent top-left light source** -- all shadows, highlights, and gradients behave as though a single diffuse light is positioned at the upper-left, creating coherent depth across the entire interface
- **Warm-tinted shadows** -- shadows use brown or warm gray tones (never pure black), giving depth a natural, organic quality rather than a harsh digital feel
- **Lightly embossed text** -- headings and labels carry subtle text-shadow effects (light highlight above-left, dark shadow below-right) that make letterforms appear gently stamped into the surface
- **Tactile button states** -- buttons have clearly differentiated rest, hover, and active (pressed) states using shadow depth changes, simulating a physical push-button mechanism
- **Generous border-radius** -- corners are softly rounded (8-16px) throughout, echoing the smooth edges of physical objects like buttons, cards, and panels
- **Soft surface materials** -- surfaces feel like matte plastic, smooth ceramic, or fine paper rather than glossy glass or raw metal
- **Gentle color shifts for depth** -- adjacent surfaces differ by subtle warm tonal shifts rather than hard borders, suggesting layered physical materials
- **Restrained physicality** -- the 3D effects are whisper-quiet; the design suggests depth without demanding attention, keeping content primary and decoration secondary
- **Smooth state transitions** -- shadow and gradient changes animate with gentle easing (200-300ms), giving interactions a satisfying physical weight
- **No heavy textures** -- unlike classic skeuomorphism, there are no leather grains, linen patterns, wood surfaces, or stitching details; physicality is achieved purely through light and shadow

---

## Color Palette

The Light Skeuomorphism palette centers on warm neutrals that evoke natural materials -- unbleached paper, smooth stone, soft clay -- with muted accent colors that feel like dyed fabric or glazed ceramic:

- **Warm cream backgrounds** -- not sterile white but gentle off-whites with yellow-brown warmth
- **Layered neutral surfaces** -- cards and panels use slightly different warm tones to create visual depth without borders
- **Brown-tinted shadows** -- all shadows derive from warm brown rather than pure black, maintaining the organic feel
- **Soft accent colors** -- muted coral, dusty blue, sage green, and warm gold provide functional color without the brightness of flat design
- **No pure black or white** -- the darkest values are warm charcoal, the lightest are soft cream
- **Highlight whites** -- subtle warm white for embossed edges and light-catch effects

### Suggested Implementation Palette

| Role                | Color            | Hex       |
|---------------------|------------------|-----------|
| Background Base     | Warm Linen       | `#F5F0EB` |
| Background Alt      | Soft Cream       | `#FAF6F0` |
| Surface Primary     | Pale Beige       | `#EDE5DC` |
| Surface Raised      | Light Sand       | `#E8E0D8` |
| Surface Pressed     | Warm Taupe       | `#D8D0C8` |
| Text Primary        | Warm Charcoal    | `#4A4240` |
| Text Secondary      | Muted Brown      | `#7A706A` |
| Text Emboss Light   | Cream White      | `#FFFEFA` |
| Text Emboss Dark    | Brown Shadow     | `#9A8A80` |
| Accent Coral        | Soft Coral       | `#D4836A` |
| Accent Blue         | Dusty Sky        | `#7CA8C8` |
| Accent Sage         | Muted Sage       | `#8AAA8A` |
| Accent Gold         | Warm Honey       | `#C8A86A` |
| Shadow Light        | Warm Tan         | `#C8BEB5` |
| Shadow Medium       | Toasted Beige    | `#B0A498` |
| Shadow Deep         | Brown Shadow     | `#8A7E72` |
| Highlight           | Warm White       | `#FFFFFF` |
| Border Subtle       | Muted Sand       | `#D0C8C0` |

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --lskeuo-bg-base: #F5F0EB;
  --lskeuo-bg-alt: #FAF6F0;
  --lskeuo-bg-surface: #EDE5DC;
  --lskeuo-bg-raised: #E8E0D8;
  --lskeuo-bg-pressed: #D8D0C8;

  /* Text */
  --lskeuo-text-primary: #4A4240;
  --lskeuo-text-secondary: #7A706A;
  --lskeuo-text-muted: #A09890;
  --lskeuo-text-emboss-light: #FFFEFA;
  --lskeuo-text-emboss-dark: #9A8A80;

  /* Accents */
  --lskeuo-accent-coral: #D4836A;
  --lskeuo-accent-blue: #7CA8C8;
  --lskeuo-accent-sage: #8AAA8A;
  --lskeuo-accent-gold: #C8A86A;

  /* Shadows (warm-tinted, never pure black) */
  --lskeuo-shadow-light: rgba(140, 120, 100, 0.15);
  --lskeuo-shadow-medium: rgba(120, 100, 80, 0.25);
  --lskeuo-shadow-deep: rgba(100, 80, 60, 0.35);
  --lskeuo-shadow-inset: rgba(100, 80, 60, 0.2);

  /* Highlights (warm white for light-catch edges) */
  --lskeuo-highlight: rgba(255, 255, 250, 0.7);
  --lskeuo-highlight-soft: rgba(255, 255, 250, 0.4);

  /* Borders */
  --lskeuo-border-subtle: #D0C8C0;
  --lskeuo-border-raised: rgba(255, 255, 250, 0.5);
  --lskeuo-border-pressed: rgba(100, 80, 60, 0.15);

  /* Surface gradients */
  --lskeuo-gradient-raised: linear-gradient(
    145deg,
    rgba(255, 255, 250, 0.5) 0%,
    rgba(255, 255, 250, 0) 50%,
    rgba(100, 80, 60, 0.08) 100%
  );
  --lskeuo-gradient-surface: linear-gradient(
    180deg,
    rgba(255, 255, 250, 0.3) 0%,
    rgba(100, 80, 60, 0.05) 100%
  );

  /* Functional mappings */
  --lskeuo-bg-primary: var(--lskeuo-bg-base);
  --lskeuo-bg-secondary: var(--lskeuo-bg-alt);
  --lskeuo-bg-card: var(--lskeuo-bg-surface);
  --lskeuo-text-heading: var(--lskeuo-text-primary);
  --lskeuo-text-body: var(--lskeuo-text-secondary);
  --lskeuo-accent-primary: var(--lskeuo-accent-coral);
  --lskeuo-accent-secondary: var(--lskeuo-accent-blue);
  --lskeuo-border: var(--lskeuo-border-subtle);

  /* Interaction */
  --lskeuo-transition: 0.2s ease;
  --lskeuo-radius-sm: 8px;
  --lskeuo-radius-md: 12px;
  --lskeuo-radius-lg: 16px;
}
```

---

## Typography

### Typeface Characteristics

Light Skeuomorphism typography is clean and modern but with a slight organic warmth that complements the tactile surfaces:

- **Rounded sans-serif typefaces** -- the soft geometry of rounded fonts mirrors the rounded corners and smooth surfaces of the design language
- **Medium weight preference (400-500)** -- text feels substantial without being heavy, matching the gentle physicality of the surfaces
- **Embossed text-shadow effects** -- headings carry a subtle dual text-shadow (light pixel above-left, dark pixel below-right) that makes text appear gently pressed into or raised from the surface
- **High readability** -- despite decorative shadow effects, text remains crisp and legible with good contrast ratios
- **Warm letter-spacing** -- slightly opened tracking (0.01-0.03em) gives text a relaxed, approachable quality
- **Generous line-height** -- 1.6-1.8 line-height provides comfortable reading rhythm
- **No display or novelty fonts** -- the aesthetic relies on clean, professional typefaces; personality comes from the embossed treatment, not the letterforms

### Recommended Web Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Nunito** | Rounded sans-serif, variable weight | Primary body text, headings -- warm and approachable with true rounded terminals |
| **Varela Round** | Geometric rounded sans | Headings, labels -- clean geometry with friendly rounded strokes |
| **Rubik** | Slightly rounded sans-serif | Body text, UI elements -- versatile with subtle rounding at corners |
| **Quicksand** | Geometric rounded sans | Lighter headings, captions -- delicate and airy |
| **DM Sans** | Geometric sans-serif | Body text alternative -- clean with slightly rounded forms |
| **Outfit** | Modern geometric sans | Headings, display -- contemporary and warm |
| **Plus Jakarta Sans** | Modern rounded sans | Body and UI text -- professional with a gentle feel |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@300;400;500;600;700&family=Varela+Round&family=Rubik:wght@300;400;500;600&display=swap');

/* Primary body text -- clean, rounded, warm */
body {
  font-family: 'Nunito', 'Rubik', -apple-system, sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 1.7;
  letter-spacing: 0.01em;
  color: var(--lskeuo-text-primary);
  -webkit-font-smoothing: antialiased;
}

/* Headings -- embossed effect with rounded font */
h1, h2, h3 {
  font-family: 'Varela Round', 'Nunito', sans-serif;
  font-weight: 500;
  color: var(--lskeuo-text-primary);
  letter-spacing: 0.02em;
  line-height: 1.3;
  /* Embossed text: light highlight top-left, shadow bottom-right */
  text-shadow:
    1px 1px 1px var(--lskeuo-text-emboss-dark),
    -1px -1px 0px var(--lskeuo-text-emboss-light);
}

h1 {
  font-size: clamp(1.6rem, 3vw, 2.4rem);
}

h2 {
  font-size: clamp(1.2rem, 2.2vw, 1.7rem);
  color: var(--lskeuo-accent-coral);
  text-shadow:
    1px 1px 1px rgba(154, 138, 128, 0.6),
    -1px -1px 0px var(--lskeuo-text-emboss-light);
}

h3 {
  font-size: clamp(1rem, 1.8vw, 1.3rem);
  text-shadow:
    1px 1px 0px rgba(154, 138, 128, 0.4),
    -1px -1px 0px rgba(255, 255, 250, 0.8);
}

/* Body paragraphs -- no text-shadow for readability */
p {
  margin-bottom: 1rem;
  color: var(--lskeuo-text-secondary);
  font-weight: 400;
}

/* Small labels -- lightly embossed */
.lskeuo-label {
  font-family: 'Nunito', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--lskeuo-text-muted);
  text-shadow:
    1px 1px 0px rgba(255, 255, 250, 0.6);
}

/* Embossed display text -- for hero sections */
.lskeuo-embossed-text {
  font-family: 'Varela Round', sans-serif;
  font-weight: 500;
  color: var(--lskeuo-bg-raised);
  text-shadow:
    1px 1px 2px rgba(100, 80, 60, 0.3),
    -1px -1px 0px rgba(255, 255, 250, 0.9);
}

/* Inset / debossed text -- text appears pressed into surface */
.lskeuo-inset-text {
  font-family: 'Nunito', sans-serif;
  color: transparent;
  background: var(--lskeuo-bg-surface);
  -webkit-background-clip: text;
  text-shadow:
    1px 1px 1px rgba(255, 255, 250, 0.5);
}
```

---

## Key Design Elements and Motifs

### Raised Surfaces (Cards and Panels)

The primary building block of Light Skeuomorphism -- surfaces that appear slightly lifted off the background:

- **Outset box-shadow** with warm tones creating a gentle drop shadow below and to the right
- **Top-left highlight edge** via a faint inner shadow or border that catches the simulated light
- **Surface gradient** running from slightly lighter at the top to slightly darker at the bottom, simulating curvature
- **Rounded corners (8-16px)** softening every surface into a tactile, holdable shape
- **No hard borders** -- depth is communicated through shadow and gradient alone, or with very subtle border colors
- **Layered elevation** -- multiple levels of surface height (background, low card, high card) create a coherent spatial hierarchy

### Pressed / Inset Surfaces

Complementing the raised surfaces, inset areas feel pushed into the background like wells or grooves:

- **Inset box-shadow** (using the `inset` keyword) creates the illusion of a surface below the surrounding plane
- **Darker at top-left** (away from light source) and lighter at bottom-right (light falling into the depression)
- **Used for input fields, text areas, and content wells** -- anywhere content should feel contained
- **Subtle background darkening** -- pressed areas use a slightly darker background color than the surrounding surface
- **Often paired with raised elements** -- a pressed well containing a raised card creates a satisfying visual hierarchy

### Tactile Buttons

Buttons are the most obviously physical element, with clear mechanical states:

- **Rest state** -- gently raised with outset shadow and top-to-bottom surface gradient
- **Hover state** -- slightly more elevated (increased shadow distance), suggesting the button is lifting to meet the finger
- **Active/pressed state** -- shadow flattens or inverts to inset, gradient reverses, button appears physically pushed down
- **Transition between states** -- smooth 150-200ms easing on shadow and transform properties gives weight to the interaction
- **Bottom edge shadow** -- a subtle darker line at the bottom edge simulates the thickness of a physical button

### Embossed Text and Decorations

Text and decorative elements carry subtle 3D treatment:

- **Dual text-shadow** -- a light shadow offset toward the light source (top-left) and a dark shadow away from it (bottom-right) creates the embossed stamp effect
- **Debossed variant** -- reversing the shadow directions makes text appear carved into the surface
- **Horizontal rules as grooves** -- dividers appear as shallow channels pressed into the surface rather than flat lines
- **Icon embossing** -- icons and small decorative elements share the embossed treatment for consistency

### Consistent Lighting Model

The single most important technical principle -- every shadow and highlight in the interface must obey a single light direction:

- **Light source: top-left (approximately 135 degrees)** -- this is the standard across all elements
- **Drop shadows fall to bottom-right** -- matching the light direction
- **Highlight edges appear on top and left sides** -- where light would catch a raised surface
- **Inset shadows are darkest at top-left** -- the interior wall facing away from light
- **Gradients run top-left light to bottom-right dark** -- on angled surfaces

---

## Layout Principles

- **Warm, neutral background canvas** -- the base page uses a warm cream or linen color that serves as the "desk" or "table" on which elements sit
- **Card-based composition** -- content is organized into raised cards and panels, each with its own subtle elevation, creating a physical collage effect
- **Layered depth hierarchy** -- background (lowest), surface panels (mid), cards (higher), buttons and interactive elements (highest) form clear spatial layers
- **Generous padding and spacing** -- elements have ample breathing room, allowing shadows to render clearly and creating a calm, uncluttered feel
- **Rounded containers throughout** -- every rectangle has rounded corners, reinforcing the tactile, physical quality
- **Input areas as pressed wells** -- form fields and text inputs appear as depressions in the surface, visually inviting content to be placed inside them
- **Consistent shadow direction** -- all elements on the page cast shadows in the same direction (bottom-right), creating a believable spatial environment
- **Subtle surface variation** -- adjacent sections use very slightly different warm neutral tones, creating depth without hard borders
- **Max-width content containers** -- centered layouts with max-width (900-1100px) keep content focused and shadows visible
- **Grid with gentle rhythm** -- card grids use consistent gaps (1.5-2rem) that allow the raised surfaces to read clearly as separate objects

### Modern Web Adaptation

- Use **CSS custom properties** for shadow values so the entire lighting model can be adjusted from one place
- **Container queries** for responsive card sizing that maintains shadow proportions
- **prefers-reduced-motion** support: disable shadow transitions and transform animations for accessibility
- **Dark mode variant**: invert the lighting model -- lighter shadows become glows, pressed surfaces become darker recesses, maintain the same physical metaphor
- **Combine with modern layout**: CSS Grid and Flexbox for positioning, with the skeuomorphic treatment applied as a visual layer on top

---

## CSS/Design Techniques

### Raised Surface (Card)

```css
/* The fundamental Light Skeuomorphism surface -- gently raised card */
.lskeuo-card {
  background: var(--lskeuo-bg-surface);
  background-image: var(--lskeuo-gradient-surface);
  border-radius: var(--lskeuo-radius-md);
  padding: 2rem;
  /* Warm outset shadow: top-left highlight, bottom-right shadow */
  box-shadow:
    /* Light catch on top-left edge */
    inset 1px 1px 0px var(--lskeuo-highlight),
    /* Subtle inner depth */
    inset -1px -1px 0px rgba(100, 80, 60, 0.06),
    /* Primary drop shadow (bottom-right) */
    3px 3px 8px var(--lskeuo-shadow-medium),
    /* Soft ambient shadow */
    1px 1px 3px var(--lskeuo-shadow-light);
  transition: box-shadow var(--lskeuo-transition),
              transform var(--lskeuo-transition);
}

/* Hover: card lifts slightly */
.lskeuo-card:hover {
  box-shadow:
    inset 1px 1px 0px var(--lskeuo-highlight),
    inset -1px -1px 0px rgba(100, 80, 60, 0.06),
    5px 5px 15px var(--lskeuo-shadow-medium),
    2px 2px 5px var(--lskeuo-shadow-light);
  transform: translateY(-1px);
}

/* Low-elevation variant */
.lskeuo-card--low {
  box-shadow:
    inset 1px 1px 0px var(--lskeuo-highlight-soft),
    2px 2px 5px var(--lskeuo-shadow-light),
    1px 1px 2px var(--lskeuo-shadow-light);
}

/* High-elevation variant */
.lskeuo-card--high {
  box-shadow:
    inset 1px 1px 0px var(--lskeuo-highlight),
    inset -1px -1px 0px rgba(100, 80, 60, 0.06),
    6px 6px 20px var(--lskeuo-shadow-medium),
    3px 3px 8px var(--lskeuo-shadow-light);
}
```

### Pressed / Inset Surface

```css
/* Inset surface -- appears pressed into the background */
.lskeuo-inset {
  background: var(--lskeuo-bg-pressed);
  border-radius: var(--lskeuo-radius-sm);
  padding: 1.5rem;
  box-shadow:
    /* Dark shadow at top-left (facing away from light) */
    inset 2px 2px 5px var(--lskeuo-shadow-medium),
    /* Subtle dark inner rim */
    inset 1px 1px 2px var(--lskeuo-shadow-light),
    /* Light catch at bottom-right (light falling into the well) */
    inset -2px -2px 4px var(--lskeuo-highlight-soft);
}

/* Shallow pressed variant (for input fields) */
.lskeuo-inset--shallow {
  background: var(--lskeuo-bg-pressed);
  border-radius: var(--lskeuo-radius-sm);
  box-shadow:
    inset 1px 1px 3px var(--lskeuo-shadow-light),
    inset -1px -1px 2px var(--lskeuo-highlight-soft);
}

/* Groove divider -- a pressed line */
.lskeuo-groove {
  height: 2px;
  background: transparent;
  border: none;
  margin: 1.5rem 0;
  box-shadow:
    inset 0 1px 1px var(--lskeuo-shadow-light),
    0 1px 0px var(--lskeuo-highlight);
}
```

### Tactile Button

```css
/* Primary button with full pressed/released states */
.lskeuo-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 0.7rem 1.8rem;
  background: var(--lskeuo-accent-coral);
  background-image: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.2) 0%,
    rgba(0, 0, 0, 0.05) 100%
  );
  color: #FFFEFA;
  font-family: 'Nunito', sans-serif;
  font-size: 0.95rem;
  font-weight: 600;
  letter-spacing: 0.02em;
  border: none;
  border-radius: var(--lskeuo-radius-sm);
  cursor: pointer;
  /* Raised appearance */
  box-shadow:
    /* Light edge (top) */
    inset 0 1px 0px rgba(255, 255, 255, 0.3),
    /* Dark bottom edge (button thickness) */
    inset 0 -2px 0px rgba(100, 60, 40, 0.25),
    /* Drop shadow */
    2px 3px 6px var(--lskeuo-shadow-medium),
    1px 1px 3px var(--lskeuo-shadow-light);
  transition:
    box-shadow 0.15s ease,
    transform 0.15s ease,
    background-image 0.15s ease;
}

/* Hover: button lifts slightly */
.lskeuo-button:hover {
  background-image: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.3) 0%,
    rgba(0, 0, 0, 0.02) 100%
  );
  box-shadow:
    inset 0 1px 0px rgba(255, 255, 255, 0.35),
    inset 0 -2px 0px rgba(100, 60, 40, 0.25),
    3px 4px 10px var(--lskeuo-shadow-medium),
    2px 2px 5px var(--lskeuo-shadow-light);
  transform: translateY(-1px);
}

/* Active: button is pressed down */
.lskeuo-button:active {
  background-image: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0.05) 0%,
    rgba(255, 255, 255, 0.1) 100%
  );
  box-shadow:
    inset 0 1px 3px rgba(100, 60, 40, 0.3),
    inset 0 -1px 0px rgba(255, 255, 255, 0.1),
    1px 1px 2px var(--lskeuo-shadow-light);
  transform: translateY(1px);
}

/* Secondary / outline button */
.lskeuo-button--secondary {
  background: var(--lskeuo-bg-surface);
  background-image: var(--lskeuo-gradient-surface);
  color: var(--lskeuo-text-primary);
  box-shadow:
    inset 0 1px 0px var(--lskeuo-highlight),
    inset 0 -2px 0px rgba(100, 80, 60, 0.12),
    2px 3px 6px var(--lskeuo-shadow-medium),
    1px 1px 3px var(--lskeuo-shadow-light);
}

.lskeuo-button--secondary:hover {
  box-shadow:
    inset 0 1px 0px var(--lskeuo-highlight),
    inset 0 -2px 0px rgba(100, 80, 60, 0.12),
    3px 4px 10px var(--lskeuo-shadow-medium),
    2px 2px 5px var(--lskeuo-shadow-light);
  transform: translateY(-1px);
}

.lskeuo-button--secondary:active {
  background-image: linear-gradient(
    180deg,
    rgba(100, 80, 60, 0.06) 0%,
    rgba(255, 255, 250, 0.2) 100%
  );
  box-shadow:
    inset 1px 1px 3px var(--lskeuo-shadow-light),
    inset -1px -1px 2px var(--lskeuo-highlight-soft);
  transform: translateY(1px);
}
```

### Embossed Text Effects

```css
/* Raised / embossed text -- text appears stamped outward */
.lskeuo-text-embossed {
  color: var(--lskeuo-text-primary);
  text-shadow:
    /* Light catch on top-left (toward light source) */
    -1px -1px 0px rgba(255, 255, 250, 0.8),
    /* Shadow on bottom-right (away from light source) */
    1px 1px 1px rgba(100, 80, 60, 0.3);
}

/* Debossed / inset text -- text appears carved into surface */
.lskeuo-text-debossed {
  color: var(--lskeuo-bg-raised);
  text-shadow:
    /* Shadow on top-left (inside the carved channel) */
    1px 1px 1px rgba(100, 80, 60, 0.25),
    /* Light catch on bottom-right (light edge of the carving) */
    -1px -1px 0px rgba(255, 255, 250, 0.6);
}

/* Soft embossed heading */
.lskeuo-heading-embossed {
  color: var(--lskeuo-text-primary);
  text-shadow:
    -1px -1px 0px rgba(255, 255, 250, 0.9),
    1px 1px 2px rgba(100, 80, 60, 0.35),
    0 0 1px rgba(100, 80, 60, 0.1);
}

/* Embossed label on colored surface */
.lskeuo-label-embossed {
  font-weight: 600;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  font-size: 0.75rem;
  color: rgba(74, 66, 64, 0.6);
  text-shadow:
    0px 1px 0px rgba(255, 255, 250, 0.7);
}
```

### Form Inputs (Inset Fields)

```css
/* Text input -- pressed into the surface like a slot */
.lskeuo-input {
  width: 100%;
  padding: 0.7rem 1rem;
  background: var(--lskeuo-bg-pressed);
  border: 1px solid var(--lskeuo-border-pressed);
  border-radius: var(--lskeuo-radius-sm);
  font-family: 'Nunito', sans-serif;
  font-size: 0.95rem;
  color: var(--lskeuo-text-primary);
  box-shadow:
    inset 2px 2px 4px var(--lskeuo-shadow-light),
    inset 1px 1px 2px rgba(100, 80, 60, 0.1),
    inset -1px -1px 2px var(--lskeuo-highlight-soft);
  outline: none;
  transition: box-shadow var(--lskeuo-transition);
}

.lskeuo-input:focus {
  box-shadow:
    inset 2px 2px 4px var(--lskeuo-shadow-light),
    inset 1px 1px 2px rgba(100, 80, 60, 0.1),
    inset -1px -1px 2px var(--lskeuo-highlight-soft),
    0 0 0 3px rgba(124, 168, 200, 0.25);
}

.lskeuo-input::placeholder {
  color: var(--lskeuo-text-muted);
}

/* Textarea variant */
.lskeuo-textarea {
  min-height: 120px;
  resize: vertical;
}

/* Select dropdown */
.lskeuo-select {
  appearance: none;
  padding-right: 2.5rem;
  background-image: url("data:image/svg+xml,%3Csvg width='12' height='8' viewBox='0 0 12 8' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1 1L6 6L11 1' stroke='%237A706A' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");
  background-repeat: no-repeat;
  background-position: right 1rem center;
}
```

### Toggle Switch

```css
/* Physical toggle switch with skeuomorphic depth */
.lskeuo-toggle {
  position: relative;
  width: 52px;
  height: 28px;
  background: var(--lskeuo-bg-pressed);
  border-radius: 14px;
  cursor: pointer;
  box-shadow:
    inset 2px 2px 4px var(--lskeuo-shadow-medium),
    inset -1px -1px 2px var(--lskeuo-highlight-soft);
  transition: background var(--lskeuo-transition);
}

/* The toggle knob -- a raised circle */
.lskeuo-toggle::after {
  content: '';
  position: absolute;
  top: 2px;
  left: 2px;
  width: 24px;
  height: 24px;
  background: var(--lskeuo-bg-alt);
  background-image: linear-gradient(
    145deg,
    rgba(255, 255, 250, 0.6) 0%,
    rgba(100, 80, 60, 0.05) 100%
  );
  border-radius: 50%;
  box-shadow:
    1px 1px 3px var(--lskeuo-shadow-medium),
    inset 0 1px 0px var(--lskeuo-highlight);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

/* Active state */
.lskeuo-toggle.active {
  background: var(--lskeuo-accent-coral);
  box-shadow:
    inset 2px 2px 4px rgba(160, 80, 60, 0.35),
    inset -1px -1px 2px rgba(255, 180, 150, 0.3);
}

.lskeuo-toggle.active::after {
  transform: translateX(24px);
}
```

### Toolbar / Navigation Bar

```css
/* Raised toolbar with embossed appearance */
.lskeuo-toolbar {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 1rem;
  background: var(--lskeuo-bg-surface);
  background-image: linear-gradient(
    180deg,
    rgba(255, 255, 250, 0.4) 0%,
    rgba(255, 255, 250, 0) 40%,
    rgba(100, 80, 60, 0.04) 100%
  );
  border-radius: var(--lskeuo-radius-md);
  box-shadow:
    inset 0 1px 0px var(--lskeuo-highlight),
    inset 0 -1px 0px rgba(100, 80, 60, 0.08),
    3px 3px 10px var(--lskeuo-shadow-medium),
    1px 1px 4px var(--lskeuo-shadow-light);
}

/* Toolbar button -- small, compact tactile buttons */
.lskeuo-toolbar-button {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  background: var(--lskeuo-bg-raised);
  background-image: var(--lskeuo-gradient-surface);
  border: none;
  border-radius: var(--lskeuo-radius-sm);
  color: var(--lskeuo-text-secondary);
  cursor: pointer;
  box-shadow:
    inset 0 1px 0px var(--lskeuo-highlight-soft),
    1px 1px 3px var(--lskeuo-shadow-light);
  transition: all 0.15s ease;
}

.lskeuo-toolbar-button:hover {
  background: var(--lskeuo-bg-alt);
  color: var(--lskeuo-text-primary);
  box-shadow:
    inset 0 1px 0px var(--lskeuo-highlight),
    2px 2px 5px var(--lskeuo-shadow-light);
}

.lskeuo-toolbar-button:active {
  box-shadow:
    inset 1px 1px 3px var(--lskeuo-shadow-light),
    inset -1px -1px 1px var(--lskeuo-highlight-soft);
  transform: scale(0.97);
}

/* Active/selected toolbar button */
.lskeuo-toolbar-button.active {
  background: var(--lskeuo-bg-pressed);
  box-shadow:
    inset 1px 1px 3px var(--lskeuo-shadow-light),
    inset -1px -1px 1px var(--lskeuo-highlight-soft);
  color: var(--lskeuo-accent-coral);
}
```

### Progress Bar and Slider

```css
/* Progress bar track -- an inset groove */
.lskeuo-progress-track {
  height: 10px;
  background: var(--lskeuo-bg-pressed);
  border-radius: 5px;
  overflow: hidden;
  box-shadow:
    inset 1px 1px 3px var(--lskeuo-shadow-light),
    inset -1px -1px 2px var(--lskeuo-highlight-soft);
}

/* Progress bar fill -- a raised surface inside the groove */
.lskeuo-progress-fill {
  height: 100%;
  background: var(--lskeuo-accent-coral);
  background-image: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.3) 0%,
    rgba(0, 0, 0, 0.05) 100%
  );
  border-radius: 5px;
  box-shadow:
    inset 0 1px 0px rgba(255, 255, 255, 0.3),
    1px 0 2px rgba(100, 60, 40, 0.2);
  transition: width 0.3s ease;
}

/* Slider thumb */
.lskeuo-slider::-webkit-slider-thumb {
  -webkit-appearance: none;
  width: 22px;
  height: 22px;
  background: var(--lskeuo-bg-alt);
  background-image: linear-gradient(
    145deg,
    rgba(255, 255, 250, 0.6) 0%,
    rgba(100, 80, 60, 0.08) 100%
  );
  border-radius: 50%;
  border: none;
  cursor: pointer;
  box-shadow:
    1px 1px 4px var(--lskeuo-shadow-medium),
    inset 0 1px 0px var(--lskeuo-highlight);
}
```

### Tabs (Raised/Active States)

```css
/* Tab container -- a slightly raised bar */
.lskeuo-tabs {
  display: flex;
  gap: 4px;
  padding: 4px;
  background: var(--lskeuo-bg-pressed);
  border-radius: var(--lskeuo-radius-md);
  box-shadow:
    inset 1px 1px 4px var(--lskeuo-shadow-light),
    inset -1px -1px 2px var(--lskeuo-highlight-soft);
}

/* Individual tab -- flat by default */
.lskeuo-tab {
  flex: 1;
  padding: 0.6rem 1.2rem;
  background: transparent;
  border: none;
  border-radius: calc(var(--lskeuo-radius-md) - 2px);
  font-family: 'Nunito', sans-serif;
  font-size: 0.9rem;
  font-weight: 500;
  color: var(--lskeuo-text-muted);
  cursor: pointer;
  transition: all 0.2s ease;
}

/* Active tab -- rises out of the pressed container */
.lskeuo-tab.active {
  background: var(--lskeuo-bg-alt);
  background-image: var(--lskeuo-gradient-surface);
  color: var(--lskeuo-text-primary);
  box-shadow:
    1px 1px 4px var(--lskeuo-shadow-light),
    inset 0 1px 0px var(--lskeuo-highlight);
  font-weight: 600;
}

.lskeuo-tab:hover:not(.active) {
  color: var(--lskeuo-text-secondary);
  background: rgba(255, 255, 250, 0.3);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical / Object Reference | Web Equivalent |
|-----------------------------|----------------|
| Matte plastic panel | Flat background with subtle `linear-gradient` (top lighter, bottom slightly darker) and warm-tinted `box-shadow` |
| Smooth ceramic button | `border-radius: 8-12px`, top highlight via `inset 0 1px 0 rgba(255,255,250,0.3)`, bottom edge via `inset 0 -2px 0` darker tone |
| Embossed metal nameplate | Dual `text-shadow` (light pixel top-left, dark pixel bottom-right) on medium-weight text |
| Pressed rubber key | `inset box-shadow` with darker top-left, lighter bottom-right, slightly darker background |
| Brushed aluminum surface | Very subtle horizontal `repeating-linear-gradient` at 1-2px scale with two near-identical warm grays |
| Fine linen paper | Warm cream background (`#FAF6F0`) with optional faint noise texture via SVG filter |
| Frosted glass knob | `border-radius: 50%`, radial gradient highlight, warm drop shadow |
| Soft clay or putty | Large `border-radius` (16-24px), gentle gradient, muted warm colors, absence of hard edges |
| Cork board | Warm beige (`#E8DDD0`) background with very subtle noise, warm shadow underneath |
| Wooden picture frame | Multi-layered `box-shadow` (highlight inner top-left, shadow inner bottom-right, outer drop shadow) around content areas |

---

## Imagery and Visual Content Guidelines

When creating or sourcing visual content for a Light Skeuomorphism styled site:

- **Warm, natural photography** -- favor images with warm color temperature, soft natural lighting, and organic subjects
- **Soft shadows in photos** -- choose images where shadows are gentle and diffused, matching the design language of the interface
- **Rounded image containers** -- always display images with `border-radius` matching the design system (8-16px), giving photos a tangible, printed quality
- **Subtle image elevation** -- photos and image containers should carry the same raised `box-shadow` as cards, making them feel like physical prints sitting on the surface
- **Avoid harsh contrast** -- images should feel warm and approachable; consider a slight CSS `filter: saturate(0.9) brightness(1.02)` to soften harsh photos
- **No flat or clinical imagery** -- avoid sterile stock photography or hard-edged graphics that conflict with the tactile warmth
- **Icons as embossed objects** -- use simple, rounded icons (line or filled) with the same embossed text-shadow treatment as text
- **Warm overlay option** -- for hero images or backgrounds, a semi-transparent warm overlay (`rgba(245, 240, 235, 0.3)`) maintains palette cohesion
- **Physical object metaphors** -- imagery of physical objects (paper, tools, food, nature) reinforces the tangible quality of the design
- **Consistent image treatment** -- all images across the interface should share the same border-radius, shadow, and optional warm filter for visual unity

---

## Related Aesthetics

| Aesthetic | Relationship to Light Skeuomorphism |
|-----------|-------------------------------------|
| **[Skeuomorphism](Skeuomorphism.md)** | Direct ancestor; Light Skeuomorphism retains the physical mimicry principle but strips away heavy material textures (leather, wood, felt) in favor of pure light-and-shadow depth |
| **[Neumorphism](Neumorphism.md)** | Close sibling; both use inset/outset shadows for depth, but Neumorphism uses monochromatic surfaces and dual-direction shadows, while Light Skeuomorphism adds warm color variation and directional gradients |
| **[Glassmorphism](Glassmorphism.md)** | Parallel modern trend; Glassmorphism uses transparency and blur for depth, Light Skeuomorphism uses shadow and gradient -- both aim to create spatial hierarchy without hard borders |
| **[Claymorphism](Claymorphism.md)** | Shares the soft, rounded, tactile quality; Claymorphism leans more colorful and playful with exaggerated inner shadows, while Light Skeuomorphism is more refined and neutral |
| **[Flat_Design](Flat_Design.md)** | Philosophical opposite; Flat Design eliminates all physical metaphor, Light Skeuomorphism carefully reintroduces it -- both react against the excesses of the other |
| **[Frutiger_Aero](Frutiger_Aero.md)** | Shares the warm, friendly, slightly glossy quality of mid-2000s UI trends; Light Skeuomorphism is a more restrained, modern evolution of this warmth |

---

## Implementation Notes

- **Shadow consistency is everything** -- the moment shadows point in different directions or use inconsistent color warmth, the illusion of physicality breaks. Audit every element to ensure top-left light source compliance. Use CSS custom properties for all shadow values so they can be adjusted globally.
- **Restraint over realism** -- the "Light" in Light Skeuomorphism is critical. The moment you add a leather texture, a stitching detail, or a heavy gloss, you have crossed into full skeuomorphism. The effects should be so subtle that a casual viewer might not consciously notice them, only feel that the interface is "nice to use."
- **Warm shadows, not black shadows** -- pure `rgba(0,0,0,...)` shadows will look cold and digital. Always tint shadows warm: `rgba(120,100,80,...)` or `rgba(100,80,60,...)`. This single detail is the difference between Light Skeuomorphism and generic shadow-heavy design.
- **Button states are the showcase** -- the rest-hover-active cycle is where this aesthetic shines most. Invest in getting button shadow transitions right. The "pressed" feeling should be unmistakable: shadows shift from outset to inset, the surface dips, the gradient subtly reverses.
- **Performance consideration** -- multiple layered `box-shadow` values are computationally heavier than flat design. Avoid applying complex shadow stacks to hundreds of elements. Use simpler shadows on list items and reserve the full treatment for cards, buttons, and key interactive elements.
- **Accessibility** -- embossed text effects can reduce contrast. Always test that the base `color` value alone (without `text-shadow`) meets WCAG AA contrast requirements against the background. The embossed effect is a visual enhancement, not a substitute for proper contrast.
- **Border-radius consistency** -- pick 2-3 border-radius values and use them everywhere. Mixing many different radii breaks the material metaphor (physical objects from the same "set" share consistent edge treatment).
- **Dark mode adaptation** -- invert the model rather than simply darkening. Light-catch shadows become subtle glows, pressed surfaces become darker recesses, and the base surface becomes a warm dark gray (not pure black). The same physical metaphor should hold.
- **Animation timing** -- shadow transitions should use `ease` or `ease-out` at 150-250ms. Too fast feels digital and snappy; too slow feels sluggish. The goal is the satisfying weight of pressing a real button.

---

## Quick-Start: Minimal Light Skeuomorphism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Light Skeuomorphism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@300;400;500;600;700&family=Varela+Round&display=swap" rel="stylesheet">
  <style>
    :root {
      /* Backgrounds */
      --lskeuo-bg-base: #F5F0EB;
      --lskeuo-bg-alt: #FAF6F0;
      --lskeuo-bg-surface: #EDE5DC;
      --lskeuo-bg-raised: #E8E0D8;
      --lskeuo-bg-pressed: #D8D0C8;

      /* Text */
      --lskeuo-text-primary: #4A4240;
      --lskeuo-text-secondary: #7A706A;
      --lskeuo-text-muted: #A09890;
      --lskeuo-text-emboss-light: #FFFEFA;
      --lskeuo-text-emboss-dark: #9A8A80;

      /* Accents */
      --lskeuo-accent-coral: #D4836A;
      --lskeuo-accent-blue: #7CA8C8;
      --lskeuo-accent-sage: #8AAA8A;
      --lskeuo-accent-gold: #C8A86A;

      /* Shadows */
      --lskeuo-shadow-light: rgba(140, 120, 100, 0.15);
      --lskeuo-shadow-medium: rgba(120, 100, 80, 0.25);
      --lskeuo-shadow-deep: rgba(100, 80, 60, 0.35);

      /* Highlights */
      --lskeuo-highlight: rgba(255, 255, 250, 0.7);
      --lskeuo-highlight-soft: rgba(255, 255, 250, 0.4);

      /* Borders */
      --lskeuo-border-subtle: #D0C8C0;

      /* Surface gradients */
      --lskeuo-gradient-surface: linear-gradient(
        180deg,
        rgba(255, 255, 250, 0.3) 0%,
        rgba(100, 80, 60, 0.05) 100%
      );

      /* Sizing */
      --lskeuo-radius-sm: 8px;
      --lskeuo-radius-md: 12px;
      --lskeuo-radius-lg: 16px;
      --lskeuo-transition: 0.2s ease;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--lskeuo-bg-base);
      color: var(--lskeuo-text-primary);
      font-family: 'Nunito', -apple-system, sans-serif;
      font-size: 16px;
      font-weight: 400;
      line-height: 1.7;
      letter-spacing: 0.01em;
      min-height: 100vh;
      -webkit-font-smoothing: antialiased;
    }

    /* Page container */
    .lskeuo-page {
      max-width: 960px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    /* Header area */
    .lskeuo-header {
      text-align: center;
      margin-bottom: 3rem;
    }

    .lskeuo-header h1 {
      font-family: 'Varela Round', 'Nunito', sans-serif;
      font-size: clamp(1.6rem, 3vw, 2.4rem);
      font-weight: 500;
      color: var(--lskeuo-text-primary);
      letter-spacing: 0.02em;
      line-height: 1.3;
      margin-bottom: 0.5rem;
      /* Embossed heading */
      text-shadow:
        -1px -1px 0px rgba(255, 255, 250, 0.9),
        1px 1px 2px rgba(100, 80, 60, 0.35);
    }

    .lskeuo-header p {
      color: var(--lskeuo-text-secondary);
      font-size: 1.05rem;
      max-width: 600px;
      margin: 0 auto;
    }

    /* Toolbar / nav bar */
    .lskeuo-toolbar {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 4px;
      padding: 4px;
      margin-bottom: 2.5rem;
      background: var(--lskeuo-bg-pressed);
      border-radius: var(--lskeuo-radius-md);
      box-shadow:
        inset 1px 1px 4px var(--lskeuo-shadow-light),
        inset -1px -1px 2px var(--lskeuo-highlight-soft);
      max-width: 420px;
      margin-left: auto;
      margin-right: auto;
    }

    .lskeuo-tab {
      flex: 1;
      padding: 0.6rem 1.2rem;
      background: transparent;
      border: none;
      border-radius: calc(var(--lskeuo-radius-md) - 2px);
      font-family: 'Nunito', sans-serif;
      font-size: 0.9rem;
      font-weight: 500;
      color: var(--lskeuo-text-muted);
      cursor: pointer;
      transition: all 0.2s ease;
    }

    .lskeuo-tab.active {
      background: var(--lskeuo-bg-alt);
      background-image: var(--lskeuo-gradient-surface);
      color: var(--lskeuo-text-primary);
      box-shadow:
        1px 1px 4px var(--lskeuo-shadow-light),
        inset 0 1px 0px var(--lskeuo-highlight);
      font-weight: 600;
    }

    .lskeuo-tab:hover:not(.active) {
      color: var(--lskeuo-text-secondary);
      background: rgba(255, 255, 250, 0.3);
    }

    /* Card grid */
    .lskeuo-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      margin-bottom: 2.5rem;
    }

    /* Raised card */
    .lskeuo-card {
      background: var(--lskeuo-bg-surface);
      background-image: var(--lskeuo-gradient-surface);
      border-radius: var(--lskeuo-radius-md);
      padding: 2rem;
      box-shadow:
        inset 1px 1px 0px var(--lskeuo-highlight),
        inset -1px -1px 0px rgba(100, 80, 60, 0.06),
        3px 3px 8px var(--lskeuo-shadow-medium),
        1px 1px 3px var(--lskeuo-shadow-light);
      transition: box-shadow var(--lskeuo-transition),
                  transform var(--lskeuo-transition);
    }

    .lskeuo-card:hover {
      box-shadow:
        inset 1px 1px 0px var(--lskeuo-highlight),
        inset -1px -1px 0px rgba(100, 80, 60, 0.06),
        5px 5px 15px var(--lskeuo-shadow-medium),
        2px 2px 5px var(--lskeuo-shadow-light);
      transform: translateY(-1px);
    }

    .lskeuo-card h2 {
      font-family: 'Varela Round', 'Nunito', sans-serif;
      font-size: 1.15rem;
      font-weight: 500;
      color: var(--lskeuo-accent-coral);
      margin-bottom: 0.8rem;
      text-shadow:
        -1px -1px 0px rgba(255, 255, 250, 0.8),
        1px 1px 1px rgba(100, 80, 60, 0.25);
    }

    .lskeuo-card p {
      color: var(--lskeuo-text-secondary);
      font-size: 0.95rem;
      margin-bottom: 1.2rem;
      line-height: 1.7;
    }

    /* Embossed label inside card */
    .lskeuo-label {
      font-size: 0.72rem;
      font-weight: 600;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      color: var(--lskeuo-text-muted);
      text-shadow: 0px 1px 0px rgba(255, 255, 250, 0.7);
      margin-bottom: 0.6rem;
    }

    /* Inset content well */
    .lskeuo-well {
      background: var(--lskeuo-bg-pressed);
      border-radius: var(--lskeuo-radius-sm);
      padding: 1.2rem;
      box-shadow:
        inset 2px 2px 5px var(--lskeuo-shadow-medium),
        inset 1px 1px 2px var(--lskeuo-shadow-light),
        inset -2px -2px 4px var(--lskeuo-highlight-soft);
    }

    .lskeuo-well p {
      font-size: 0.88rem;
      color: var(--lskeuo-text-secondary);
      margin: 0;
    }

    /* Groove divider */
    .lskeuo-groove {
      height: 2px;
      border: none;
      background: transparent;
      margin: 1.5rem 0;
      box-shadow:
        inset 0 1px 1px var(--lskeuo-shadow-light),
        0 1px 0px var(--lskeuo-highlight);
    }

    /* Stats / metric row */
    .lskeuo-stats {
      display: flex;
      gap: 1rem;
      margin-bottom: 2.5rem;
    }

    .lskeuo-stat {
      flex: 1;
      background: var(--lskeuo-bg-surface);
      background-image: var(--lskeuo-gradient-surface);
      border-radius: var(--lskeuo-radius-md);
      padding: 1.5rem;
      text-align: center;
      box-shadow:
        inset 1px 1px 0px var(--lskeuo-highlight),
        inset -1px -1px 0px rgba(100, 80, 60, 0.06),
        3px 3px 8px var(--lskeuo-shadow-medium),
        1px 1px 3px var(--lskeuo-shadow-light);
    }

    .lskeuo-stat .number {
      display: block;
      font-family: 'Varela Round', sans-serif;
      font-size: 2rem;
      font-weight: 500;
      color: var(--lskeuo-text-primary);
      text-shadow:
        -1px -1px 0px rgba(255, 255, 250, 0.9),
        1px 1px 2px rgba(100, 80, 60, 0.3);
      line-height: 1.2;
    }

    .lskeuo-stat .stat-label {
      font-size: 0.75rem;
      font-weight: 600;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      color: var(--lskeuo-text-muted);
      text-shadow: 0px 1px 0px rgba(255, 255, 250, 0.6);
      margin-top: 0.3rem;
    }

    /* Buttons */
    .lskeuo-actions {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
      margin-bottom: 2.5rem;
      justify-content: center;
    }

    .lskeuo-button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 0.75rem 2rem;
      font-family: 'Nunito', sans-serif;
      font-size: 0.95rem;
      font-weight: 600;
      letter-spacing: 0.02em;
      border: none;
      border-radius: var(--lskeuo-radius-sm);
      cursor: pointer;
      transition:
        box-shadow 0.15s ease,
        transform 0.15s ease,
        background-image 0.15s ease;
    }

    /* Primary button (coral) */
    .lskeuo-button--primary {
      background: var(--lskeuo-accent-coral);
      background-image: linear-gradient(
        180deg,
        rgba(255, 255, 255, 0.2) 0%,
        rgba(0, 0, 0, 0.05) 100%
      );
      color: #FFFEFA;
      box-shadow:
        inset 0 1px 0px rgba(255, 255, 255, 0.3),
        inset 0 -2px 0px rgba(100, 60, 40, 0.25),
        2px 3px 6px var(--lskeuo-shadow-medium),
        1px 1px 3px var(--lskeuo-shadow-light);
    }

    .lskeuo-button--primary:hover {
      background-image: linear-gradient(
        180deg,
        rgba(255, 255, 255, 0.3) 0%,
        rgba(0, 0, 0, 0.02) 100%
      );
      box-shadow:
        inset 0 1px 0px rgba(255, 255, 255, 0.35),
        inset 0 -2px 0px rgba(100, 60, 40, 0.25),
        3px 4px 10px var(--lskeuo-shadow-medium),
        2px 2px 5px var(--lskeuo-shadow-light);
      transform: translateY(-1px);
    }

    .lskeuo-button--primary:active {
      background-image: linear-gradient(
        180deg,
        rgba(0, 0, 0, 0.05) 0%,
        rgba(255, 255, 255, 0.1) 100%
      );
      box-shadow:
        inset 0 1px 3px rgba(100, 60, 40, 0.3),
        inset 0 -1px 0px rgba(255, 255, 255, 0.1),
        1px 1px 2px var(--lskeuo-shadow-light);
      transform: translateY(1px);
    }

    /* Secondary button (neutral surface) */
    .lskeuo-button--secondary {
      background: var(--lskeuo-bg-surface);
      background-image: var(--lskeuo-gradient-surface);
      color: var(--lskeuo-text-primary);
      box-shadow:
        inset 0 1px 0px var(--lskeuo-highlight),
        inset 0 -2px 0px rgba(100, 80, 60, 0.12),
        2px 3px 6px var(--lskeuo-shadow-medium),
        1px 1px 3px var(--lskeuo-shadow-light);
    }

    .lskeuo-button--secondary:hover {
      box-shadow:
        inset 0 1px 0px var(--lskeuo-highlight),
        inset 0 -2px 0px rgba(100, 80, 60, 0.12),
        3px 4px 10px var(--lskeuo-shadow-medium),
        2px 2px 5px var(--lskeuo-shadow-light);
      transform: translateY(-1px);
    }

    .lskeuo-button--secondary:active {
      background-image: linear-gradient(
        180deg,
        rgba(100, 80, 60, 0.06) 0%,
        rgba(255, 255, 250, 0.2) 100%
      );
      box-shadow:
        inset 1px 1px 3px var(--lskeuo-shadow-light),
        inset -1px -1px 2px var(--lskeuo-highlight-soft);
      transform: translateY(1px);
    }

    /* Blue accent button */
    .lskeuo-button--blue {
      background: var(--lskeuo-accent-blue);
      background-image: linear-gradient(
        180deg,
        rgba(255, 255, 255, 0.2) 0%,
        rgba(0, 0, 0, 0.05) 100%
      );
      color: #FFFEFA;
      box-shadow:
        inset 0 1px 0px rgba(255, 255, 255, 0.3),
        inset 0 -2px 0px rgba(60, 80, 100, 0.25),
        2px 3px 6px var(--lskeuo-shadow-medium),
        1px 1px 3px var(--lskeuo-shadow-light);
    }

    .lskeuo-button--blue:hover {
      box-shadow:
        inset 0 1px 0px rgba(255, 255, 255, 0.35),
        inset 0 -2px 0px rgba(60, 80, 100, 0.25),
        3px 4px 10px var(--lskeuo-shadow-medium),
        2px 2px 5px var(--lskeuo-shadow-light);
      transform: translateY(-1px);
    }

    .lskeuo-button--blue:active {
      background-image: linear-gradient(
        180deg,
        rgba(0, 0, 0, 0.05) 0%,
        rgba(255, 255, 255, 0.1) 100%
      );
      box-shadow:
        inset 0 1px 3px rgba(60, 80, 100, 0.3),
        inset 0 -1px 0px rgba(255, 255, 255, 0.1),
        1px 1px 2px var(--lskeuo-shadow-light);
      transform: translateY(1px);
    }

    /* Input field */
    .lskeuo-input-group {
      margin-bottom: 2.5rem;
      max-width: 480px;
      margin-left: auto;
      margin-right: auto;
    }

    .lskeuo-input-group label {
      display: block;
      font-size: 0.8rem;
      font-weight: 600;
      letter-spacing: 0.04em;
      color: var(--lskeuo-text-secondary);
      text-shadow: 0px 1px 0px rgba(255, 255, 250, 0.6);
      margin-bottom: 0.5rem;
    }

    .lskeuo-input {
      width: 100%;
      padding: 0.75rem 1rem;
      background: var(--lskeuo-bg-pressed);
      border: 1px solid rgba(100, 80, 60, 0.1);
      border-radius: var(--lskeuo-radius-sm);
      font-family: 'Nunito', sans-serif;
      font-size: 0.95rem;
      color: var(--lskeuo-text-primary);
      box-shadow:
        inset 2px 2px 4px var(--lskeuo-shadow-light),
        inset 1px 1px 2px rgba(100, 80, 60, 0.1),
        inset -1px -1px 2px var(--lskeuo-highlight-soft);
      outline: none;
      transition: box-shadow var(--lskeuo-transition);
    }

    .lskeuo-input:focus {
      box-shadow:
        inset 2px 2px 4px var(--lskeuo-shadow-light),
        inset 1px 1px 2px rgba(100, 80, 60, 0.1),
        inset -1px -1px 2px var(--lskeuo-highlight-soft),
        0 0 0 3px rgba(124, 168, 200, 0.25);
    }

    .lskeuo-input::placeholder {
      color: var(--lskeuo-text-muted);
    }

    /* Progress bar */
    .lskeuo-progress-section {
      max-width: 480px;
      margin: 0 auto 2.5rem;
    }

    .lskeuo-progress-label {
      display: flex;
      justify-content: space-between;
      margin-bottom: 0.5rem;
    }

    .lskeuo-progress-label span {
      font-size: 0.8rem;
      font-weight: 600;
      color: var(--lskeuo-text-secondary);
      text-shadow: 0px 1px 0px rgba(255, 255, 250, 0.6);
    }

    .lskeuo-progress-track {
      height: 10px;
      background: var(--lskeuo-bg-pressed);
      border-radius: 5px;
      overflow: hidden;
      box-shadow:
        inset 1px 1px 3px var(--lskeuo-shadow-light),
        inset -1px -1px 2px var(--lskeuo-highlight-soft);
    }

    .lskeuo-progress-fill {
      height: 100%;
      width: 68%;
      background: var(--lskeuo-accent-coral);
      background-image: linear-gradient(
        180deg,
        rgba(255, 255, 255, 0.3) 0%,
        rgba(0, 0, 0, 0.05) 100%
      );
      border-radius: 5px;
      box-shadow:
        inset 0 1px 0px rgba(255, 255, 255, 0.3),
        1px 0 2px rgba(100, 60, 40, 0.2);
    }

    /* Footer */
    .lskeuo-footer {
      text-align: center;
      padding-top: 2rem;
      border-top: none;
    }

    .lskeuo-footer::before {
      content: '';
      display: block;
      height: 2px;
      margin-bottom: 2rem;
      box-shadow:
        inset 0 1px 1px var(--lskeuo-shadow-light),
        0 1px 0px var(--lskeuo-highlight);
    }

    .lskeuo-footer p {
      font-size: 0.85rem;
      color: var(--lskeuo-text-muted);
      text-shadow: 0px 1px 0px rgba(255, 255, 250, 0.5);
    }

    /* Responsive */
    @media (max-width: 640px) {
      .lskeuo-page { padding: 2rem 1rem; }
      .lskeuo-stats { flex-direction: column; }
      .lskeuo-grid { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <div class="lskeuo-page">

    <!-- Header -->
    <header class="lskeuo-header">
      <h1>Title Here</h1>
      <p>A warm, tactile interface built with subtle real-world object mimicry. Light and shadow create depth without heavy textures.</p>
    </header>

    <!-- Tab navigation -->
    <nav class="lskeuo-toolbar">
      <button class="lskeuo-tab active">Overview</button>
      <button class="lskeuo-tab">Details</button>
      <button class="lskeuo-tab">Settings</button>
    </nav>

    <!-- Stats row -->
    <div class="lskeuo-stats">
      <div class="lskeuo-stat">
        <span class="number">128</span>
        <span class="stat-label">Projects</span>
      </div>
      <div class="lskeuo-stat">
        <span class="number">4.8</span>
        <span class="stat-label">Rating</span>
      </div>
      <div class="lskeuo-stat">
        <span class="number">12k</span>
        <span class="stat-label">Users</span>
      </div>
    </div>

    <!-- Card grid -->
    <div class="lskeuo-grid">
      <div class="lskeuo-card">
        <div class="lskeuo-label">Feature</div>
        <h2>Raised Surfaces</h2>
        <p>Cards lift gently off the background with warm shadows falling to the bottom-right, obeying a consistent top-left light source.</p>
        <div class="lskeuo-well">
          <p>This inset well feels pressed into the card surface, creating a natural container for secondary content.</p>
        </div>
      </div>
      <div class="lskeuo-card">
        <div class="lskeuo-label">Interaction</div>
        <h2>Tactile Buttons</h2>
        <p>Buttons have clear rest, hover, and pressed states. Try clicking the buttons below to feel the physical push.</p>
        <hr class="lskeuo-groove">
        <div style="display: flex; gap: 0.8rem; flex-wrap: wrap;">
          <button class="lskeuo-button lskeuo-button--primary">Press Me</button>
          <button class="lskeuo-button lskeuo-button--secondary">Secondary</button>
        </div>
      </div>
      <div class="lskeuo-card">
        <div class="lskeuo-label">Typography</div>
        <h2>Embossed Text</h2>
        <p>Headings carry a subtle dual text-shadow that makes letterforms appear gently stamped into the surface. Clean and readable.</p>
        <hr class="lskeuo-groove">
        <p style="font-size: 0.88rem; color: var(--lskeuo-text-muted); text-shadow: 0 1px 0 rgba(255,255,250,0.7);">Warm shadows. Rounded corners. Gentle gradients. No heavy textures.</p>
      </div>
    </div>

    <!-- Input and progress -->
    <div class="lskeuo-input-group">
      <label>Search</label>
      <input type="text" class="lskeuo-input" placeholder="Type something here...">
    </div>

    <div class="lskeuo-progress-section">
      <div class="lskeuo-progress-label">
        <span>Progress</span>
        <span>68%</span>
      </div>
      <div class="lskeuo-progress-track">
        <div class="lskeuo-progress-fill"></div>
      </div>
    </div>

    <!-- Action buttons -->
    <div class="lskeuo-actions">
      <button class="lskeuo-button lskeuo-button--primary">Get Started</button>
      <button class="lskeuo-button lskeuo-button--blue">Learn More</button>
      <button class="lskeuo-button lskeuo-button--secondary">Documentation</button>
    </div>

    <!-- Footer -->
    <footer class="lskeuo-footer">
      <p>Light Skeuomorphism -- subtle physicality through light and shadow alone.</p>
    </footer>

  </div>
</body>
</html>
```
