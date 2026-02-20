# Brutalist Web Design

## Overview

Brutalist Web Design is a raw, confrontational digital aesthetic directly descended from the Brutalist architecture movement of the 1950s-1970s, which celebrated exposed concrete (beton brut) and unadorned structural honesty. On the web, it translates into pages that strip away visual polish, reject conventional UI patterns, and expose the underlying structure of HTML itself as a design feature. Content is presented with minimal CSS intervention -- default fonts, unstyled links, visible document flow, and a deliberate refusal to "beautify" the interface. The philosophy is anti-design: function is the aesthetic, the medium is the message, and ornamentation is considered dishonest. Unlike its descendant Neubrutalism (which re-introduces bold color and thick borders as stylistic flourishes), pure Brutalist Web Design embraces the raw, undecorated, sometimes uncomfortable reality of the document as delivered by the browser. It is the web equivalent of an exposed concrete wall -- honest, stark, and unapologetically functional.

---

## Visual Characteristics

### Core Design Traits

- **Exposed HTML structure**: Pages reveal their underlying document hierarchy with minimal styling, treating raw HTML elements as the primary visual language rather than hiding them behind CSS decoration
- **Monochrome or severely limited palettes**: Black text on white backgrounds dominates, with hyperlink blue (#0000EE) often the only color, echoing the unstyled default browser aesthetic of the early web
- **Monospaced and system fonts**: Typography favors monospaced faces (Courier, monospace system stacks) or basic system sans-serifs, rejecting the curated font pairings of modern design
- **Dense, text-heavy layouts**: Pages prioritize content density over whitespace, with long columns of text, lists, and links presented without visual relief or decorative imagery
- **Intentional visual discomfort**: Clashing sizes, misaligned elements, jarring color contrasts, and unconventional layouts are deployed deliberately to challenge user expectations
- **Absence of imagery and icons**: Photography, illustrations, and iconography are minimized or eliminated entirely; when images appear, they are often unstyled, full-width, or crudely placed
- **Visible borders and gridlines**: Structural dividers like `<hr>` tags, table borders, and CSS outlines are left visible or exaggerated, making the page's skeleton apparent to the viewer

### Design Principles

- **Function dictates form**: Every element exists to serve a purpose; decoration that does not communicate information is removed
- **Structural honesty**: The underlying HTML document structure should be visible and comprehensible; hiding complexity behind smooth surfaces is considered dishonest
- **Rejection of convention**: Brutalist design deliberately breaks accepted UI/UX patterns (centered layouts, hamburger menus, hero images) to provoke thought about why those conventions exist
- **Content supremacy**: Text content is the primary interface element; navigation, branding, and chrome are subordinated to the words on the page
- **Performance as ethics**: Minimal CSS, no JavaScript frameworks, few or no images -- the resulting speed and accessibility are not side effects but core values of the approach

---

## Color Palette

Brutalist Web Design draws from two traditions: the stark monochromes of raw concrete architecture, and the default browser colors of the unstyled early web. Palettes are intentionally limited, high-contrast, and avoid harmonious relationships.

| Swatch | Hex | Role |
|--------|-----|------|
| ![#000000](https://via.placeholder.com/20/000000/000000) | `#000000` | Primary text, borders, structural elements |
| ![#FFFFFF](https://via.placeholder.com/20/FFFFFF/FFFFFF) | `#FFFFFF` | Default background, negative space |
| ![#C0C0C0](https://via.placeholder.com/20/C0C0C0/C0C0C0) | `#C0C0C0` | Secondary background, table cells, dividers |
| ![#808080](https://via.placeholder.com/20/808080/808080) | `#808080` | Muted text, disabled states, metadata |
| ![#0000EE](https://via.placeholder.com/20/0000EE/0000EE) | `#0000EE` | Default hyperlink blue, primary interactive color |
| ![#551A8B](https://via.placeholder.com/20/551A8B/551A8B) | `#551A8B` | Visited link purple, secondary interactive color |
| ![#FF0000](https://via.placeholder.com/20/FF0000/FF0000) | `#FF0000` | Accent, warnings, aggressive highlights |
| ![#FFFF00](https://via.placeholder.com/20/FFFF00/FFFF00) | `#FFFF00` | Highlight marker, attention callouts |
| ![#00FF00](https://via.placeholder.com/20/00FF00/00FF00) | `#00FF00` | Terminal green, success states, hacker aesthetic |
| ![#0000FF](https://via.placeholder.com/20/0000FF/0000FF) | `#0000FF` | Pure blue accent, bold structural color blocks |
| ![#333333](https://via.placeholder.com/20/333333/333333) | `#333333` | Dark background variant, near-black surfaces |
| ![#F0F0F0](https://via.placeholder.com/20/F0F0F0/F0F0F0) | `#F0F0F0` | Light gray background, subtle section differentiation |

### CSS Custom Properties

```css
:root {
  /* Core monochrome */
  --brutal-black: #000000;
  --brutal-white: #ffffff;
  --brutal-gray-light: #f0f0f0;
  --brutal-gray-mid: #c0c0c0;
  --brutal-gray-dark: #808080;
  --brutal-near-black: #333333;

  /* Browser-default interactive colors */
  --brutal-link: #0000ee;
  --brutal-visited: #551a8b;

  /* Raw accent colors (web-safe primaries) */
  --brutal-red: #ff0000;
  --brutal-yellow: #ffff00;
  --brutal-green: #00ff00;
  --brutal-blue: #0000ff;

  /* Functional tokens */
  --brutal-bg: var(--brutal-white);
  --brutal-text: var(--brutal-black);
  --brutal-border: var(--brutal-black);
  --brutal-accent: var(--brutal-red);
  --brutal-highlight: var(--brutal-yellow);
  --brutal-muted: var(--brutal-gray-dark);
}
```

---

## Typography

Brutalist Web Design treats typography as the primary (and often only) design element. Fonts are chosen for their rawness, mechanical quality, or association with code and early computing. Oversized headings, monospaced body text, and system font stacks are all hallmarks of the style.

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| Space Mono | 400, 700 | Body text, code blocks, monospaced layouts | [fonts.google.com/specimen/Space+Mono](https://fonts.google.com/specimen/Space+Mono) |
| Darker Grotesque | 400, 700, 900 | Headlines, display text, oversized titles | [fonts.google.com/specimen/Darker+Grotesque](https://fonts.google.com/specimen/Darker+Grotesque) |
| IBM Plex Mono | 400, 500, 700 | Body text, technical content, metadata | [fonts.google.com/specimen/IBM+Plex+Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) |
| Inter | 400, 700, 900 | Clean sans-serif body, UI elements, navigation | [fonts.google.com/specimen/Inter](https://fonts.google.com/specimen/Inter) |
| Archivo Black | 400 | Impact headlines, all-caps display text | [fonts.google.com/specimen/Archivo+Black](https://fonts.google.com/specimen/Archivo+Black) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Archivo Black | Space Mono | Heavy industrial impact meets typewriter rawness |
| Darker Grotesque (900) | IBM Plex Mono | Stretched grotesque headings with technical monospace precision |
| Inter (900) | Space Mono | Clean geometric authority paired with mechanical rhythm |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Archivo+Black&family=Space+Mono:wght@400;700&display=swap');

/* === Base Typography === */
body {
  font-family: 'Space Mono', 'Courier New', Courier, monospace;
  font-size: 16px;
  line-height: 1.6;
  color: var(--brutal-text);
  background-color: var(--brutal-bg);
  -webkit-font-smoothing: none; /* Deliberately disable anti-aliasing for raw feel */
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Archivo Black', 'Impact', 'Arial Black', sans-serif;
  text-transform: uppercase;
  letter-spacing: -0.02em;
  line-height: 1.0;
  margin: 0 0 0.5em 0;
}

h1 {
  font-size: clamp(3rem, 8vw, 8rem);
}

h2 {
  font-size: clamp(2rem, 5vw, 4rem);
}

h3 {
  font-size: clamp(1.5rem, 3vw, 2.5rem);
}

a {
  color: var(--brutal-link);
  text-decoration: underline;
}

a:visited {
  color: var(--brutal-visited);
}

a:hover {
  background-color: var(--brutal-highlight);
  color: var(--brutal-black);
}

code, pre {
  font-family: 'Space Mono', 'Courier New', monospace;
  background-color: var(--brutal-gray-light);
  border: 1px solid var(--brutal-black);
  padding: 0.2em 0.4em;
}

pre {
  padding: 1em;
  overflow-x: auto;
  white-space: pre;
}

blockquote {
  border-left: 4px solid var(--brutal-black);
  margin: 1em 0;
  padding: 0.5em 1em;
  background-color: var(--brutal-gray-light);
  font-style: normal;
}
```

---

## Layout Principles

- **Single-column document flow**: Embrace the natural top-to-bottom flow of HTML; avoid complex multi-column grid layouts unless they serve a clear structural purpose like a link directory
- **No centered hero sections**: Content begins immediately at the top-left of the viewport; large centered hero images and taglines are antithetical to the raw document approach
- **Full viewport width usage**: Elements often span the full width of the browser window without max-width constraints, reinforcing the idea of the page as an unmediated document
- **Visible structural borders**: Use `border`, `outline`, and `<hr>` elements to make section boundaries explicit rather than relying on whitespace and subtle background color shifts
- **Dense information architecture**: Prioritize fitting more content into visible space rather than spreading it thin across scroll-length; think Craigslist, not Apple.com
- **Flat document hierarchy**: Minimize nesting depth; pages should read as flat lists, tables, and text blocks rather than deeply nested component trees
- **No sticky or fixed navigation**: Navigation should scroll with the document like any other content; persistent floating headers contradict the document-first philosophy

---

## CSS / Design Techniques

### Raw Border Card

A content card that exposes its structure through visible borders and minimal styling, rejecting rounded corners and soft shadows.

```css
.brutal-card {
  border: 2px solid var(--brutal-black);
  padding: 1.5rem;
  margin: 1rem 0;
  background-color: var(--brutal-white);
  transition: none; /* No smooth transitions */
}

.brutal-card:hover {
  background-color: var(--brutal-highlight);
}

.brutal-card h3 {
  margin-top: 0;
  border-bottom: 1px solid var(--brutal-black);
  padding-bottom: 0.5rem;
}

.brutal-card p {
  margin-bottom: 0;
}
```

### Raw Button

Buttons that look like buttons -- rectangular, bordered, with obvious hover states. No gradients, no border-radius, no box-shadows.

```css
.brutal-button {
  display: inline-block;
  font-family: 'Space Mono', monospace;
  font-size: 1rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  padding: 0.75rem 1.5rem;
  border: 2px solid var(--brutal-black);
  background-color: var(--brutal-white);
  color: var(--brutal-black);
  cursor: pointer;
  text-decoration: none;
  transition: none;
}

.brutal-button:hover {
  background-color: var(--brutal-black);
  color: var(--brutal-white);
}

.brutal-button:active {
  background-color: var(--brutal-red);
  color: var(--brutal-white);
  border-color: var(--brutal-red);
}

```

### Navigation

A flat navigation list that treats links as text anchors. No hamburger menus, no dropdowns.

```css
.brutal-nav {
  border-bottom: 2px solid var(--brutal-black);
  padding: 1rem 0;
  margin-bottom: 2rem;
}

.brutal-nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-wrap: wrap;
}

.brutal-nav a {
  display: block;
  padding: 0.5rem 1rem;
  color: var(--brutal-black);
  text-decoration: none;
  font-family: 'Space Mono', monospace;
  font-size: 0.875rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

.brutal-nav a:hover {
  background-color: var(--brutal-black);
  color: var(--brutal-white);
}
```

### Hero Section

A stark, text-only hero with oversized typography. No background image, no gradient -- just words.

```css
.brutal-hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 2rem;
  border-bottom: 4px solid var(--brutal-black);
}

.brutal-hero h1 {
  font-size: clamp(4rem, 12vw, 12rem);
  line-height: 0.9;
  margin: 0;
}

.brutal-hero p {
  font-family: 'Space Mono', monospace;
  font-size: clamp(1rem, 2vw, 1.5rem);
  max-width: 60ch;
  margin-top: 2rem;
}
```

### Exposed Link Directory

A dense, Craigslist-inspired link grid with visible borders exposing the underlying structure.

```css
.brutal-link-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  border: 2px solid var(--brutal-black);
  border-bottom: 0;
  border-right: 0;
}

.brutal-link-grid section {
  border-right: 2px solid var(--brutal-black);
  border-bottom: 2px solid var(--brutal-black);
  padding: 1rem;
}

.brutal-link-grid h4 {
  font-family: 'Space Mono', monospace;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--brutal-gray-dark);
  border-bottom: 1px solid var(--brutal-gray-mid);
  padding-bottom: 0.25rem;
  margin: 0 0 0.5rem 0;
}

.brutal-link-grid ul { list-style: none; padding: 0; margin: 0; }
.brutal-link-grid li { padding: 0.15rem 0; }
.brutal-link-grid a { color: var(--brutal-link); font-size: 0.875rem; }
.brutal-link-grid a:hover { background-color: var(--brutal-highlight); }
```

### Exposed Table Style

Tables that celebrate their grid structure with thick visible borders. Data is king.

```css
.brutal-table {
  width: 100%;
  border-collapse: collapse;
  font-family: 'Space Mono', monospace;
  font-size: 0.875rem;
}

.brutal-table th,
.brutal-table td {
  border: 2px solid var(--brutal-black);
  padding: 0.75rem 1rem;
  text-align: left;
}

.brutal-table th {
  background-color: var(--brutal-black);
  color: var(--brutal-white);
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

.brutal-table tr:hover td {
  background-color: var(--brutal-highlight);
}
```

---

## Design Do's and Don'ts

### Do's

- **Use system and monospaced fonts** to maintain the raw, undesigned feel and improve page load performance
- **Let HTML defaults show through** -- default link colors, visible focus outlines, native form controls all reinforce the honest aesthetic
- **Expose structural elements** like borders, horizontal rules, and table grids as visible design features rather than hiding them
- **Prioritize content density** by fitting meaningful information into every visible area of the viewport; treat whitespace as a luxury, not a requirement
- **Embrace browser defaults** as a starting point; a Brutalist page with zero CSS is closer to the ideal than a heavily styled one
- **Ensure fast load times** by minimizing HTTP requests, avoiding JavaScript frameworks, and keeping image usage to an absolute minimum
- **Test without CSS** to verify that the page remains functional and readable when stylesheets fail to load; the HTML document should stand on its own

### Don'ts

- **Don't use border-radius** -- rounded corners soften the raw edges that define the aesthetic; keep all corners sharp at 0px
- **Don't add smooth transitions or animations** -- movement and easing contradict the static, document-like nature of the design; hover states should snap instantly
- **Don't use hero images or background photos** -- if the design needs a photograph to communicate, the typography and structure have failed
- **Don't rely on JavaScript for layout** -- if the page breaks without JS, it violates the principle of structural honesty; HTML and CSS should do all the work
- **Don't use hamburger menus or hidden navigation** -- concealing navigation behind icons contradicts the transparency philosophy; all links should be visible
- **Don't apply box-shadows with blur** -- if depth is needed, use hard-offset shadows (Neubrutalism territory) or simple borders; soft shadows belong to a different aesthetic
- **Don't optimize for "user delight"** -- Brutalist design intentionally rejects the frictionless, pleasant browsing experience; discomfort and confrontation are valid design outcomes

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Neubrutalism](Neubrutalism.md) | Direct descendant that adds thick borders, hard shadows, and bold color to the Brutalist foundation while maintaining modern usability |
| [Minimalism](Minimalism.md) | Shares the reduction of elements but pursues elegance and calm rather than raw confrontation; Minimalism beautifies, Brutalism exposes |
| [Constructivism](Constructivism.md) | Historical parallel -- both movements use bold geometry, limited color, and structural exposure as ideological statements about honesty and function |
| [Raw Industrial](Raw_Industrial.md) | Kindred spirit in material honesty; Raw Industrial celebrates exposed metal, concrete, and machinery; Brutalist Web celebrates exposed HTML and system fonts |
| [DIY Punk](DIY_Punk.md) | Shares the anti-establishment, anti-polish ethos; both reject professional design conventions in favor of direct, unmediated communication |
| [Flat Design](Flat_Design.md) | Both reject skeuomorphism and depth illusions, but Flat Design still pursues visual harmony and brand consistency where Brutalism rejects all ornamentation |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Brutalist Web Design Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Archivo+Black&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* --- Custom Properties --- */
    :root {
      --brutal-black: #000000;
      --brutal-white: #ffffff;
      --brutal-gray-light: #f0f0f0;
      --brutal-gray-mid: #c0c0c0;
      --brutal-gray-dark: #808080;
      --brutal-near-black: #333333;
      --brutal-link: #0000ee;
      --brutal-visited: #551a8b;
      --brutal-red: #ff0000;
      --brutal-yellow: #ffff00;
      --brutal-green: #00ff00;
      --brutal-blue: #0000ff;
    }

    /* --- Reset & Base --- */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Space Mono', 'Courier New', Courier, monospace;
      font-size: 16px;
      line-height: 1.6;
      color: var(--brutal-black);
      background-color: var(--brutal-white);
    }

    /* --- Typography --- */
    h1, h2, h3, h4 {
      font-family: 'Archivo Black', 'Impact', 'Arial Black', sans-serif;
      text-transform: uppercase;
      letter-spacing: -0.02em;
      line-height: 1.0;
    }

    a {
      color: var(--brutal-link);
      text-decoration: underline;
      transition: none;
    }

    a:visited {
      color: var(--brutal-visited);
    }

    a:hover {
      background-color: var(--brutal-yellow);
      color: var(--brutal-black);
    }

    /* --- Navigation --- */
    .nav {
      border-bottom: 2px solid var(--brutal-black);
      padding: 0.75rem 2rem;
    }

    .nav ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 0;
    }

    .nav a {
      display: block;
      padding: 0.5rem 1rem;
      color: var(--brutal-black);
      text-decoration: none;
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-weight: 700;
    }

    .nav a:hover {
      background-color: var(--brutal-black);
      color: var(--brutal-white);
    }

    /* --- Hero --- */
    .hero {
      min-height: 90vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 2rem;
      border-bottom: 4px solid var(--brutal-black);
    }

    .hero h1 {
      font-size: clamp(3.5rem, 11vw, 11rem);
      line-height: 0.9;
    }

    .hero p {
      font-size: clamp(0.9rem, 1.5vw, 1.25rem);
      max-width: 55ch;
      margin-top: 2rem;
      line-height: 1.7;
    }

    .hero .btn-row {
      margin-top: 2rem;
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    /* --- Buttons --- */
    .btn {
      display: inline-block;
      font-family: 'Space Mono', monospace;
      font-size: 0.875rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      padding: 0.75rem 1.5rem;
      border: 2px solid var(--brutal-black);
      background-color: var(--brutal-white);
      color: var(--brutal-black);
      cursor: pointer;
      text-decoration: none;
      transition: none;
    }

    .btn:hover {
      background-color: var(--brutal-black);
      color: var(--brutal-white);
    }

    .btn:active {
      background-color: var(--brutal-red);
      color: var(--brutal-white);
      border-color: var(--brutal-red);
    }

    .btn--inverted {
      background-color: var(--brutal-black);
      color: var(--brutal-white);
    }

    .btn--inverted:hover {
      background-color: var(--brutal-white);
      color: var(--brutal-black);
    }

    /* --- Section Container --- */
    .section {
      padding: 3rem 2rem;
      border-bottom: 2px solid var(--brutal-black);
    }

    .section h2 {
      font-size: clamp(2rem, 5vw, 4rem);
      margin-bottom: 1.5rem;
    }

    .section p {
      max-width: 70ch;
      margin-bottom: 1rem;
    }

    /* --- Card Grid --- */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      border-top: 2px solid var(--brutal-black);
      border-left: 2px solid var(--brutal-black);
    }

    .card {
      border-right: 2px solid var(--brutal-black);
      border-bottom: 2px solid var(--brutal-black);
      padding: 1.5rem;
      background-color: var(--brutal-white);
    }

    .card:hover { background-color: var(--brutal-yellow); }
    .card h3 { font-size: 1.25rem; margin-bottom: 0.75rem; border-bottom: 1px solid var(--brutal-black); padding-bottom: 0.5rem; }
    .card p { font-size: 0.875rem; line-height: 1.6; margin-bottom: 1rem; }
    .card .tag { display: inline-block; font-size: 0.7rem; text-transform: uppercase; letter-spacing: 0.1em; border: 1px solid var(--brutal-black); padding: 0.2rem 0.5rem; margin-right: 0.25rem; }

    /* --- Link Directory --- */
    .link-directory {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      border-top: 2px solid var(--brutal-black);
      border-left: 2px solid var(--brutal-black);
    }

    .link-directory .col {
      border-right: 2px solid var(--brutal-black);
      border-bottom: 2px solid var(--brutal-black);
      padding: 1rem;
    }

    .link-directory h4 {
      font-family: 'Space Mono', monospace;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--brutal-gray-dark);
      border-bottom: 1px solid var(--brutal-gray-mid);
      padding-bottom: 0.25rem;
      margin-bottom: 0.5rem;
    }

    .link-directory ul { list-style: none; }
    .link-directory li { padding: 0.15rem 0; }
    .link-directory a { font-size: 0.85rem; }

    /* --- Exposed Table --- */
    .data-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.85rem;
      margin-top: 1.5rem;
    }

    .data-table th,
    .data-table td {
      border: 2px solid var(--brutal-black);
      padding: 0.6rem 0.8rem;
      text-align: left;
      vertical-align: top;
    }

    .data-table th {
      background-color: var(--brutal-black);
      color: var(--brutal-white);
      text-transform: uppercase;
      letter-spacing: 0.08em;
      font-weight: 700;
    }

    .data-table tr:hover td { background-color: var(--brutal-gray-light); }

    /* --- Footer --- */
    .footer {
      padding: 2rem;
      border-top: 4px solid var(--brutal-black);
      background-color: var(--brutal-gray-light);
    }

    .footer p { font-size: 0.8rem; color: var(--brutal-gray-dark); }
    .footer a { color: var(--brutal-black); }

    /* --- Utilities --- */
    .mt-1 { margin-top: 1rem; }
    .mt-2 { margin-top: 2rem; }

    /* --- Responsive --- */
    @media (max-width: 600px) {
      .hero {
        min-height: 70vh;
        padding: 1.5rem;
      }

      .section {
        padding: 2rem 1.5rem;
      }

      .nav {
        padding: 0.5rem 1rem;
      }

      .nav a {
        padding: 0.4rem 0.6rem;
        font-size: 0.7rem;
      }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="nav">
    <ul>
      <li><a href="#manifesto">Manifesto</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#directory">Directory</a></li>
      <li><a href="#data">Data</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <section class="hero" id="manifesto">
    <h1>Brutalist<br>Web Design</h1>
    <p>
      This page is a document. Not an app. Not an experience.
      Not a journey. A document. It contains text, links, and
      structural borders. Nothing more is needed. Nothing more
      is honest.
    </p>
    <div class="btn-row">
      <a href="#projects" class="btn">View Projects</a>
      <a href="#directory" class="btn btn--inverted">Browse Directory</a>
    </div>
  </section>

  <!-- PROJECTS (CARD GRID) -->
  <section class="section" id="projects">
    <h2>Projects</h2>
    <p>
      Each project is a rectangle containing text. The borders are visible
      because structure should not be hidden. Hover states exist because
      interaction should be acknowledged, not decorated.
    </p>
    <div class="card-grid mt-2">
      <div class="card">
        <h3>Project Alpha</h3>
        <p>A static site generator that outputs valid HTML with zero CSS. The document is the design. The browser provides the stylesheet.</p>
        <span class="tag">HTML</span>
        <span class="tag">Static</span>
        <span class="tag">No CSS</span>
      </div>
      <div class="card">
        <h3>Project Beta</h3>
        <p>An archive of 10,000 web pages rendered with their stylesheets disabled. A study in what the web looks like when you remove the paint.</p>
        <span class="tag">Archive</span>
        <span class="tag">Research</span>
      </div>
      <div class="card">
        <h3>Project Gamma</h3>
        <p>A monospaced font designed for maximum character density on screen. Every glyph occupies the same width. No kerning. No ligatures.</p>
        <span class="tag">Typography</span>
        <span class="tag">Monospace</span>
      </div>
      <div class="card">
        <h3>Project Delta</h3>
        <p>Performance benchmark: a fully functional e-commerce site in under 14KB. Every byte is accountable. Every element is necessary.</p>
        <span class="tag">Performance</span>
        <span class="tag">Minimal</span>
      </div>
    </div>
  </section>

  <!-- LINK DIRECTORY -->
  <section class="section" id="directory">
    <h2>Directory</h2>
    <p>Links organized by category. No descriptions needed. The URL tells you what you need to know.</p>
    <div class="link-directory mt-2">
      <div class="col">
        <h4>Resources</h4>
        <ul>
          <li><a href="#">HTML Specification</a></li>
          <li><a href="#">CSS Reference</a></li>
          <li><a href="#">Web Standards</a></li>
          <li><a href="#">Accessibility Guide</a></li>
        </ul>
      </div>
      <div class="col">
        <h4>Inspiration</h4>
        <ul>
          <li><a href="#">brutalistwebsites.com</a></li>
          <li><a href="#">Craigslist</a></li>
          <li><a href="#">Hacker News</a></li>
          <li><a href="#">Berkshire Hathaway</a></li>
        </ul>
      </div>
      <div class="col">
        <h4>Tools</h4>
        <ul>
          <li><a href="#">HTML Validator</a></li>
          <li><a href="#">PageSpeed Insights</a></li>
          <li><a href="#">WebPageTest</a></li>
          <li><a href="#">Lighthouse CLI</a></li>
        </ul>
      </div>
      <div class="col">
        <h4>Reading</h4>
        <ul>
          <li><a href="#">The Web's Grain</a></li>
          <li><a href="#">A Dao of Web Design</a></li>
          <li><a href="#">Resilient Web Design</a></li>
          <li><a href="#">HTML Energy</a></li>
        </ul>
      </div>
    </div>
  </section>

  <!-- DATA TABLE -->
  <section class="section" id="data">
    <h2>Data</h2>
    <p>Tables display data. Borders make cells visible. Headers are inverted.</p>
    <table class="data-table">
      <thead>
        <tr>
          <th>Site</th>
          <th>Weight</th>
          <th>Requests</th>
          <th>Load Time</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>This Page</td>
          <td>12 KB</td>
          <td>3</td>
          <td>0.4s</td>
        </tr>
        <tr>
          <td>Avg. News Site</td>
          <td>6,200 KB</td>
          <td>287</td>
          <td>8.7s</td>
        </tr>
        <tr>
          <td>Craigslist</td>
          <td>59 KB</td>
          <td>12</td>
          <td>0.8s</td>
        </tr>
      </tbody>
    </table>
  </section>

  <!-- CONTACT -->
  <section class="section" id="contact">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:hello@example.com">hello@example.com</a> / Source: <a href="#">view on sourcehut</a> / License: Public Domain</p>
  </section>

  <footer class="footer">
    <p>
      Built with HTML and CSS. No build step. No dependencies.
      No tracking. No cookies. View source to verify.
    </p>
    <p class="mt-1">
      <a href="#">Top of page</a> &bull;
      <a href="#">Sitemap</a> &bull;
      <a href="#">RSS Feed</a>
    </p>
  </footer>

</body>
</html>
```

---

## Implementation Tips

- **Start with zero CSS and add only what is necessary**: Open your HTML file in a browser with no stylesheet at all; then add CSS rules one at a time, asking whether each addition serves a functional purpose or merely a cosmetic one
- **Use a system font stack as your default** (`font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace`) to achieve the raw monospaced look without any external font requests, then optionally layer on a Google Font for headings only
- **Set `transition: none` globally** to prevent browsers or CSS resets from introducing smooth state changes; Brutalist hover and focus states should snap immediately between visual states without easing or duration
- **Test your page with images disabled and JavaScript blocked**: a properly Brutalist page should lose zero functionality and minimal visual integrity under these conditions; if something breaks, the design is relying on something it should not
- **Use semantic HTML elements** (`<nav>`, `<article>`, `<section>`, `<table>`, `<hr>`) and let them do the structural work; avoid `<div>` soup -- the point is that the document structure is visible, so it should be meaningful structure worth seeing
- **Keep total page weight under 50KB** (excluding fonts) as a hard constraint; this forces the kind of ruthless reduction that defines the aesthetic and provides the performance-as-ethics benefit that Brutalist design values
