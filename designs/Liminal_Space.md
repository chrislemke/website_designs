# Liminal Space - Design Reference

## Overview

Liminal Space is a digital aesthetic rooted in the unsettling familiarity of transitional, in-between environments devoid of human presence. Derived from the Latin "limen" (threshold), the style captures the eerie quality of places designed for occupancy but found empty -- abandoned malls at 3am, fluorescent-lit office corridors after hours, drained hotel pools, endless airport terminals, and school hallways during summer break. The aesthetic surged in internet culture after the 2019 "Backrooms" phenomenon and draws its visual power from the uncanny valley of architecture: spaces that feel deeply familiar yet profoundly wrong. On the web, Liminal Space design translates this atmosphere through washed-out institutional color palettes, degraded visual quality (noise, blur, compression artifacts), oppressively repetitive layouts, artificial lighting effects, and typography that evokes late-1990s to early-2000s signage systems. The goal is not comfort or usability in the traditional sense, but the cultivation of an ambient unease -- a digital environment that feels like somewhere you have been before, in a dream you cannot quite remember.

---

## Visual Characteristics

### Core Design Traits

- **Absence of human presence**: Layouts and imagery emphasize emptiness and vacancy; hero sections show environments without people, reinforcing the feeling that the viewer is alone in a space designed for crowds
- **Fluorescent lighting simulation**: Backgrounds, overlays, and color treatments mimic the harsh, flat illumination of overhead fluorescent tubes -- slightly green-tinted whites, blown-out highlights, and the absence of natural shadow gradients
- **Institutional material textures**: Surfaces reference the tactile vocabulary of transitional architecture -- drop ceiling tiles, linoleum flooring, commercial carpet patterns, vinyl wallcovering, and laminate countertops, achieved through subtle CSS texture overlays and background patterns
- **Compression artifacts and image degradation**: Intentional visual noise, JPEG compression, slight blur, and low resolution evoke the feeling of images captured on old phone cameras or recovered from forgotten security footage
- **Repetitive geometric patterns**: Corridors, hallways, and gridded ceiling tiles inspire layouts built on monotonous, near-identical repeating modules that stretch toward implied vanishing points
- **Temporal ambiguity**: Design elements avoid clear dating; typography, color, and layout choices blend late-1990s and early-2000s institutional aesthetics to create a timeless-yet-dated atmosphere
- **Liminal depth and perspective**: Strategic use of CSS perspective, gradients, and layered elements creates the illusion of receding hallways and infinite empty rooms
- **Low contrast, desaturated imagery**: Photographs and illustrations are processed to appear faded, slightly overexposed, and drained of vivid color, as if viewed through old glass or remembered imperfectly

### Design Principles

- **Familiarity corrupted**: Every element should feel almost recognizable -- a layout that looks like a building directory, typography that resembles exit signage -- but with subtle wrongness that prevents comfort
- **Emptiness as content**: Negative space is not minimalist refinement; it is the uncomfortable void left by missing people and purpose; whitespace should feel like absence, not elegance
- **Atmosphere over information**: The emotional tone of unease and nostalgia takes priority over clear information hierarchy; users should feel the design before they read it
- **Temporal dislocation**: Mix design cues from different decades (90s web, 2000s institutional, modern CSS) to create an environment that feels unstuck in time
- **Infinite continuation**: Layouts should imply that the space extends beyond the viewport in all directions; avoid definitive endings and clean footers that signal completion
- **Degraded fidelity**: Embrace visual imperfection -- noise overlays, slight misalignment, color banding, and compression textures all contribute to the sense that this digital space is deteriorating or was never quite finished

---

## Color Palette

The Liminal Space palette draws from institutional architecture, fluorescent lighting, and the washed-out memory of transitional environments. Colors are desaturated, slightly sickly, and avoid warmth or vibrancy. The dominant impression should be of artificial light on aging surfaces.

