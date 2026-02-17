# Neon Ooze

An aesthetic rooted in 1980s--90s children's gross-out marketing culture, defined by **dripping slime, toxic waste imagery, radioactive glow, lurid neon colors, and gleefully disgusting motifs**. Neon Ooze channels the visual language of Nickelodeon slime dumps, B-movie toxic mutants, mad-scientist laboratories, and creepy-crawly creature features into a hyper-saturated, deliberately provocative design style. The mood is playfully menacing -- gross enough to thrill kids, bright enough to sell toys, and just unsettling enough to hint at genuine environmental anxiety about nuclear waste and pollution.

---

## Color Palette

### Core Principle

Neon Ooze uses **toxic neon colors at maximum saturation** against **dark, murky backgrounds**. The palette simulates the glow of radioactive substances in a dark laboratory or sewer. Colors should look like they emit light -- luminous, almost painful to look at, and distinctly unnatural.

### Primary Scheme

| Role | Colors |
|------|--------|
| **Backgrounds** | Deep black, dark sewer greens, murky purple-black |
| **Primary accent** | Toxic / slime green (the signature color) |
| **Secondary accents** | Electric purple, neon blue |
| **Tertiary / highlights** | Hot pink / magenta, hazard yellow-orange |

### Full Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Slime Green | `#39FF14`, `#00FF41` | Primary accent, slime effects, glowing elements, headings |
| Toxic Yellow-Green | `#CCFF00`, `#B8FF00` | Secondary green, radioactive glow, highlights |
| Electric Purple | `#BF00FF`, `#9B30FF` | Accent panels, borders, secondary headings |
| Deep Purple | `#4B0082`, `#3A0066` | Dark accent backgrounds, gradient endpoints |
| Neon Blue | `#00BFFF`, `#00E5FF` | Tertiary accent, cool glow effects, links |
| Hot Pink / Magenta | `#FF00FF`, `#FF1493` | Display text, call-to-action elements, decorative splats |
| Hazard Orange | `#FF6600`, `#FF4500` | Warning elements, tertiary accents, small highlights |
| Sewer Black | `#0A0A0A`, `#0D1117` | Primary background |
| Murky Green-Black | `#0B1A0B`, `#0F1F0F` | Alternative dark background with green undertone |
| Toxic Sludge Brown | `#2D1F0E`, `#3B2F1B` | Accent background suggesting contaminated earth |
| Biohazard Yellow | `#FFD700`, `#FFC200` | Hazard symbols, small warning details |
| Bone White | `#E8E8D0`, `#D4D4AA` | Body text (slightly yellowed, never pure white) |

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --ooze-black: #0a0a0a;
  --ooze-dark-green: #0b1a0b;
  --ooze-deep-purple: #1a0033;
  --ooze-sludge: #2d1f0e;

  /* Neon accents */
  --ooze-slime: #39ff14;
  --ooze-slime-bright: #00ff41;
  --ooze-toxic-yellow: #ccff00;
  --ooze-purple: #bf00ff;
  --ooze-blue: #00bfff;
  --ooze-pink: #ff00ff;
  --ooze-orange: #ff6600;
  --ooze-hazard-yellow: #ffd700;

  /* Text */
  --ooze-text: #e8e8d0;
  --ooze-text-dim: #9a9a7a;

  /* Functional */
  --ooze-bg-primary: var(--ooze-black);
  --ooze-bg-secondary: var(--ooze-dark-green);
  --ooze-accent-primary: var(--ooze-slime);
  --ooze-accent-secondary: var(--ooze-purple);
  --ooze-border: var(--ooze-slime);
}
```

### Color Usage Principles

- **Dark, cold base with neon overlays** -- near-black backgrounds so neon colors appear to glow through contrast
- **Green dominates** -- slime green is the signature color and should be the most prominent accent
- **Purple and blue as supporting neons** -- used for variety but never overwhelming the green
- **Hot pink / magenta for typography** -- especially display text and logos, as seen in classic Nickelodeon and toy branding
- **Avoid pastels, earth tones, or muted colors** -- everything should feel radioactive and oversaturated
- **Hazard yellow sparingly** -- used for biohazard/warning symbols and small detail elements

---

## Typography

### Typeface Characteristics

Neon Ooze typography is **chunky, exaggerated, distorted, and dripping**. Letters should look like they are melting, oozing, or mutating. The style draws from 1990s toy packaging, VHS horror covers, and Nickelodeon show titles.

- **Thick, heavy letterforms** -- bold or black weights, wide proportions
- **Irregular baselines** -- letters wobble, tilt, and bounce unevenly
- **Dripping / melting effects** -- descenders and terminals that trail off into gooey drips
- **3D extrusion and drop shadows** -- chunky depth suggesting slimy physical mass
- **Outline and stroke treatments** -- bright outlines around dark fills, or neon fills with dark outlines
- **All-caps dominant** -- loud, aggressive, attention-grabbing
- **Rounded and bubbly forms** -- letters that look inflated, bloated, or swollen

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Bungee Shade** | Chunky layered display | Hero headings, titles |
| **Creepster** | Horror-tinged display | Section headings, spooky emphasis |
| **Fredoka One** | Rounded bold display | Friendly-grotesque headings |
| **Bangers** | Comic book display | Subheadings, callouts |
| **Permanent Marker** | Hand-drawn marker | Accent text, labels |
| **Rubik Mono One** | Heavy monospace display | Technical / lab-style headings |
| **Nunito** | Rounded sans-serif | Body text (readable but soft) |
| **Exo 2** | Geometric sans-serif | Body text alternative, UI elements |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Bungee+Shade&family=Creepster&family=Bangers&family=Nunito:wght@400;700&display=swap');

/* Display / Hero headings */
h1 {
  font-family: 'Bungee Shade', 'Creepster', cursive;
  font-size: clamp(3rem, 8vw, 7rem);
  text-transform: uppercase;
  color: var(--ooze-slime);
  text-shadow:
    0 0 10px var(--ooze-slime),
    0 0 20px var(--ooze-slime),
    0 0 40px rgba(57, 255, 20, 0.5),
    4px 4px 0 var(--ooze-deep-purple);
  letter-spacing: 0.05em;
  line-height: 1.1;
}

/* Section headings */
h2, h3 {
  font-family: 'Creepster', 'Bangers', cursive;
  text-transform: uppercase;
  color: var(--ooze-pink);
  text-shadow:
    0 0 7px var(--ooze-pink),
    0 0 15px rgba(255, 0, 255, 0.4),
    3px 3px 0 rgba(0, 0, 0, 0.8);
  letter-spacing: 0.04em;
}

/* Body text */
body {
  font-family: 'Nunito', 'Exo 2', sans-serif;
  font-weight: 400;
  font-size: 1.05rem;
  line-height: 1.7;
  color: var(--ooze-text);
  letter-spacing: 0.01em;
}

/* Accent text / callouts */
.ooze-callout {
  font-family: 'Bangers', cursive;
  font-size: 1.4em;
  color: var(--ooze-toxic-yellow);
  text-shadow: 0 0 8px rgba(204, 255, 0, 0.6);
  text-transform: uppercase;
}
```

