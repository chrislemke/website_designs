# Human Scribble Aesthetic -- Design Reference

Human Scribble is the anti-AI aesthetic -- a deliberate embrace of imperfection, hand-drawn marks, and visible human authorship in an age of algorithmically generated content. Scribbles over logos, doodles on photographs, sketch-like overlays, handwritten margin notes, signature typography. Every wobble and ink blot says "a human made this." The style draws from notebook margins, whiteboard sketches, Post-it annotations, and the unselfconscious marks people leave on paper when thinking out loud. Where polished digital design strives for pixel-perfect alignment and mathematical precision, Human Scribble celebrates the warmth of a shaky hand, the charm of crossed-out corrections, and the personality embedded in someone's actual handwriting. It is a counter-movement to sterile AI-generated perfection -- asserting that imperfection is not a flaw but a signature of genuine human presence.

---

## Visual Characteristics

- **Hand-drawn scribbles on and around headings** -- wobbly lines, circles, underlines, and arrows that look sketched with a pen or marker rather than rendered by software
- **Doodle overlays on photographs and images** -- stars, hearts, arrows, speech bubbles, and abstract squiggles layered on top of imagery as if someone doodled on a printed photo
- **Sketch-like border decorations** -- borders that look drawn by hand rather than computed: uneven thickness, slightly curved lines that were meant to be straight, corner gaps
- **Handwritten annotation-style notes** -- margin comments, labels, and callouts written in a casual handwriting font, often at slight angles
- **Signature and autograph typography** -- headings and accent text in script fonts that mimic actual human signatures, with natural variation in letterforms
- **Deliberately wobbly and imperfect lines** -- SVG paths and CSS borders that include intentional irregularities, avoiding geometric precision
- **Organic blob shapes** -- containers and backgrounds using irregular border-radius values that create amoeba-like, hand-drawn-feeling silhouettes
- **Ink splatter and blot accents** -- decorative elements that resemble actual ink dropped or flicked onto paper
- **Crossed-out text with corrections** -- text with visible strikethroughs and handwritten replacements above, as if someone edited a draft in pen
- **Arrow annotations pointing to content** -- hand-drawn-style arrows with labels calling attention to specific elements, like a teacher marking up a student's work
- **Underlines that are not straight** -- wavy, sketchy underlines under important text, achieved through SVG or wavy text-decoration
- **Notebook and paper textures** -- backgrounds that evoke lined paper, graph paper, kraft paper, or torn notebook pages
- **Slight rotation on elements** -- cards, images, and text blocks tilted 1-3 degrees as if casually placed rather than grid-aligned
- **Mixed typography contrast** -- clean digital sans-serif body text alongside handwritten headings and annotations, emphasizing the human-over-machine layering
- **Warm, lived-in color temperature** -- cream backgrounds, ink-like darks, and natural accent colors that feel like real art supplies rather than hex-picker selections

---

## Color Palette

The Human Scribble palette is rooted in real-world art supplies and paper -- warm naturals, actual ink colors, and the accidental tones of pens, markers, and highlighters on imperfect paper:

- **Cream and off-white paper tones** dominate backgrounds -- not stark white (#FFFFFF) but the warm, slightly yellow cast of actual paper
- **Kraft brown** for secondary backgrounds and accent areas, evoking cardboard, packing paper, and natural materials
- **Ink black with warmth** -- not pure #000000 but a slightly brown-tinted dark that looks like real ink on paper
- **Olive and sage greens** for natural, earthy accent areas -- the green of a faded notebook cover or dried plant
- **Terracotta and warm sienna** for warm accents -- the color of brick, dried clay, or a well-worn leather journal
- **Red pen** -- the classic teacher's correction color, used sparingly for emphasis and strikethroughs
- **Blue ink** -- ballpoint pen blue for annotations and secondary handwritten elements
- **Highlighter yellow** -- bright, slightly transparent yellow for emphasis marks, as if swiped with a real highlighter
- **Charcoal gray** for softer text and secondary elements, like pencil marks on paper

### Suggested Implementation Palette

Based on characteristic real-world art supply and paper colors:

| Role               | Color            | Hex       |
|--------------------|------------------|-----------|
| Paper Light        | Warm Cream       | `#FBF7F0` |
| Paper Mid          | Parchment        | `#F5EDE0` |
| Paper Dark         | Aged Cream       | `#EDE3D2` |
| Kraft              | Kraft Brown      | `#C4A97D` |
| Ink Primary        | Warm Black       | `#2A2520` |
| Ink Secondary      | Charcoal         | `#4A4540` |
| Text Body          | Dark Brown       | `#3D3530` |
| Accent Olive       | Sage Green       | `#7D8C64` |
| Accent Terracotta  | Warm Sienna      | `#C47D5A` |
| Accent Red         | Red Pen          | `#D45040` |
| Accent Blue        | Ballpoint Blue   | `#4A6FA5` |
| Accent Yellow      | Highlighter      | `#FFE066` |
| Accent Coral       | Soft Coral       | `#E8927C` |
| Border Sketch      | Pencil Gray      | `#9E9588` |
| Shadow             | Warm Shadow      | `#D5CBBC` |
| Doodle Ink         | Marker Dark      | `#35302B` |

### Suggested CSS Custom Properties

```css
:root {
  /* Paper backgrounds */
  --scribble-paper-light: #FBF7F0;
  --scribble-paper-mid: #F5EDE0;
  --scribble-paper-dark: #EDE3D2;
  --scribble-kraft: #C4A97D;

  /* Ink and text */
  --scribble-ink: #2A2520;
  --scribble-ink-soft: #4A4540;
  --scribble-text-body: #3D3530;
  --scribble-text-muted: #7A7168;
  --scribble-pencil: #9E9588;

  /* Accent colors -- art supply palette */
  --scribble-olive: #7D8C64;
  --scribble-terracotta: #C47D5A;
  --scribble-red-pen: #D45040;
  --scribble-blue-ink: #4A6FA5;
  --scribble-highlighter: #FFE066;
  --scribble-coral: #E8927C;

  /* Shadows and depth */
  --scribble-shadow: #D5CBBC;
  --scribble-shadow-soft: rgba(42, 37, 32, 0.08);
  --scribble-shadow-medium: rgba(42, 37, 32, 0.15);

  /* Functional mappings */
  --scribble-bg-primary: var(--scribble-paper-light);
  --scribble-bg-secondary: var(--scribble-paper-mid);
  --scribble-bg-card: var(--scribble-paper-dark);
  --scribble-text-heading: var(--scribble-ink);
  --scribble-text-primary: var(--scribble-text-body);
  --scribble-accent-primary: var(--scribble-terracotta);
  --scribble-accent-secondary: var(--scribble-olive);
  --scribble-border: var(--scribble-pencil);
}
```

---

## Typography

### Typeface Characteristics

Human Scribble typography is defined by the contrast between hand-drawn and machine-set text -- the juxtaposition is the entire point:

- **Handwritten headings** -- primary headings use script or casual handwriting fonts that look like real human writing, with natural variation in stroke width, baseline, and letter spacing
- **Signature-style accent text** -- key phrases, pull quotes, and names rendered in flowing script fonts that evoke actual signatures and autographs
- **Marker and brush fonts** -- bolder headings and emphasis text in fonts that simulate thick markers or brush pens, with visible stroke texture
- **Clean sans-serif body text** -- paragraphs and long-form content use readable, modern sans-serif fonts, creating deliberate contrast with the handwritten elements
- **The contrast is the message** -- clean body text says "this is the content," while handwritten overlays say "a person was here, reacting to it"
- **Varied baselines and sizes** -- handwritten text does not sit on a perfect baseline; slight wobble and size variation increases authenticity
- **Mixed within single compositions** -- a heading might combine a clean sans-serif word with a handwritten annotation or correction layered on top
- **Casual, not calligraphic** -- the target is everyday handwriting and quick sketches, not formal calligraphy or elaborate lettering

### Recommended Web Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Caveat** | Casual handwriting | Primary handwritten headings, annotations, margin notes |
| **Patrick Hand** | Neat casual handwriting | Section headings, labels, longer handwritten passages |
| **Indie Flower** | Loose, playful handwriting | Doodle labels, fun annotations, informal callouts |
| **Dancing Script** | Flowing signature script | Signature-style accent text, pull quotes, author names |
| **Satisfy** | Brush script | Elegant handwritten accents, featured quotes |
| **Permanent Marker** | Thick marker/felt-tip | Bold emphasis headings, highlighted labels, shout-outs |
| **Inter** | Clean geometric sans-serif | Primary body text, structured content, data |
| **DM Sans** | Friendly geometric sans-serif | Secondary body text, UI labels, captions |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Caveat:wght@400;700&family=Patrick+Hand&family=Indie+Flower&family=Dancing+Script:wght@400;700&family=Permanent+Marker&family=Inter:wght@400;500;600&family=DM+Sans:wght@400;500&display=swap');

/* Primary body text -- clean, readable, modern */
body {
  font-family: 'Inter', 'DM Sans', -apple-system, sans-serif;
  font-size: 17px;
  line-height: 1.7;
  letter-spacing: -0.01em;
  color: var(--scribble-text-body);
}

/* Handwritten headings -- the human touch */
h1, h2, h3 {
  font-family: 'Caveat', 'Patrick Hand', cursive;
  color: var(--scribble-ink);
  letter-spacing: 0.01em;
  line-height: 1.3;
  font-weight: 700;
}

h1 {
  font-size: clamp(2.5rem, 6vw, 4rem);
  transform: rotate(-1deg);
}

h2 {
  font-size: clamp(1.8rem, 4vw, 2.8rem);
  color: var(--scribble-ink-soft);
  transform: rotate(0.5deg);
}

h3 {
  font-family: 'Patrick Hand', 'Caveat', cursive;
  font-size: clamp(1.4rem, 3vw, 2rem);
  color: var(--scribble-terracotta);
}

/* Signature-style accent text */
.scribble-signature {
  font-family: 'Dancing Script', 'Satisfy', cursive;
  font-size: 1.6rem;
  color: var(--scribble-blue-ink);
  transform: rotate(-2deg);
  display: inline-block;
}

/* Marker emphasis */
.scribble-marker {
  font-family: 'Permanent Marker', cursive;
  font-size: 1.3rem;
  color: var(--scribble-red-pen);
  letter-spacing: 0.02em;
}

/* Margin annotation */
.scribble-note {
  font-family: 'Indie Flower', 'Caveat', cursive;
  font-size: 1rem;
  color: var(--scribble-blue-ink);
  transform: rotate(-1.5deg);
  display: inline-block;
}

/* Body text paragraphs */
p {
  margin-bottom: 1.2rem;
  color: var(--scribble-text-body);
}

/* Small labels and captions */
.scribble-caption {
  font-family: 'DM Sans', sans-serif;
  font-size: 0.85rem;
  color: var(--scribble-text-muted);
  letter-spacing: 0.02em;
}
```

---

## Key Design Elements and Motifs

### Hand-Drawn Borders and Frames

The defining decorative element -- borders that look sketched by hand rather than rendered by a computer:

- **Wobbly rectangular borders** using SVG paths with slight irregularities in the line, simulating a pen drawn freehand along a ruler's edge
- **Double-line sketch borders** -- two slightly offset imperfect lines creating a casual frame, as if drawn quickly
- **Corner flourishes** -- small doodle marks (stars, crosses, circles) at border corners instead of precise right angles
- **Torn-edge effects** -- borders that look like torn paper edges, achieved through irregular SVG clip-paths
- **Incomplete borders** -- lines that do not quite meet at corners, or that trail off, suggesting a quick sketch
- **Variable stroke width** -- border paths that vary in thickness along their length, mimicking real pen pressure

### Doodle Overlays

- **Stars, hearts, arrows, and squiggles** scattered around headings and images as decorative elements
- **Speech bubbles and thought clouds** drawn in a sketchy style for callouts and quotes
- **Underline scribbles** -- multiple quick lines under important words, like emphatic underlining in a notebook
- **Circle-and-arrow annotations** -- elements circled with a wobbly line and an arrow pointing to a label, like a teacher marking up a document
- **Abstract squiggles and swirls** used as section dividers or decorative fills
- **Checkbox-style list markers** -- hand-drawn checkboxes, some checked with a casual tick mark

### Crossed-Out Corrections

- **Strikethrough text with handwritten replacement** -- original text crossed out (not neatly, but with a scribbled line) and new text written above in a handwriting font
- **Editing marks** -- carets, insertion marks, and marginal additions that mimic the look of a hand-edited manuscript
- **"Oops" corrections** -- visible mistakes that have been scribbled over, conveying authenticity and process

### Ink Blots and Splatter

- **Small ink spots** placed near text as if a pen dripped -- decorative accent marks
- **Splatter patterns** used as background textures or section transitions
- **Watercolor-style washes** -- semi-transparent color areas with irregular, organic edges

### Sticky Notes and Paper Scraps

- **Sticky note callouts** -- elements styled as yellow or pastel Post-it notes, slightly rotated and overlapping content
- **Torn paper fragments** -- content sections styled as scraps of paper with irregular edges, pinned or taped to the page
- **Notebook page backgrounds** -- lined or grid paper textures behind content areas
- **Tape and pin decorations** -- small decorative elements suggesting content is taped or pinned to a surface

### Arrow Annotations

- **Curved hand-drawn arrows** pointing from labels to content areas
- **Arrows with handwritten labels** -- "look here!", "important!", "this one" -- in a casual handwriting font
- **Looping, playful arrow paths** that curve and double back, not straight mechanical lines

---

## Layout Principles

- **Warm paper background** -- the entire page sits on a cream or off-white base that feels like paper, not a screen
- **Intentionally imperfect alignment** -- elements are placed with slight rotations (1-3 degrees) and offsets, avoiding the rigid grid feel of typical web layouts
- **Layered composition** -- doodles, annotations, and decorative marks are layered over structured content, creating depth between the "typed" layer and the "hand-drawn" layer
- **Generous whitespace** -- like a notebook page, content does not fill every available pixel; breathing room suggests a human laid this out casually
- **Mixed media zones** -- areas of clean typography adjacent to areas of handwritten text and doodles, creating visual rhythm through contrast
- **Margin annotations** -- important notes and callouts positioned in margins or overlapping content edges, like real margin notes
- **Organic grouping** -- related content grouped by proximity and visual connection (arrows, circles) rather than rigid grid cells
- **Vertical rhythm through variety** -- sections alternate between structured (clean text blocks) and loose (doodled, annotated, tilted) to maintain interest
- **Sticky note and scrap overlays** -- secondary content presented on "stuck-on" elements that break the grid
- **Bottom-heavy compositions** -- signatures, dates, and personal marks anchored at the bottom, like a signed letter

### Modern Web Adaptation

- Use **CSS Grid or Flexbox** for underlying structure, then apply **slight rotations and offsets** to individual elements to break the mechanical feel
- **Paper texture backgrounds** via subtle CSS gradients or background-image with a paper texture
- **SVG doodle elements** positioned absolutely over content for the hand-drawn overlay layer
- **Mix of font stacks** -- handwriting fonts for headings and annotations, clean sans-serif for body text
- **CSS `transform: rotate()`** on cards, images, and callouts for the imperfect-placement feel
- **Organic `border-radius`** values on containers (e.g., `60% 40% 50% 50% / 40% 60% 50% 50%`) for blob-like shapes
- **Wavy text-decoration** and SVG underlines instead of straight `border-bottom` for emphasis
- **Max-width containers** (700-900px) centered on the page for a comfortable reading width, like a notebook page

---

## CSS/Design Techniques

### SVG Hand-Drawn Border

```css
/* Hand-drawn border using an inline SVG as border-image.
   The SVG path has intentional wobble to simulate a pen-drawn rectangle. */
.scribble-border {
  border: none;
  padding: 2rem;
  position: relative;
}

.scribble-border::before {
  content: '';
  position: absolute;
  inset: 0;
  /* SVG with a wobbly rectangle path */
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25'%3E%3Crect x='4' y='4' width='calc(100%25-8)' height='calc(100%25-8)' rx='2' ry='2' fill='none' stroke='%232A2520' stroke-width='2' stroke-dasharray='none' stroke-linecap='round' style='filter:url(%23wobble)'/%3E%3C/svg%3E");
  pointer-events: none;
}

/* Alternative: use an SVG background with a hand-drawn-feel path */
.scribble-border-svg {
  padding: 2rem;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 200' preserveAspectRatio='none'%3E%3Cpath d='M4,4 C4,2 8,4 40,3 C80,2 120,5 160,3 C190,2 196,4 196,4 C198,4 196,8 197,40 C198,80 195,120 197,160 C198,190 196,196 196,196 C196,198 192,196 160,197 C120,198 80,195 40,197 C10,198 4,196 4,196 C2,196 4,192 3,160 C2,120 5,80 3,40 C2,10 4,4 4,4Z' fill='none' stroke='%232A2520' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
  background-size: 100% 100%;
  background-repeat: no-repeat;
}
```

### Wavy / Sketchy Underlines

```css
/* Native CSS wavy underline */
.scribble-underline-wavy {
  text-decoration: underline wavy var(--scribble-red-pen);
  text-decoration-thickness: 1.5px;
  text-underline-offset: 4px;
}

/* SVG-based hand-drawn underline for more organic feel */
.scribble-underline-svg {
  text-decoration: none;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='8' viewBox='0 0 200 8'%3E%3Cpath d='M0,5 C10,3 20,7 30,5 C40,3 50,6 60,5 C70,3 80,7 90,4 C100,2 110,6 120,5 C130,3 140,7 150,4 C160,2 170,6 180,5 C190,3 200,6 200,5' fill='none' stroke='%23D45040' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
  background-position: 0 100%;
  background-repeat: repeat-x;
  background-size: 200px 8px;
  padding-bottom: 6px;
}

/* Multiple scribble lines (emphatic underline) */
.scribble-underline-emphatic {
  text-decoration: none;
  background-image:
    url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='12' viewBox='0 0 200 12'%3E%3Cpath d='M0,4 C15,2 30,6 50,4 C70,2 90,6 110,3 C130,1 150,5 170,4 C185,3 195,5 200,4' fill='none' stroke='%232A2520' stroke-width='1.2' stroke-linecap='round'/%3E%3Cpath d='M0,8 C20,6 35,10 55,8 C75,6 95,10 115,7 C135,5 155,9 175,8 C190,7 198,9 200,8' fill='none' stroke='%232A2520' stroke-width='1.2' stroke-linecap='round'/%3E%3C/svg%3E");
  background-position: 0 100%;
  background-repeat: repeat-x;
  background-size: 200px 12px;
  padding-bottom: 10px;
}

/* Highlighter-style mark */
.scribble-highlight {
  background: linear-gradient(
    to bottom,
    transparent 40%,
    rgba(255, 224, 102, 0.45) 40%,
    rgba(255, 224, 102, 0.45) 85%,
    transparent 85%
  );
  padding: 0 4px;
}
```

### Organic Blob Shapes

```css
/* Organic blob container -- asymmetric border-radius creates a hand-drawn feel */
.scribble-blob {
  border-radius: 60% 40% 50% 50% / 40% 60% 50% 50%;
  background: var(--scribble-paper-dark);
  padding: 3rem;
  position: relative;
}

/* Variation: more irregular blob */
.scribble-blob--irregular {
  border-radius: 30% 70% 55% 45% / 55% 30% 70% 45%;
  background: var(--scribble-olive);
  color: var(--scribble-paper-light);
  padding: 2rem 2.5rem;
}

/* Animated blob that gently shifts shape */
@keyframes scribble-blob-morph {
  0%   { border-radius: 60% 40% 50% 50% / 40% 60% 50% 50%; }
  25%  { border-radius: 45% 55% 60% 40% / 55% 45% 40% 60%; }
  50%  { border-radius: 50% 50% 40% 60% / 60% 40% 55% 45%; }
  75%  { border-radius: 40% 60% 55% 45% / 45% 55% 60% 40%; }
  100% { border-radius: 60% 40% 50% 50% / 40% 60% 50% 50%; }
}

.scribble-blob--animated {
  animation: scribble-blob-morph 8s ease-in-out infinite;
}

/* Blob used as a background accent */
.scribble-blob-accent {
  position: absolute;
  width: 200px;
  height: 200px;
  border-radius: 55% 45% 60% 40% / 45% 55% 40% 60%;
  background: rgba(125, 140, 100, 0.12);
  z-index: 0;
  pointer-events: none;
}
```

### Imperfect Rotation and Placement

```css
/* Slight rotation on elements for the "casually placed" feel */
.scribble-tilt-left {
  transform: rotate(-1.5deg);
}

.scribble-tilt-right {
  transform: rotate(1.2deg);
}

.scribble-tilt-subtle {
  transform: rotate(-0.5deg);
}

/* Randomized tilt using nth-child for lists/grids */
.scribble-tilt-vary > *:nth-child(4n+1) { transform: rotate(-1.2deg); }
.scribble-tilt-vary > *:nth-child(4n+2) { transform: rotate(0.8deg); }
.scribble-tilt-vary > *:nth-child(4n+3) { transform: rotate(-0.5deg); }
.scribble-tilt-vary > *:nth-child(4n+4) { transform: rotate(1.5deg); }

/* Hover: straighten up (the "picked up" effect) */
.scribble-tilt-interactive {
  transform: rotate(-1.5deg);
  transition: transform 0.3s ease;
}

.scribble-tilt-interactive:hover {
  transform: rotate(0deg) scale(1.02);
}
```

### Sticky Note Callout

```css
/* Post-it note style element */
.scribble-sticky {
  background: var(--scribble-highlighter);
  padding: 1.5rem;
  font-family: 'Caveat', cursive;
  font-size: 1.2rem;
  color: var(--scribble-ink);
  transform: rotate(-2deg);
  box-shadow:
    2px 3px 8px var(--scribble-shadow-medium),
    inset 0 -2px 4px rgba(0, 0, 0, 0.04);
  position: relative;
  max-width: 280px;
  line-height: 1.5;
}

/* Tape effect on top */
.scribble-sticky::before {
  content: '';
  position: absolute;
  top: -8px;
  left: 50%;
  transform: translateX(-50%) rotate(1deg);
  width: 60px;
  height: 16px;
  background: rgba(255, 255, 255, 0.6);
  border: 1px solid rgba(0, 0, 0, 0.06);
}

/* Color variants */
.scribble-sticky--blue {
  background: #D4E4F7;
}

.scribble-sticky--pink {
  background: #F7D4DC;
}

.scribble-sticky--green {
  background: #D4EDDA;
}
```

### Notebook Paper Background

```css
/* Lined notebook paper */
.scribble-lined-paper {
  background-color: var(--scribble-paper-light);
  background-image:
    linear-gradient(
      transparent 0px,
      transparent 31px,
      var(--scribble-shadow) 31px,
      var(--scribble-shadow) 32px
    );
  background-size: 100% 32px;
  background-position: 0 8px;
  padding: 0.5rem 1.5rem 0.5rem 4rem;
  position: relative;
}

/* Red margin line */
.scribble-lined-paper::before {
  content: '';
  position: absolute;
  left: 3.2rem;
  top: 0;
  bottom: 0;
  width: 1px;
  background: var(--scribble-red-pen);
  opacity: 0.4;
}

/* Graph paper variant */
.scribble-graph-paper {
  background-color: var(--scribble-paper-light);
  background-image:
    linear-gradient(var(--scribble-shadow) 1px, transparent 1px),
    linear-gradient(90deg, var(--scribble-shadow) 1px, transparent 1px);
  background-size: 24px 24px;
}

/* Kraft paper texture */
.scribble-kraft {
  background-color: var(--scribble-kraft);
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100' height='100'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.06'/%3E%3C/svg%3E");
}
```

### Crossed-Out Correction Text

```css
/* Crossed-out word with handwritten correction above */
.scribble-correction {
  position: relative;
  display: inline-block;
}

.scribble-correction .original {
  text-decoration: line-through;
  text-decoration-color: var(--scribble-red-pen);
  text-decoration-thickness: 2px;
  color: var(--scribble-text-muted);
  text-decoration-style: wavy;
}

.scribble-correction .replacement {
  position: absolute;
  top: -1.3em;
  left: 0;
  font-family: 'Caveat', cursive;
  font-size: 1.1em;
  color: var(--scribble-red-pen);
  white-space: nowrap;
  transform: rotate(-2deg);
}

/* Inline strikethrough with different scribble intensity */
.scribble-strike-light {
  text-decoration: line-through;
  text-decoration-color: var(--scribble-pencil);
  text-decoration-thickness: 1px;
}

.scribble-strike-heavy {
  text-decoration: line-through;
  text-decoration-color: var(--scribble-ink);
  text-decoration-thickness: 3px;
  text-decoration-style: wavy;
}
```

### Hand-Drawn Arrow Annotation

```css
/* Arrow annotation container */
.scribble-arrow-note {
  position: relative;
  display: inline-block;
}

/* SVG arrow pointing down-right, used as a before pseudo-element */
.scribble-arrow-note::before {
  content: '';
  position: absolute;
  top: -30px;
  left: -20px;
  width: 50px;
  height: 40px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='50' height='40' viewBox='0 0 50 40'%3E%3Cpath d='M5,5 C10,8 20,12 30,20 C35,24 38,28 42,32' fill='none' stroke='%23D45040' stroke-width='2' stroke-linecap='round'/%3E%3Cpath d='M36,28 L42,32 L38,26' fill='none' stroke='%23D45040' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
  background-size: contain;
  background-repeat: no-repeat;
  pointer-events: none;
}

/* Label for the arrow annotation */
.scribble-arrow-label {
  font-family: 'Caveat', cursive;
  font-size: 1rem;
  color: var(--scribble-red-pen);
  transform: rotate(-5deg);
  display: inline-block;
  position: absolute;
  top: -50px;
  left: -40px;
  white-space: nowrap;
}
```

### Doodle-Style List Markers

```css
/* Replace standard bullets with hand-drawn marks */
.scribble-list {
  list-style: none;
  padding-left: 2rem;
}

.scribble-list li {
  position: relative;
  margin-bottom: 0.8rem;
  padding-left: 0.5rem;
}

/* Hand-drawn checkbox marker */
.scribble-list li::before {
  content: '';
  position: absolute;
  left: -1.5rem;
  top: 0.3em;
  width: 14px;
  height: 14px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='14' height='14' viewBox='0 0 14 14'%3E%3Crect x='1' y='1' width='12' height='12' rx='1' fill='none' stroke='%234A4540' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
  background-size: contain;
  background-repeat: no-repeat;
}

/* Checked item */
.scribble-list li.checked::before {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='14' height='14' viewBox='0 0 14 14'%3E%3Crect x='1' y='1' width='12' height='12' rx='1' fill='none' stroke='%234A4540' stroke-width='1.5'/%3E%3Cpath d='M3,7 L6,10 L11,4' fill='none' stroke='%23D45040' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
}

/* Star bullet variant */
.scribble-list--stars li::before {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='14' height='14' viewBox='0 0 14 14'%3E%3Cpath d='M7,1 L8.5,5 L13,5.5 L9.5,8.5 L10.5,13 L7,10.5 L3.5,13 L4.5,8.5 L1,5.5 L5.5,5Z' fill='none' stroke='%23C47D5A' stroke-width='1.2' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
}

/* Arrow bullet variant */
.scribble-list--arrows li::before {
  width: 16px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='14' viewBox='0 0 16 14'%3E%3Cpath d='M2,7 C4,7 8,7 12,7' fill='none' stroke='%234A6FA5' stroke-width='1.5' stroke-linecap='round'/%3E%3Cpath d='M9,4 L12,7 L9,10' fill='none' stroke='%234A6FA5' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
}
```

### Card / Content Panel

```css
/* Scribble-style content card */
.scribble-card {
  background: var(--scribble-paper-dark);
  padding: 2rem;
  position: relative;
  transform: rotate(-0.5deg);
  box-shadow: 3px 4px 12px var(--scribble-shadow-medium);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

/* Hand-drawn border via SVG */
.scribble-card::before {
  content: '';
  position: absolute;
  inset: -2px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 200' preserveAspectRatio='none'%3E%3Cpath d='M3,5 C3,3 7,3 40,4 C80,3 120,5 160,4 C192,3 197,5 197,5 C199,5 197,7 196,40 C197,80 196,120 197,160 C198,192 196,197 196,197 C196,199 192,197 160,196 C120,197 80,196 40,197 C8,198 3,196 3,196 C1,196 3,192 4,160 C3,120 4,80 3,40 C2,8 3,5 3,5Z' fill='none' stroke='%232A2520' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
  background-size: 100% 100%;
  background-repeat: no-repeat;
  pointer-events: none;
}

/* Hover: straighten slightly and lift */
.scribble-card:hover {
  transform: rotate(0deg) translateY(-2px);
  box-shadow: 4px 6px 16px var(--scribble-shadow-medium);
}

/* Card with tape decoration */
.scribble-card--taped {
  position: relative;
}

.scribble-card--taped::after {
  content: '';
  position: absolute;
  top: -6px;
  right: 20px;
  width: 50px;
  height: 18px;
  background: rgba(255, 255, 255, 0.5);
  border: 1px solid rgba(0, 0, 0, 0.05);
  transform: rotate(3deg);
}
```

### Button

```css
/* Hand-drawn style button */
.scribble-button {
  display: inline-block;
  padding: 0.7rem 2rem;
  background: var(--scribble-paper-light);
  color: var(--scribble-ink);
  font-family: 'Patrick Hand', 'Caveat', cursive;
  font-size: 1.15rem;
  text-decoration: none;
  cursor: pointer;
  border: none;
  position: relative;
  transform: rotate(-0.5deg);
  transition: transform 0.2s ease;
}

/* SVG hand-drawn border */
.scribble-button::before {
  content: '';
  position: absolute;
  inset: -2px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 60' preserveAspectRatio='none'%3E%3Cpath d='M4,4 C4,2 10,4 50,3 C100,2 150,5 190,3 C196,2 197,4 197,6 C198,10 196,20 197,30 C198,40 196,50 197,55 C198,57 196,58 190,57 C150,58 100,56 50,57 C10,58 4,57 3,56 C2,55 3,45 4,30 C3,15 4,6 4,4Z' fill='none' stroke='%232A2520' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");
  background-size: 100% 100%;
  background-repeat: no-repeat;
  pointer-events: none;
}

.scribble-button:hover {
  transform: rotate(0deg) scale(1.03);
  background: var(--scribble-paper-mid);
}

.scribble-button:active {
  transform: rotate(0.5deg) scale(0.98);
}

/* Filled accent button */
.scribble-button--accent {
  background: var(--scribble-terracotta);
  color: var(--scribble-paper-light);
}

.scribble-button--accent::before {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 60' preserveAspectRatio='none'%3E%3Cpath d='M4,4 C4,2 10,4 50,3 C100,2 150,5 190,3 C196,2 197,4 197,6 C198,10 196,20 197,30 C198,40 196,50 197,55 C198,57 196,58 190,57 C150,58 100,56 50,57 C10,58 4,57 3,56 C2,55 3,45 4,30 C3,15 4,6 4,4Z' fill='none' stroke='%23FBF7F0' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");
}
```

### Ink Splatter Decoration

```css
/* Decorative ink splatter using radial gradients */
.scribble-splatter {
  position: relative;
}

.scribble-splatter::after {
  content: '';
  position: absolute;
  width: 80px;
  height: 80px;
  top: -20px;
  right: -15px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='80' height='80' viewBox='0 0 80 80'%3E%3Ccircle cx='40' cy='40' r='6' fill='%232A2520' opacity='0.7'/%3E%3Ccircle cx='50' cy='35' r='3' fill='%232A2520' opacity='0.5'/%3E%3Ccircle cx='32' cy='48' r='2.5' fill='%232A2520' opacity='0.6'/%3E%3Ccircle cx='55' cy='45' r='1.5' fill='%232A2520' opacity='0.4'/%3E%3Ccircle cx='28' cy='35' r='2' fill='%232A2520' opacity='0.5'/%3E%3Ccircle cx='45' cy='52' r='1' fill='%232A2520' opacity='0.4'/%3E%3Ccircle cx='37' cy='30' r='1.5' fill='%232A2520' opacity='0.35'/%3E%3C/svg%3E");
  background-size: contain;
  background-repeat: no-repeat;
  pointer-events: none;
  z-index: 2;
}
```

### Section Divider (Sketchy Line)

```css
/* Hand-drawn horizontal rule */
.scribble-divider {
  border: none;
  height: 8px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='8' viewBox='0 0 400 8'%3E%3Cpath d='M0,4 C20,2 40,6 60,4 C80,2 100,5 120,4 C140,3 160,6 180,4 C200,2 220,5 240,3 C260,2 280,6 300,4 C320,2 340,5 360,4 C380,3 395,5 400,4' fill='none' stroke='%239E9588' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-position: center;
  background-size: 400px 8px;
  margin: 2.5rem 0;
}

/* Divider with small doodle in center */
.scribble-divider--doodle {
  border: none;
  height: 24px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='24' viewBox='0 0 400 24'%3E%3Cpath d='M0,12 C40,10 80,14 160,12' fill='none' stroke='%239E9588' stroke-width='1' stroke-linecap='round'/%3E%3Cpath d='M240,12 C300,10 340,14 400,12' fill='none' stroke='%239E9588' stroke-width='1' stroke-linecap='round'/%3E%3Cpath d='M185,6 L200,18 L215,6' fill='none' stroke='%23C47D5A' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 24px;
  margin: 2.5rem 0;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical / Stationery Reference | Web Equivalent |
|--------------------------------|----------------|
| Cream/off-white notebook paper | Warm background color (`#FBF7F0`) with subtle CSS noise texture or grain overlay |
| Lined notebook page | `repeating-linear-gradient` creating horizontal ruled lines at regular intervals |
| Graph/grid paper | Two-axis `linear-gradient` creating a light grid pattern |
| Kraft / brown packing paper | Warm brown background (`#C4A97D`) with SVG fractal noise for fiber texture |
| Pen ink on paper | Dark brown-black text (`#2A2520`) in handwriting fonts with slight variation |
| Ballpoint pen annotations | Blue ink color (`#4A6FA5`) in italic or script fonts at slight angles |
| Red pen corrections | Red accent (`#D45040`) for strikethroughs, underlines, and margin marks |
| Highlighter marker | Semi-transparent yellow (`rgba(255, 224, 102, 0.45)`) background behind text |
| Adhesive tape | Semi-transparent white rectangle with subtle border, rotated slightly |
| Pushpin / thumbtack | Small radial gradient circle with shadow, positioned at element corner |
| Torn paper edge | Irregular SVG `clip-path` polygon along one or more edges |
| Ink splatter / blots | SVG circles of varying size and opacity clustered in organic arrangements |
| Pencil sketch lines | Light gray strokes (`#9E9588`) with slight irregularity in SVG paths |
| Whiteboard marker | Thick strokes in bold color with rounded ends and slight transparency |
| Washi tape strip | Colored semi-transparent rectangle with patterned background, rotated |
| Notebook spiral binding | Repeating SVG circles along the left edge of a container |

---

## Imagery and Visual Content Guidelines

When creating or sourcing imagery for a Human Scribble styled site:

- **Layer hand-drawn elements over photography** -- add SVG scribbles, arrows, circles, and doodles on top of photos to create the annotation effect
- **Use warm, naturally-lit photographs** -- candid shots, natural light, slightly desaturated or warm-filtered images that feel approachable
- **Favor imperfect, candid compositions** -- avoid overly polished stock photography; images should feel personal and unstaged
- **Mix media types** -- combine photographs with hand-drawn illustrations, sketches alongside screenshots, collage-style compositions
- **Apply paper textures as overlays** -- subtle paper grain or noise over images softens the digital feel
- **Avoid AI-generated imagery** -- the entire point of this aesthetic is asserting human authorship; AI-generated images contradict the message
- **Scan real sketches and handwriting** -- authentic scanned doodles and notes, even rough ones, carry more visual truth than digitally drawn equivalents
- **Use visible brush strokes and pen marks** -- illustrations should show the tool that made them, whether pen, marker, brush, or pencil
- **Polaroid and snapshot framing** -- images presented with white borders, slight tilt, and casual placement as if scattered on a desk
- **Include "making of" elements** -- show drafts, sketches, notes, and process artifacts alongside finished content to reinforce the human-made narrative
- **Muted, warm color grading** -- images should lean warm (cream, amber, soft brown) rather than cool or hyper-saturated
- **Handwritten labels on images** -- captions and labels in handwriting fonts positioned at angles over or near images, connected by hand-drawn arrows

---

## Related Aesthetics

| Aesthetic | Relationship to Human Scribble |
|-----------|-------------------------------|
| **Cottagecore** | Shares warmth, handmade quality, and natural materials -- Cottagecore is the domestic/rural expression, Human Scribble is the graphic/annotation expression of the same impulse toward the handmade |
| **Craftcore** | Overlapping emphasis on visible human craft and imperfection -- Craftcore celebrates the process of making, Human Scribble celebrates the marks left by human hands |
| **DIY Punk** | Shares the anti-polished, hand-made ethos -- DIY Punk is angrier and more subversive, while Human Scribble is warmer and more inviting, but both reject digital perfection |
| **Corporate Grunge** | Both react against sterile corporate design, but Corporate Grunge uses decay and distortion while Human Scribble uses warmth and hand-drawn marks |
| **Cluttercore** | Shares the embrace of imperfection and accumulation -- Cluttercore fills space maximally, while Human Scribble layers annotations and marks over cleaner content |
| **Dadaism** | Historical precedent for anti-establishment, anti-perfection design -- Dada's collage and randomness echo in Human Scribble's layered annotations, though Scribble is less chaotic |

---

## Implementation Notes

- The Human Scribble aesthetic is **warm and inviting**, not messy or chaotic. The goal is visible human presence, not visual disorder. Every scribble and doodle should feel intentional, as if placed by a thoughtful person, not randomly generated.
- **Contrast between clean and hand-drawn is essential** -- without the clean sans-serif body text underneath, the handwritten overlays lose their meaning. The aesthetic depends on the tension between machine-precise content and human-imprecise annotation. Removing either layer breaks the effect.
- **Imperfection must be designed** -- paradoxically, achieving the "imperfect" look requires careful design choices. Rotations should be subtle (0.5-3 degrees), wobbles gentle, and doodles purposeful. Over-rotating or over-scribbling becomes distracting rather than charming.
- **SVG is your primary tool** -- CSS alone cannot produce convincingly hand-drawn lines. Inline SVG paths with deliberate irregularities in their control points create the organic, human quality. Prepare a library of reusable SVG elements: wobbly borders, arrows, underlines, checkmarks, stars, speech bubbles.
- **Performance consideration** -- inline SVGs in CSS `background-image` or `border-image` can be heavy. Use `url("data:image/svg+xml,...")` for small elements and external `.svg` files for larger decorative pieces. Optimize SVG paths to minimize file size.
- **Accessibility is critical** -- handwriting fonts are harder to read than standard typefaces, especially for users with dyslexia or visual impairments. Use handwriting fonts only for headings, short labels, and decorative text. All body content must use a clean, readable font. Ensure sufficient color contrast between ink-colored text and paper backgrounds.
- **Do not use this aesthetic to disguise AI-generated content** -- the entire philosophical foundation is human authenticity. Using the visual language of human craft to present machine-generated material is contradictory and dishonest.
- **Touch and cursor interactions** should feel analog -- hover effects that gently straighten tilted elements (as if picking up a piece of paper), click effects that press down slightly, transitions that feel physical rather than digital.
- **Color restraint matters** -- limit accent colors to 2-3 per view. Real notebooks and annotated documents use one or two pen colors, not a rainbow. Too many colors breaks the illusion of a single person's markings.

---

## Quick-Start: Minimal Human Scribble Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Human Scribble Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400;700&family=Patrick+Hand&family=Indie+Flower&family=Dancing+Script:wght@400;700&family=Permanent+Marker&family=Inter:wght@400;500;600&family=DM+Sans:wght@400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --scribble-paper-light: #FBF7F0;
      --scribble-paper-mid: #F5EDE0;
      --scribble-paper-dark: #EDE3D2;
      --scribble-kraft: #C4A97D;
      --scribble-ink: #2A2520;
      --scribble-ink-soft: #4A4540;
      --scribble-text-body: #3D3530;
      --scribble-text-muted: #7A7168;
      --scribble-pencil: #9E9588;
      --scribble-olive: #7D8C64;
      --scribble-terracotta: #C47D5A;
      --scribble-red-pen: #D45040;
      --scribble-blue-ink: #4A6FA5;
      --scribble-highlighter: #FFE066;
      --scribble-coral: #E8927C;
      --scribble-shadow: #D5CBBC;
      --scribble-shadow-soft: rgba(42, 37, 32, 0.08);
      --scribble-shadow-medium: rgba(42, 37, 32, 0.15);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--scribble-paper-light);
      color: var(--scribble-text-body);
      font-family: 'Inter', 'DM Sans', -apple-system, sans-serif;
      font-size: 17px;
      line-height: 1.7;
      min-height: 100vh;
      overflow-x: hidden;
    }

    /* Subtle lined-paper background */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image:
        linear-gradient(
          transparent 0px,
          transparent 31px,
          var(--scribble-shadow) 31px,
          var(--scribble-shadow) 32px
        );
      background-size: 100% 32px;
      opacity: 0.25;
      pointer-events: none;
      z-index: 0;
    }

    /* Page container */
    .scribble-page {
      max-width: 820px;
      margin: 0 auto;
      padding: 3rem 2.5rem;
      position: relative;
      z-index: 1;
    }

    /* Red margin line */
    .scribble-page::before {
      content: '';
      position: fixed;
      left: calc(50% - 410px + 2.5rem);
      top: 0;
      bottom: 0;
      width: 1px;
      background: var(--scribble-red-pen);
      opacity: 0.2;
      z-index: 0;
    }

    /* Hero heading -- big, handwritten, slightly tilted */
    h1 {
      font-family: 'Caveat', cursive;
      font-size: clamp(2.8rem, 7vw, 4.5rem);
      font-weight: 700;
      color: var(--scribble-ink);
      line-height: 1.2;
      transform: rotate(-1.5deg);
      margin-bottom: 0.5rem;
      position: relative;
      display: inline-block;
    }

    /* Sketchy underline on h1 */
    h1::after {
      content: '';
      display: block;
      height: 8px;
      margin-top: 4px;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='8' viewBox='0 0 300 8'%3E%3Cpath d='M0,5 C15,3 30,7 45,5 C60,3 75,6 90,5 C105,3 120,7 135,4 C150,2 165,6 180,5 C195,3 210,7 225,4 C240,2 255,6 270,5 C285,3 300,6 300,5' fill='none' stroke='%23D45040' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: repeat-x;
      background-size: 300px 8px;
    }

    /* Subtitle in signature style */
    .subtitle {
      font-family: 'Dancing Script', cursive;
      font-size: 1.5rem;
      color: var(--scribble-blue-ink);
      transform: rotate(-1deg);
      display: inline-block;
      margin-bottom: 2rem;
      margin-top: 0.5rem;
    }

    h2 {
      font-family: 'Patrick Hand', 'Caveat', cursive;
      font-size: clamp(1.6rem, 4vw, 2.4rem);
      color: var(--scribble-ink-soft);
      margin: 2.5rem 0 1rem;
      transform: rotate(0.5deg);
      position: relative;
      display: inline-block;
    }

    h3 {
      font-family: 'Caveat', cursive;
      font-size: clamp(1.3rem, 3vw, 1.8rem);
      color: var(--scribble-terracotta);
      margin: 2rem 0 0.8rem;
    }

    p {
      margin-bottom: 1.2rem;
      max-width: 65ch;
    }

    /* Highlighter mark */
    mark {
      background: linear-gradient(
        to bottom,
        transparent 40%,
        rgba(255, 224, 102, 0.45) 40%,
        rgba(255, 224, 102, 0.45) 85%,
        transparent 85%
      );
      padding: 0 4px;
      color: inherit;
    }

    /* Hand-drawn card */
    .scribble-card {
      background: var(--scribble-paper-dark);
      padding: 2rem;
      margin: 2rem 0;
      transform: rotate(-0.5deg);
      position: relative;
      box-shadow: 3px 4px 12px var(--scribble-shadow-medium);
      transition: transform 0.3s ease;
    }

    .scribble-card::before {
      content: '';
      position: absolute;
      inset: -2px;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 200' preserveAspectRatio='none'%3E%3Cpath d='M3,5 C3,3 7,3 40,4 C80,3 120,5 160,4 C192,3 197,5 197,5 C199,5 197,7 196,40 C197,80 196,120 197,160 C198,192 196,197 196,197 C196,199 192,197 160,196 C120,197 80,196 40,197 C8,198 3,196 3,196 C1,196 3,192 4,160 C3,120 4,80 3,40 C2,8 3,5 3,5Z' fill='none' stroke='%232A2520' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
      background-size: 100% 100%;
      background-repeat: no-repeat;
      pointer-events: none;
    }

    .scribble-card:hover {
      transform: rotate(0deg) translateY(-2px);
    }

    /* Tilted card variant */
    .scribble-card:nth-of-type(even) {
      transform: rotate(0.7deg);
    }

    .scribble-card:nth-of-type(even):hover {
      transform: rotate(0deg) translateY(-2px);
    }

    /* Sticky note */
    .scribble-sticky {
      background: var(--scribble-highlighter);
      padding: 1.2rem 1.5rem;
      font-family: 'Caveat', cursive;
      font-size: 1.2rem;
      color: var(--scribble-ink);
      transform: rotate(-2.5deg);
      box-shadow: 2px 3px 8px var(--scribble-shadow-medium);
      max-width: 260px;
      line-height: 1.5;
      position: relative;
      margin: 1.5rem 0 1.5rem auto;
    }

    .scribble-sticky::before {
      content: '';
      position: absolute;
      top: -7px;
      left: 50%;
      transform: translateX(-50%) rotate(1deg);
      width: 55px;
      height: 14px;
      background: rgba(255, 255, 255, 0.55);
      border: 1px solid rgba(0, 0, 0, 0.06);
    }

    /* Annotation in margin */
    .margin-note {
      font-family: 'Indie Flower', 'Caveat', cursive;
      font-size: 0.95rem;
      color: var(--scribble-blue-ink);
      transform: rotate(-2deg);
      display: inline-block;
      margin-left: 1rem;
      position: relative;
    }

    .margin-note::before {
      content: '';
      display: inline-block;
      width: 20px;
      height: 16px;
      margin-right: 4px;
      vertical-align: middle;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='16' viewBox='0 0 20 16'%3E%3Cpath d='M2,10 C5,8 10,6 14,4' fill='none' stroke='%234A6FA5' stroke-width='1.5' stroke-linecap='round'/%3E%3Cpath d='M11,2 L14,4 L11,6' fill='none' stroke='%234A6FA5' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
      background-size: contain;
      background-repeat: no-repeat;
    }

    /* Correction / strikethrough */
    .correction {
      position: relative;
      display: inline-block;
    }

    .correction .old {
      text-decoration: line-through wavy;
      text-decoration-color: var(--scribble-red-pen);
      text-decoration-thickness: 2px;
      color: var(--scribble-text-muted);
    }

    .correction .new {
      font-family: 'Caveat', cursive;
      color: var(--scribble-red-pen);
      font-size: 1.15em;
      margin-left: 4px;
      transform: rotate(-1deg);
      display: inline-block;
    }

    /* Hand-drawn list */
    .scribble-list {
      list-style: none;
      padding-left: 2rem;
      margin: 1rem 0;
    }

    .scribble-list li {
      position: relative;
      margin-bottom: 0.7rem;
      padding-left: 0.5rem;
    }

    .scribble-list li::before {
      content: '';
      position: absolute;
      left: -1.5rem;
      top: 0.35em;
      width: 14px;
      height: 14px;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='14' height='14' viewBox='0 0 14 14'%3E%3Crect x='1' y='1' width='12' height='12' rx='1' fill='none' stroke='%234A4540' stroke-width='1.5'/%3E%3Cpath d='M3,7 L6,10 L11,4' fill='none' stroke='%23D45040' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E");
      background-size: contain;
      background-repeat: no-repeat;
    }

    /* Blob shape accent */
    .blob-accent {
      position: absolute;
      border-radius: 60% 40% 55% 45% / 45% 55% 40% 60%;
      background: rgba(125, 140, 100, 0.1);
      pointer-events: none;
      z-index: 0;
    }

    /* Hand-drawn divider */
    hr {
      border: none;
      height: 8px;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='8' viewBox='0 0 400 8'%3E%3Cpath d='M0,4 C20,2 40,6 60,4 C80,2 100,5 120,4 C140,3 160,6 180,4 C200,2 220,5 240,3 C260,2 280,6 300,4 C320,2 340,5 360,4 C380,3 395,5 400,4' fill='none' stroke='%239E9588' stroke-width='1.5' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: repeat-x;
      background-position: center;
      background-size: 400px 8px;
      margin: 2.5rem 0;
    }

    /* Button */
    .scribble-button {
      display: inline-block;
      padding: 0.7rem 2rem;
      background: var(--scribble-paper-light);
      color: var(--scribble-ink);
      font-family: 'Patrick Hand', cursive;
      font-size: 1.15rem;
      text-decoration: none;
      cursor: pointer;
      border: none;
      position: relative;
      transform: rotate(-0.5deg);
      transition: transform 0.2s ease;
    }

    .scribble-button::before {
      content: '';
      position: absolute;
      inset: -2px;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 60' preserveAspectRatio='none'%3E%3Cpath d='M4,4 C4,2 10,4 50,3 C100,2 150,5 190,3 C196,2 197,4 197,6 C198,10 196,20 197,30 C198,40 196,50 197,55 C198,57 196,58 190,57 C150,58 100,56 50,57 C10,58 4,57 3,56 C2,55 3,45 4,30 C3,15 4,6 4,4Z' fill='none' stroke='%232A2520' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");
      background-size: 100% 100%;
      background-repeat: no-repeat;
      pointer-events: none;
    }

    .scribble-button:hover {
      transform: rotate(0deg) scale(1.03);
    }

    /* Marker emphasis text */
    .marker {
      font-family: 'Permanent Marker', cursive;
      color: var(--scribble-red-pen);
    }

    /* Wavy underline emphasis */
    .wavy {
      text-decoration: underline wavy var(--scribble-terracotta);
      text-decoration-thickness: 1.5px;
      text-underline-offset: 4px;
    }

    /* Footer signature */
    .scribble-footer {
      margin-top: 4rem;
      padding-top: 2rem;
      text-align: right;
    }

    .scribble-footer .signature {
      font-family: 'Dancing Script', cursive;
      font-size: 1.8rem;
      color: var(--scribble-ink);
      transform: rotate(-3deg);
      display: inline-block;
    }

    .scribble-footer .date {
      font-family: 'Caveat', cursive;
      font-size: 1rem;
      color: var(--scribble-text-muted);
      display: block;
      margin-top: 0.3rem;
    }

    /* Responsive */
    @media (max-width: 860px) {
      .scribble-page {
        padding: 2rem 1.5rem;
      }

      .scribble-page::before {
        display: none;
      }

      .scribble-sticky {
        margin: 1.5rem auto;
      }
    }
  </style>
