# Film Noir Design Reference

Film Noir is a visual and narrative style rooted in the crime cinema of the 1940s and 1950s -- an era that produced some of the most atmospherically charged imagery in film history. Originating from the intersection of American hard-boiled detective fiction and German Expressionist cinematography brought by European emigre filmmakers, Film Noir is defined by its high-contrast black-and-white photography, chiaroscuro lighting, dramatic shadow play, rain-slicked urban settings, and a pervasive mood of tension, moral ambiguity, and fatalism. Iconic visual motifs include venetian blind shadow patterns cast across faces and walls, cigarette smoke curling through shafts of light, fedora-wearing detectives in trench coats, and femme fatales silhouetted in doorways. In web and UI design, the Film Noir aesthetic translates to deep monochrome palettes with strategic warm accents, high-contrast typography reminiscent of vintage movie titles, dramatic shadow and lighting effects achieved through CSS gradients and overlays, atmospheric texture layers (grain, smoke, rain), and cinematic compositions that evoke the claustrophobic tension and moody elegance of classic noirs like The Maltese Falcon, Double Indemnity, and The Third Man. The result is a digital experience that feels like stepping into a shadowy detective's office at midnight -- dangerous, beautiful, and impossible to look away from.

---

## Visual Characteristics

### Core Design Traits

- **High-contrast chiaroscuro lighting**: Extreme contrast between deep blacks and bright whites dominates every composition, with shadows used as active design elements rather than mere absence of light -- directly echoing the low-key lighting techniques of noir cinematography
- **Venetian blind shadow patterns**: Horizontal stripe patterns cast across backgrounds, images, and text containers simulate the iconic look of light filtering through window blinds, one of the most recognizable Film Noir visual signatures
- **Monochrome-dominant palette with warm accents**: The primary palette is grayscale (near-black through white), punctuated sparingly by warm amber, gold, or deep crimson accents that evoke neon signs, cigarette embers, and whiskey in a tumbler
- **Atmospheric smoke and fog effects**: Translucent gradient overlays, animated particle effects, or static texture layers simulate the ever-present cigarette smoke and urban fog that softens and obscures noir environments
- **Rain and wet surface reflections**: Glossy, reflective surfaces and rain streak effects recall the perpetually rain-slicked streets and alleyways of the noir urban landscape
- **Dramatic diagonal compositions**: Tilted elements, angled dividers, and asymmetric layouts reference the Dutch angle camera work and skewed perspectives characteristic of noir cinematography
- **Film grain and analog texture**: Subtle noise overlays and grain textures add the tactile quality of aged 35mm celluloid, grounding digital designs in the materiality of the original film medium
- **Silhouette and partial reveal**: Key visual elements are shown in silhouette or partially obscured by shadow, creating mystery and visual tension -- figures in doorways, half-lit faces, objects emerging from darkness
- **Cinematic letterboxing and framing**: Wide aspect ratios, dark vignette edges, and border framing techniques create the feeling of looking through a movie screen or a detective's window
- **Art Deco-influenced decorative elements**: Geometric borders, angular ornaments, and stylized line work draw from the Art Deco period concurrent with classic noir, adding period-appropriate elegance

### Design Principles

- **Shadow is as important as light**: Design with negative space and darkness as primary compositional tools; what is hidden or obscured matters as much as what is revealed
- **Atmosphere over information density**: Every element should contribute to the overall mood; prioritize cinematic tension and immersive feeling over packing in content
- **Restraint in color creates impact**: When the world is grayscale, even a small touch of amber or red becomes electric; use accent colors with the precision of a single lit match in a dark room
- **Typography tells the story**: Headlines should carry the weight and drama of a movie title card; the font itself should evoke danger, elegance, or moral ambiguity
- **Texture creates time period**: Grain, noise, and analog artifacts anchor the design in its historical era; without texture, high-contrast monochrome becomes generic rather than specifically noir
- **Asymmetry creates tension**: Reject perfect balance in favor of compositions that feel slightly unstable, slightly dangerous -- like the narrative moral universe of noir itself
- **Every element should cast a shadow**: Depth and dimensionality come from consistent, dramatic shadow application across all UI components, reinforcing the lighting-driven aesthetic

---

## Color Palette

The Film Noir palette is built on a foundation of deep blacks and luminous whites, with a carefully controlled range of grays for depth and atmosphere. Accent colors are drawn from the warm glow of neon signs, amber streetlights, and the deep reds of lipstick and blood -- used sparingly for maximum dramatic impact.