---

## Key Design Elements and Motifs

### Slime and Ooze Effects

The defining visual element. Dripping, splattered, and flowing slime should appear on borders, headers, dividers, and decorative elements.

- **Drip borders** -- top or bottom edges of containers that appear to ooze downward
- **Splat shapes** -- irregular blob shapes as decorative backgrounds or image masks
- **Slime trails** -- thin rivulets connecting elements or following scroll direction
- **Bubble clusters** -- small circular shapes suggesting gas bubbles in viscous liquid

### Toxic / Nuclear Imagery

- **Biohazard symbols** (Unicode: `\2622`) -- used as decorative accents and dividers
- **Radioactive trefoil** (Unicode: `\2622`) -- section markers and icons
- **Warning stripes** -- black and hazard-yellow diagonal stripes for borders and accents
- **Barrels and drums** -- implied through cylindrical shapes and hazard markings
- **Glowing containers** -- elements that appear to hold luminous liquid

### Mad Science / Laboratory

- **Test tubes and beakers** -- as decorative icons or section markers
- **Bubbling liquid** -- animated bubble effects rising through containers
- **Electrical arcs** -- jagged lightning-bolt shapes connecting elements
- **Circuit and pipe patterns** -- suggesting laboratory plumbing and wiring

### Creepy Crawlies

- **Insects** -- flies, spiders, cockroaches as small decorative details
- **Eyeballs** -- floating, bulging eyes as icons or bullet points
- **Tentacles** -- curving organic shapes used as borders or frames
- **Worms and maggots** -- squirming shapes in backgrounds or dividers

### Design Principles

