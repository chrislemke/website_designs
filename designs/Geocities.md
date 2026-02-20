# Geocities Design Reference

GeoCities was a free web hosting service founded in 1994 that became the defining platform of the personal web, accumulating over 38 million user-created pages before Yahoo shut down the US service in 2009. The GeoCities aesthetic embodies the raw, unpolished creativity of self-taught web designers who built pages through trial and error -- garish tiled backgrounds, animated GIFs, blinking text, rainbow horizontal rules, visitor counters, guestbooks, "under construction" banners, and the unmistakable marquee scroll. Every page was a fever dream of personal expression, unconstrained by design systems, brand guidelines, or any concept of visual restraint. As a deliberate retro style in modern web and UI design, GeoCities channels that anarchic energy into intentionally chaotic layouts that celebrate maximalism, amateur charm, and the lost frontier spirit of the early internet -- a direct rejection of the sleek, corporate homogeneity that defines most contemporary web experiences.

---

## Visual Characteristics

### Core Design Traits

- **Tiled background patterns** -- repeating small images (stars, marble, flames, geometric patterns) covering the entire page background via `background-repeat: repeat`, often clashing violently with foreground content
- **Animated GIFs everywhere** -- spinning globes, dancing babies, flaming text, construction workers, rotating envelopes, waving flags, and blinking divider bars used as decoration in every available space
- **Marquee scrolling text** -- horizontal text tickers created with the `<marquee>` tag, typically containing welcome messages, announcements, or site status updates
- **"Under Construction" banners** -- animated warning signs and hard-hat graphics signaling pages that were perpetually unfinished, treated as a badge of active development rather than a problem
- **Visitor counters** -- numeric hit counters embedded near the footer, often with odometer-style or LCD digit graphics, proudly displaying (or exaggerating) page traffic
- **Rainbow horizontal rules** -- multicolored gradient divider bars separating sections, often animated or featuring sparkle effects
- **Comic Sans and system fonts** -- typography limited to web-safe fonts like Comic Sans MS, Times New Roman, Arial, and Courier, mixed freely within the same page at varying sizes and colors
- **Table-based layouts** -- rigid grid structures built entirely from HTML `<table>` elements with visible or invisible borders, creating columns, sidebars, and nested content areas
- **Garish color combinations** -- bright yellow text on blue backgrounds, lime green on purple, red on black -- chosen for personal expression rather than readability
- **Web rings and link collections** -- navigation banners at the page bottom connecting to other personal sites in themed communities, with "Previous / Next / Random" navigation buttons

### Design Principles

- Personal expression trumps professional polish -- every page should feel handmade by a real person
- More is more -- fill empty space with animated GIFs, colored text, dividers, badges, and decorative elements
- Every technology available should be used at once -- marquees, blinking text, colored fonts, tiled backgrounds, and animated images all on the same page
- Navigation is an adventure, not a utility -- visitors explore through curiosity rather than clear information architecture
- The page is never finished -- "under construction" is a permanent state of creative evolution
- Community connection matters -- guestbooks, web rings, and email links create human connections between page owners and visitors
- Accessibility and readability are secondary to visual impact and self-expression

---

## Color Palette

The GeoCities palette is rooted in the 216 web-safe colors -- a constrained set where each RGB channel was limited to values of 00, 33, 66, 99, CC, or FF. Within those limits, site owners gravitated toward maximum contrast and saturation.

| Swatch Name | Hex | Role / Usage |
|-------------|-----|-------------|
| **Electric Blue** | `#0000FF` | Default hyperlink color, heading text, background panels |
| **Hot Magenta** | `#FF00FF` | Accent text, decorative borders, heading highlights |
| **Lime Green** | `#00FF00` | "Matrix-style" text, status indicators, link hover states |
| **Bright Red** | `#FF0000` | Alert text, "NEW!" badges, emphasis on announcements |
| **Cyber Yellow** | `#FFFF00` | Body text on dark backgrounds, highlight color, star accents |
| **Aqua Cyan** | `#00FFFF` | Secondary link color, decorative text, divider accents |
| **Royal Purple** | `#660099` | Background panels, heading text, visited link color |
| **Black Void** | `#000000` | Page background, text shadow base, border color |
| **Space Navy** | `#000066` | Dark page backgrounds, table cell fills, header bars |
| **White Flash** | `#FFFFFF` | Body text on dark backgrounds, table borders, spacer cells |
| **Neon Orange** | `#FF6600` | "Under construction" accents, warning text, badge backgrounds |
| **Teal Classic** | `#008080` | Sidebar backgrounds, secondary panels, subtle accents |
| **Hot Pink** | `#FF69B4` | Personal page accents, decorative text, sparkle elements |
| **Silver Grey** | `#C0C0C0` | Table borders, horizontal rules, button surfaces |

### CSS Custom Properties

```css
:root {
  /* Core backgrounds */
  --geo-bg-primary: #000000;
  --geo-bg-secondary: #000066;
  --geo-bg-panel: #000033;
  --geo-bg-sidebar: #008080;

  /* Primary text colors */
  --geo-text-light: #FFFFFF;
  --geo-text-yellow: #FFFF00;
  --geo-text-lime: #00FF00;
  --geo-text-cyan: #00FFFF;

  /* Accent colors */
  --geo-accent-blue: #0000FF;
  --geo-accent-magenta: #FF00FF;
  --geo-accent-red: #FF0000;
  --geo-accent-orange: #FF6600;
  --geo-accent-pink: #FF69B4;
  --geo-accent-purple: #660099;

  /* Links */
  --geo-link: #0000FF;
  --geo-link-visited: #660099;
  --geo-link-hover: #FF00FF;
  --geo-link-active: #FF0000;

  /* UI elements */
  --geo-border: #C0C0C0;
  --geo-button-face: #C0C0C0;
  --geo-button-highlight: #FFFFFF;
  --geo-button-shadow: #808080;

  /* Rainbow gradient */
  --geo-rainbow: linear-gradient(
    90deg,
    #FF0000, #FF6600, #FFFF00, #00FF00,
    #00FFFF, #0000FF, #660099, #FF00FF
  );
}
```

---

## Typography

