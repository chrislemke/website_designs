# Terminal / CLI Aesthetic - Design Reference

The Terminal / CLI Aesthetic is a web design style rooted in the visual language of command-line interfaces, text-based computing, and early CRT monitor displays. It celebrates the raw, utilitarian beauty of monospaced type rendered on dark screens -- green phosphor on black, amber characters glowing against the void, blinking cursors awaiting input. The aesthetic draws from Unix terminals, DOS prompts, mainframe consoles, and the hacker culture immortalized in films like WarGames and The Matrix. In modern web design, it translates to stark monochrome palettes, rigid grid structures dictated by character cells, simulated CRT scan lines, phosphor glow effects, and interfaces that feel like they could process a shell command. It is simultaneously retro and timeless, appealing to developers, security professionals, and anyone who finds elegance in the unadorned logic of the command line.

---

## Visual Characteristics

### Core Design Traits

- **Monospaced typography throughout** -- every character occupies the same horizontal space, creating a rigid, grid-like text layout reminiscent of actual terminal emulators
- **Dark backgrounds with luminous text** -- black or near-black canvases with bright foreground text that appears to emit its own light, simulating phosphor display technology
- **Phosphor glow effects** -- text-shadow halos in green, amber, or white that mimic the soft bleed of CRT phosphor coatings
- **CRT scan line overlays** -- faint horizontal lines across the viewport that simulate the raster scanning of cathode ray tube monitors
- **Blinking cursor animations** -- block or underscore cursors that blink at a steady cadence, suggesting an active, waiting terminal session
- **Command-line UI patterns** -- prompts with user@host prefixes, directory paths, piped commands, and ASCII-bordered panels instead of conventional web UI elements
- **ASCII art and box drawing** -- decorative elements, borders, and illustrations constructed entirely from text characters and Unicode box-drawing glyphs
- **Minimal to zero imagery** -- photographs and icons are replaced by ASCII representations or omitted entirely; content is conveyed through text alone
- **Fixed-width grid layouts** -- page structure follows character-cell grids, with columns and spacing measured in character units rather than fluid percentages
- **Screen flicker and noise** -- subtle CSS animations that simulate CRT refresh flicker, static noise, and occasional glitch distortion

### Design Principles

- Content is king -- strip away all visual decoration that does not serve information delivery
- The interface should feel functional and alive, as though it is an active computing session
- Embrace constraints: limited color, fixed-width type, and character-cell grids force creative problem-solving
- Hierarchy is established through color, brightness, and text formatting (bold, underline, inverse) rather than font size variation
- Animation should be purposeful and subtle -- a blinking cursor, a scrolling log, a brief flicker -- never gratuitous
- Whitespace is structured: spacing follows character-cell multiples, not arbitrary pixel values
- Every element should feel as though it could plausibly exist inside a real terminal emulator
- Accessibility remains paramount: despite the aesthetic, text must remain selectable, readable, and navigable

---

## Color Palette