- **Deliberate grossness** -- the design should provoke a visceral "ewww" reaction while remaining fun
- **Aggressive energy** -- nothing should feel calm, sterile, or refined
- **Playful menace** -- threatening enough to be exciting, bright enough to be entertaining
- **Maximum contrast** -- neon on black, always pushing toward the limits of readability
- **Organic chaos over geometric order** -- blobs, splats, and drips instead of straight lines and grids

---

## Layout Principles

### Structure

- **Dark, immersive backgrounds** -- the page should feel like peering into a murky sewer or abandoned laboratory
- **Asymmetric, irregular compositions** -- avoid rigid grids; use off-kilter placement suggesting things that have oozed into position
- **Generous use of neon borders and dividers** -- glowing lines that separate content areas
- **Layered depth** -- overlapping drip effects, splat shapes, and glow layers creating visual richness
- **Contained chaos** -- within each section, allow messy organic shapes, but maintain overall navigability

### Section Organization

- Use **slime-drip dividers** between sections (SVG drip shapes along horizontal rules)
- Apply **neon glow borders** around content panels
- Create **hierarchy through color temperature** -- slime green for primary, pink/purple for secondary, blue for tertiary
- Employ **splat-shaped containers** for featured content (irregular blob outlines instead of rectangles)
- Allow **elements to break out of their containers** -- drips that extend beyond borders, splats that overlap sections

---

## CSS / Design Techniques

### Neon Glow Effects

```css
/* Primary slime glow for text */
.ooze-glow {
  color: var(--ooze-slime);
  text-shadow:
    0 0 7px var(--ooze-slime),
    0 0 10px var(--ooze-slime),
    0 0 21px var(--ooze-slime),
    0 0 42px rgba(57, 255, 20, 0.5),
    0 0 82px rgba(57, 255, 20, 0.3);
}

/* Purple neon glow */
.ooze-glow-purple {
  color: var(--ooze-purple);
  text-shadow:
    0 0 7px var(--ooze-purple),
    0 0 10px var(--ooze-purple),
    0 0 21px var(--ooze-purple),
    0 0 42px rgba(191, 0, 255, 0.4);
}

/* Glowing box border */
.ooze-box-glow {
  border: 2px solid var(--ooze-slime);
  box-shadow:
    0 0 5px var(--ooze-slime),
    0 0 15px rgba(57, 255, 20, 0.3),
    inset 0 0 15px rgba(57, 255, 20, 0.05);
}
```

### Slime Drip Border (SVG-based)

```css
/* Dripping slime effect along a container's bottom edge */
.ooze-drip-bottom {
  position: relative;
  overflow: visible;
}

.ooze-drip-bottom::after {
  content: '';
  position: absolute;
  bottom: -20px;
  left: 0;
  right: 0;
  height: 30px;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 30' preserveAspectRatio='none'%3E%3Cpath d='M0,0 Q10,0 10,8 Q10,20 15,25 Q18,28 20,20 Q22,8 25,0 Q40,0 45,0 Q45,10 50,18 Q53,22 55,15 Q57,5 60,0 Q80,0 85,0 Q85,12 90,22 Q92,26 95,18 Q98,8 100,0 Q120,0 125,0 Q125,6 128,12 Q130,16 132,10 Q135,4 138,0 Q155,0 160,0 Q160,14 165,24 Q168,30 172,20 Q175,10 178,0 L200,0' fill='%2339ff14' /%3E%3C/svg%3E") repeat-x;
  background-size: 200px 30px;
  pointer-events: none;
  filter: drop-shadow(0 0 6px rgba(57, 255, 20, 0.6));
}
```

### Toxic Bubble Animation

```css
@keyframes bubble-rise {
  0% {
    transform: translateY(0) scale(1);
    opacity: 0.7;
  }
  50% {
    transform: translateY(-40px) scale(1.1);
    opacity: 0.5;
  }
  100% {
    transform: translateY(-80px) scale(0.8);
    opacity: 0;
  }
}

.ooze-bubbles::before,
.ooze-bubbles::after {
  content: '';
  position: absolute;
  border-radius: 50%;
  background: radial-gradient(circle at 30% 30%,
    rgba(57, 255, 20, 0.4),
    rgba(57, 255, 20, 0.1));
  animation: bubble-rise 3s ease-in-out infinite;
}

.ooze-bubbles::before {
  width: 12px;
  height: 12px;
  bottom: 10%;
  left: 20%;
}

.ooze-bubbles::after {
  width: 8px;
  height: 8px;
  bottom: 15%;
  left: 35%;
  animation-delay: 1.5s;
}
```