| Swatch | Hex | Role / Usage |
|--------|-----|-------------|
| ![#0A0A0A](https://via.placeholder.com/20/0A0A0A/0A0A0A) | `#0A0A0A` | Deepest black -- primary background, the void of a dark alley |
| ![#1A1A1A](https://via.placeholder.com/20/1A1A1A/1A1A1A) | `#1A1A1A` | Surface black -- card backgrounds, elevated panels |
| ![#2A2A2A](https://via.placeholder.com/20/2A2A2A/2A2A2A) | `#2A2A2A` | Shadow gray -- borders, dividers, secondary surfaces |
| ![#3D3D3D](https://via.placeholder.com/20/3D3D3D/3D3D3D) | `#3D3D3D` | Mid-shadow -- inactive states, subtle structural elements |
| ![#6B6B6B](https://via.placeholder.com/20/6B6B6B/6B6B6B) | `#6B6B6B` | Smoke gray -- secondary text, muted metadata, fog overlays |
| ![#9A9A9A](https://via.placeholder.com/20/9A9A9A/9A9A9A) | `#9A9A9A` | Silver -- tertiary text, timestamps, captions |
| ![#C8C8C8](https://via.placeholder.com/20/C8C8C8/C8C8C8) | `#C8C8C8` | Light silver -- body text on dark backgrounds |
| ![#E8E8E8](https://via.placeholder.com/20/E8E8E8/E8E8E8) | `#E8E8E8` | Near-white -- primary text, high-emphasis headings |
| ![#F5F5F0](https://via.placeholder.com/20/F5F5F0/F5F5F0) | `#F5F5F0` | Cream white -- headline text, dramatic spotlight areas |
| ![#D4A847](https://via.placeholder.com/20/D4A847/D4A847) | `#D4A847` | Amber gold -- primary accent, neon glow, links, CTAs |
| ![#C19A3E](https://via.placeholder.com/20/C19A3E/C19A3E) | `#C19A3E` | Antique gold -- hover states, secondary accent, ornamental details |
| ![#8B1A1A](https://via.placeholder.com/20/8B1A1A/8B1A1A) | `#8B1A1A` | Blood crimson -- danger, alerts, dramatic emphasis |
| ![#A0522D](https://via.placeholder.com/20/A0522D/A0522D) | `#A0522D` | Sienna brown -- warm undertones, leather, aged paper |
| ![#1C2833](https://via.placeholder.com/20/1C2833/1C2833) | `#1C2833` | Midnight blue -- cool shadow alternative, night sky undertone |
| ![#D4A84780](https://via.placeholder.com/20/D4A847/D4A847) | `#D4A84780` | Amber glow (50% opacity) -- soft light halos, atmospheric warmth |

### CSS Custom Properties

```css
:root {
  /* Core noir blacks */
  --noir-black-void: #0a0a0a;
  --noir-black-surface: #1a1a1a;
  --noir-black-shadow: #2a2a2a;
  --noir-gray-dark: #3d3d3d;

  /* Gray scale -- the smoke and silver */
  --noir-gray-smoke: #6b6b6b;
  --noir-gray-silver: #9a9a9a;
  --noir-gray-light: #c8c8c8;

  /* Light tones */
  --noir-white-near: #e8e8e8;
  --noir-white-cream: #f5f5f0;

  /* Accent -- neon and danger */
  --noir-amber: #d4a847;
  --noir-amber-dark: #c19a3e;
  --noir-amber-glow: rgba(212, 168, 71, 0.5);
  --noir-crimson: #8b1a1a;
  --noir-sienna: #a05230;
  --noir-midnight: #1c2833;

  /* Functional tokens */
  --noir-bg: var(--noir-black-void);
  --noir-bg-elevated: var(--noir-black-surface);
  --noir-text-primary: var(--noir-white-near);
  --noir-text-secondary: var(--noir-gray-light);
  --noir-text-muted: var(--noir-gray-smoke);
  --noir-border: var(--noir-gray-dark);
  --noir-accent: var(--noir-amber);
  --noir-accent-hover: var(--noir-amber-dark);
  --noir-danger: var(--noir-crimson);

  /* Gradients */
  --noir-gradient-shadow: linear-gradient(180deg, transparent 0%, var(--noir-black-void) 100%);
  --noir-gradient-spotlight: radial-gradient(ellipse at 30% 20%, rgba(212, 168, 71, 0.08) 0%, transparent 60%);
  --noir-gradient-vignette: radial-gradient(ellipse at center, transparent 40%, var(--noir-black-void) 100%);

  /* Overlays */
  --noir-overlay-dark: rgba(10, 10, 10, 0.85);
  --noir-overlay-smoke: rgba(10, 10, 10, 0.4);
}
```

---

## Typography

Film Noir typography draws from two traditions: the dramatic, often hand-painted title cards of 1940s-50s crime films, and the utilitarian typewriter text of detective reports and ransom notes. Headlines use bold serif and display faces with sharp angles, elongated strokes, and Art Deco influences that convey danger and elegance. Body text favors clean, high-legibility serifs or refined sans-serifs that maintain readability against dark backgrounds while preserving the period atmosphere.

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| Playfair Display | 400, 700, 900 | Primary headlines, title cards, dramatic display text | [fonts.google.com/specimen/Playfair+Display](https://fonts.google.com/specimen/Playfair+Display) |
| Cinzel | 400, 700, 900 | Uppercase display headings, Art Deco-influenced titles | [fonts.google.com/specimen/Cinzel](https://fonts.google.com/specimen/Cinzel) |
| Libre Baskerville | 400, 400i, 700 | Body text, long-form reading, narrative content | [fonts.google.com/specimen/Libre+Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) |
| Special Elite | 400 | Typewriter effect, detective notes, accent text | [fonts.google.com/specimen/Special+Elite](https://fonts.google.com/specimen/Special+Elite) |
| Cormorant Garamond | 400, 600, 700 | Elegant body text, pull quotes, captions | [fonts.google.com/specimen/Cormorant+Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) |
| Bodoni Moda | 400, 700, 900 | High-contrast display headlines, dramatic serif statements | [fonts.google.com/specimen/Bodoni+Moda](https://fonts.google.com/specimen/Bodoni+Moda) |
| Oswald | 400, 500, 700 | Condensed sans-serif for navigation, labels, metadata | [fonts.google.com/specimen/Oswald](https://fonts.google.com/specimen/Oswald) |
| EB Garamond | 400, 500, 700 | Classic serif body text, refined reading experience | [fonts.google.com/specimen/EB+Garamond](https://fonts.google.com/specimen/EB+Garamond) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Playfair Display (900) | Libre Baskerville | Classic noir elegance -- dramatic high-contrast serif headlines with refined body text |
| Cinzel (700) | Cormorant Garamond | Art Deco meets 1940s sophistication -- all-caps monumental headings with graceful prose |
| Bodoni Moda (900) | EB Garamond | Maximum typographic contrast -- extreme thick-thin strokes in headlines with old-style body |
| Playfair Display (700) | Special Elite | Detective case file -- elegant headlines paired with typewriter body for narrative mystery |
| Oswald (700) | Libre Baskerville | Modern noir reinterpretation -- bold condensed sans headings with traditional serif body |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Special+Elite&family=Oswald:wght@400;500;700&display=swap');

/* === Base Typography === */
body {
  font-family: 'Libre Baskerville', 'Georgia', 'Times New Roman', serif;
  font-size: 17px;
  line-height: 1.75;
  color: var(--noir-text-primary);
  background-color: var(--noir-bg);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Playfair Display', 'Georgia', serif;
  font-weight: 900;
  line-height: 1.1;
  color: var(--noir-white-cream);
  letter-spacing: 0.02em;
  text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.6);
}

h1 {
  font-size: clamp(2.5rem, 7vw, 5.5rem);
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

h2 {
  font-size: clamp(1.8rem, 4vw, 3rem);
  letter-spacing: 0.04em;
}

h3 {
  font-size: clamp(1.3rem, 2.5vw, 2rem);
}

a {
  color: var(--noir-accent);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: color 0.3s ease, border-color 0.3s ease;
}

a:hover {
  color: var(--noir-white-cream);
  border-bottom-color: var(--noir-accent);
}

/* Typewriter accent class */
.typewriter {
  font-family: 'Special Elite', 'Courier New', monospace;
  letter-spacing: 0.05em;
  color: var(--noir-gray-light);
}

/* Navigation label style */
.label {
  font-family: 'Oswald', 'Arial Narrow', sans-serif;
  font-weight: 500;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--noir-gray-smoke);
}

blockquote {
  font-family: 'Libre Baskerville', serif;
  font-style: italic;
  font-size: 1.15rem;
  line-height: 1.8;
  color: var(--noir-gray-light);
  border-left: 3px solid var(--noir-accent);
  padding-left: 1.5rem;
  margin: 2rem 0;
}
```

---

## Layout Principles

- **Dark canvas as default**: The background should always be deep black or near-black; Film Noir is fundamentally a dark aesthetic -- light backgrounds break the illusion entirely
- **Cinematic aspect ratios**: Hero sections and image containers should favor wide, letterboxed proportions (16:9, 2.35:1) that evoke the movie screen and create horizontal dramatic tension
- **Vignette framing**: Apply dark radial gradients to page edges, creating a natural focus toward the center of the viewport -- the viewer is always looking through a frame into a scene
- **Layered depth through overlapping elements**: Stack translucent overlays, shadow layers, and content panels to create a sense of atmospheric depth, as if peering through smoke-filled rooms
- **Asymmetric compositions with weighted anchors**: Place primary content off-center, weighted to one side, with dramatic negative space on the other -- like a figure standing in a pool of light on one side of a dark room
- **Vertical rhythm through light and shadow**: Alternate between lighter content sections and darker transitional zones to create the effect of moving between pools of light in a dark environment
- **Generous vertical spacing**: Allow sections to breathe with ample padding; Film Noir is not about density but about mood, tension, and the dramatic pause between revelations
- **Single-column narrative flow**: The content should unfold like a story -- one scene after another, scrolling downward through the narrative, rather than spreading across complex multi-column grids

---

## CSS / Design Techniques

### Noir Card Component

A content card with dramatic shadow, subtle border glow, and atmospheric depth -- like a case file pulled from a dark filing cabinet.

```css
.noir-card {
  background-color: var(--noir-black-surface);
  border: 1px solid var(--noir-gray-dark);
  padding: 2rem;
  position: relative;
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  box-shadow:
    0 4px 20px rgba(0, 0, 0, 0.5),
    0 0 1px rgba(212, 168, 71, 0.1);
}

.noir-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--noir-amber), transparent);
  opacity: 0;
  transition: opacity 0.3s ease;
}

.noir-card:hover {
  transform: translateY(-2px);
  box-shadow:
    0 8px 40px rgba(0, 0, 0, 0.7),
    0 0 20px rgba(212, 168, 71, 0.05);
}

.noir-card:hover::before {
  opacity: 1;
}

.noir-card h3 {
  font-family: 'Playfair Display', serif;
  font-size: 1.4rem;
  color: var(--noir-white-cream);
  margin-bottom: 0.75rem;
}

.noir-card p {
  color: var(--noir-gray-light);
  font-size: 0.95rem;
  line-height: 1.7;
}

.noir-card .meta {
  font-family: 'Oswald', sans-serif;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--noir-gray-smoke);
  margin-top: 1.5rem;
  padding-top: 1rem;
  border-top: 1px solid var(--noir-gray-dark);
}
```

### Noir Button Component

Buttons that channel the restrained tension of noir -- understated until activated, with a warm amber glow that suggests danger.

```css
.noir-button {
  display: inline-block;
  font-family: 'Oswald', sans-serif;
  font-size: 0.85rem;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  padding: 0.85rem 2.5rem;
  border: 1px solid var(--noir-amber);
  background-color: transparent;
  color: var(--noir-amber);
  cursor: pointer;
  text-decoration: none;
  position: relative;
  overflow: hidden;
  transition: all 0.3s ease;
}

.noir-button::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background-color: var(--noir-amber);
  transition: left 0.3s ease;
  z-index: -1;
}

.noir-button:hover {
  color: var(--noir-black-void);
  border-color: var(--noir-amber);
}

.noir-button:hover::before {
  left: 0;
}

.noir-button:active {
  background-color: var(--noir-amber-dark);
  border-color: var(--noir-amber-dark);
  transform: scale(0.98);
}

/* Ghost variant -- more subtle, for secondary actions */
.noir-button--ghost {
  border-color: var(--noir-gray-dark);
  color: var(--noir-gray-light);
}

.noir-button--ghost::before {
  background-color: var(--noir-gray-dark);
}

.noir-button--ghost:hover {
  color: var(--noir-white-cream);
}

/* Danger variant -- blood crimson for destructive actions */
.noir-button--danger {
  border-color: var(--noir-crimson);
  color: var(--noir-crimson);
}

.noir-button--danger::before {
  background-color: var(--noir-crimson);
}

.noir-button--danger:hover {
  color: var(--noir-white-cream);
}
```

### Noir Navigation Bar

A top navigation bar that emerges subtly from the darkness, with gold accents and a refined, understated presence.

```css
.noir-nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 3rem;
  background-color: rgba(10, 10, 10, 0.9);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid rgba(61, 61, 61, 0.5);
}

.noir-nav .logo {
  font-family: 'Playfair Display', serif;
  font-weight: 900;
  font-size: 1.3rem;
  color: var(--noir-white-cream);
  text-transform: uppercase;
  letter-spacing: 0.15em;
}

.noir-nav .logo span {
  color: var(--noir-amber);
}

.noir-nav ul {
  list-style: none;
  display: flex;
  gap: 0.5rem;
  margin: 0;
  padding: 0;
}

.noir-nav a {
  display: block;
  font-family: 'Oswald', sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  padding: 0.5rem 1rem;
  color: var(--noir-gray-silver);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: color 0.3s ease, border-color 0.3s ease;
}

.noir-nav a:hover,
.noir-nav a.active {
  color: var(--noir-amber);
  border-bottom-color: var(--noir-amber);
}
```

### Noir Hero Section

A full-viewport cinematic hero with layered atmosphere -- vignette, spotlight, and film grain creating an immersive opening scene.

```css
.noir-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 6rem 4rem;
  background-color: var(--noir-black-void);
  overflow: hidden;
}

/* Spotlight effect -- warm light from upper left */
.noir-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse at 25% 30%,
    rgba(212, 168, 71, 0.06) 0%,
    transparent 50%
  );
  pointer-events: none;
}

/* Vignette overlay -- dark edges */
.noir-hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse at center,
    transparent 30%,
    rgba(10, 10, 10, 0.7) 100%
  );
  pointer-events: none;
}

.noir-hero .content {
  position: relative;
  z-index: 1;
  max-width: 800px;
}

.noir-hero h1 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(3rem, 8vw, 6rem);
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--noir-white-cream);
  line-height: 1.05;
  text-shadow: 0 0 40px rgba(212, 168, 71, 0.15);
}

.noir-hero h1 em {
  font-style: italic;
  color: var(--noir-amber);
  text-shadow: 0 0 30px rgba(212, 168, 71, 0.3);
}

.noir-hero .tagline {
  font-family: 'Oswald', sans-serif;
  font-size: 0.8rem;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.3em;
  color: var(--noir-gray-smoke);
  margin-bottom: 1.5rem;
}

.noir-hero .description {
  font-family: 'Libre Baskerville', serif;
  font-size: 1.1rem;
  line-height: 1.8;
  color: var(--noir-gray-light);
  max-width: 55ch;
  margin-top: 1.5rem;
}

.noir-hero .btn-row {
  display: flex;
  gap: 1rem;
  margin-top: 2.5rem;
}
```

### Venetian Blind Shadow Effect

The signature Film Noir lighting pattern -- horizontal light stripes across a surface simulating light through window blinds.

```css
/* Apply to any container to get the venetian blind stripe overlay */
.venetian-blinds {
  position: relative;
  overflow: hidden;
}

.venetian-blinds::after {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    180deg,
    transparent 0px,
    transparent 18px,
    rgba(0, 0, 0, 0.4) 18px,
    rgba(0, 0, 0, 0.4) 28px
  );
  pointer-events: none;
  z-index: 2;
  /* Angle the blinds slightly for realism */
  transform: rotate(-5deg) scale(1.2);
}

/* Animated version -- slowly shifting light */
.venetian-blinds--animated::after {
  animation: blinds-shift 8s ease-in-out infinite alternate;
}

@keyframes blinds-shift {
  0% {
    transform: rotate(-5deg) scale(1.2) translateY(0);
  }
  100% {
    transform: rotate(-3deg) scale(1.2) translateY(10px);
  }
}

/* Stronger variant for hero images */
.venetian-blinds--strong::after {
  background: repeating-linear-gradient(
    180deg,
    transparent 0px,
    transparent 22px,
    rgba(0, 0, 0, 0.6) 22px,
    rgba(0, 0, 0, 0.6) 36px
  );
}
```

### Smoke / Fog Atmospheric Effect

A layered CSS-only smoke effect using animated pseudo-elements and gradients, creating the haze of a noir interior.

```css
.smoke-overlay {
  position: relative;
  overflow: hidden;
}

.smoke-overlay::before,
.smoke-overlay::after {
  content: '';
  position: absolute;
  width: 200%;
  height: 200%;
  top: -50%;
  left: -50%;
  pointer-events: none;
  z-index: 3;
  opacity: 0.12;
}

/* Primary smoke layer -- slow drift */
.smoke-overlay::before {
  background:
    radial-gradient(ellipse at 20% 50%, rgba(200, 200, 200, 0.3) 0%, transparent 50%),
    radial-gradient(ellipse at 80% 30%, rgba(200, 200, 200, 0.2) 0%, transparent 40%),
    radial-gradient(ellipse at 50% 80%, rgba(200, 200, 200, 0.15) 0%, transparent 45%);
  animation: smoke-drift-1 20s ease-in-out infinite alternate;
}

/* Secondary smoke layer -- counter-drift */
.smoke-overlay::after {
  background:
    radial-gradient(ellipse at 70% 60%, rgba(200, 200, 200, 0.25) 0%, transparent 45%),
    radial-gradient(ellipse at 30% 20%, rgba(200, 200, 200, 0.2) 0%, transparent 50%);
  animation: smoke-drift-2 25s ease-in-out infinite alternate;
}

@keyframes smoke-drift-1 {
  0%   { transform: translate(0, 0) rotate(0deg); }
  100% { transform: translate(5%, -3%) rotate(2deg); }
}

@keyframes smoke-drift-2 {
  0%   { transform: translate(0, 0) rotate(0deg); }
  100% { transform: translate(-4%, 2%) rotate(-1.5deg); }
}
```

### Spotlight / Interrogation Lamp Effect

A dramatic spotlight cone that illuminates a focused area, as if a desk lamp or interrogation light is casting a harsh pool of light.

```css
.spotlight {
  position: relative;
}

.spotlight::before {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse 300px 400px at var(--spotlight-x, 50%) var(--spotlight-y, 30%),
    rgba(245, 245, 240, 0.08) 0%,
    rgba(212, 168, 71, 0.04) 30%,
    transparent 70%
  );
  pointer-events: none;
  z-index: 1;
}

/* Interactive spotlight that follows cursor */
.spotlight--interactive {
  /* Use JS to set --spotlight-x and --spotlight-y */
}

/* Fixed position variants */
.spotlight--top-left::before {
  --spotlight-x: 20%;
  --spotlight-y: 15%;
}

.spotlight--center::before {
  --spotlight-x: 50%;
  --spotlight-y: 40%;
}

.spotlight--bottom-right::before {
  --spotlight-x: 75%;
  --spotlight-y: 70%;
}
```

### Film Grain Texture Overlay

An animated CSS film grain effect that adds the tactile quality of vintage 35mm film stock to any section.

```css
.film-grain {
  position: relative;
  overflow: hidden;
}

.film-grain::after {
  content: '';
  position: absolute;
  inset: -50%;
  width: 200%;
  height: 200%;
  pointer-events: none;
  z-index: 10;
  opacity: 0.04;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='1'/%3E%3C/svg%3E");
  background-size: 256px 256px;
  animation: grain-shift 0.5s steps(4) infinite;
}

@keyframes grain-shift {
  0%   { transform: translate(0, 0); }
  25%  { transform: translate(-5%, -5%); }
  50%  { transform: translate(5%, 0); }
  75%  { transform: translate(0, 5%); }
  100% { transform: translate(-5%, 5%); }
}

/* Heavier grain for hero images */
.film-grain--heavy::after {
  opacity: 0.08;
}

/* Subtle grain for content areas */
.film-grain--subtle::after {
  opacity: 0.02;
  animation: none;
}
```

### CSS Rain Effect

Animated diagonal rain streaks for atmospheric noir backgrounds, purely CSS-driven.

```css
.rain {
  position: relative;
  overflow: hidden;
}

.rain::before,
.rain::after {
  content: '';
  position: absolute;
  top: -100%;
  left: 0;
  right: 0;
  bottom: 0;
  pointer-events: none;
  z-index: 5;
}

.rain::before {
  background: repeating-linear-gradient(
    100deg,
    transparent,
    transparent 97%,
    rgba(200, 200, 220, 0.07) 97%,
    rgba(200, 200, 220, 0.07) 97.5%,
    transparent 97.5%
  );
  background-size: 30px 100%;
  animation: rain-fall-1 0.8s linear infinite;
}

.rain::after {
  background: repeating-linear-gradient(
    97deg,
    transparent,
    transparent 98%,
    rgba(200, 200, 220, 0.05) 98%,
    rgba(200, 200, 220, 0.05) 98.3%,
    transparent 98.3%
  );
  background-size: 50px 100%;
  animation: rain-fall-2 1.1s linear infinite;
}

@keyframes rain-fall-1 {
  0%   { transform: translateY(0); }
  100% { transform: translateY(50%); }
}

@keyframes rain-fall-2 {
  0%   { transform: translateY(0); }
  100% { transform: translateY(50%); }
}
```

---

## Design Do's and Don'ts

### Do's

- **Commit to darkness**: Make deep black the dominant surface; Film Noir lives in shadow and loses all identity on light backgrounds
- **Use amber and gold as your primary accent**: These warm tones evoke streetlights, neon signs, and whiskey -- the luminous punctuation marks of the noir visual world
- **Layer atmospheric effects**: Combine grain, smoke, vignette, and spotlight overlays to build immersive depth; a single flat dark background is not noir, it is just dark
- **Let typography carry dramatic weight**: Headlines should feel like movie title cards -- bold, seriffed, with generous letter-spacing and the authority of a 1940s movie poster
- **Use shadows on everything**: Cards, buttons, text, images -- every element should cast or sit within dramatic shadows that reinforce the lighting-driven aesthetic
- **Embrace negative space as tension**: Dark empty areas are not wasted space; they are the silence between lines of dialogue, the darkness at the edge of the frame
- **Apply venetian blind patterns strategically**: Use the stripe overlay on hero images, section backgrounds, or card headers to instantly signal the noir aesthetic
- **Maintain high text contrast**: Even in a dark design, body text must be clearly legible; use light silver or near-white text (minimum 7:1 contrast ratio) against dark backgrounds
- **Add subtle animation**: Slow-moving smoke, gently shifting grain, pulsing amber glows -- small motions that breathe life into the scene without breaking the somber mood

### Don'ts

- **Don't use bright, saturated colors**: Neon greens, electric blues, hot pinks -- these belong to cyberpunk and synthwave, not Film Noir; keep chromatic accents muted and warm
- **Don't use light or white backgrounds**: A Film Noir design on a white background is a contradiction; the entire aesthetic depends on darkness as the default state
- **Don't over-animate**: Film Noir is slow, deliberate, and brooding; flashy animations, bouncing elements, or rapid transitions destroy the atmospheric tension
- **Don't use rounded, friendly shapes**: Excessive border-radius, bubble elements, and soft organic forms contradict the angular, hard-edged visual language of noir
- **Don't use playful or casual typefaces**: Comic Sans, handwriting fonts, and bouncy display faces have no place in the world of shadows and danger; typography should convey weight and gravity
- **Don't neglect texture**: Flat, untextured dark surfaces look like generic dark mode, not Film Noir; grain, noise, and atmospheric overlays are essential differentiators
- **Don't make everything equally dark**: Without variation in shadow depth and the occasional pool of light, the design becomes a monotonous dark rectangle; contrast between darkness and light is the core principle
- **Don't use emoji or playful iconography**: The visual language should remain cinematic and serious; icons, if used, should be minimal line-art in the style of the period

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Art Deco](Art_Deco.md) | Period contemporary -- Art Deco architecture and design were the visual backdrop of the Film Noir era; both share geometric elegance, gold accents, and dramatic symmetry |
| [Dark Academia](Dark_Academia.md) | Kindred mood of scholarly mystery and atmospheric darkness, though Dark Academia channels libraries and tweed where Noir channels alleys and trench coats |
| [Synthwave](Synthwave.md) | Both are cinematic and neon-inflected, but where Noir is monochrome and restrained, Synthwave explodes into saturated purple and magenta retrofuturism |
| [Gothic](Gothic.md) | Shares the love of darkness, dramatic atmosphere, and moral ambiguity; Gothic tends toward supernatural horror while Noir stays grounded in urban crime and human vice |
| [Dark Mode Neon](Dark_Mode_Neon.md) | Modern dark interfaces with bright accents share structural DNA with Noir, but Neon skews toward technology and cyberpunk where Noir channels the analog past |
| [Monochrome Luxe](Monochrome_Luxe.md) | Both build entire visual systems from black, white, and gray; Monochrome Luxe pursues minimalist elegance while Noir adds atmospheric tension and period narrative |
| [Raw Industrial](Raw_Industrial.md) | Shares the gritty, dark, textured surface quality; Industrial exposes metal and machinery, Noir exposes shadows and moral decay |
| [Terminal CLI Aesthetic](Terminal_CLI_Aesthetic.md) | Both operate in low-light, high-contrast environments; Terminal channels hacker culture while Noir channels detective culture, but the moody atmosphere is shared |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Film Noir Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Oswald:wght@400;500;700&family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,400;1,900&family=Special+Elite&display=swap" rel="stylesheet">
  <style>
    /* --- Custom Properties --- */
    :root {
      --noir-black-void: #0a0a0a;
      --noir-black-surface: #1a1a1a;
      --noir-black-shadow: #2a2a2a;
      --noir-gray-dark: #3d3d3d;
      --noir-gray-smoke: #6b6b6b;
      --noir-gray-silver: #9a9a9a;
      --noir-gray-light: #c8c8c8;
      --noir-white-near: #e8e8e8;
      --noir-white-cream: #f5f5f0;
      --noir-amber: #d4a847;
      --noir-amber-dark: #c19a3e;
      --noir-amber-glow: rgba(212, 168, 71, 0.5);
      --noir-crimson: #8b1a1a;
      --noir-sienna: #a05230;
      --noir-midnight: #1c2833;
    }

    /* --- Reset --- */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    /* --- Base --- */
    body {
      font-family: 'Libre Baskerville', Georgia, serif;
      font-size: 17px;
      line-height: 1.75;
      color: var(--noir-white-near);
      background-color: var(--noir-black-void);
      -webkit-font-smoothing: antialiased;
      overflow-x: hidden;
    }

    /* --- Film Grain (global) --- */
    body::after {
      content: '';
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 9999;
      opacity: 0.035;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
      background-size: 256px 256px;
      animation: grain 0.4s steps(3) infinite;
    }

    @keyframes grain {
      0%   { transform: translate(0, 0); }
      33%  { transform: translate(-3%, -3%); }
      66%  { transform: translate(3%, 1%); }
      100% { transform: translate(1%, -2%); }
    }

    /* --- Navigation --- */
    .nav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 100;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 3rem;
      background: rgba(10, 10, 10, 0.92);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(61, 61, 61, 0.4);
    }

    .nav .logo {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      font-size: 1.2rem;
      color: var(--noir-white-cream);
      text-transform: uppercase;
      letter-spacing: 0.15em;
      text-decoration: none;
    }

    .nav .logo span {
      color: var(--noir-amber);
    }

    .nav ul {
      list-style: none;
      display: flex;
      gap: 0.25rem;
    }

    .nav a {
      display: block;
      font-family: 'Oswald', sans-serif;
      font-size: 0.72rem;
      font-weight: 500;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      padding: 0.5rem 1rem;
      color: var(--noir-gray-silver);
      text-decoration: none;
      border-bottom: 1px solid transparent;
      transition: color 0.3s ease, border-color 0.3s ease;
    }

    .nav a:hover {
      color: var(--noir-amber);
      border-bottom-color: var(--noir-amber);
    }

    /* --- Hero --- */
    .hero {
      position: relative;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 8rem 4rem 6rem;
      overflow: hidden;
    }

    /* Spotlight */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(
        ellipse at 20% 35%,
        rgba(212, 168, 71, 0.06) 0%,
        transparent 55%
      );
      pointer-events: none;
    }

    /* Vignette */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(
        ellipse at center,
        transparent 25%,
        rgba(10, 10, 10, 0.75) 100%
      );
      pointer-events: none;
    }

    /* Venetian blind overlay on hero */
    .hero-blinds {
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        180deg,
        transparent 0px,
        transparent 20px,
        rgba(0, 0, 0, 0.3) 20px,
        rgba(0, 0, 0, 0.3) 32px
      );
      transform: rotate(-4deg) scale(1.3);
      pointer-events: none;
      z-index: 1;
      animation: blinds-drift 10s ease-in-out infinite alternate;
    }

    @keyframes blinds-drift {
      0%   { transform: rotate(-4deg) scale(1.3) translateY(0); }
      100% { transform: rotate(-2.5deg) scale(1.3) translateY(8px); }
    }

    .hero .content {
      position: relative;
      z-index: 2;
      max-width: 750px;
    }

    .hero .tagline {
      font-family: 'Oswald', sans-serif;
      font-size: 0.75rem;
      font-weight: 500;
      text-transform: uppercase;
      letter-spacing: 0.35em;
      color: var(--noir-gray-smoke);
      margin-bottom: 1.5rem;
    }

    .hero .tagline::before {
      content: '';
      display: inline-block;
      width: 40px;
      height: 1px;
      background: var(--noir-amber);
      vertical-align: middle;
      margin-right: 1rem;
    }

    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2.8rem, 7vw, 5.5rem);
      font-weight: 900;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      line-height: 1.05;
      color: var(--noir-white-cream);
      text-shadow: 0 0 50px rgba(212, 168, 71, 0.1);
    }

    .hero h1 em {
      font-style: italic;
      color: var(--noir-amber);
      text-shadow: 0 0 30px rgba(212, 168, 71, 0.25);
    }

    .hero .description {
      font-size: 1.05rem;
      line-height: 1.85;
      color: var(--noir-gray-light);
      max-width: 52ch;
      margin-top: 2rem;
    }

    .hero .btn-row {
      display: flex;
      gap: 1rem;
      margin-top: 2.5rem;
      flex-wrap: wrap;
    }

    /* --- Buttons --- */
    .btn {
      display: inline-block;
      font-family: 'Oswald', sans-serif;
      font-size: 0.8rem;
      font-weight: 500;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      padding: 0.85rem 2.2rem;
      border: 1px solid var(--noir-amber);
      background: transparent;
      color: var(--noir-amber);
      cursor: pointer;
      text-decoration: none;
      position: relative;
      overflow: hidden;
      transition: color 0.3s ease;
    }

    .btn::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: var(--noir-amber);
      transition: left 0.3s ease;
      z-index: -1;
    }

    .btn:hover {
      color: var(--noir-black-void);
    }

    .btn:hover::before {
      left: 0;
    }

    .btn--ghost {
      border-color: var(--noir-gray-dark);
      color: var(--noir-gray-light);
    }

    .btn--ghost::before {
      background: var(--noir-gray-dark);
    }

    .btn--ghost:hover {
      color: var(--noir-white-cream);
    }

    /* --- Section --- */
    .section {
      position: relative;
      padding: 6rem 4rem;
      border-top: 1px solid var(--noir-gray-dark);
    }

    .section-label {
      font-family: 'Oswald', sans-serif;
      font-size: 0.7rem;
      font-weight: 500;
      text-transform: uppercase;
      letter-spacing: 0.3em;
      color: var(--noir-amber);
      margin-bottom: 1rem;
    }

    .section h2 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2rem, 4.5vw, 3.5rem);
      font-weight: 900;
      color: var(--noir-white-cream);
      letter-spacing: 0.03em;
      margin-bottom: 1.5rem;
      text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
    }

    .section p.lead {
      font-size: 1.05rem;
      color: var(--noir-gray-light);
      max-width: 60ch;
      line-height: 1.85;
    }

    /* --- Card Grid --- */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 1.5rem;
      margin-top: 3rem;
    }

    .card {
      background: var(--noir-black-surface);
      border: 1px solid var(--noir-gray-dark);
      padding: 2rem;
      position: relative;
      overflow: hidden;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow: 0 4px 25px rgba(0, 0, 0, 0.4);
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 2px;
      background: linear-gradient(90deg, transparent, var(--noir-amber), transparent);
      opacity: 0;
      transition: opacity 0.3s ease;
    }

    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 10px 40px rgba(0, 0, 0, 0.6), 0 0 20px rgba(212, 168, 71, 0.04);
    }

    .card:hover::before {
      opacity: 1;
    }

    .card .card-number {
      font-family: 'Playfair Display', serif;
      font-size: 3rem;
      font-weight: 900;
      color: var(--noir-gray-dark);
      line-height: 1;
      margin-bottom: 1rem;
    }

    .card h3 {
      font-family: 'Playfair Display', serif;
      font-size: 1.35rem;
      font-weight: 700;
      color: var(--noir-white-cream);
      margin-bottom: 0.75rem;
      line-height: 1.3;
    }

    .card p {
      color: var(--noir-gray-light);
      font-size: 0.92rem;
      line-height: 1.7;
    }

    .card .meta {
      font-family: 'Oswald', sans-serif;
      font-size: 0.65rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--noir-gray-smoke);
      margin-top: 1.5rem;
      padding-top: 1rem;
      border-top: 1px solid var(--noir-gray-dark);
    }

    /* --- Divider --- */
    .divider {
      display: flex;
      align-items: center;
      gap: 1.5rem;
      margin: 4rem 0;
      padding: 0 4rem;
    }

    .divider::before,
    .divider::after {
      content: '';
      flex: 1;
      height: 1px;
      background: linear-gradient(90deg, transparent, var(--noir-gray-dark), transparent);
    }

    .divider span {
      font-family: 'Playfair Display', serif;
      font-size: 1.2rem;
      color: var(--noir-amber);
      font-style: italic;
    }

    /* --- Testimonial / Quote Block --- */
    .quote-block {
      position: relative;
      padding: 3rem 4rem;
      max-width: 700px;
      margin: 0 auto;
    }

    .quote-block::before {
      content: '\201C';
      font-family: 'Playfair Display', serif;
      font-size: 8rem;
      color: var(--noir-amber);
      opacity: 0.2;
      position: absolute;
      top: -1rem;
      left: 1rem;
      line-height: 1;
    }

    .quote-block blockquote {
      font-family: 'Libre Baskerville', serif;
      font-style: italic;
      font-size: 1.25rem;
      line-height: 1.9;
      color: var(--noir-gray-light);
      border: none;
      padding: 0;
      margin: 0;
    }

    .quote-block cite {
      display: block;
      font-family: 'Oswald', sans-serif;
      font-style: normal;
      font-size: 0.72rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--noir-gray-smoke);
      margin-top: 1.5rem;
    }

    .quote-block cite strong {
      color: var(--noir-amber);
      font-weight: 500;
    }

    /* --- Contact / CTA Section --- */
    .cta-section {
      position: relative;
      padding: 6rem 4rem;
      text-align: center;
      overflow: hidden;
    }

    /* Spotlight on CTA */
    .cta-section::before {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(
        ellipse at 50% 40%,
        rgba(212, 168, 71, 0.05) 0%,
        transparent 60%
      );
      pointer-events: none;
    }

    .cta-section h2 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2rem, 5vw, 4rem);
      font-weight: 900;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--noir-white-cream);
      margin-bottom: 1rem;
    }

    .cta-section p {
      font-size: 1.05rem;
      color: var(--noir-gray-light);
      max-width: 50ch;
      margin: 0 auto 2.5rem;
      line-height: 1.85;
    }

    /* --- Footer --- */
    .footer {
      padding: 3rem 4rem;
      border-top: 1px solid var(--noir-gray-dark);
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 1rem;
    }

    .footer p {
      font-family: 'Oswald', sans-serif;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--noir-gray-smoke);
    }

    .footer a {
      color: var(--noir-gray-silver);
      text-decoration: none;
      font-family: 'Oswald', sans-serif;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      transition: color 0.3s ease;
    }

    .footer a:hover {
      color: var(--noir-amber);
    }

    .footer .footer-links {
      display: flex;
      gap: 2rem;
    }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      .nav {
        padding: 0.75rem 1.5rem;
      }

      .nav ul {
        display: none;
      }

      .hero {
        padding: 7rem 2rem 4rem;
      }

      .section {
        padding: 4rem 2rem;
      }

      .card-grid {
        grid-template-columns: 1fr;
      }

      .quote-block {
        padding: 2rem;
      }

      .divider {
        padding: 0 2rem;
      }

      .cta-section {
        padding: 4rem 2rem;
      }

      .footer {
        padding: 2rem;
        flex-direction: column;
        text-align: center;
      }

      .hero-blinds {
        opacity: 0.5;
      }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="nav">
    <a href="#" class="logo">Shadow<span>&</span>Light</a>
    <ul>
      <li><a href="#cases">Cases</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#testimony">Testimony</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <section class="hero">
    <div class="hero-blinds"></div>
    <div class="content">
      <p class="tagline">Private Investigations</p>
      <h1>Every Shadow<br>Tells a <em>Story</em></h1>
      <p class="description">
        The city never sleeps, and neither do its secrets. In the space between
        streetlight and shadow, truth waits for those willing to look. We find
        what others cannot -- or will not -- see.
      </p>
      <div class="btn-row">
        <a href="#cases" class="btn">View Our Cases</a>
        <a href="#contact" class="btn btn--ghost">Make Contact</a>
      </div>
    </div>
  </section>

  <!-- CASES -->
  <section class="section" id="cases">
    <p class="section-label">Case Files</p>
    <h2>Recent Investigations</h2>
    <p class="lead">
      Each case is a door into darkness. Some doors lead to answers.
      Others lead to more questions. All of them lead somewhere you
      have never been before.
    </p>
    <div class="card-grid">
      <div class="card">
        <div class="card-number">01</div>
        <h3>The Vanishing Heiress</h3>
        <p>A socialite disappears on the eve of her inheritance. The family says she ran. The evidence says otherwise. Three weeks. Two cities. One answer nobody wanted to hear.</p>
        <div class="meta">Status: Closed &bull; Duration: 23 Days</div>
      </div>
      <div class="card">
        <div class="card-number">02</div>
        <h3>Midnight at the Pier</h3>
        <p>A shipping magnate's ledger tells two stories. The one in ink is for the tax man. The one in pencil is for us. Following the money always leads somewhere cold.</p>
        <div class="meta">Status: Closed &bull; Duration: 41 Days</div>
      </div>
      <div class="card">
        <div class="card-number">03</div>
        <h3>The Gilded Frame</h3>
        <p>An art dealer's reputation hangs on a single painting. So does someone's alibi. When provenance becomes evidence, every brushstroke is a potential witness.</p>
        <div class="meta">Status: Active &bull; Duration: Ongoing</div>
      </div>
    </div>
  </section>

  <!-- DIVIDER -->
  <div class="divider">
    <span>&diams;</span>
  </div>

  <!-- ABOUT -->
  <section class="section" id="about">
    <p class="section-label">The Method</p>
    <h2>How We Work</h2>
    <p class="lead">
      We operate in the margins -- the overlooked details, the
      contradictions in testimony, the things people forget they said.
      Patience is not a virtue in this line of work. It is a weapon.
    </p>
  </section>

  <!-- TESTIMONY -->
  <section class="section" id="testimony">
    <p class="section-label">Testimony</p>
    <h2>From the Record</h2>
    <div class="quote-block">
      <blockquote>
        They found what the police had written off in forty-eight hours. I do not
        know how they did it, and frankly, I do not want to know. What matters
        is that the truth came out, and it came out because of them.
      </blockquote>
      <cite><strong>Margaret Caldwell</strong> &mdash; Client, Case No. 1247</cite>
    </div>
  </section>

  <!-- CTA -->
  <section class="section cta-section" id="contact">
    <h2>Need Answers?</h2>
    <p>
      The first conversation is always in confidence.
      The second one depends on what we find.
    </p>
    <a href="#" class="btn">Begin Consultation</a>
  </section>

  <!-- FOOTER -->
  <footer class="footer">
    <p>Shadow & Light Investigations &bull; Est. 1947</p>
    <div class="footer-links">
      <a href="#">Privacy</a>
      <a href="#">Terms</a>
      <a href="#">Archive</a>
    </div>
  </footer>

</body>
</html>
```

---

## Implementation Tips

- **Layer your atmosphere incrementally**: Start with the dark background and typography, then add vignette, then grain, then venetian blinds -- each layer should enhance the mood without overwhelming the content; test readability at each stage
- **Use CSS custom properties for the spotlight position**: Setting `--spotlight-x` and `--spotlight-y` via JavaScript `mousemove` creates an interactive lighting effect where the spotlight follows the cursor, dramatically increasing immersion
- **Optimize grain and smoke animations for performance**: Use `will-change: transform` and `transform: translateZ(0)` on animated overlay layers; avoid animating `opacity` or `background-position` which trigger repaints on every frame
- **Test on OLED and LCD screens**: True black (#0A0A0A) looks different on OLED (pixels off) vs LCD (backlit); consider `#111111` or `#121212` as the base if pure black creates too harsh a contrast on OLED displays
- **Pair with ambient sound for maximum immersion**: If building an interactive experience, consider subtle ambient audio (rain, jazz, distant traffic) triggered on user interaction to complete the multi-sensory noir atmosphere
- **Maintain accessibility despite the dark theme**: Use the `prefers-color-scheme` media query to detect system preferences; consider offering a higher-contrast mode that increases text brightness without losing the noir atmosphere; aim for WCAG AA contrast ratios at minimum
- **Keep the venetian blind effect subtle on mobile**: On smaller screens, dense stripe patterns can create visual vibration and moire effects; reduce opacity or increase stripe spacing on viewports below 768px