### Phosphor Terminal Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Terminal Black** | `#0C0C0C` | Primary background, deepest terminal void |
| **Soft Black** | `#1A1A1A` | Elevated panels, secondary surfaces, card backgrounds |
| **Dark Gray** | `#2D2D2D` | Borders, dividers, inactive UI elements |
| **Matrix Green** | `#00FF41` | Primary accent, command output text, success states |
| **Phosphor Green** | `#33FF33` | Headings, highlighted text, active elements with glow |
| **Dim Green** | `#0A6E0A` | Secondary text, comments, muted information |
| **Amber Phosphor** | `#FFB000` | Alternate terminal theme, warnings, emphasis |
| **Bright Amber** | `#FFCC00` | Highlighted amber elements, active prompts |
| **CRT White** | `#CCCCCC` | White phosphor theme text, neutral body copy |
| **Bright White** | `#F0F0F0` | High-emphasis text, headings in white-phosphor mode |
| **Error Red** | `#FF3333` | Error messages, fatal output, STDERR text |
| **Cyan Accent** | `#00CCCC` | Links, interactive elements, info-level messages |
| **Pale Blue** | `#5C5CFF` | Directory listings, special file types, decorative |
| **Magenta** | `#CC00CC` | Syntax highlighting, prompt decorations |
| **Scanline Tint** | `rgba(0,255,65,0.03)` | CRT scan line overlay color |
| **Glow Halo** | `rgba(0,255,65,0.4)` | Text-shadow and box-shadow glow spread |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --term-bg-primary: #0c0c0c;
  --term-bg-secondary: #1a1a1a;
  --term-bg-elevated: #2d2d2d;

  /* Green phosphor theme */
  --term-green: #00ff41;
  --term-green-bright: #33ff33;
  --term-green-dim: #0a6e0a;

  /* Amber phosphor theme */
  --term-amber: #ffb000;
  --term-amber-bright: #ffcc00;

  /* White phosphor theme */
  --term-white: #cccccc;
  --term-white-bright: #f0f0f0;

  /* ANSI-style accents */
  --term-red: #ff3333;
  --term-cyan: #00cccc;
  --term-blue: #5c5cff;
  --term-magenta: #cc00cc;

  /* Glow effects (text-shadow / box-shadow) */
  --term-glow-green: 0 0 5px rgba(0, 255, 65, 0.4), 0 0 20px rgba(0, 255, 65, 0.1);
  --term-glow-amber: 0 0 5px rgba(255, 176, 0, 0.4), 0 0 20px rgba(255, 176, 0, 0.1);
  --term-glow-white: 0 0 5px rgba(204, 204, 204, 0.3), 0 0 15px rgba(204, 204, 204, 0.08);

  /* Borders */
  --term-border: 1px solid #2d2d2d;
  --term-border-green: 1px solid rgba(0, 255, 65, 0.25);

  /* Scanline */
  --term-scanline-color: rgba(0, 255, 65, 0.03);
  --term-scanline-size: 2px;
}
```

---

## Typography

### Typeface Characteristics

Terminal / CLI typography is defined by absolute uniformity and mechanical precision:

- **Strictly monospaced** -- every glyph occupies the same width, enabling perfect vertical alignment of columns, tables, and ASCII art
- **No font-size hierarchy for body content** -- headings and body text often share the same size; hierarchy is achieved through color, brightness, prefixes (like `##` or `===`), and text decoration
- **Bitmap-inspired or technically utilitarian** -- fonts should feel engineered for legibility at small sizes on low-resolution displays, not designed for aesthetic beauty
- **Line-height is generous** -- terminal text is easier to scan with comfortable vertical spacing (1.6 to 1.8)
- **No italics in classic mode** -- traditional terminals lacked italic support; emphasis is conveyed through color, brightness, underline, or UPPERCASE

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Fira Code** | Monospace with ligatures | Code blocks, technical content, developer-facing text |
| **IBM Plex Mono** | Clean, corporate monospace | Body text, readable terminal output, professional tone |
| **Source Code Pro** | Adobe's coding font, crisp | Body text, all-purpose terminal content |
| **JetBrains Mono** | Modern developer monospace | Code-heavy layouts, IDE-inspired interfaces |
| **Space Mono** | Retro-futuristic monospace | Headlines, editorial terminal layouts |
| **Share Tech Mono** | Compact, techy | Data readouts, dashboards, compact displays |
| **VT323** | Pixel/bitmap CRT style | Decorative headings, retro authenticity, ASCII art |
| **Press Start 2P** | 8-bit pixel font | Nostalgic accents, game-inspired terminal themes |
| **Courier Prime** | Refined Courier | Classic typewriter-terminal hybrid, literary tone |
| **Ubuntu Mono** | Humanist monospace | Friendly terminal tone, Linux-themed projects |
| **Roboto Mono** | Geometric, balanced | Neutral modern terminal, UI labels |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **VT323** (400) | **Fira Code** (400) | Retro CRT headings with modern readable body |
| **Space Mono** (700) | **IBM Plex Mono** (400) | Editorial hacker aesthetic, polished |
| **Share Tech Mono** (400) | **Source Code Pro** (400) | Compact tech dashboard, data-dense |
| **Press Start 2P** (400) | **VT323** (400) | Full retro pixel aesthetic, nostalgic |
| **JetBrains Mono** (700) | **JetBrains Mono** (400) | Pure developer tool, IDE-inspired |
| **Courier Prime** (700) | **IBM Plex Mono** (400) | Literary-meets-technical, sophisticated |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;700&family=VT323&family=Space+Mono:wght@400;700&display=swap');

/* Base terminal text */
body {
  font-family: 'Fira Code', 'Source Code Pro', 'Courier New', monospace;
  font-size: 15px;
  line-height: 1.7;
  color: var(--term-green);
  -webkit-font-smoothing: none;  /* Disable anti-aliasing for sharper retro feel */
  -moz-osx-font-smoothing: auto;
}

/* Headings -- same font, differentiated by color and prefix */
h1, h2, h3, h4, h5, h6 {
  font-family: 'VT323', 'Fira Code', monospace;
  font-weight: 400;
  color: var(--term-green-bright);
  text-shadow: var(--term-glow-green);
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

h1 { font-size: 2rem; }
h2 { font-size: 1.5rem; }
h3 { font-size: 1.2rem; }

/* Blinking cursor effect */
.cursor::after {
  content: '\2588';  /* Full block character */
  animation: blink 1s step-end infinite;
  color: var(--term-green);
}

@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0; }
}

/* Command prompt styling */
.prompt {
  color: var(--term-green-dim);
}

.prompt::before {
  content: '$ ';
  color: var(--term-cyan);
}

/* Highlighted / bold text (simulated with brightness) */
strong, b {
  font-weight: 700;
  color: var(--term-green-bright);
  text-shadow: var(--term-glow-green);
}

/* Links styled as interactive terminal elements */
a {
  color: var(--term-cyan);
  text-decoration: underline;
  text-underline-offset: 3px;
}

a:hover {
  color: var(--term-green-bright);
  text-shadow: var(--term-glow-green);
}
```

---

## Layout Principles

### Grid and Structure

- **Character-cell grid** -- layout dimensions are ideally multiples of character width and line height, creating alignment reminiscent of actual terminal grids
- **Full-width dark canvas** -- the entire viewport is a single dark background with no white margins or decorative sidebars
- **Single-column primary flow** -- content flows top-to-bottom like terminal output; multi-column layouts are used sparingly and only where they mimic side-by-side terminal panes (like `tmux` splits)
- **Max-width constrained to ~80 characters** -- honoring the traditional 80-column terminal width for the primary content area
- **Fixed padding in character units** -- margins and padding should feel consistent with monospaced character spacing (e.g., 2ch or 4ch)
- **ASCII box-drawing borders** -- panels and sections are bordered using Unicode box-drawing characters or CSS borders styled to look like them
- **No rounded corners** -- everything is rectilinear, sharp, and grid-aligned

### Section Organization

- **Header / Title Bar**: Styled as a terminal window title bar with session name, hostname, and timestamp
- **Navigation**: A list of commands or a prompt-based menu (e.g., `[1] Home  [2] About  [3] Projects  [4] Contact`)
- **Hero / MOTD**: A "Message of the Day" block displayed on login, using ASCII art and introductory text
- **Content Sections**: Terminal output blocks with command prefixes, directory listings, or log-formatted entries
- **Sidebar (optional)**: A second terminal pane displaying system stats, recent activity, or a file tree
- **Footer**: Session info, uptime, or a command prompt inviting the user to continue

### Responsive Approach

- Maintain dark backgrounds at all breakpoints; never introduce light backgrounds on smaller screens
- Reduce max-width from 80ch to fit narrower viewports while preserving monospaced alignment
- Stack side-by-side terminal panes vertically on mobile, simulating tabbed terminal sessions
- Preserve text glow effects but reduce blur radius on low-powered mobile devices
- Font size can decrease slightly but should never go below legibility thresholds for monospaced text (~13px)
- ASCII art may be replaced with simpler text alternatives at narrow widths
- Scan line effects can be disabled on mobile for performance via `prefers-reduced-motion`

---

## CSS / Design Techniques

### Terminal Card / Panel Component

```css
.term-panel {
  background: var(--term-bg-secondary);
  border: 1px solid var(--term-green-dim);
  padding: 20px 24px;
  position: relative;
  font-family: 'Fira Code', monospace;
  color: var(--term-green);
}