</head>
<body>
  <div class="scribble-page">
    <!-- Decorative blob accent -->
    <div class="blob-accent" style="width: 180px; height: 180px; top: 60px; right: -40px;"></div>
    <div class="blob-accent" style="width: 120px; height: 120px; top: 400px; left: -30px; border-radius: 40% 60% 45% 55% / 55% 40% 60% 45%; background: rgba(196, 125, 90, 0.08);"></div>

    <h1>A Human Made This</h1>
    <p class="subtitle">imperfect by design, honest by intention</p>

    <p>This is what it looks like when a real person touches a page. Not an algorithm, not a template engine, not a prompt. A hand holding a pen, <mark>thinking out loud</mark>, crossing things out, starting over, and leaving every mark behind as proof.</p>

    <hr>

    <h2>Why Imperfection Matters</h2>

    <p>In an age where machines can generate <span class="wavy">flawless layouts</span> in milliseconds, the deliberate wobble of a hand-drawn line carries new meaning. It says: someone cared enough to do this themselves.</p>

    <div class="scribble-card">
      <h3>The Warmth of Visible Process</h3>
      <p>Every crossed-out word is a decision. Every arrow in the margin is a thought connecting to another thought. The
      <span class="correction">
        <span class="old">perfection</span>
        <span class="new">personality</span>
      </span>
      is in the process, not the polish.</p>
      <span class="margin-note">this is the key insight</span>
    </div>

    <div class="scribble-card">
      <h3>What Makes It Human</h3>
      <ul class="scribble-list">
        <li>Lines that wobble because hands wobble</li>
        <li>Notes in margins because thoughts overflow</li>
        <li>Corrections that show the thinking, not just the conclusion</li>
        <li>Signatures at the bottom because someone stands behind this</li>
      </ul>
    </div>

    <div class="scribble-sticky">
      Remember: the goal isn't to look messy. It's to look <em>alive</em>. There's a difference.
    </div>

    <h2>How to Use This</h2>

    <p>Pair clean, readable body text with <span class="marker">handwritten headings</span>. Layer annotations over structure. Let the digital and analog coexist on the same page -- that contrast is the whole point.</p>

    <p>Use rotation sparingly. A card tilted 1 degree feels human. A card tilted 15 degrees feels broken. The magic is in <mark>subtlety</mark>.</p>

    <div style="margin: 2rem 0; display: flex; gap: 1rem; flex-wrap: wrap;">
      <a href="#" class="scribble-button">Read More</a>
      <a href="#" class="scribble-button" style="background: var(--scribble-terracotta); color: var(--scribble-paper-light);">Get Started</a>
    </div>

    <hr>

    <div class="scribble-footer">
      <span class="signature">Made by a human</span>
      <span class="date">feb 2026, with coffee and a felt-tip pen</span>
    </div>
  </div>
</body>
</html>
```