| Swatch | Hex | Role |
|--------|-----|------|
| ![#C8C29D](https://via.placeholder.com/20/C8C29D/C8C29D) | `#C8C29D` | Backrooms yellow -- the iconic mono-yellow of fluorescent-lit wallpaper and aged office walls |
| ![#E8E4D0](https://via.placeholder.com/20/E8E4D0/E8E4D0) | `#E8E4D0` | Institutional cream -- drop ceiling tiles, laminate surfaces, and off-white wall paint |
| ![#D4CDB6](https://via.placeholder.com/20/D4CDB6/D4CDB6) | `#D4CDB6` | Carpet beige -- commercial-grade loop carpet and waiting room upholstery |
| ![#A8B5A2](https://via.placeholder.com/20/A8B5A2/A8B5A2) | `#A8B5A2` | Fluorescent green cast -- the subtle green tint that cheap fluorescent tubes throw on white surfaces |
| ![#7A8B8F](https://via.placeholder.com/20/7A8B8F/7A8B8F) | `#7A8B8F` | Corridor gray-blue -- institutional hallway paint, hospital blues faded by decades of fluorescent exposure |
| ![#4D5A5E](https://via.placeholder.com/20/4D5A5E/4D5A5E) | `#4D5A5E` | Shadow teal -- the dark recesses of empty stairwells and unlit storage rooms |
| ![#2C2E33](https://via.placeholder.com/20/2C2E33/2C2E33) | `#2C2E33` | Void charcoal -- deep darkness beyond the reach of overhead lighting, doorways leading nowhere |
| ![#F5F0E1](https://via.placeholder.com/20/F5F0E1/F5F0E1) | `#F5F0E1` | Blown-out white -- overexposed fluorescent glare on smooth surfaces |
| ![#B8A88A](https://via.placeholder.com/20/B8A88A/B8A88A) | `#B8A88A` | Water stain tan -- aged acoustic tile, ceiling leaks, oxidized fixtures |
| ![#6B7F5E](https://via.placeholder.com/20/6B7F5E/6B7F5E) | `#6B7F5E` | Muted institutional green -- school hallway tiles, hospital corridors, public bathroom surfaces |
| ![#8E7C68](https://via.placeholder.com/20/8E7C68/8E7C68) | `#8E7C68` | Worn laminate brown -- fake wood grain on cafeteria tables and reception desks |
| ![#5C6B8A](https://via.placeholder.com/20/5C6B8A/5C6B8A) | `#5C6B8A` | Pool tile blue -- the unsettling cyan of drained swimming pools and empty water parks lit from below |
| ![#9B9880](https://via.placeholder.com/20/9B9880/9B9880) | `#9B9880` | Concrete neutral -- poured concrete floors, parking garage surfaces, loading dock walls |
| ![#D1C4A1](https://via.placeholder.com/20/D1C4A1/D1C4A1) | `#D1C4A1` | Linoleum gold -- the yellowed, wax-coated institutional floor under buzzing lights |

### CSS Custom Properties

```css
:root {
  /* Core liminal palette */
  --liminal-backrooms-yellow: #c8c29d;
  --liminal-cream: #e8e4d0;
  --liminal-carpet-beige: #d4cdb6;
  --liminal-fluorescent-green: #a8b5a2;
  --liminal-corridor-blue: #7a8b8f;
  --liminal-shadow-teal: #4d5a5e;
  --liminal-void: #2c2e33;
  --liminal-blown-white: #f5f0e1;
  --liminal-stain-tan: #b8a88a;
  --liminal-institutional-green: #6b7f5e;
  --liminal-worn-laminate: #8e7c68;
  --liminal-pool-blue: #5c6b8a;
  --liminal-concrete: #9b9880;
  --liminal-linoleum-gold: #d1c4a1;

  /* Functional tokens */
  --liminal-bg: var(--liminal-cream);
  --liminal-bg-deep: var(--liminal-void);
  --liminal-text: var(--liminal-void);
  --liminal-text-muted: var(--liminal-corridor-blue);
  --liminal-text-faded: var(--liminal-concrete);
  --liminal-border: var(--liminal-carpet-beige);
  --liminal-border-strong: var(--liminal-stain-tan);
  --liminal-accent: var(--liminal-backrooms-yellow);
  --liminal-accent-cool: var(--liminal-pool-blue);
  --liminal-surface: var(--liminal-blown-white);
  --liminal-surface-dark: var(--liminal-shadow-teal);

  /* Lighting effects */
  --liminal-fluorescent-glow: rgba(200, 194, 157, 0.15);
  --liminal-fluorescent-flicker: rgba(168, 181, 162, 0.08);
  --liminal-shadow-fade: rgba(44, 46, 51, 0.4);
}
```

---

## Typography

Liminal Space typography evokes institutional wayfinding systems, emergency exit signage, outdated building directories, and the generic sans-serif faces found on 1990s-2000s office suite default installations. Fonts should feel familiar but slightly off -- clean enough to read, generic enough to be placeless, dated enough to feel like a memory.

### Typeface Characteristics

- **Generic institutional sans-serifs**: Fonts that feel like they belong on hospital floor directories, airport gate displays, and government building signage -- functional, anonymous, and vaguely authoritarian
- **Monospaced fallbacks for system text**: Security camera timestamps, building management readouts, and access control logs use monospaced faces that reference the digital infrastructure of empty buildings
- **Condensed or narrow weights**: Institutional signage often uses condensed faces to fit more text into limited space; this compressed quality adds to the claustrophobic atmosphere
- **Slightly outdated but not retro**: Fonts should not be trendy or deliberately retro; they should simply feel like they were chosen decades ago by a facilities manager and never updated
- **Minimal variation**: Liminal spaces use the same font everywhere -- the same face on the directory, the exit signs, the restroom plaques -- so typographic variety should be extremely limited

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| Inter | 300, 400, 600 | Primary body text -- clean, generic, slightly institutional; its optical sizing creates the anonymous feel of a building directory |
| Roboto Condensed | 300, 400, 700 | Headlines and signage-style text -- the condensed width evokes wayfinding systems and directory boards |
| IBM Plex Mono | 300, 400 | System readouts, timestamps, metadata -- references building management systems and security infrastructure |
| DM Sans | 400, 500, 700 | Secondary body text and navigation -- slightly geometric, slightly generic, slightly forgettable |
| Space Grotesk | 400, 500, 700 | Display text and section headers -- a geometric grotesk that feels like it belongs on a 2003 office building lobby sign |
| Overpass | 300, 400, 600 | Wayfinding and directional text -- originally designed for highway signage, it carries the feeling of transitional infrastructure |
| Share Tech Mono | 400 | Terminal displays, status indicators -- evokes the monochrome screens of building access systems |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Roboto Condensed (700) | Inter (300) | Institutional wayfinding sign above a building directory listing -- authoritative yet anonymous |
| Space Grotesk (700) | DM Sans (400) | Modern office lobby signage with a generic corporate body -- clean but soulless |
| Overpass (600) | IBM Plex Mono (300) | Highway exit sign meets building management terminal -- infrastructure speaking to infrastructure |
| DM Sans (700) | Inter (300) | Generic corporate heading over equally generic body text -- the typographic equivalent of a beige cubicle |
| Space Grotesk (500) | Share Tech Mono (400) | Slightly futuristic directory paired with system readout text -- an empty building that still has power |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@300;400&family=Inter:wght@300;400;600&family=Roboto+Condensed:wght@300;400;700&display=swap');

/* === Base Typography === */
body {
  font-family: 'Inter', 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  font-weight: 300;
  line-height: 1.7;
  color: var(--liminal-text);
  letter-spacing: 0.01em;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Roboto Condensed', 'Arial Narrow', sans-serif;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  line-height: 1.1;
  color: var(--liminal-text);
}

h1 {
  font-size: clamp(2.5rem, 6vw, 5rem);
  letter-spacing: 0.12em;
}

h2 {
  font-size: clamp(1.5rem, 3.5vw, 2.5rem);
  letter-spacing: 0.1em;
}

h3 {
  font-size: clamp(1.1rem, 2vw, 1.5rem);
}

/* Monospaced system text */
.system-text, .timestamp, .meta {
  font-family: 'IBM Plex Mono', 'Courier New', monospace;
  font-size: 0.75rem;
  font-weight: 300;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--liminal-text-muted);
}

a {
  color: var(--liminal-accent-cool);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-color 0.6s ease, color 0.6s ease;
}

a:hover {
  color: var(--liminal-text);
  border-bottom-color: var(--liminal-text-muted);
}

blockquote {
  border-left: 2px solid var(--liminal-border-strong);
  padding: 1rem 1.5rem;
  color: var(--liminal-text-muted);
  font-style: italic;
  background: var(--liminal-fluorescent-glow);
}
```

---

## Layout Principles

### Grid and Structure

- **Corridor-inspired linear layouts**: Primary content flows in a single, elongated column that evokes the experience of walking down an endless hallway; sidebars and multi-column layouts are rare and claustrophobic when used
- **Repetitive grid modules**: Card grids and section layouts use identical, evenly-spaced modules that repeat without variation, mimicking the monotonous regularity of ceiling tiles, floor tiles, and identical doors lining a corridor
- **Vanishing-point perspective**: Where possible, layouts imply depth through CSS perspective transforms or graduated sizing -- elements that shrink toward a focal point suggest receding architecture
- **Generous but oppressive padding**: Sections have significant internal padding, but rather than creating breathing room, the space feels like the emptiness of a vacated room; padding should be uniform and slightly too large
- **Subtle asymmetry**: Layouts are mostly regular but with occasional, barely-perceptible misalignment -- a margin that is 2px off, a border that does not quite connect -- suggesting something is slightly wrong with the space

### Section Organization

- **Entry threshold**: The page opens with a stark, minimal hero that establishes the atmosphere -- a single phrase, a timestamp, or a cryptic institutional notice against a vast empty background
- **Repeating chambers**: Content sections are structured as near-identical containers, each feeling like a room in an infinite sequence; visual differentiation between sections is minimal
- **Transitional corridors**: Between major sections, narrow divider zones with different background colors or subtle texture shifts act as the hallways between rooms
- **System notices and metadata**: Small, monospaced text blocks appear periodically with timestamps, location codes, or procedural language that reference the invisible infrastructure maintaining the empty space
- **No definitive ending**: Footers are minimal or absent; the page should feel like it continues beyond what is visible, or loops back to the beginning

### Responsive Approach

- **Collapse to single corridor**: On mobile, the layout compresses to a single narrow column that heightens the claustrophobic hallway effect
- **Maintain oppressive padding ratios**: Even on small screens, internal padding remains proportionally large to preserve the feeling of emptiness within each section
- **Scale fluorescent overlay effects**: Noise textures and lighting overlays are adjusted for smaller screens to remain subtle rather than overwhelming on reduced viewport areas
- **Preserve repetitive rhythm**: Grid modules collapse from multi-column to single-column but maintain identical spacing and sizing so the repetitive quality persists
- **Reduce perspective effects**: CSS perspective transforms and parallax-like depth cues are simplified on mobile to prevent disorientation and maintain performance

---

## CSS / Design Techniques

### Fluorescent Lighting Overlay

A full-page overlay that simulates the flat, slightly green-tinted wash of institutional fluorescent lighting, with a subtle animated flicker.

```css
.fluorescent-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 1000;
  background: linear-gradient(
    180deg,
    rgba(168, 181, 162, 0.04) 0%,
    rgba(200, 194, 157, 0.06) 50%,
    rgba(168, 181, 162, 0.03) 100%
  );
  animation: fluorescent-flicker 8s ease-in-out infinite;
}

@keyframes fluorescent-flicker {
  0%, 100% { opacity: 1; }
  47% { opacity: 1; }
  48% { opacity: 0.92; }
  49% { opacity: 1; }
  72% { opacity: 1; }
  72.5% { opacity: 0.95; }
  73% { opacity: 1; }
}
```

### Liminal Card

A content card that resembles a notice pinned to a corridor bulletin board or a directory listing in a building lobby -- institutional, flat, and slightly faded.

```css
.liminal-card {
  background-color: var(--liminal-surface);
  border: 1px solid var(--liminal-border);
  padding: 2rem;
  position: relative;
  transition: box-shadow 0.6s ease, border-color 0.6s ease;
}

.liminal-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: linear-gradient(
    90deg,
    var(--liminal-carpet-beige) 0%,
    var(--liminal-backrooms-yellow) 50%,
    var(--liminal-carpet-beige) 100%
  );
  opacity: 0.6;
}

.liminal-card:hover {
  border-color: var(--liminal-border-strong);
  box-shadow: 0 0 30px var(--liminal-fluorescent-glow);
}

.liminal-card .card-label {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.65rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--liminal-text-faded);
  margin-bottom: 1rem;
}

.liminal-card h3 {
  font-size: 1.1rem;
  margin-bottom: 0.75rem;
}

.liminal-card p {
  color: var(--liminal-text-muted);
  font-size: 0.9rem;
}
```

### Liminal Button

A button inspired by institutional signage and elevator call buttons -- flat, bordered, and unadorned, with a slow, eerie hover transition.

```css
.liminal-button {
  display: inline-block;
  font-family: 'Roboto Condensed', sans-serif;
  font-size: 0.8rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  padding: 0.75rem 2rem;
  border: 1px solid var(--liminal-text-muted);
  background-color: transparent;
  color: var(--liminal-text);
  cursor: pointer;
  text-decoration: none;
  position: relative;
  overflow: hidden;
  transition: all 0.8s ease;
}

.liminal-button::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: var(--liminal-fluorescent-glow);
  transition: left 0.8s ease;
}

.liminal-button:hover {
  border-color: var(--liminal-text);
  color: var(--liminal-text);
}

.liminal-button:hover::before {
  left: 0;
}

.liminal-button--filled {
  background-color: var(--liminal-shadow-teal);
  color: var(--liminal-blown-white);
  border-color: var(--liminal-shadow-teal);
}

.liminal-button--filled:hover {
  background-color: var(--liminal-void);
  border-color: var(--liminal-void);
  color: var(--liminal-backrooms-yellow);
}
```

### Navigation Bar

A navigation bar that resembles the wayfinding strip along the top of an institutional corridor wall -- minimal, uppercase, evenly spaced.

```css
.liminal-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1.25rem 3rem;
  border-bottom: 1px solid var(--liminal-border);
  background-color: var(--liminal-surface);
  position: relative;
}

.liminal-nav::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    var(--liminal-backrooms-yellow) 50%,
    transparent 100%
  );
  opacity: 0.3;
}

.liminal-nav .brand {
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 700;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--liminal-text);
}

.liminal-nav ul {
  list-style: none;
  display: flex;
  gap: 0;
  margin: 0;
  padding: 0;
}

.liminal-nav a {
  display: block;
  padding: 0.5rem 1.25rem;
  font-family: 'Inter', sans-serif;
  font-size: 0.7rem;
  font-weight: 400;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--liminal-text-muted);
  text-decoration: none;
  border: none;
  transition: color 0.5s ease, background-color 0.5s ease;
}

.liminal-nav a:hover {
  color: var(--liminal-text);
  background-color: var(--liminal-fluorescent-glow);
}
```

### Hero Section

A vast, empty hero that establishes atmosphere through scale and emptiness, like standing at the end of a long corridor and seeing only space ahead.

```css
.liminal-hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 4rem 3rem;
  position: relative;
  background-color: var(--liminal-bg);
  overflow: hidden;
}

.liminal-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 98px,
      rgba(180, 170, 140, 0.08) 98px,
      rgba(180, 170, 140, 0.08) 100px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 98px,
      rgba(180, 170, 140, 0.08) 98px,
      rgba(180, 170, 140, 0.08) 100px
    );
  pointer-events: none;
}

.liminal-hero::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: radial-gradient(
    ellipse at 50% 40%,
    rgba(200, 194, 157, 0.1) 0%,
    transparent 70%
  );
  pointer-events: none;
}