/* Title bar */
.term-panel__header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-bottom: 12px;
  margin-bottom: 16px;
  border-bottom: 1px solid var(--term-green-dim);
  font-size: 0.85rem;
  color: var(--term-green-dim);
}

.term-panel__header .title {
  color: var(--term-green-bright);
  text-shadow: var(--term-glow-green);
}

.term-panel:hover {
  border-color: var(--term-green);
  box-shadow: 0 0 8px rgba(0, 255, 65, 0.1);
}

/* Panel grid */
.term-panel-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 16px;
}
```

### Terminal Button

```css
.term-btn {
  display: inline-block;
  background: transparent;
  color: var(--term-green);
  border: 1px solid var(--term-green);
  padding: 8px 24px;
  font-family: 'Fira Code', monospace;
  font-size: 0.9rem;
  cursor: pointer;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  transition: all 0.15s ease;
  position: relative;
}

/* Bracket-style decoration */
.term-btn::before { content: '[ '; }
.term-btn::after { content: ' ]'; }

.term-btn:hover {
  background: var(--term-green);
  color: var(--term-bg-primary);
  box-shadow: var(--term-glow-green);
}

.term-btn:active {
  background: var(--term-green-bright);
}

/* Danger variant */
.term-btn--danger {
  color: var(--term-red);
  border-color: var(--term-red);
}

.term-btn--danger:hover {
  background: var(--term-red);
  color: var(--term-bg-primary);
  box-shadow: 0 0 5px rgba(255, 51, 51, 0.4);
}
```

### Navigation Bar

```css
.term-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 900px;
  margin: 0 auto;
  padding: 12px 24px;
  background: var(--term-bg-primary);
  border-bottom: 1px solid var(--term-green-dim);
  font-family: 'Fira Code', monospace;
  font-size: 0.9rem;
}

.term-nav__host {
  color: var(--term-cyan);
}

.term-nav__host::before {
  content: '';
}

.term-nav__links {
  display: flex;
  gap: 4px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.term-nav__links a {
  color: var(--term-green-dim);
  text-decoration: none;
  padding: 4px 12px;
  transition: color 0.15s, background 0.15s;
}

.term-nav__links a:hover,
.term-nav__links a.active {
  color: var(--term-bg-primary);
  background: var(--term-green);
}

.term-nav__links a::before { content: '['; color: var(--term-green-dim); }
.term-nav__links a::after { content: ']'; color: var(--term-green-dim); }
.term-nav__links a:hover::before,
.term-nav__links a:hover::after { color: var(--term-bg-primary); }
```

### Hero / MOTD Section

```css
.term-hero {
  position: relative;
  padding: 60px 24px;
  max-width: 900px;
  margin: 0 auto;
  text-align: left;
  overflow: hidden;
}

/* CRT scan line overlay */
.term-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent var(--term-scanline-size),
    var(--term-scanline-color) var(--term-scanline-size),
    var(--term-scanline-color) calc(var(--term-scanline-size) * 2)
  );
  pointer-events: none;
  z-index: 2;
}

.term-hero__ascii {
  color: var(--term-green-bright);
  text-shadow: var(--term-glow-green);
  font-size: clamp(0.5rem, 1.5vw, 0.9rem);
  line-height: 1.2;
  margin-bottom: 24px;
  white-space: pre;
  overflow-x: auto;
}

.term-hero__prompt {
  color: var(--term-green);
  font-size: 1rem;
  margin-bottom: 8px;
}

.term-hero__prompt .user { color: var(--term-cyan); }
.term-hero__prompt .path { color: var(--term-magenta); }
.term-hero__prompt .cmd { color: var(--term-green-bright); }

.term-hero__output {
  color: var(--term-green);
  font-size: 0.95rem;
  line-height: 1.7;
  padding-left: 2ch;
  border-left: 2px solid var(--term-green-dim);
  margin-top: 16px;
}
```

### CRT Scan Line and Flicker Effects

```css
/* Full-page scan line overlay */
.crt-overlay {
  position: fixed;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 2px,
    rgba(0, 0, 0, 0.12) 2px,
    rgba(0, 0, 0, 0.12) 4px
  );
  pointer-events: none;
  z-index: 9999;
}

/* Screen flicker animation */
@keyframes flicker {
  0%   { opacity: 0.97; }
  5%   { opacity: 0.95; }
  10%  { opacity: 0.98; }
  15%  { opacity: 0.96; }
  20%  { opacity: 0.99; }
  100% { opacity: 0.98; }
}