### Radioactive Pulsing Glow

```css
@keyframes radioactive-pulse {
  0%, 100% {
    box-shadow:
      0 0 5px var(--ooze-slime),
      0 0 15px rgba(57, 255, 20, 0.3);
  }
  50% {
    box-shadow:
      0 0 10px var(--ooze-slime),
      0 0 30px rgba(57, 255, 20, 0.5),
      0 0 50px rgba(57, 255, 20, 0.2);
  }
}

.ooze-pulse {
  animation: radioactive-pulse 2s ease-in-out infinite;
}
```

### Hazard Stripe Border

```css
/* Black and yellow diagonal warning stripes */
.ooze-hazard-border {
  border: 4px solid transparent;
  border-image: repeating-linear-gradient(
    -45deg,
    #000 0px,
    #000 8px,
    var(--ooze-hazard-yellow) 8px,
    var(--ooze-hazard-yellow) 16px
  ) 4;
}
```

### Slime Splat Background Shape

```css
/* Irregular blob shape for featured content */
.ooze-splat {
  background: radial-gradient(
    ellipse at 40% 50%,
    rgba(57, 255, 20, 0.12) 0%,
    rgba(57, 255, 20, 0.04) 50%,
    transparent 70%
  );
  border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%;
  padding: 3rem;
}
```

### Ooze Card / Panel

```css
.ooze-card {
  background: linear-gradient(
    170deg,
    rgba(11, 26, 11, 0.9) 0%,
    rgba(10, 10, 10, 0.95) 100%
  );
  border: 2px solid var(--ooze-slime);
  border-radius: 4px;
  padding: 2rem;
  position: relative;
  box-shadow:
    0 0 8px rgba(57, 255, 20, 0.2),
    inset 0 0 30px rgba(57, 255, 20, 0.03);
}

.ooze-card::before {
  content: '\2622'; /* biohazard symbol */
  position: absolute;
  top: -12px;
  right: 16px;
  font-size: 1.4rem;
  color: var(--ooze-hazard-yellow);
  background: var(--ooze-black);
  padding: 0 0.4em;
  text-shadow: 0 0 8px rgba(255, 215, 0, 0.5);
}
```

### Sewer / Laboratory Background Textures

```css
/* Dark background with subtle green noise */
.ooze-bg-sewer {
  background-color: var(--ooze-black);
  background-image:
    radial-gradient(ellipse at 20% 80%, rgba(57, 255, 20, 0.03) 0%, transparent 50%),
    radial-gradient(ellipse at 80% 20%, rgba(191, 0, 255, 0.02) 0%, transparent 50%);
}

/* Vignette overlay for dark tunnel / sewer feel */
.ooze-vignette::after {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse at center,
    transparent 30%,
    rgba(0, 0, 0, 0.6) 100%
  );
  pointer-events: none;
}

/* Subtle grid pattern suggesting laboratory tiles */
.ooze-lab-grid {
  background-image:
    linear-gradient(rgba(57, 255, 20, 0.04) 1px, transparent 1px),
    linear-gradient(90deg, rgba(57, 255, 20, 0.04) 1px, transparent 1px);
  background-size: 40px 40px;
}
```

### Slime Drip Divider

```css
.ooze-divider {
  height: 0;
  border: none;
  border-top: 2px solid var(--ooze-slime);
  margin: 3rem auto;
  width: 70%;
  position: relative;
  filter: drop-shadow(0 0 4px rgba(57, 255, 20, 0.5));
}

.ooze-divider::before {
  content: '\2622'; /* biohazard */
  position: absolute;
  top: -0.7em;
  left: 50%;
  transform: translateX(-50%);
  background: var(--ooze-black);
  padding: 0 0.6em;
  color: var(--ooze-slime);
  font-size: 1.2rem;
  text-shadow: 0 0 8px rgba(57, 255, 20, 0.6);
}
```

---

## CSS Techniques Summary