.liminal-hero h1 {
  font-size: clamp(3rem, 8vw, 7rem);
  letter-spacing: 0.15em;
  position: relative;
  z-index: 1;
}

.liminal-hero .subtitle {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.8rem;
  font-weight: 300;
  letter-spacing: 0.08em;
  color: var(--liminal-text-muted);
  margin-top: 2rem;
  max-width: 50ch;
  line-height: 1.8;
  position: relative;
  z-index: 1;
}

.liminal-hero .timestamp {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.65rem;
  color: var(--liminal-text-faded);
  letter-spacing: 0.12em;
  text-transform: uppercase;
  margin-top: 3rem;
  position: relative;
  z-index: 1;
}
```

### Noise Texture Overlay

A subtle film grain / noise texture applied via CSS to simulate the degraded visual quality of old photographs, security camera footage, or compressed digital images.

```css
.noise-overlay {
  position: fixed;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  pointer-events: none;
  z-index: 999;
  opacity: 0.035;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
  background-repeat: repeat;
  animation: noise-shift 0.5s steps(10) infinite;
}

@keyframes noise-shift {
  0% { transform: translate(0, 0); }
  10% { transform: translate(-5%, -5%); }
  20% { transform: translate(3%, -8%); }
  30% { transform: translate(-8%, 2%); }
  40% { transform: translate(5%, 5%); }
  50% { transform: translate(-3%, 8%); }
  60% { transform: translate(8%, -2%); }
  70% { transform: translate(-5%, 5%); }
  80% { transform: translate(2%, -5%); }
  90% { transform: translate(-2%, 3%); }
  100% { transform: translate(0, 0); }
}
```

### Corridor Section Divider

A horizontal divider between content sections that suggests a doorway or threshold between rooms -- a line of light beneath a closed door.

```css
.corridor-divider {
  width: 100%;
  height: 40px;
  position: relative;
  margin: 0;
  background-color: var(--liminal-carpet-beige);
  overflow: hidden;
}