### Typeface Characteristics

GeoCities typography was dictated by the web-safe font stack -- whatever was installed on the visitor's computer. Pages mixed fonts, sizes, colors, and styles within single paragraphs. Bold, italic, underline, and even `<blink>` were applied liberally and simultaneously.

### Recommended Google Fonts

| Font | Style | Best For |
|------|-------|----------|
| **Comic Neue** | Rounded casual sans-serif | Body text, headings -- the Google Fonts stand-in for Comic Sans MS |
| **VT323** | Pixel monospace CRT | Visitor counters, terminal-style text, retro data displays |
| **Press Start 2P** | Chunky pixel bitmap | Headers, badges, retro emphasis text |
| **Courier Prime** | Refined monospace | Code blocks, guestbook entries, old-school email styling |
| **Pixelify Sans** | Clean pixel sans-serif | Navigation labels, sidebar text, button labels |
| **Bungee** | Chunky display | Page titles, banner headings, bold announcements |
| **Lobster** | Script display | Decorative titles, personal page names, whimsical headings |
| **Permanent Marker** | Handwritten bold | Annotation text, "sign my guestbook" callouts |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Comic Neue** (700) | **Comic Neue** (400) | All-in on the Comic Sans homage for maximum authenticity |
| **Bungee** (400) | **Comic Neue** (400) | Bold display headings with casual body text |
| **Press Start 2P** (400) | **VT323** (400) | Full retro pixel aesthetic, early web terminal feel |
| **Lobster** (400) | **Courier Prime** (400) | Decorative script headings with monospace body for personal page charm |
| **Permanent Marker** (400) | **Pixelify Sans** (400) | Handmade heading energy with clean pixel body text |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Comic+Neue:wght@400;700&family=VT323&family=Press+Start+2P&family=Courier+Prime&family=Pixelify+Sans:wght@400;700&family=Bungee&family=Permanent+Marker&display=swap');

/* Body text -- Comic Sans homage */
body {
  font-family: 'Comic Neue', 'Comic Sans MS', 'Chalkboard SE', cursive;
  font-size: 16px;
  line-height: 1.6;
  color: var(--geo-text-yellow);
  background: var(--geo-bg-primary);
}

/* Headings -- loud and colorful */
h1 {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-weight: 700;
  font-size: 2.5rem;
  color: var(--geo-accent-magenta);
  text-align: center;
  text-shadow: 2px 2px 0px #000000;
}

h2 {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-weight: 700;
  font-size: 1.8rem;
  color: var(--geo-accent-blue);
  text-decoration: underline;
}

h3 {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-weight: 700;
  font-size: 1.3rem;
  color: var(--geo-text-cyan);
}

/* Pixel font for counters and status text */
.geo-pixel-text {
  font-family: 'Press Start 2P', monospace;
  font-size: 0.65rem;
  letter-spacing: 0.05em;
  color: var(--geo-text-lime);
}

/* Monospace for guestbook and code-like content */
.geo-mono {
  font-family: 'Courier Prime', 'Courier New', monospace;
  font-size: 14px;
  line-height: 1.5;
}