| Technique | CSS Property / Approach |
|-----------|------------------------|
| Neon glow text | Multiple `text-shadow` layers with same-hue colors at increasing blur |
| Glowing borders | `box-shadow` with neon colors + `border` in matching hue |
| Slime drips | SVG `path` with irregular curves as `background-image` or `::after` pseudo-element |
| Radioactive pulse | `@keyframes` animating `box-shadow` spread and opacity |
| Hazard stripes | `repeating-linear-gradient(-45deg, ...)` as `border-image` |
| Splat shapes | Irregular `border-radius` values (e.g., `60% 40% 55% 45% / 50% 60% 40% 50%`) |
| Sewer atmosphere | Radial gradients with very low-opacity greens and purples on black |
| Bubble effects | `@keyframes` with `translateY` and `opacity` on `::before`/`::after` circles |
| Lab tile grid | `linear-gradient` grid pattern at low opacity |
| Vignette | `radial-gradient` from transparent center to dark edges via `::after` overlay |
| Toxic glow containers | `inset box-shadow` with green tint + solid neon border |

---

## Animation and Motion

- **Dripping motion** -- slow, viscous downward movement on drip elements using `translateY` with ease-in timing
- **Bubbling** -- small circles rising and fading, staggered with `animation-delay`
- **Pulsing glow** -- rhythmic brightening and dimming of neon borders and text shadows simulating radioactive energy
- **Splattering** -- on hover or click, elements can "splat" outward with a scale + irregular border-radius transition
- **Flickering** -- occasional rapid opacity flicker on neon elements suggesting unstable electrical power
- **Oozing text reveal** -- text that appears to drip into place from above using `clip-path` animation

```css
/* Flickering neon effect */
@keyframes neon-flicker {
  0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% {
    text-shadow:
      0 0 7px var(--ooze-slime),
      0 0 10px var(--ooze-slime),
      0 0 21px var(--ooze-slime);
  }
  20%, 24%, 55% {
    text-shadow: none;
  }
}

.ooze-flicker {
  animation: neon-flicker 4s infinite;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Green slime / ooze | Semi-transparent green gradients with irregular edges, `border-radius` blobs |
| Toxic waste barrels | Cylindrical shapes with hazard-stripe borders and yellow warning text |
| Sewer walls / pipes | Dark textured backgrounds with subtle green-tinted grid patterns |
| Glowing radioactive liquid | `radial-gradient` with neon green center fading to dark, animated pulse |
| Rubber / latex (lab gloves) | Glossy solid-color surfaces with specular highlight gradients |
| Corroded metal | Dark metallic gradients with green oxidation patches (green-tinted noise) |
| Laboratory glass (beakers) | Semi-transparent panels with green or purple tint and subtle refraction effect |
| VHS packaging / 90s plastic | High-contrast neon-on-black with chunky type and splatter elements |
| Nickelodeon slime | Bright green with yellow-green highlights and drip morphology |
| Bug carapace / insect wings | Iridescent purple-green gradients with high gloss |

---

## Cultural References and Exemplars

The visual identity draws from:

- **Nickelodeon** (1990s era) -- green slime, bright orange-and-green branding, chaotic kid energy
- **Goosebumps book covers** -- dripping typography, lurid greens and purples, creepy-fun horror
- **EarthBound (1995)** -- green slime splatter graphic design on Nintendo marketing
- **Toxic Avenger / Troma Films** -- low-budget horror with neon-toxic color grading
- **Creepy Crawlers oven toys** -- gooey, brightly colored mold-making aesthetic
- **Captain Planet villains** -- toxic waste, pollution, radioactive sludge as visual motifs
- **Boogerman (1994)** -- gross-out video game with slime, snot, and neon palette
- **Trash Pack / Garbage Pail Kids** -- grotesque character design in neon packaging
- **90s skateboard graphics** (Slime Balls brand) -- dripping slime logos on neon backgrounds

---

## Related Aesthetics

| Aesthetic | Relationship to Neon Ooze |
|-----------|--------------------------|
| **Slimepunk** | Closely related; emphasizes toxic/radioactive imagery with punk-adjacent DIY attitude |
| **Wacky Pomo** | Shares 90s kid-culture roots, bright neons, blob shapes, and anti-refined sensibility |
| **Acid Design** | Parallel neon-on-black palette but more rave/club culture vs. kid/gross-out culture |
| **Psychedelia** | Shared interest in lurid color and visual distortion, but different cultural origin |
| **Kidcore** | Overlapping era and child-targeting aesthetic, but Kidcore is wholesome where Neon Ooze is gross |
| **Y2K Futurism** | Shares neon palette and 90s nostalgia, but cleaner and more tech-optimistic |
| **Goblincore** | Shared love of the grotesque and creepy-crawly, but Goblincore is earthy/natural vs. neon/synthetic |