.corridor-divider::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--liminal-backrooms-yellow),
    var(--liminal-blown-white),
    var(--liminal-backrooms-yellow),
    transparent
  );
  opacity: 0.5;
}

.corridor-divider::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 4px;
  height: 4px;
  background: var(--liminal-stain-tan);
  border-radius: 50%;
  box-shadow: 0 0 8px var(--liminal-backrooms-yellow);
  opacity: 0.4;
}
```

### Repeating Room Grid

A grid of identical content modules that creates the unsettling sense of infinite repetition -- every room looks the same.

```css
.room-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 1px;
  background-color: var(--liminal-border);
  border: 1px solid var(--liminal-border);
}

.room-grid .room {
  background-color: var(--liminal-surface);
  padding: 2.5rem 2rem;
  position: relative;
  transition: background-color 1.2s ease;
}

.room-grid .room::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 60%;
  height: 1px;
  background: var(--liminal-fluorescent-glow);
}

.room-grid .room:hover {
  background-color: var(--liminal-bg);
}

.room-grid .room-number {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.6rem;
  color: var(--liminal-text-faded);
  letter-spacing: 0.2em;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
}

.room-grid .room h3 {
  font-size: 0.95rem;
  letter-spacing: 0.08em;
  margin-bottom: 0.75rem;
}