.crt-flicker {
  animation: flicker 0.15s infinite;
}

/* Vignette darkening at screen edges */
.crt-vignette::after {
  content: '';
  position: fixed;
  inset: 0;
  background: radial-gradient(
    ellipse at center,
    transparent 60%,
    rgba(0, 0, 0, 0.5) 100%
  );
  pointer-events: none;
  z-index: 9998;
}

/* Disable effects for users who prefer reduced motion */
@media (prefers-reduced-motion: reduce) {
  .crt-flicker { animation: none; }
}
```

### Terminal Input / Command Prompt

```css
.term-input {
  display: flex;
  align-items: center;
  background: var(--term-bg-primary);
  border: 1px solid var(--term-green-dim);
  padding: 12px 16px;
  font-family: 'Fira Code', monospace;
  font-size: 0.95rem;
}

.term-input__prompt {
  color: var(--term-cyan);
  white-space: nowrap;
  margin-right: 8px;
}

.term-input__field {
  flex: 1;
  background: transparent;
  border: none;
  outline: none;
  color: var(--term-green);
  font-family: inherit;
  font-size: inherit;
  caret-color: var(--term-green);
}

.term-input__field::placeholder {
  color: var(--term-green-dim);
}
```

### ASCII Box / Info Panel

```css
.ascii-box {
  font-family: 'Fira Code', monospace;
  color: var(--term-green);
  padding: 16px 20px;
  white-space: pre;
  line-height: 1.4;
  position: relative;
}

/* Top border using box-drawing characters */
.ascii-box::before {
  content: attr(data-title);
  display: block;
  color: var(--term-green-bright);
  text-shadow: var(--term-glow-green);
  margin-bottom: 8px;
  padding-bottom: 8px;
  border-bottom: 1px dashed var(--term-green-dim);
}

/* Log-style entries with timestamps */
.log-entry {
  display: flex;
  gap: 2ch;
  padding: 2px 0;
  font-family: 'Fira Code', monospace;
  font-size: 0.85rem;
}

.log-entry__time {
  color: var(--term-green-dim);
  white-space: nowrap;
}

.log-entry__level--info { color: var(--term-cyan); }
.log-entry__level--warn { color: var(--term-amber); }
.log-entry__level--error { color: var(--term-red); }
.log-entry__message { color: var(--term-green); }
```

### Progress Bar (Text-Based)

```css
.term-progress {
  font-family: 'Fira Code', monospace;
  font-size: 0.9rem;
  color: var(--term-green);
}

.term-progress__bar {
  display: inline-block;
  width: 30ch;
  background: var(--term-bg-secondary);
  border: 1px solid var(--term-green-dim);
  height: 1.2em;
  position: relative;
  overflow: hidden;
  vertical-align: middle;
}

.term-progress__fill {
  height: 100%;
  background: var(--term-green);
  box-shadow: var(--term-glow-green);
  transition: width 0.3s ease;
}