/* Display font for banner titles */
.geo-banner-title {
  font-family: 'Bungee', 'Impact', sans-serif;
  font-size: clamp(2rem, 5vw, 4rem);
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

---

## Layout Principles

- **Table-based structure** -- recreate the classic `<table>` layout using CSS Grid with visible borders, fixed column widths, and nested cells for authentic period-correct composition
- **Center-aligned content** -- the vast majority of GeoCities pages centered all content within a fixed-width container (typically 600-800px), mirroring the `<center>` tag era
- **Single long-scrolling page** -- most personal homepages were one enormous page with all content stacked vertically, divided by horizontal rules and animated GIF dividers
- **Sidebar navigation in table cells** -- a narrow left column with link lists, badges, and web ring banners alongside a wider main content column
- **Fixed-width containers** -- use `max-width: 800px` to evoke 800x600 screen resolution constraints; never go full-width fluid
- **Generous use of `<br>` spacing** -- vertical spacing was achieved through multiple line breaks rather than CSS margins, creating inconsistent but characterful rhythm
- **Nested tables for complex layouts** -- tables within tables within tables, creating deeply nested grid structures for sidebars, headers, and content areas
- **Visible table borders** -- tables often had `border="1"` or colored borders, making the structural grid explicitly visible
- **Footer as community hub** -- the bottom of every page contained the guestbook link, email address, visitor counter, web ring navigation, and "last updated" timestamp
- **No responsive design** -- pages were built for a single screen resolution; horizontal scrolling and broken layouts on other sizes were accepted

---

## CSS / Design Techniques

### Card / Content Panel

```css
/* GeoCities-style content panel mimicking a table cell */
.geo-card {
  background: var(--geo-bg-secondary);
  border: 2px solid var(--geo-border);
  padding: 16px;
  margin: 8px 0;
  text-align: center;
  color: var(--geo-text-yellow);
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
}

.geo-card h2 {
  color: var(--geo-accent-magenta);
  font-size: 1.5rem;
  text-decoration: underline;
  margin-bottom: 8px;
}

.geo-card p {
  font-size: 14px;
  line-height: 1.6;
  color: var(--geo-text-light);
}

/* Card with visible "table border" styling */
.geo-card--bordered {
  border: 3px ridge var(--geo-border);
  box-shadow:
    inset 2px 2px 0 rgba(255, 255, 255, 0.15),
    inset -2px -2px 0 rgba(0, 0, 0, 0.3);
}

/* Card with tiled background */
.geo-card--tiled {
  background-color: #000033;
  background-image: url("data:image/svg+xml,%3Csvg width='20' height='20' xmlns='http://www.w3.org/2000/svg'%3E%3Crect width='20' height='20' fill='%23000033'/%3E%3Ccircle cx='10' cy='10' r='1.5' fill='%23003366'/%3E%3C/svg%3E");
  background-repeat: repeat;
}
```

### Button Component

```css
/* 90s beveled button -- the classic grey raised look */
.geo-button {
  display: inline-block;
  padding: 4px 16px;
  background: var(--geo-button-face);
  color: #000000;
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-size: 14px;
  font-weight: 700;
  border-top: 2px solid var(--geo-button-highlight);
  border-left: 2px solid var(--geo-button-highlight);
  border-right: 2px solid #000000;
  border-bottom: 2px solid #000000;
  box-shadow:
    inset 1px 1px 0 #DFDFDF,
    inset -1px -1px 0 var(--geo-button-shadow);
  cursor: pointer;
  text-decoration: none;
}

.geo-button:active {
  border-top: 2px solid #000000;
  border-left: 2px solid #000000;
  border-right: 2px solid var(--geo-button-highlight);
  border-bottom: 2px solid var(--geo-button-highlight);
  box-shadow:
    inset 1px 1px 0 var(--geo-button-shadow),
    inset -1px -1px 0 #DFDFDF;
  padding: 5px 15px 3px 17px;
}

/* Colorful GeoCities-style link button */
.geo-button--colorful {
  background: linear-gradient(180deg, #FF6600 0%, #CC3300 100%);
  color: #FFFFFF;
  font-weight: 700;
  border: 2px outset #FF9933;
  text-shadow: 1px 1px 0 #000000;
}

.geo-button--colorful:hover {
  background: linear-gradient(180deg, #FF9933 0%, #FF6600 100%);
}

/* Animated "click me" button */
@keyframes geo-button-pulse {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.05); }
}

.geo-button--animated {
  animation: geo-button-pulse 1s ease-in-out infinite;
}
```

### Navigation Bar

```css
/* GeoCities-style sidebar navigation */
.geo-nav {
  background: var(--geo-bg-secondary);
  border: 2px ridge var(--geo-border);
  padding: 8px;
  width: 180px;
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
}

.geo-nav h3 {
  color: var(--geo-accent-magenta);
  font-size: 1rem;
  text-align: center;
  text-decoration: underline;
  margin-bottom: 8px;
}

.geo-nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.geo-nav li {
  padding: 2px 0;
  text-align: center;
}

/* Classic underlined blue links */
.geo-nav a {
  color: var(--geo-link);
  text-decoration: underline;
  font-size: 14px;
  font-weight: 700;
}

.geo-nav a:visited {
  color: var(--geo-link-visited);
}

.geo-nav a:hover {
  color: var(--geo-link-hover);
  text-decoration: underline;
}

.geo-nav a:active {
  color: var(--geo-link-active);
}

/* Bullet dividers between nav items */
.geo-nav li + li::before {
  content: '';
  display: block;
  height: 2px;
  background: var(--geo-rainbow);
  margin: 4px 0;
}

/* Navigation badge */
.geo-nav-badge {
  display: inline-block;
  background: var(--geo-accent-red);
  color: var(--geo-text-light);
  font-family: 'Press Start 2P', monospace;
  font-size: 0.5rem;
  padding: 2px 6px;
  margin-left: 4px;
  animation: geo-blink 1s step-end infinite;
}

@keyframes geo-blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0; }
}
```

### Hero Section

```css
/* GeoCities homepage hero / welcome banner */
.geo-hero {
  text-align: center;
  padding: 24px 16px;
  background: var(--geo-bg-secondary);
  border: 3px ridge var(--geo-border);
  margin-bottom: 8px;
}

.geo-hero h1 {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-weight: 700;
  font-size: clamp(2rem, 6vw, 3.5rem);
  color: var(--geo-text-yellow);
  text-shadow:
    2px 2px 0px #FF0000,
    4px 4px 0px #000000;
  margin-bottom: 8px;
  letter-spacing: 0.05em;
}

.geo-hero .subtitle {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-size: 1.2rem;
  color: var(--geo-text-cyan);
}

/* Blinking "welcome" text */
.geo-hero .blink {
  animation: geo-blink 1s step-end infinite;
  color: var(--geo-accent-magenta);
  font-weight: 700;
}

/* Rainbow gradient divider under hero */
.geo-hero::after {
  content: '';
  display: block;
  height: 6px;
  margin-top: 16px;
  background: var(--geo-rainbow);
}
```

### Visitor Counter

```css
/* Classic GeoCities hit counter */
.geo-counter {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  font-family: 'VT323', monospace;
  font-size: 14px;
  color: var(--geo-text-light);
}

.geo-counter-label {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-size: 12px;
  color: var(--geo-text-cyan);
}

.geo-counter-digits {
  display: inline-flex;
  gap: 1px;
  background: #000000;
  border: 2px inset var(--geo-border);
  padding: 2px;
}

.geo-counter-digit {
  display: inline-block;
  width: 18px;
  height: 24px;
  background: #1a1a1a;
  color: #00FF00;
  font-family: 'VT323', 'Courier New', monospace;
  font-size: 20px;
  line-height: 24px;
  text-align: center;
  border: 1px solid #333333;
}

/* Animated counter increment */
@keyframes geo-counter-roll {
  0%   { transform: translateY(0); }
  10%  { transform: translateY(-2px); }
  20%  { transform: translateY(0); }
  100% { transform: translateY(0); }
}

.geo-counter-digit--active {
  animation: geo-counter-roll 3s ease-in-out infinite;
}
```

### Marquee Scrolling Text

```css
/* CSS-only recreation of the <marquee> tag */
@keyframes geo-marquee-scroll {
  0%   { transform: translateX(100%); }
  100% { transform: translateX(-100%); }
}

.geo-marquee {
  overflow: hidden;
  white-space: nowrap;
  background: var(--geo-bg-primary);
  border-top: 2px solid var(--geo-accent-magenta);
  border-bottom: 2px solid var(--geo-accent-magenta);
  padding: 6px 0;
}

.geo-marquee span {
  display: inline-block;
  animation: geo-marquee-scroll 20s linear infinite;
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-size: 1rem;
  font-weight: 700;
  color: var(--geo-text-yellow);
}

/* Reverse direction variant */
.geo-marquee--reverse span {
  animation-direction: reverse;
  color: var(--geo-text-cyan);
}

/* Fast-scrolling variant */
.geo-marquee--fast span {
  animation-duration: 8s;
  color: var(--geo-accent-red);
}
```

### Under Construction Banner

```css
/* "Under Construction" section banner */
.geo-construction {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  background: repeating-linear-gradient(
    45deg,
    #000000 0px,
    #000000 10px,
    #FFFF00 10px,
    #FFFF00 20px
  );
  padding: 12px 20px;
  border: 3px solid #FFFF00;
  margin: 16px 0;
  text-align: center;
}

.geo-construction-text {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-weight: 700;
  font-size: 1.2rem;
  color: #FFFF00;
  background: #000000;
  padding: 4px 12px;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

/* Animated caution stripes */
@keyframes geo-stripes-move {
  0%   { background-position: 0 0; }
  100% { background-position: 28.28px 0; }
}

.geo-construction--animated {
  animation: geo-stripes-move 1s linear infinite;
  background-size: 28.28px 28.28px;
}

/* Spinning construction icon (pure CSS) */
@keyframes geo-spin {
  0%   { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}

.geo-construction-icon {
  display: inline-block;
  font-size: 2rem;
  animation: geo-spin 2s linear infinite;
}
```

### Rainbow Divider

```css
/* Animated rainbow horizontal rule */
@keyframes geo-rainbow-shift {
  0%   { background-position: 0% 50%; }
  100% { background-position: 200% 50%; }
}

.geo-rainbow-hr {
  border: none;
  height: 6px;
  background: linear-gradient(
    90deg,
    #FF0000, #FF6600, #FFFF00, #00FF00,
    #00FFFF, #0000FF, #660099, #FF00FF, #FF0000
  );
  background-size: 200% 100%;
  animation: geo-rainbow-shift 3s linear infinite;
  margin: 16px 0;
}

/* Sparkle divider variant */
.geo-rainbow-hr--sparkle {
  height: 8px;
  position: relative;
}

.geo-rainbow-hr--sparkle::before,
.geo-rainbow-hr--sparkle::after {
  content: '\2726';
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  font-size: 16px;
  color: #FFFF00;
  animation: geo-blink 0.8s step-end infinite;
}

.geo-rainbow-hr--sparkle::before { left: -20px; }
.geo-rainbow-hr--sparkle::after  { right: -20px; }
```

### Tiled Background

```css
/* Classic GeoCities tiled star background */
.geo-bg-stars {
  background-color: #000033;
  background-image: url("data:image/svg+xml,%3Csvg width='40' height='40' xmlns='http://www.w3.org/2000/svg'%3E%3Crect width='40' height='40' fill='%23000033'/%3E%3Ccircle cx='20' cy='20' r='1' fill='%23FFFFFF'/%3E%3Ccircle cx='5' cy='8' r='0.5' fill='%23AAAAFF'/%3E%3Ccircle cx='35' cy='32' r='0.8' fill='%23FFFFFF'/%3E%3Ccircle cx='12' cy='30' r='0.5' fill='%23AAAAFF'/%3E%3C/svg%3E");
  background-repeat: repeat;
}

/* Tiled marble texture */
.geo-bg-marble {
  background-color: #1a1a2e;
  background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' xmlns='http://www.w3.org/2000/svg'%3E%3Crect width='60' height='60' fill='%231a1a2e'/%3E%3Cpath d='M0 30 Q15 25 30 30 Q45 35 60 30' stroke='%23252545' fill='none' stroke-width='1'/%3E%3Cpath d='M0 15 Q20 10 40 15 Q50 18 60 15' stroke='%23202040' fill='none' stroke-width='0.8'/%3E%3Cpath d='M0 45 Q10 42 25 45 Q40 48 60 45' stroke='%23252545' fill='none' stroke-width='0.8'/%3E%3C/svg%3E");
  background-repeat: repeat;
}

/* Animated flame background */
@keyframes geo-flame-flicker {
  0%, 100% { opacity: 0.8; }
  50%      { opacity: 1; }
}

.geo-bg-flames {
  background-color: #000000;
  background-image: linear-gradient(
    0deg,
    #FF0000 0%,
    #FF6600 20%,
    #FFFF00 40%,
    transparent 60%
  );
  background-size: 100% 200px;
  background-repeat: no-repeat;
  background-position: bottom;
  animation: geo-flame-flicker 0.3s ease-in-out infinite alternate;
}
```

### Guestbook

```css
/* GeoCities guestbook panel */
.geo-guestbook {
  background: var(--geo-bg-secondary);
  border: 3px ridge var(--geo-border);
  padding: 16px;
  max-width: 600px;
  margin: 16px auto;
}

.geo-guestbook h3 {
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-weight: 700;
  font-size: 1.3rem;
  color: var(--geo-accent-magenta);
  text-align: center;
  text-decoration: underline;
  margin-bottom: 12px;
}

.geo-guestbook-entry {
  background: #000033;
  border: 1px solid #333366;
  padding: 8px 12px;
  margin-bottom: 8px;
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-size: 14px;
  color: var(--geo-text-light);
}

.geo-guestbook-entry .author {
  color: var(--geo-text-cyan);
  font-weight: 700;
}

.geo-guestbook-entry .date {
  color: var(--geo-border);
  font-size: 12px;
}

/* Guestbook form */
.geo-guestbook-form input,
.geo-guestbook-form textarea {
  width: 100%;
  background: #FFFFFF;
  color: #000000;
  font-family: 'Comic Neue', 'Comic Sans MS', cursive;
  font-size: 14px;
  padding: 4px 6px;
  border: 2px inset var(--geo-border);
  margin-bottom: 6px;
}

.geo-guestbook-form textarea {
  height: 80px;
  resize: vertical;
}
```

---

## Design Do's and Don'ts

### Do

- Use web-safe colors and maximum-contrast color combinations -- yellow on navy, lime on black, magenta on dark blue
- Center-align everything and wrap content in a fixed-width container (600-800px)
- Include a visitor counter, guestbook section, and "last updated" date in the footer
- Mix multiple font styles, sizes, and colors within the same page for authentic chaos
- Add animated rainbow dividers between every major section
- Use table-based layouts (or CSS Grid styled to look like visible-border HTML tables)
- Include at least one marquee scrolling text element
- Place an "under construction" banner somewhere on the page, even if the page is finished
- Link to a guestbook and display web ring navigation at the bottom
- Use `<blink>` animation on "NEW!" badges and important announcements
- Tile a repeating background pattern across the entire page body
- Stack content vertically in one long scrolling page rather than using multi-page navigation

### Don't

- Do not use modern design systems, component libraries, or clean grid layouts -- the aesthetic is the opposite of systematic
- Do not choose subtle, muted, or pastel color palettes -- GeoCities demands maximum saturation and contrast
- Do not apply consistent spacing, alignment, or typographic hierarchy -- intentional inconsistency is the point
- Do not use responsive design techniques -- build for one fixed width and accept that other screen sizes may break
- Do not omit decorative elements to achieve "clean" whitespace -- every gap should be filled with a GIF, badge, or divider
- Do not use modern sans-serif fonts like Inter, Roboto, or system-ui -- stick to Comic Sans, Times New Roman, Courier, and pixel fonts
- Do not apply smooth transitions or sophisticated animations -- movements should be jerky, blinking, and step-based
- Do not remove underlines from links -- blue underlined hyperlinks are sacred in this aesthetic
- Do not follow WCAG contrast guidelines as a primary concern -- the aesthetic intentionally prioritizes expression over accessibility (though provide alt text for meaningful content)
- Do not use SVG icons or icon fonts -- era-appropriate elements use text characters, emoji, or inline pixel art

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **[Dial-Up Delight](Dial_Up_Delight.md)** | The Gen Z reinterpretation of GeoCities culture through a gothic-neon lens; shares marquee text, sparkles, and under-construction energy but adds chrome gradients and glitch effects |
| **[Early Cyber](Early_Cyber.md)** | Both emerged from 1990s internet culture; Early Cyber focuses on digital manipulation tools (fractals, thermographic imagery) while GeoCities focuses on personal homepage chaos |
| **[Windows 95/98](Windows_95_98.md)** | Shares the era and the beveled grey button aesthetic; Windows 95/98 focuses on the operating system shell while GeoCities focuses on the web pages viewed within it |
| **[8-Bit](8-Bit.md)** | Shares pixel-grid precision and bitmap rendering sensibility; 8-Bit references gaming consoles while GeoCities references web browsers and HTML |
| **[Maximalism](Maximalism.md)** | GeoCities is maximalism in its purest digital form -- every surface filled, every technique used simultaneously, visual restraint rejected entirely |
| **[DIY Punk](DIY_Punk.md)** | Shares the handmade, anti-professional ethos; DIY Punk expresses it through photocopied zines and hand-drawn flyers, GeoCities through hand-coded HTML |
| **[Dopamine Design](Dopamine_Design.md)** | Both pursue maximum visual stimulation through bright colors and dense compositions; Dopamine Design is a modern professional trend while GeoCities is its accidental amateur ancestor |
| **[Cluttercore](Cluttercore.md)** | Shares the philosophy that more is more and empty space is wasted space; Cluttercore applies this to physical spaces while GeoCities applies it to digital pages |
| **[Kidcore](Kidcore.md)** | Both embrace childlike exuberance, bright primary colors, and a rejection of sophisticated taste; Kidcore references physical toys and media while GeoCities references digital self-expression |
| **[Weirdcore](Weirdcore.md)** | Both mine the early internet for aesthetic material; Weirdcore extracts the uncanny and unsettling qualities of low-resolution web graphics while GeoCities celebrates the joyful chaos |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>~*~ Welcome to My Homepage ~*~</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Comic+Neue:wght@400;700&family=VT323&family=Press+Start+2P&family=Courier+Prime&display=swap" rel="stylesheet">
  <style>
    /* ========================================
       CSS CUSTOM PROPERTIES
    ======================================== */
    :root {
      --geo-bg-primary: #000000;
      --geo-bg-secondary: #000066;
      --geo-bg-panel: #000033;
      --geo-text-light: #FFFFFF;
      --geo-text-yellow: #FFFF00;
      --geo-text-lime: #00FF00;
      --geo-text-cyan: #00FFFF;
      --geo-accent-blue: #0000FF;
      --geo-accent-magenta: #FF00FF;
      --geo-accent-red: #FF0000;
      --geo-accent-orange: #FF6600;
      --geo-accent-pink: #FF69B4;
      --geo-accent-purple: #660099;
      --geo-link: #0000FF;
      --geo-link-visited: #660099;
      --geo-link-hover: #FF00FF;
      --geo-border: #C0C0C0;
      --geo-rainbow: linear-gradient(90deg, #FF0000, #FF6600, #FFFF00, #00FF00, #00FFFF, #0000FF, #660099, #FF00FF);
    }

    /* ========================================
       RESET & BASE
    ======================================== */
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Comic Neue', 'Comic Sans MS', 'Chalkboard SE', cursive;
      font-size: 16px;
      line-height: 1.6;
      color: var(--geo-text-yellow);
      /* Tiled star background */
      background-color: #000033;
      background-image: url("data:image/svg+xml,%3Csvg width='40' height='40' xmlns='http://www.w3.org/2000/svg'%3E%3Crect width='40' height='40' fill='%23000033'/%3E%3Ccircle cx='20' cy='20' r='1' fill='%23FFFFFF'/%3E%3Ccircle cx='5' cy='8' r='0.5' fill='%23AAAAFF'/%3E%3Ccircle cx='35' cy='32' r='0.8' fill='%23FFFFFF'/%3E%3Ccircle cx='12' cy='30' r='0.5' fill='%23AAAAFF'/%3E%3C/svg%3E");
      background-repeat: repeat;
      overflow-x: hidden;
    }

    a { color: var(--geo-link); }
    a:visited { color: var(--geo-link-visited); }
    a:hover { color: var(--geo-link-hover); }

    /* ========================================
       PAGE WRAPPER (fixed-width center)
    ======================================== */
    .geo-page {
      max-width: 780px;
      margin: 0 auto;
      padding: 8px;
    }

    /* ========================================
       MARQUEE BANNER
    ======================================== */
    @keyframes marquee-scroll {
      0%   { transform: translateX(100%); }
      100% { transform: translateX(-100%); }
    }

    .geo-marquee {
      overflow: hidden;
      white-space: nowrap;
      background: #000000;
      border-top: 2px solid var(--geo-accent-magenta);
      border-bottom: 2px solid var(--geo-accent-magenta);
      padding: 6px 0;
      margin-bottom: 8px;
    }

    .geo-marquee span {
      display: inline-block;
      animation: marquee-scroll 18s linear infinite;
      font-weight: 700;
      color: var(--geo-text-yellow);
      font-size: 1rem;
    }

    /* ========================================
       RAINBOW DIVIDER
    ======================================== */
    @keyframes rainbow-shift {
      0%   { background-position: 0% 50%; }
      100% { background-position: 200% 50%; }
    }

    .geo-hr {
      border: none;
      height: 6px;
      background: linear-gradient(90deg, #FF0000, #FF6600, #FFFF00, #00FF00, #00FFFF, #0000FF, #660099, #FF00FF, #FF0000);
      background-size: 200% 100%;
      animation: rainbow-shift 3s linear infinite;
      margin: 12px 0;
    }

    /* ========================================
       HERO / WELCOME BANNER
    ======================================== */
    .geo-hero {
      text-align: center;
      background: var(--geo-bg-secondary);
      border: 3px ridge var(--geo-border);
      padding: 20px 16px;
      margin-bottom: 8px;
    }

    .geo-hero h1 {
      font-family: 'Comic Neue', 'Comic Sans MS', cursive;
      font-weight: 700;
      font-size: clamp(2rem, 6vw, 3rem);
      color: var(--geo-text-yellow);
      text-shadow: 2px 2px 0px #FF0000, 4px 4px 0px #000000;
      margin-bottom: 4px;
    }

    .geo-hero .subtitle {
      font-size: 1.1rem;
      color: var(--geo-text-cyan);
    }

    @keyframes blink-anim {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    .blink {
      animation: blink-anim 1s step-end infinite;
    }

    /* ========================================
       TABLE LAYOUT (sidebar + main)
    ======================================== */
    .geo-table {
      display: grid;
      grid-template-columns: 180px 1fr;
      gap: 4px;
      margin: 8px 0;
    }

    /* ========================================
       SIDEBAR NAVIGATION
    ======================================== */
    .geo-sidebar {
      background: var(--geo-bg-secondary);
      border: 2px ridge var(--geo-border);
      padding: 8px;
      font-size: 14px;
    }

    .geo-sidebar h3 {
      color: var(--geo-accent-magenta);
      text-align: center;
      text-decoration: underline;
      font-size: 1rem;
      margin-bottom: 6px;
    }

    .geo-sidebar ul {
      list-style: none;
      padding: 0;
    }

    .geo-sidebar li {
      text-align: center;
      padding: 3px 0;
      border-bottom: 1px solid #333366;
    }

    .geo-sidebar li:last-child { border-bottom: none; }

    .geo-sidebar a {
      font-weight: 700;
      font-size: 13px;
    }

    .geo-sidebar .badge {
      display: inline-block;
      background: var(--geo-accent-red);
      color: var(--geo-text-light);
      font-family: 'Press Start 2P', monospace;
      font-size: 0.4rem;
      padding: 1px 4px;
      margin-left: 2px;
      animation: blink-anim 1s step-end infinite;
    }

    /* ========================================
       MAIN CONTENT AREA
    ======================================== */
    .geo-main {
      background: var(--geo-bg-panel);
      border: 2px ridge var(--geo-border);
      padding: 16px;
    }

    .geo-main h2 {
      color: var(--geo-accent-magenta);
      font-size: 1.5rem;
      text-decoration: underline;
      text-align: center;
      margin-bottom: 8px;
    }

    .geo-main p {
      color: var(--geo-text-light);
      font-size: 15px;
      margin-bottom: 12px;
    }

    /* ========================================
       UNDER CONSTRUCTION BANNER
    ======================================== */
    @keyframes stripes-move {
      0%   { background-position: 0 0; }
      100% { background-position: 28.28px 0; }
    }

    .geo-construction {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      background: repeating-linear-gradient(
        45deg,
        #000000 0px, #000000 10px,
        #FFFF00 10px, #FFFF00 20px
      );
      background-size: 28.28px 28.28px;
      animation: stripes-move 1s linear infinite;
      padding: 10px 16px;
      border: 3px solid #FFFF00;
      margin: 12px 0;
      text-align: center;
    }

    .geo-construction-text {
      font-weight: 700;
      font-size: 1rem;
      color: #FFFF00;
      background: #000000;
      padding: 4px 12px;
      text-transform: uppercase;
      letter-spacing: 0.1em;
    }

    @keyframes spin {
      0%   { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    .spin { animation: spin 2s linear infinite; display: inline-block; }

    /* ========================================
       CONTENT CARD
    ======================================== */
    .geo-card {
      background: var(--geo-bg-secondary);
      border: 2px solid var(--geo-border);
      padding: 12px;
      margin: 8px 0;
      text-align: center;
    }

    .geo-card h3 {
      color: var(--geo-text-cyan);
      font-size: 1.1rem;
      text-decoration: underline;
      margin-bottom: 6px;
    }

    .geo-card p {
      color: var(--geo-text-light);
      font-size: 14px;
    }

    /* ========================================
       VISITOR COUNTER
    ======================================== */
    .geo-counter {
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .geo-counter-label {
      font-size: 12px;
      color: var(--geo-text-cyan);
    }

    .geo-counter-digits {
      display: inline-flex;
      gap: 1px;
      background: #000000;
      border: 2px inset var(--geo-border);
      padding: 2px;
    }

    .geo-counter-digit {
      display: inline-block;
      width: 16px;
      height: 22px;
      background: #111111;
      color: #00FF00;
      font-family: 'VT323', monospace;
      font-size: 18px;
      line-height: 22px;
      text-align: center;
      border: 1px solid #333333;
    }

    /* ========================================
       GUESTBOOK
    ======================================== */
    .geo-guestbook {
      background: var(--geo-bg-secondary);
      border: 3px ridge var(--geo-border);
      padding: 12px;
      margin: 12px 0;
    }

    .geo-guestbook h3 {
      color: var(--geo-accent-magenta);
      text-align: center;
      text-decoration: underline;
      font-size: 1.2rem;
      margin-bottom: 8px;
    }

    .geo-guestbook-entry {
      background: #000033;
      border: 1px solid #333366;
      padding: 8px;
      margin-bottom: 6px;
      font-size: 14px;
      color: var(--geo-text-light);
    }

    .geo-guestbook-entry .author { color: var(--geo-text-cyan); font-weight: 700; }
    .geo-guestbook-entry .date { color: #999999; font-size: 12px; }

    .geo-guestbook input,
    .geo-guestbook textarea {
      width: 100%;
      background: #FFFFFF;
      color: #000000;
      font-family: 'Comic Neue', 'Comic Sans MS', cursive;
      font-size: 14px;
      padding: 4px 6px;
      border: 2px inset var(--geo-border);
      margin-bottom: 6px;
    }

    .geo-guestbook textarea { height: 60px; resize: vertical; }

    /* ========================================
       BUTTONS
    ======================================== */
    .geo-btn {
      display: inline-block;
      padding: 4px 16px;
      background: #C0C0C0;
      color: #000000;
      font-family: 'Comic Neue', 'Comic Sans MS', cursive;
      font-size: 14px;
      font-weight: 700;
      border-top: 2px solid #FFFFFF;
      border-left: 2px solid #FFFFFF;
      border-right: 2px solid #000000;
      border-bottom: 2px solid #000000;
      box-shadow: inset 1px 1px 0 #DFDFDF, inset -1px -1px 0 #808080;
      cursor: pointer;
      text-decoration: none;
    }

    .geo-btn:active {
      border-top-color: #000000;
      border-left-color: #000000;
      border-right-color: #FFFFFF;
      border-bottom-color: #FFFFFF;
    }

    .geo-btn--color {
      background: linear-gradient(180deg, #FF6600 0%, #CC3300 100%);
      color: #FFFFFF;
      border: 2px outset #FF9933;
      text-shadow: 1px 1px 0 #000000;
    }

    /* ========================================
       WEB RING
    ======================================== */
    .geo-webring {
      text-align: center;
      background: var(--geo-bg-secondary);
      border: 2px ridge var(--geo-border);
      padding: 8px;
      margin: 12px 0;
      font-size: 13px;
    }

    .geo-webring p {
      color: var(--geo-text-light);
      margin-bottom: 4px;
    }

    .geo-webring strong {
      color: var(--geo-accent-pink);
    }

    .geo-webring-nav {
      display: flex;
      justify-content: center;
      gap: 8px;
      margin-top: 6px;
    }

    /* ========================================
       FOOTER
    ======================================== */
    .geo-footer {
      text-align: center;
      padding: 12px;
      font-size: 12px;
      color: var(--geo-text-light);
    }

    .geo-footer a {
      font-weight: 700;
    }

    /* ========================================
       SPARKLE CURSOR TRAIL
    ======================================== */
    .geo-sparkle-field {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 9999;
      overflow: hidden;
    }

    @keyframes twinkle {
      0%, 100% { opacity: 0; transform: scale(0) rotate(0deg); }
      50%      { opacity: 1; transform: scale(1) rotate(180deg); }
    }

    .geo-sparkle-field .star {
      position: absolute;
      width: 8px;
      height: 8px;
      background: #FFFF00;
      clip-path: polygon(
        50% 0%, 61% 35%, 98% 35%, 68% 57%,
        79% 91%, 50% 70%, 21% 91%, 32% 57%,
        2% 35%, 39% 35%
      );
      animation: twinkle 2.5s ease-in-out infinite;
      pointer-events: none;
    }

    .geo-sparkle-field .star:nth-child(1) { top: 5%; left: 3%; animation-delay: 0s; }
    .geo-sparkle-field .star:nth-child(2) { top: 12%; left: 90%; animation-delay: 0.5s; background: #FF69B4; }
    .geo-sparkle-field .star:nth-child(3) { top: 28%; left: 95%; animation-delay: 1.2s; width: 6px; height: 6px; }
    .geo-sparkle-field .star:nth-child(4) { top: 42%; left: 2%; animation-delay: 0.8s; background: #00FFFF; }
    .geo-sparkle-field .star:nth-child(5) { top: 58%; left: 92%; animation-delay: 1.8s; }
    .geo-sparkle-field .star:nth-child(6) { top: 72%; left: 5%; animation-delay: 0.3s; background: #FF00FF; width: 10px; height: 10px; }
    .geo-sparkle-field .star:nth-child(7) { top: 85%; left: 88%; animation-delay: 2.1s; width: 6px; height: 6px; background: #00FF00; }
    .geo-sparkle-field .star:nth-child(8) { top: 95%; left: 50%; animation-delay: 1.5s; background: #FF69B4; }

    /* ========================================
       REDUCED MOTION
    ======================================== */
    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
      }
    }

    /* ========================================
       MOBILE STACK (not authentic, but usable)
    ======================================== */
    @media (max-width: 600px) {
      .geo-table {
        grid-template-columns: 1fr;
      }
      .geo-sidebar {
        order: 2;
      }
    }
  </style>
</head>
<body>

  <!-- Sparkle decorations -->
  <div class="geo-sparkle-field">
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
    <div class="star"></div>
  </div>

  <div class="geo-page">

    <!-- Marquee banner -->
    <div class="geo-marquee">
      <span>~*~ WELCOME TO MY HOMEPAGE ~*~ YOU ARE VISITOR #004,782 ~*~ BEST VIEWED IN NETSCAPE NAVIGATOR AT 800x600 ~*~ SIGN MY GUESTBOOK ~*~ LAST UPDATED 03/14/1999 ~*~</span>
    </div>

    <!-- Hero / Welcome banner -->
    <div class="geo-hero">
      <h1>~*~ Welcome To My Homepage ~*~</h1>
      <p class="subtitle">The Official Internet Home of CyberSurfer2000</p>
      <br>
      <span class="blink" style="color: #FF00FF; font-weight: 700; font-size: 1.1rem;">*** YOU HAVE FOUND THE COOLEST PAGE ON THE WEB ***</span>
    </div>

    <!-- Rainbow divider -->
    <hr class="geo-hr">

    <!-- Table layout: sidebar + main content -->
    <div class="geo-table">

      <!-- Sidebar navigation -->
      <div class="geo-sidebar">
        <h3>Navigation</h3>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About Me</a></li>
          <li><a href="#">My Pets</a> <span class="badge">NEW!</span></li>
          <li><a href="#">Cool Links</a></li>
          <li><a href="#">Guestbook</a></li>
          <li><a href="#">Awards</a></li>
          <li><a href="#">Webrings</a></li>
          <li><a href="#">Email Me!</a></li>
        </ul>
        <br>
        <div style="text-align: center;">
          <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='88' height='31'%3E%3Crect width='88' height='31' fill='%23000066' stroke='%23C0C0C0'/%3E%3Ctext x='44' y='20' fill='%2300FFFF' font-family='monospace' font-size='10' text-anchor='middle'%3EGeoCities%3C/text%3E%3C/svg%3E" alt="GeoCities badge" width="88" height="31" style="margin: 4px 0;">
          <br>
          <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='88' height='31'%3E%3Crect width='88' height='31' fill='%23000000' stroke='%23FF6600'/%3E%3Ctext x='44' y='20' fill='%23FF6600' font-family='monospace' font-size='9' text-anchor='middle'%3ENetscape Now%3C/text%3E%3C/svg%3E" alt="Netscape Now badge" width="88" height="31" style="margin: 4px 0;">
        </div>
      </div>

      <!-- Main content area -->
      <div class="geo-main">
        <h2>About This Page</h2>
        <p>
          Hey there! Welcome to my corner of the World Wide Web! My name is Chris and I
          live in California. I made this page to share my interests with everyone on the
          Internet. I like computers, skateboarding, and collecting cool animated GIFs.
          This page is always being updated so check back often!!
        </p>

        <!-- Under construction banner -->
        <div class="geo-construction">
          <span class="spin">&#9888;</span>
          <span class="geo-construction-text">Under Construction!!</span>
          <span class="spin">&#9888;</span>
        </div>

        <p>
          I am still working on adding more pages to this site. Come back soon to see
          my collection of cool links and my page about my dog Buster!
        </p>

        <hr class="geo-hr">

        <!-- Content cards -->
        <div class="geo-card">
          <h3>My Favorite Links</h3>
          <p>
            <a href="#">Yahoo!</a> |
            <a href="#">AltaVista</a> |
            <a href="#">Angelfire</a> |
            <a href="#">Neopets</a> |
            <a href="#">Hamster Dance</a>
          </p>
        </div>

        <div class="geo-card">
          <h3>Cool Facts About Me</h3>
          <p style="text-align: left; color: #00FF00;">
            <span style="color: #FF00FF;">&#9733;</span> I have been making web pages since 1997!<br>
            <span style="color: #FF00FF;">&#9733;</span> My favorite color is <span style="color: #00FFFF;">cyan</span><br>
            <span style="color: #FF00FF;">&#9733;</span> I know HTML, and I'm learning JavaScript!<br>
            <span style="color: #FF00FF;">&#9733;</span> I have a <span style="color: #FFFF00;">28.8k modem</span> (upgrading soon!!)<br>
            <span style="color: #FF00FF;">&#9733;</span> This page was made in Notepad!
          </p>
        </div>

        <hr class="geo-hr">

        <!-- Guestbook section -->
        <div class="geo-guestbook">
          <h3>&#9997; Sign My Guestbook! &#9997;</h3>

          <div class="geo-guestbook-entry">
            <span class="author">SurfDude99</span> - <span class="date">02/28/1999</span><br>
            Cool page dude!! Check out my site too -> <a href="#">SurfDude's Shack</a>
          </div>

          <div class="geo-guestbook-entry">
            <span class="author">~*StarGirl*~</span> - <span class="date">02/15/1999</span><br>
            Love the animated GIFs!! How did you make the background?? Email me!
          </div>

          <div class="geo-guestbook-entry">
            <span class="author">WebMaster_Jim</span> - <span class="date">01/30/1999</span><br>
            Nice page! I added you to my links section. Keep up the good work!
          </div>

          <br>
          <input type="text" placeholder="Your Name">
          <textarea placeholder="Leave a message!"></textarea>
          <button class="geo-btn">Sign Guestbook</button>
        </div>

      </div>
    </div>

    <hr class="geo-hr">

    <!-- Web ring -->
    <div class="geo-webring">
      <p>This site is part of the <strong>Cool Homepages Web Ring</strong></p>
      <div class="geo-webring-nav">
        <a href="#" class="geo-btn" style="min-width: auto; font-size: 12px; padding: 2px 10px;">&#9664; Prev</a>
        <a href="#" class="geo-btn" style="min-width: auto; font-size: 12px; padding: 2px 10px;">Random</a>
        <a href="#" class="geo-btn" style="min-width: auto; font-size: 12px; padding: 2px 10px;">List</a>
        <a href="#" class="geo-btn" style="min-width: auto; font-size: 12px; padding: 2px 10px;">Next &#9654;</a>
      </div>
    </div>

    <!-- Footer with counter -->
    <div class="geo-footer">
      <div class="geo-counter" style="margin-bottom: 8px; display: inline-flex;">
        <span class="geo-counter-label">You are visitor #</span>
        <div class="geo-counter-digits">
          <span class="geo-counter-digit">0</span>
          <span class="geo-counter-digit">0</span>
          <span class="geo-counter-digit">4</span>
          <span class="geo-counter-digit">7</span>
          <span class="geo-counter-digit">8</span>
          <span class="geo-counter-digit">2</span>
        </div>
      </div>
      <br><br>
      <a href="#">Guestbook</a> | <a href="#">Links</a> | <a href="#">Email Me</a>
      <br><br>
      <span style="color: #999999;">
        &copy; 1999 CyberSurfer2000. All Rights Reserved.<br>
        Made with Notepad. Best viewed in Netscape Navigator 4.0 at 800x600.
      </span>
      <br>
      <span style="font-size: 10px; color: #666666;">
        This page is part of GeoCities / SunsetStrip / 4782
      </span>
    </div>

  </div>

</body>
</html>
```