.room-grid .room p {
  font-size: 0.85rem;
  color: var(--liminal-text-muted);
  line-height: 1.7;
}
```

---

## Design Do's and Don'ts

### Do

- **Use desaturated, institutional color palettes** with yellowed whites, muted greens, and corridor grays that evoke fluorescent-lit transitional architecture
- **Apply subtle noise and grain overlays** to all surfaces to create the impression of degraded visual fidelity and surveillance-camera texture
- **Let emptiness carry emotional weight** by using generous padding and negative space that feels like vacancy rather than minimalist elegance
- **Use slow, eerie transition speeds** (0.6s-1.2s) on hover effects to make interactions feel dreamlike and slightly wrong
- **Reference institutional typography** with generic sans-serifs, condensed wayfinding faces, and small monospaced metadata text
- **Create repetitive, identical modules** in grids and lists that reinforce the sense of infinite, monotonous continuation
- **Simulate fluorescent lighting** through subtle color overlays, blown-out highlights, and the faint green-yellow cast of cheap tube lighting
- **Include system-like metadata** with timestamps, location codes, and procedural language that imply invisible infrastructure
- **Let layouts feel slightly unfinished** -- borders that fade, sections that seem to continue beyond the viewport, footers that barely exist

### Don't

- **Don't use warm, saturated colors** -- vivid oranges, rich reds, and bright yellows destroy the washed-out institutional atmosphere; all colors should feel like they have been under fluorescent light for decades
- **Don't add natural lighting or sunlight effects** -- warm gradients, golden hour tones, and lens flare effects contradict the artificial, enclosed quality of liminal spaces
- **Don't populate layouts with human figures** -- people, avatars, profile photos, and user-generated content featuring faces break the essential emptiness of the aesthetic
- **Don't use playful or rounded typography** -- bubbly fonts, script faces, and heavily stylized display types introduce personality and warmth that liminal spaces lack
- **Don't apply snappy, responsive animations** -- quick transitions, bouncy easing, and springy micro-interactions feel alive and present; liminal design should feel suspended and sluggish
- **Don't create clear visual hierarchies** with bold color contrast -- the flatness and sameness of institutional environments means elements should not compete aggressively for attention
- **Don't use decorative illustrations or icons** -- clean, designed iconography implies intentional craft; liminal spaces feel like they were built by committee and maintained by no one
- **Don't end pages with definitive, well-designed footers** -- comprehensive footer sections with sitemaps, social links, and copyright notices signal a maintained, inhabited digital space

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Dreamcore](Dreamcore.md) | Shares the surreal, nostalgic unease but amplifies it with more overt visual distortion, saturated color bleed, and explicitly dreamlike imagery; Dreamcore is the dream, Liminal Space is the room you wake up in |
| [Weirdcore](Weirdcore.md) | A more aggressively distorted cousin that uses heavy image manipulation, text overlays, and glitch effects; where Liminal Space is subtly wrong, Weirdcore is overtly broken |
| [Mallsoft](Mallsoft.md) | Focuses specifically on the abandoned commercial spaces (malls, food courts, retail) that are a subset of liminal imagery; Mallsoft adds muzak-era nostalgia and consumerist melancholy |
| [Frutiger Aero](Frutiger_Aero.md) | Represents the optimistic, glossy digital aesthetic of the same 2004-2013 era that Liminal Space renders as eerie and abandoned; they are the same spaces viewed with different emotional filters |
| [Poolcore](Poolcore.md) | Isolates the specific liminal quality of empty swimming pools, water parks, and aquatic facilities; a focused branch of the broader Liminal Space family |
| [Vaporwave](Vaporwave.md) | Shares the nostalgic recontextualization of late-capitalist commercial spaces but aestheticizes them through color saturation and gloss rather than desaturation and decay |
| [Dark Aero](Dark_Aero.md) | A moody, desaturated relative that shares the sense of technological environments without human presence but leans more toward sleek digital interfaces than physical architecture |
| [Brutalist Web Design](Brutalist_Web_Design.md) | Both embrace discomfort and reject polished usability, but Brutalism is confrontational and structural while Liminal Space is atmospheric and psychological |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Liminal Space Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@300;400&family=Inter:wght@300;400;600&family=Roboto+Condensed:wght@300;400;700&display=swap" rel="stylesheet">
  <style>
    /* --- Custom Properties --- */
    :root {
      --liminal-backrooms-yellow: #c8c29d;
      --liminal-cream: #e8e4d0;
      --liminal-carpet-beige: #d4cdb6;
      --liminal-fluorescent-green: #a8b5a2;
      --liminal-corridor-blue: #7a8b8f;
      --liminal-shadow-teal: #4d5a5e;
      --liminal-void: #2c2e33;
      --liminal-blown-white: #f5f0e1;
      --liminal-stain-tan: #b8a88a;
      --liminal-institutional-green: #6b7f5e;
      --liminal-worn-laminate: #8e7c68;
      --liminal-pool-blue: #5c6b8a;
      --liminal-concrete: #9b9880;
      --liminal-linoleum-gold: #d1c4a1;

      --liminal-bg: var(--liminal-cream);
      --liminal-text: var(--liminal-void);
      --liminal-text-muted: var(--liminal-corridor-blue);
      --liminal-text-faded: var(--liminal-concrete);
      --liminal-border: var(--liminal-carpet-beige);
      --liminal-border-strong: var(--liminal-stain-tan);
      --liminal-surface: var(--liminal-blown-white);
      --liminal-fluorescent-glow: rgba(200, 194, 157, 0.15);
      --liminal-shadow-fade: rgba(44, 46, 51, 0.4);
    }

    /* --- Reset --- */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    /* --- Base --- */
    body {
      font-family: 'Inter', 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
      font-size: 16px;
      font-weight: 300;
      line-height: 1.7;
      color: var(--liminal-text);
      background-color: var(--liminal-bg);
      -webkit-font-smoothing: antialiased;
    }

    /* --- Fluorescent Overlay --- */
    .fluorescent-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 1000;
      background: linear-gradient(
        180deg,
        rgba(168, 181, 162, 0.04) 0%,
        rgba(200, 194, 157, 0.06) 50%,
        rgba(168, 181, 162, 0.03) 100%
      );
      animation: fluorescent-flicker 8s ease-in-out infinite;
    }

    @keyframes fluorescent-flicker {
      0%, 100% { opacity: 1; }
      47% { opacity: 1; }
      48% { opacity: 0.92; }
      49% { opacity: 1; }
      72% { opacity: 1; }
      72.5% { opacity: 0.95; }
      73% { opacity: 1; }
    }

    /* --- Noise Overlay --- */
    .noise-overlay {
      position: fixed;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      pointer-events: none;
      z-index: 999;
      opacity: 0.03;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
      animation: noise-shift 0.5s steps(10) infinite;
    }

    @keyframes noise-shift {
      0% { transform: translate(0, 0); }
      20% { transform: translate(-5%, -5%); }
      40% { transform: translate(5%, 5%); }
      60% { transform: translate(-3%, 3%); }
      80% { transform: translate(3%, -3%); }
      100% { transform: translate(0, 0); }
    }

    /* --- Typography --- */
    h1, h2, h3, h4, h5, h6 {
      font-family: 'Roboto Condensed', 'Arial Narrow', sans-serif;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      line-height: 1.1;
    }

    a {
      color: var(--liminal-pool-blue);
      text-decoration: none;
      border-bottom: 1px solid transparent;
      transition: border-color 0.6s ease, color 0.6s ease;
    }

    a:hover {
      color: var(--liminal-text);
      border-bottom-color: var(--liminal-text-muted);
    }

    /* --- Navigation --- */
    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1.25rem 3rem;
      border-bottom: 1px solid var(--liminal-border);
      background-color: var(--liminal-surface);
      position: relative;
    }

    .nav::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 1px;
      background: linear-gradient(90deg, transparent 0%, var(--liminal-backrooms-yellow) 50%, transparent 100%);
      opacity: 0.3;
    }

    .nav .brand {
      font-family: 'Roboto Condensed', sans-serif;
      font-weight: 700;
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--liminal-text);
    }

    .nav ul {
      list-style: none;
      display: flex;
      gap: 0;
    }

    .nav a {
      display: block;
      padding: 0.5rem 1.25rem;
      font-size: 0.7rem;
      font-weight: 400;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--liminal-text-muted);
      border-bottom: none;
      transition: color 0.5s ease, background-color 0.5s ease;
    }

    .nav a:hover {
      color: var(--liminal-text);
      background-color: var(--liminal-fluorescent-glow);
    }

    /* --- Hero --- */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 4rem 3rem;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background:
        repeating-linear-gradient(0deg, transparent, transparent 98px, rgba(180,170,140,0.07) 98px, rgba(180,170,140,0.07) 100px),
        repeating-linear-gradient(90deg, transparent, transparent 98px, rgba(180,170,140,0.07) 98px, rgba(180,170,140,0.07) 100px);
      pointer-events: none;
    }

    .hero::after {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: radial-gradient(ellipse at 50% 40%, rgba(200,194,157,0.1) 0%, transparent 70%);
      pointer-events: none;
    }

    .hero h1 {
      font-size: clamp(3rem, 8vw, 7rem);
      letter-spacing: 0.15em;
      position: relative;
      z-index: 1;
    }

    .hero .subtitle {
      font-family: 'IBM Plex Mono', monospace;
      font-size: 0.8rem;
      font-weight: 300;
      letter-spacing: 0.08em;
      color: var(--liminal-text-muted);
      margin-top: 2rem;
      max-width: 55ch;
      line-height: 1.9;
      position: relative;
      z-index: 1;
    }

    .hero .timestamp {
      font-family: 'IBM Plex Mono', monospace;
      font-size: 0.65rem;
      color: var(--liminal-text-faded);
      letter-spacing: 0.12em;
      text-transform: uppercase;
      margin-top: 3rem;
      position: relative;
      z-index: 1;
    }

    .hero .btn-row {
      margin-top: 2.5rem;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      position: relative;
      z-index: 1;
    }

    /* --- Buttons --- */
    .btn {
      display: inline-block;
      font-family: 'Roboto Condensed', sans-serif;
      font-size: 0.75rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      padding: 0.75rem 2rem;
      border: 1px solid var(--liminal-text-muted);
      background-color: transparent;
      color: var(--liminal-text);
      cursor: pointer;
      text-decoration: none;
      position: relative;
      overflow: hidden;
      transition: all 0.8s ease;
    }

    .btn::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: var(--liminal-fluorescent-glow);
      transition: left 0.8s ease;
    }

    .btn:hover {
      border-color: var(--liminal-text);
      border-bottom: 1px solid var(--liminal-text);
    }

    .btn:hover::before {
      left: 0;
    }

    .btn--filled {
      background-color: var(--liminal-shadow-teal);
      color: var(--liminal-blown-white);
      border-color: var(--liminal-shadow-teal);
    }

    .btn--filled:hover {
      background-color: var(--liminal-void);
      border-color: var(--liminal-void);
      color: var(--liminal-backrooms-yellow);
    }

    /* --- Corridor Divider --- */
    .corridor-divider {
      width: 100%;
      height: 40px;
      position: relative;
      background-color: var(--liminal-carpet-beige);
      overflow: hidden;
    }

    .corridor-divider::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 10%;
      right: 10%;
      height: 1px;
      background: linear-gradient(90deg, transparent, var(--liminal-backrooms-yellow), var(--liminal-blown-white), var(--liminal-backrooms-yellow), transparent);
      opacity: 0.5;
    }

    /* --- Content Section --- */
    .content-section {
      padding: 5rem 3rem;
      max-width: 900px;
      margin: 0 auto;
    }

    .content-section h2 {
      font-size: clamp(1.5rem, 3.5vw, 2.5rem);
      letter-spacing: 0.1em;
      margin-bottom: 1rem;
    }

    .content-section .section-meta {
      font-family: 'IBM Plex Mono', monospace;
      font-size: 0.65rem;
      color: var(--liminal-text-faded);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      margin-bottom: 2.5rem;
    }

    .content-section p {
      margin-bottom: 1.5rem;
      color: var(--liminal-text-muted);
      max-width: 65ch;
    }

    /* --- Room Grid --- */
    .room-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 1px;
      background-color: var(--liminal-border);
      border: 1px solid var(--liminal-border);
      margin: 3rem 0;
    }

    .room {
      background-color: var(--liminal-surface);
      padding: 2.5rem 2rem;
      position: relative;
      transition: background-color 1.2s ease;
    }

    .room::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 60%;
      height: 1px;
      background: var(--liminal-fluorescent-glow);
    }

    .room:hover {
      background-color: var(--liminal-bg);
    }

    .room .room-number {
      font-family: 'IBM Plex Mono', monospace;
      font-size: 0.6rem;
      color: var(--liminal-text-faded);
      letter-spacing: 0.2em;
      text-transform: uppercase;
      margin-bottom: 1.5rem;
    }

    .room h3 {
      font-size: 0.95rem;
      letter-spacing: 0.08em;
      margin-bottom: 0.75rem;
    }

    .room p {
      font-size: 0.85rem;
      color: var(--liminal-text-muted);
      line-height: 1.7;
    }

    /* --- Liminal Card --- */
    .card {
      background-color: var(--liminal-surface);
      border: 1px solid var(--liminal-border);
      padding: 2rem;
      margin-bottom: 1.5rem;
      position: relative;
      transition: box-shadow 0.6s ease, border-color 0.6s ease;
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0;
      height: 3px;
      background: linear-gradient(90deg, var(--liminal-carpet-beige) 0%, var(--liminal-backrooms-yellow) 50%, var(--liminal-carpet-beige) 100%);
      opacity: 0.6;
    }

    .card:hover {
      border-color: var(--liminal-border-strong);
      box-shadow: 0 0 30px var(--liminal-fluorescent-glow);
    }

    .card .card-label {
      font-family: 'IBM Plex Mono', monospace;
      font-size: 0.65rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--liminal-text-faded);
      margin-bottom: 1rem;
    }

    .card h3 {
      font-size: 1.1rem;
      margin-bottom: 0.75rem;
    }

    .card p {
      color: var(--liminal-text-muted);
      font-size: 0.9rem;
    }

    /* --- System Notice --- */
    .system-notice {
      font-family: 'IBM Plex Mono', monospace;
      font-size: 0.7rem;
      color: var(--liminal-text-faded);
      letter-spacing: 0.06em;
      padding: 1.5rem 3rem;
      border-top: 1px solid var(--liminal-border);
      border-bottom: 1px solid var(--liminal-border);
      background: repeating-linear-gradient(
        90deg,
        transparent 0px,
        transparent 4px,
        rgba(200, 194, 157, 0.03) 4px,
        rgba(200, 194, 157, 0.03) 5px
      );
      text-align: center;
      text-transform: uppercase;
    }

    /* --- Blockquote --- */
    blockquote {
      border-left: 2px solid var(--liminal-border-strong);
      padding: 1rem 1.5rem;
      color: var(--liminal-text-muted);
      font-style: italic;
      background: var(--liminal-fluorescent-glow);
      margin: 2rem 0;
    }

    /* --- Footer --- */
    .footer {
      padding: 3rem;
      text-align: center;
      font-family: 'IBM Plex Mono', monospace;
      font-size: 0.6rem;
      color: var(--liminal-text-faded);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      border-top: 1px solid var(--liminal-border);
      opacity: 0.6;
    }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      .nav {
        flex-direction: column;
        gap: 1rem;
        padding: 1rem 1.5rem;
      }

      .nav ul {
        flex-wrap: wrap;
        justify-content: center;
      }

      .hero {
        padding: 3rem 1.5rem;
        min-height: 90vh;
      }

      .hero h1 {
        letter-spacing: 0.08em;
      }

      .content-section {
        padding: 3rem 1.5rem;
      }

      .room-grid {
        grid-template-columns: 1fr;
      }

      .system-notice {
        padding: 1rem 1.5rem;
        font-size: 0.6rem;
      }
    }
  </style>
</head>
<body>

  <!-- Atmospheric overlays -->
  <div class="fluorescent-overlay"></div>
  <div class="noise-overlay"></div>

  <!-- Navigation -->
  <nav class="nav">
    <div class="brand">Level 0</div>
    <ul>
      <li><a href="#threshold">Threshold</a></li>
      <li><a href="#rooms">Rooms</a></li>
      <li><a href="#corridors">Corridors</a></li>
      <li><a href="#notices">Notices</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero" id="threshold">
    <h1>You have been<br>here before</h1>
    <p class="subtitle">
      A place between places. Not a destination but a passage --
      the hallway you walk through without noticing, the room
      you remember but cannot find on any floor plan.
      Somewhere the lights are still on.
    </p>
    <p class="timestamp">Facility status: nominal &mdash; Sector 7-G &mdash; Last inspection: unknown</p>
    <div class="btn-row">
      <a href="#rooms" class="btn">Enter</a>
      <a href="#corridors" class="btn btn--filled">Continue</a>
    </div>
  </section>

  <!-- Corridor Divider -->
  <div class="corridor-divider"></div>

  <!-- Content Section -->
  <section class="content-section" id="corridors">
    <p class="section-meta">Section 02 // Corridor B-14 // Status: Unoccupied</p>
    <h2>The Space Between</h2>
    <p>
      These are the rooms that exist in the margins of architecture. Designed for
      passage, not permanence. You were never meant to stay here, yet the fluorescent
      lights remain on. The carpet is the same in every direction.
    </p>
    <p>
      The hum of the building systems is the only confirmation that time continues to
      pass. Every door leads to another corridor. Every corridor leads to another room
      identical to the last.
    </p>

    <blockquote>
      You are in a place that was built for thousands and occupied by no one.
      The architecture remembers a purpose you have forgotten.
    </blockquote>

    <!-- Cards -->
    <div class="card">
      <div class="card-label">Notice 2019-04-27 // Classification: Ambient</div>
      <h3>Temporal Displacement Protocol</h3>
      <p>
        If you find yourself in a space you recognize but cannot place, do not
        attempt to retrace your steps. Proceed forward. The exit is always ahead,
        never behind.
      </p>
    </div>

    <div class="card">
      <div class="card-label">Notice 2003-11-15 // Classification: Environmental</div>
      <h3>Fluorescent Maintenance Schedule</h3>
      <p>
        All overhead lighting units in Sectors 4 through 9 are scheduled for
        replacement. Current estimated completion date has been deferred indefinitely.
        Report any flickering to facilities management.
      </p>
    </div>
  </section>

  <!-- System Notice -->
  <div class="system-notice">
    Automated system &mdash; No personnel required &mdash; Monitoring active &mdash; Do not adjust environmental controls
  </div>

  <!-- Room Grid -->
  <section style="padding: 3rem;" id="rooms">
    <div class="room-grid">
      <div class="room">
        <div class="room-number">Room 001</div>
        <h3>Reception Area</h3>
        <p>A desk with no chair. A sign-in sheet with no names. The pen is attached to a chain that leads nowhere.</p>
      </div>
      <div class="room">
        <div class="room-number">Room 002</div>
        <h3>Waiting Room</h3>
        <p>Magazines from a year that may not have happened. The clock on the wall has no hands. Your appointment was scheduled for always.</p>
      </div>
      <div class="room">
        <div class="room-number">Room 003</div>
        <h3>Pool Level</h3>
        <p>The water is still. The diving board casts a shadow with no source. The lifeguard chair faces the wrong direction.</p>
      </div>
      <div class="room">
        <div class="room-number">Room 004</div>
        <h3>Food Court</h3>
        <p>Every restaurant is open. Every menu is the same. The trays on the conveyor belt circle endlessly, carrying nothing.</p>
      </div>
      <div class="room">
        <div class="room-number">Room 005</div>
        <h3>Stairwell B</h3>
        <p>The stairs go up. The stairs also go up. The floor numbers increment by values that are not quite one.</p>
      </div>
      <div class="room">
        <div class="room-number">Room 006</div>
        <h3>Corridor East</h3>
        <p>This hallway is three hundred meters long and contains forty-two identical doors. None of them are locked. All of them open to this hallway.</p>
      </div>
    </div>
  </section>

  <!-- Another divider -->
  <div class="corridor-divider"></div>

  <!-- Final section -->
  <section class="content-section" id="notices">
    <p class="section-meta">Section 04 // Terminal Output // Last Modified: --/--/----</p>
    <h2>Notices</h2>
    <p>
      This facility operates on a maintenance cycle of indeterminate length. All
      systems are functioning within expected parameters. If you are reading this,
      environmental conditions in your sector are stable.
    </p>
    <p>
      There is no cause for concern. Proceed to the nearest exit. The exit is
      located at the end of the corridor. The corridor continues.
    </p>
    <div style="margin-top: 2rem;">
      <a href="#threshold" class="btn">Return to threshold</a>
    </div>
  </section>

  <!-- Footer (deliberately minimal) -->
  <footer class="footer">
    Sector 7-G &mdash; Sublevel -- &mdash; Facility management system v0.0.1 &mdash; Status: operational
  </footer>

</body>
</html>
```