/* Alternative: ASCII progress bar rendered in text */
.term-progress-ascii::before {
  content: '[';
  color: var(--term-green-dim);
}
.term-progress-ascii::after {
  content: ']';
  color: var(--term-green-dim);
}
```

---

## Design Do's and Don'ts

### Do

- Use monospaced fonts exclusively -- they are the foundation of the entire aesthetic
- Apply subtle phosphor glow via `text-shadow` on headings and interactive elements
- Constrain primary content width to 80 characters to honor traditional terminal dimensions
- Use CRT scan line overlays sparingly as atmosphere, not as the dominant visual element
- Employ ASCII art and box-drawing characters for decoration, logos, and section dividers
- Structure navigation as numbered lists, bracket-enclosed links, or command menus
- Create hierarchy through color and brightness rather than dramatically different font sizes
- Include interactive touches like blinking cursors, typing animations, and simulated command output
- Respect `prefers-reduced-motion` by disabling flicker and scan line animations
- Use ANSI-inspired color coding: green for success, red for errors, amber for warnings, cyan for info

### Don't

- Use sans-serif or serif fonts for any visible text -- it immediately breaks the illusion
- Introduce white or light backgrounds -- the terminal is always dark
- Add rounded corners, gradients, or drop shadows -- these belong to modern UI, not terminals
- Use photographs or complex imagery -- the terminal world is text-only
- Over-animate with constant glitching, heavy flicker, or rapid scan lines -- subtlety preserves the effect
- Mix more than one phosphor color theme on the same page (pick green, amber, or white and commit)
- Forget about readability -- phosphor glow should enhance, not obscure the text
- Use wide letter-spacing or decorative text transforms -- terminal text is compact and utilitarian
- Create overly complex multi-column layouts -- terminals are fundamentally single-stream output devices
- Ignore keyboard navigation -- a terminal aesthetic should be fully navigable without a mouse

---

## Related Aesthetics

| Aesthetic | Relationship to Terminal / CLI |
|-----------|-------------------------------|
| **Cyberpunk** | Shares the monospaced type and dark backgrounds, but Cyberpunk adds neon maximalism, glitch effects, and dystopian narrative; Terminal / CLI is austere and utilitarian |
| **8-Bit** | Both reference early computing, but 8-Bit focuses on pixel art and game culture while Terminal / CLI centers on text-based interfaces |
| **Brutalist Web Design** | Shares the raw, undecorated philosophy and rejection of conventional polish; Brutalist is broader in scope while Terminal / CLI is specifically computer-themed |
| **Dark Mode Neon** | Both use dark backgrounds with luminous accents; Dark Mode Neon is a modern UI pattern while Terminal / CLI is a specific retro-computing aesthetic |
| **Cyberminimalism** | Shares the reductive approach and dark palette; Cyberminimalism is a contemporary design trend while Terminal / CLI has roots in actual computing history |
| **Early Cyber** | Both draw from 1990s internet and hacker culture; Early Cyber is broader, encompassing early web design and digital art |
| **Synthwave** | Shares the retro-tech nostalgia and neon-on-dark colors; Synthwave is rooted in 1980s music culture while Terminal / CLI is rooted in computing |
| **Material Design** | The philosophical opposite -- Material Design uses depth, color, motion, and richness; Terminal / CLI rejects all of these in favor of text purity |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>~/terminal</title>
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;700&family=VT323&display=swap" rel="stylesheet">
  <style>
    :root {
      --term-bg: #0c0c0c;
      --term-bg-alt: #1a1a1a;
      --term-border: #2d2d2d;
      --term-green: #00ff41;
      --term-green-bright: #33ff33;
      --term-green-dim: #0a6e0a;
      --term-amber: #ffb000;
      --term-red: #ff3333;
      --term-cyan: #00cccc;
      --term-magenta: #cc00cc;
      --term-white: #cccccc;
      --term-glow: 0 0 5px rgba(0,255,65,0.4), 0 0 20px rgba(0,255,65,0.1);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--term-bg);
      color: var(--term-green);
      font-family: 'Fira Code', 'Courier New', monospace;
      font-size: 15px;
      line-height: 1.7;
      min-height: 100vh;
      position: relative;
    }

    /* CRT Scan Lines */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background: repeating-linear-gradient(
        0deg,
        transparent,
        transparent 2px,
        rgba(0,0,0,0.1) 2px,
        rgba(0,0,0,0.1) 4px
      );
      pointer-events: none;
      z-index: 9999;
    }

    /* CRT Vignette */
    body::after {
      content: '';
      position: fixed;
      inset: 0;
      background: radial-gradient(ellipse at center, transparent 65%, rgba(0,0,0,0.4) 100%);
      pointer-events: none;
      z-index: 9998;
    }

    .container {
      max-width: 80ch;
      margin: 0 auto;
      padding: 0 24px;
    }

    /* Navigation */
    nav {
      border-bottom: 1px solid var(--term-border);
      padding: 12px 0;
    }

    nav .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .nav-host {
      color: var(--term-cyan);
      font-size: 0.9rem;
    }

    .nav-host .at { color: var(--term-green-dim); }
    .nav-host .host { color: var(--term-green); }

    .nav-links {
      display: flex;
      gap: 4px;
      list-style: none;
    }

    .nav-links a {
      color: var(--term-green-dim);
      text-decoration: none;
      padding: 2px 10px;
      font-size: 0.9rem;
      transition: color 0.15s, background 0.15s;
    }

    .nav-links a::before { content: '['; }
    .nav-links a::after { content: ']'; }

    .nav-links a:hover,
    .nav-links a.active {
      color: var(--term-bg);
      background: var(--term-green);
    }

    .nav-links a:hover::before,
    .nav-links a:hover::after,
    .nav-links a.active::before,
    .nav-links a.active::after {
      color: var(--term-bg);
    }

    /* Hero / MOTD */
    .hero {
      padding: 48px 0 40px;
      border-bottom: 1px dashed var(--term-border);
    }

    .ascii-art {
      color: var(--term-green-bright);
      text-shadow: var(--term-glow);
      font-size: clamp(0.45rem, 1.4vw, 0.8rem);
      line-height: 1.15;
      white-space: pre;
      overflow-x: auto;
      margin-bottom: 24px;
      font-family: 'Fira Code', monospace;
    }

    .motd {
      background: var(--term-bg-alt);
      border: 1px solid var(--term-border);
      padding: 16px 20px;
      margin-bottom: 20px;
      color: var(--term-white);
      font-size: 0.9rem;
    }

    .motd-label {
      color: var(--term-amber);
      margin-bottom: 8px;
      font-size: 0.8rem;
    }

    .prompt-line {
      margin-top: 16px;
      font-size: 0.95rem;
    }

    .prompt-line .user { color: var(--term-cyan); }
    .prompt-line .at { color: var(--term-green-dim); }
    .prompt-line .host { color: var(--term-magenta); }
    .prompt-line .path { color: var(--term-cyan); }
    .prompt-line .dollar { color: var(--term-white); }
    .prompt-line .cmd { color: var(--term-green-bright); }

    .cursor {
      display: inline-block;
      width: 0.6em;
      height: 1.1em;
      background: var(--term-green);
      vertical-align: text-bottom;
      animation: blink 1s step-end infinite;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    /* Section headings */
    .section-heading {
      font-family: 'VT323', monospace;
      font-size: 1.4rem;
      color: var(--term-green-bright);
      text-shadow: var(--term-glow);
      text-transform: uppercase;
      margin-bottom: 20px;
      padding-bottom: 8px;
      border-bottom: 1px solid var(--term-green-dim);
    }

    .section-heading::before {
      content: '## ';
      color: var(--term-green-dim);
    }

    /* Content sections */
    section {
      padding: 40px 0;
      border-bottom: 1px dashed var(--term-border);
    }

    /* Panels / Cards */
    .panels {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 16px;
      margin-top: 16px;
    }

    .panel {
      background: var(--term-bg-alt);
      border: 1px solid var(--term-border);
      padding: 16px 20px;
      transition: border-color 0.2s;
    }

    .panel:hover {
      border-color: var(--term-green);
    }

    .panel-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      color: var(--term-green-dim);
      font-size: 0.8rem;
      margin-bottom: 12px;
      padding-bottom: 8px;
      border-bottom: 1px dashed var(--term-border);
    }

    .panel-header .title {
      color: var(--term-green-bright);
      text-shadow: var(--term-glow);
    }

    .panel-content {
      color: var(--term-white);
      font-size: 0.9rem;
      line-height: 1.6;
    }

    .panel-content .label {
      color: var(--term-cyan);
    }

    /* System stats table */
    .stats-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.9rem;
      margin-top: 12px;
    }

    .stats-table th {
      text-align: left;
      color: var(--term-cyan);
      padding: 6px 12px;
      border-bottom: 1px solid var(--term-green-dim);
      font-weight: 400;
      font-size: 0.8rem;
      text-transform: uppercase;
    }

    .stats-table td {
      padding: 6px 12px;
      color: var(--term-green);
      border-bottom: 1px solid var(--term-border);
    }

    .stats-table tr:hover td {
      background: rgba(0, 255, 65, 0.03);
    }

    .status-ok { color: var(--term-green-bright); }
    .status-warn { color: var(--term-amber); }
    .status-err { color: var(--term-red); }

    /* Log entries */
    .log-section {
      background: var(--term-bg-alt);
      border: 1px solid var(--term-border);
      padding: 16px 20px;
      margin-top: 16px;
      max-height: 300px;
      overflow-y: auto;
    }

    .log-entry {
      display: flex;
      gap: 2ch;
      font-size: 0.85rem;
      padding: 3px 0;
    }

    .log-time { color: var(--term-green-dim); white-space: nowrap; }
    .log-info { color: var(--term-cyan); }
    .log-warn { color: var(--term-amber); }
    .log-error { color: var(--term-red); }
    .log-msg { color: var(--term-green); }

    /* Progress bars (ASCII style) */
    .progress-row {
      display: flex;
      align-items: center;
      gap: 1ch;
      font-size: 0.85rem;
      margin-bottom: 6px;
    }

    .progress-label {
      color: var(--term-white);
      width: 12ch;
    }

    .progress-bar-ascii {
      color: var(--term-green);
      white-space: nowrap;
    }

    .progress-pct {
      color: var(--term-green-bright);
      width: 5ch;
      text-align: right;
    }

    /* Command output */
    .cmd-block {
      background: var(--term-bg-alt);
      border-left: 2px solid var(--term-green-dim);
      padding: 12px 16px;
      margin: 12px 0;
      font-size: 0.9rem;
    }

    .cmd-block .comment { color: var(--term-green-dim); }
    .cmd-block .output { color: var(--term-white); }
    .cmd-block .highlight { color: var(--term-green-bright); text-shadow: var(--term-glow); }

    /* Buttons */
    .term-btn {
      display: inline-block;
      background: transparent;
      color: var(--term-green);
      border: 1px solid var(--term-green);
      padding: 8px 20px;
      font-family: 'Fira Code', monospace;
      font-size: 0.9rem;
      cursor: pointer;
      transition: all 0.15s;
      text-decoration: none;
      margin-right: 8px;
      margin-top: 12px;
    }

    .term-btn:hover {
      background: var(--term-green);
      color: var(--term-bg);
      box-shadow: var(--term-glow);
    }

    .term-btn--amber {
      color: var(--term-amber);
      border-color: var(--term-amber);
    }

    .term-btn--amber:hover {
      background: var(--term-amber);
      color: var(--term-bg);
      box-shadow: 0 0 5px rgba(255,176,0,0.4);
    }

    /* Directory listing */
    .dir-listing {
      list-style: none;
      font-size: 0.9rem;
    }

    .dir-listing li {
      padding: 2px 0;
    }

    .dir-listing li::before {
      content: '';
      display: inline-block;
      width: 2ch;
    }

    .dir-listing .dir { color: var(--term-cyan); font-weight: 700; }
    .dir-listing .exec { color: var(--term-green-bright); }
    .dir-listing .file { color: var(--term-white); }
    .dir-listing .link { color: var(--term-magenta); }
    .dir-listing .perms { color: var(--term-green-dim); display: inline-block; width: 12ch; }
    .dir-listing .size { color: var(--term-green-dim); display: inline-block; width: 8ch; text-align: right; margin-right: 2ch; }

    /* Contact / Form section */
    .term-form {
      margin-top: 16px;
    }

    .term-form .field {
      margin-bottom: 12px;
    }

    .term-form label {
      color: var(--term-cyan);
      display: block;
      margin-bottom: 4px;
      font-size: 0.85rem;
    }

    .term-form label::after {
      content: ':';
    }

    .term-form input,
    .term-form textarea {
      width: 100%;
      max-width: 50ch;
      background: var(--term-bg-alt);
      border: 1px solid var(--term-border);
      color: var(--term-green);
      font-family: 'Fira Code', monospace;
      font-size: 0.9rem;
      padding: 8px 12px;
      outline: none;
      caret-color: var(--term-green);
    }

    .term-form input:focus,
    .term-form textarea:focus {
      border-color: var(--term-green);
      box-shadow: 0 0 4px rgba(0,255,65,0.15);
    }

    .term-form textarea {
      height: 100px;
      resize: vertical;
    }

    /* Footer */
    footer {
      padding: 24px 0;
      text-align: center;
      color: var(--term-green-dim);
      font-size: 0.8rem;
    }

    footer .separator {
      color: var(--term-border);
      margin-bottom: 12px;
    }

    /* Responsive */
    @media (max-width: 600px) {
      .container { padding: 0 16px; }
      nav .container { flex-direction: column; gap: 8px; }
      .nav-links { flex-wrap: wrap; justify-content: center; }
      .ascii-art { font-size: 0.4rem; }
      .panels { grid-template-columns: 1fr; }
      .dir-listing .perms { display: none; }
      .dir-listing .size { display: none; }
    }

    @media (prefers-reduced-motion: reduce) {
      .cursor { animation: none; opacity: 1; }
      body::before { background: none; }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <div class="container">
      <span class="nav-host"><span class="user">visitor</span><span class="at">@</span><span class="host">sierra</span>:~</span>
      <ul class="nav-links">
        <li><a href="#home" class="active">home</a></li>
        <li><a href="#services">services</a></li>
        <li><a href="#status">status</a></li>
        <li><a href="#logs">logs</a></li>
        <li><a href="#contact">contact</a></li>
      </ul>
    </div>
  </nav>

  <!-- Hero / MOTD -->
  <section class="hero" id="home">
    <div class="container">
      <div class="ascii-art">
 ____  _                         ____                  _
/ ___|(_) ___ _ __ _ __ __ _   / ___|  ___ _ ____   _(_) ___ ___  ___
\___ \| |/ _ \ '__| '__/ _` |  \___ \ / _ \ '__\ \ / / |/ __/ _ \/ __|
 ___) | |  __/ |  | | | (_| |   ___) |  __/ |   \ V /| | (_|  __/\__ \
|____/|_|\___|_|  |_|  \__,_|  |____/ \___|_|    \_/ |_|\___\___||___/
      </div>

      <div class="motd">
        <div class="motd-label">-- Message of the Day --</div>
        Welcome to Sierra Services, a systems administration and infrastructure
        consulting firm. We specialize in Linux server management, network
        security auditing, and high-availability architecture design. All
        sessions are monitored and logged for security purposes.
      </div>

      <div class="prompt-line">
        <span class="user">visitor</span><span class="at">@</span><span class="host">sierra</span>:<span class="path">~</span><span class="dollar">$</span> <span class="cmd">cat /etc/motd</span>
      </div>
      <div class="prompt-line" style="margin-top: 12px;">
        Last login: Tue Feb 17 09:42:31 2026 from 192.168.1.42
      </div>
      <div class="prompt-line" style="margin-top: 4px; color: var(--term-green-dim);">
        System uptime: 142 days, 7:23:15 &nbsp;|&nbsp; Load avg: 0.12, 0.08, 0.05
      </div>
      <div class="prompt-line" style="margin-top: 16px;">
        <span class="user">visitor</span><span class="at">@</span><span class="host">sierra</span>:<span class="path">~</span><span class="dollar">$</span> <span class="cursor"></span>
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services">
    <div class="container">
      <h2 class="section-heading">Services</h2>

      <div class="prompt-line" style="margin-bottom: 16px;">
        <span class="user">visitor</span><span class="at">@</span><span class="host">sierra</span>:<span class="path">~</span><span class="dollar">$</span> <span class="cmd">ls -la /srv/offerings/</span>
      </div>

      <div class="panels">
        <div class="panel">
          <div class="panel-header">
            <span class="title">infrastructure.conf</span>
            <span>-rwxr--r--</span>
          </div>
          <div class="panel-content">
            <span class="label"># Infrastructure Management</span><br><br>
            Bare-metal and cloud server provisioning,
            configuration management with Ansible and
            Terraform, container orchestration via
            Kubernetes. 24/7 monitoring and alerting
            with automated incident response.
          </div>
        </div>

        <div class="panel">
          <div class="panel-header">
            <span class="title">security.conf</span>
            <span>-rwxr--r--</span>
          </div>
          <div class="panel-content">
            <span class="label"># Security Auditing</span><br><br>
            Penetration testing, vulnerability
            assessment, compliance auditing (SOC 2,
            ISO 27001). Network segmentation review,
            firewall rule optimization, and intrusion
            detection system deployment.
          </div>
        </div>

        <div class="panel">
          <div class="panel-header">
            <span class="title">reliability.conf</span>
            <span>-rwxr--r--</span>
          </div>
          <div class="panel-content">
            <span class="label"># High Availability</span><br><br>
            Multi-region failover architecture,
            database replication, load balancing,
            and disaster recovery planning. Targeting
            99.99% uptime SLAs with automated
            health checks and self-healing systems.
          </div>
        </div>

        <div class="panel">
          <div class="panel-header">
            <span class="title">devops.conf</span>
            <span>-rwxr--r--</span>
          </div>
          <div class="panel-content">
            <span class="label"># DevOps Consulting</span><br><br>
            CI/CD pipeline design, GitOps workflows,
            artifact management, and deployment
            automation. We help teams ship faster
            with fewer incidents through robust
            tooling and process optimization.
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- System Status Section -->
  <section id="status">
    <div class="container">
      <h2 class="section-heading">System Status</h2>

      <div class="prompt-line" style="margin-bottom: 16px;">
        <span class="user">visitor</span><span class="at">@</span><span class="host">sierra</span>:<span class="path">~</span><span class="dollar">$</span> <span class="cmd">systemctl status --all</span>
      </div>

      <table class="stats-table">
        <thead>
          <tr>
            <th>Service</th>
            <th>Status</th>
            <th>Uptime</th>
            <th>Port</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>nginx</td>
            <td class="status-ok">[ RUNNING ]</td>
            <td>142d 07:23</td>
            <td>443/tcp</td>
          </tr>
          <tr>
            <td>postgresql</td>
            <td class="status-ok">[ RUNNING ]</td>
            <td>142d 07:22</td>
            <td>5432/tcp</td>
          </tr>
          <tr>
            <td>redis</td>
            <td class="status-ok">[ RUNNING ]</td>
            <td>138d 14:07</td>
            <td>6379/tcp</td>
          </tr>
          <tr>
            <td>prometheus</td>
            <td class="status-ok">[ RUNNING ]</td>
            <td>142d 07:20</td>
            <td>9090/tcp</td>
          </tr>
          <tr>
            <td>backup-agent</td>
            <td class="status-warn">[ DEGRADED ]</td>
            <td>2d 11:45</td>
            <td>--</td>
          </tr>
          <tr>
            <td>legacy-api</td>
            <td class="status-err">[ STOPPED ]</td>
            <td>--</td>
            <td>8080/tcp</td>
          </tr>
        </tbody>
      </table>

      <div style="margin-top: 24px;">
        <p style="color: var(--term-white); margin-bottom: 12px; font-size: 0.9rem;">Resource utilization:</p>
        <div class="progress-row">
          <span class="progress-label">CPU</span>
          <span class="progress-bar-ascii">[##########.............................]</span>
          <span class="progress-pct">23%</span>
        </div>
        <div class="progress-row">
          <span class="progress-label">Memory</span>
          <span class="progress-bar-ascii">[######################.................]</span>
          <span class="progress-pct">57%</span>
        </div>
        <div class="progress-row">
          <span class="progress-label">Disk /</span>
          <span class="progress-bar-ascii">[###############........................]</span>
          <span class="progress-pct">38%</span>
        </div>
        <div class="progress-row">
          <span class="progress-label">Disk /data</span>
          <span class="progress-bar-ascii">[############################...........]</span>
          <span class="progress-pct">71%</span>
        </div>
        <div class="progress-row">
          <span class="progress-label">Network I/O</span>
          <span class="progress-bar-ascii">[####...................................]</span>
          <span class="progress-pct">12%</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Logs Section -->
  <section id="logs">
    <div class="container">
      <h2 class="section-heading">Recent Logs</h2>

      <div class="prompt-line" style="margin-bottom: 16px;">
        <span class="user">visitor</span><span class="at">@</span><span class="host">sierra</span>:<span class="path">~</span><span class="dollar">$</span> <span class="cmd">journalctl -n 12 --no-pager</span>
      </div>

      <div class="log-section">
        <div class="log-entry">
          <span class="log-time">2026-02-18 08:01:12</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">nginx: upstream connection established to 10.0.1.4:8080</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 08:01:09</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">certbot: certificate renewal check passed (expires 2026-04-14)</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 07:58:44</span>
          <span class="log-warn">[WARN]</span>
          <span class="log-msg">backup-agent: retry attempt 3/5 for snapshot upload to s3://vault</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 07:55:01</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">cron: executing scheduled job /etc/cron.d/log-rotate</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 07:45:22</span>
          <span class="log-warn">[WARN]</span>
          <span class="log-msg">backup-agent: connection timeout to storage endpoint (attempt 2/5)</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 07:30:00</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">prometheus: scrape cycle completed, 847 metrics collected</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 07:15:33</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">sshd: accepted publickey for admin from 10.0.0.1 port 52341</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 06:42:18</span>
          <span class="log-error">[ERR ]</span>
          <span class="log-msg">legacy-api: process exited with code 137 (OOM killed)</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 06:42:17</span>
          <span class="log-warn">[WARN]</span>
          <span class="log-msg">kernel: memory cgroup out of memory: legacy-api (pid 28441)</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 06:30:00</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">redis: RDB snapshot saved to disk (2.4MB, 0.003s)</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 06:00:01</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">postgresql: automatic vacuum completed on table 'events' (4201 rows)</span>
        </div>
        <div class="log-entry">
          <span class="log-time">2026-02-18 05:45:09</span>
          <span class="log-info">[INFO]</span>
          <span class="log-msg">ufw: [BLOCK] IN=eth0 SRC=45.33.12.88 DST=10.0.1.2 PROTO=TCP DPT=22</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <div class="container">
      <h2 class="section-heading">Contact</h2>

      <div class="prompt-line" style="margin-bottom: 16px;">
        <span class="user">visitor</span><span class="at">@</span><span class="host">sierra</span>:<span class="path">~</span><span class="dollar">$</span> <span class="cmd">cat /srv/contact.txt</span>
      </div>

      <div class="cmd-block">
        <span class="comment"># Reach us through any of the following channels:</span><br>
        <span class="output">Email .......... ops@sierra-services.io</span><br>
        <span class="output">IRC ............ irc.libera.chat #sierra</span><br>
        <span class="output">PGP Key ........ 0xAB12 CD34 EF56 7890</span><br>
        <span class="output">Response SLA ... &lt; 4 hours (business days)</span>
      </div>

      <p style="margin-top: 20px; color: var(--term-white); font-size: 0.9rem;">Or submit a request directly:</p>

      <form class="term-form" onsubmit="return false;">
        <div class="field">
          <label for="name">name</label>
          <input type="text" id="name" placeholder="your_name">
        </div>
        <div class="field">
          <label for="email">email</label>
          <input type="email" id="email" placeholder="user@domain.tld">
        </div>
        <div class="field">
          <label for="message">message</label>
          <textarea id="message" placeholder="Describe your infrastructure needs..."></textarea>
        </div>
        <button type="submit" class="term-btn">submit</button>
        <button type="reset" class="term-btn--amber term-btn">clear</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <div class="separator">- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -</div>
      <p>Sierra Services | EST 2019 | All sessions logged</p>
      <p style="margin-top: 4px;">PID 1 | TTY pts/0 | ENV production | SHELL /bin/zsh</p>
      <p style="margin-top: 8px; color: var(--term-green-dim);">Connection closed by remote host.</p>
    </div>
  </footer>

</body>
</html>
```
