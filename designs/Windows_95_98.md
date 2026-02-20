# Windows 95/98 - Design Reference

The Windows 95/98 aesthetic recreates the iconic graphical user interface of Microsoft's mid-to-late 1990s operating systems. It is defined by grey panel surfaces, beveled 3D borders achieved through layered highlights and shadows, pixel-perfect bitmap typography, and a restrained palette anchored by silver-grey and teal. Every element -- buttons, title bars, scrollbars, dialog boxes -- uses a strict system of raised and sunken borders to communicate interactivity and depth on low-resolution CRT monitors. The style evokes nostalgia for an era when personal computing first became mainstream, and it has experienced a strong revival in web design, indie games, and digital art as designers embrace its lo-fi charm, rigorous structure, and unapologetic utilitarianism.

---

## Visual Characteristics

### Core Design Traits

- **Beveled 3D borders** -- every interactive element uses a four-tone border system (white highlight on top-left, light grey inner highlight, dark grey inner shadow, black outer shadow) to simulate raised or sunken surfaces
- **Grey panel surfaces** -- the universal background is a neutral silver-grey (#C0C0C0), creating a flat, industrial canvas for all UI elements
- **Pixel-perfect rendering** -- text, icons, and borders align precisely to a pixel grid with no anti-aliasing, sub-pixel rendering, or fractional sizing
- **System title bars** -- windows feature a dark blue gradient title bar with white text, minimize/maximize/close buttons, and a distinct active/inactive state
- **Teal desktop background** -- the default #008080 teal wallpaper is as iconic as the UI itself, providing the signature color accent
- **Chunky scrollbars** -- wide scrollbar tracks with beveled arrow buttons and a draggable thumb, all rendered in the grey-and-bevel system
- **256-color icon system** -- small, meticulously pixeled icons at 16x16 and 32x32 sizes with limited color palettes and dithering patterns
- **Rigid rectangular geometry** -- no rounded corners, no curves, no organic shapes; every element is a sharp-edged rectangle
- **Status bars and toolbars** -- sunken text fields at the bottom of windows and raised toolbar strips with icon buttons at the top
- **Modal dialog boxes** -- centered system dialogs with icon, message text, and a row of beveled buttons for user decisions
- **Start menu paradigm** -- hierarchical cascading menus emerging from the bottom-left taskbar button

### Design Principles

- Communicate state through border direction: raised means clickable, sunken means active or input area
- Maintain absolute consistency across every element -- the same border widths, the same grey tones, the same padding
- Prioritize clarity and function over decoration; every pixel serves a purpose
- Use system fonts at fixed sizes for legibility on low-resolution screens
- Restrict the color palette to system-safe colors; avoid gradients and blending
- Enforce a strict visual hierarchy through window layering (z-index stacking), not through size or color variation
- Design for mouse interaction: visible focus states, hover affordances, drag handles
- Keep layouts compact and information-dense; screen real estate is precious at 640x480 or 800x600

---

## Color Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Desktop Teal** | `#008080` | Default desktop wallpaper background, signature accent color |
| **Button Face** | `#C0C0C0` | Default surface color for windows, buttons, panels, dialogs, and toolbars |
| **Button Highlight** | `#FFFFFF` | Top and left outer border edge on raised elements; brightest highlight |
| **Button Light** | `#DFDFDF` | Top and left inner border edge on raised elements; secondary highlight |
| **Button Shadow** | `#808080` | Bottom and right inner border edge on raised elements; secondary shadow |
| **Button Dark Shadow** | `#000000` | Bottom and right outer border edge on raised elements; deepest shadow |
| **Active Title Bar** | `#000080` | Background gradient start for active window title bars |
| **Active Title Bar End** | `#1084D0` | Background gradient end for active window title bars |
| **Inactive Title Bar** | `#808080` | Background for inactive window title bars |
| **Title Bar Text** | `#FFFFFF` | White text rendered on title bars |
| **Window Background** | `#FFFFFF` | White content area inside text fields, list boxes, tree views |
| **Window Text** | `#000000` | Black text inside content areas and body copy |
| **Selected Item** | `#000080` | Background for selected/highlighted items in lists and menus |
| **Selected Text** | `#FFFFFF` | White text on selected item backgrounds |
| **Disabled Text** | `#808080` | Greyed-out text for unavailable menu items and disabled buttons |
| **Menu Bar** | `#C0C0C0` | Background for menu bars, matching the button face |
| **Tooltip Background** | `#FFFFE1` | Pale yellow background for system tooltips |
| **Tooltip Text** | `#000000` | Black text rendered inside tooltips |
| **Link Blue** | `#0000FF` | Hyperlink text in help files and early Internet Explorer |
| **Visited Link** | `#800080` | Visited hyperlink purple |

### CSS Custom Properties

```css
:root {
  /* Surface colors */
  --win98-desktop: #008080;
  --win98-surface: #C0C0C0;
  --win98-window-bg: #FFFFFF;
  --win98-tooltip-bg: #FFFFE1;

  /* Border system (raised) */
  --win98-border-lightest: #FFFFFF;
  --win98-border-light: #DFDFDF;
  --win98-border-dark: #808080;
  --win98-border-darkest: #000000;

  /* Title bar */
  --win98-titlebar-active: #000080;
  --win98-titlebar-active-end: #1084D0;
  --win98-titlebar-inactive: #808080;
  --win98-titlebar-inactive-end: #B5B5B5;
  --win98-titlebar-text: #FFFFFF;

  /* Text */
  --win98-text: #000000;
  --win98-text-disabled: #808080;
  --win98-text-link: #0000FF;
  --win98-text-visited: #800080;

  /* Selection */
  --win98-selection-bg: #000080;
  --win98-selection-text: #FFFFFF;

  /* Accent */
  --win98-teal: #008080;
  --win98-navy: #000080;
}
```

---

## Typography

### Typeface Characteristics

Windows 95/98 typography is:

- **Bitmap/raster-based** -- the system font MS Sans Serif was a pixel font defined dot-by-dot, not as vector outlines
- **Non-anti-aliased** -- text renders with hard pixel edges and no smoothing, giving it a crisp, crunchy appearance
- **Small and compact** -- default sizes are 8pt for UI labels and menus, maximizing information density
- **Monospaced for code contexts** -- Fixedsys and Courier served terminal windows, Notepad, and developer tools
- **Limited weight variation** -- only regular and bold weights were commonly available; no light, thin, or black variants
- **Latin-script optimized** -- character sets were limited; ClearType and Unicode support came later
- **Strictly left-aligned** -- center and right alignment were rare outside of dialog button rows

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **VT323** | Pixel/monospace, classic CRT feel | Headings, display text, terminal output, nostalgic accents |
| **Press Start 2P** | Chunky 8-bit pixel font | Logos, hero headlines, decorative display text |
| **Pixelify Sans** | Clean pixel sans-serif | Body text in pixel style, UI labels, menus |
| **IBM Plex Mono** | Modern monospace with retro roots | Code blocks, status bars, system information text |
| **IBM Plex Sans** | Clean humanist sans-serif | Body text alternative when pixel fonts reduce readability |
| **Roboto** | Neo-grotesque, neutral | Body text fallback, readable at all sizes |
| **Courier Prime** | Refined Courier revival | Code, terminal output, monospaced content |
| **Share Tech Mono** | Technical monospace | Toolbars, system stats, address bars |
| **Silkscreen** | Bitmap-style pixel font | Navigation, buttons, small UI labels |
| **DotGothic16** | Japanese pixel font | Multilingual pixel interfaces, decorative headers |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **VT323** (400) | **IBM Plex Sans** (400) | Nostalgic headings with readable body text |
| **Press Start 2P** (400) | **Pixelify Sans** (400) | Full pixel aesthetic, game/retro feel |
| **Pixelify Sans** (700) | **Roboto** (400) | Balanced retro heading with modern readability |
| **Silkscreen** (400) | **IBM Plex Mono** (400) | System UI feel, technical documentation |
| **Share Tech Mono** (400) | **IBM Plex Sans** (400) | Technical/developer oriented retro layout |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=VT323&family=IBM+Plex+Sans:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&family=Pixelify+Sans:wght@400;700&display=swap');

/* Headings -- pixel font for nostalgic feel */
h1, h2, h3, h4, h5, h6 {
  font-family: 'VT323', 'Pixelify Sans', monospace;
  font-weight: 400;
  color: var(--win98-text);
  line-height: 1.2;
  letter-spacing: 0.02em;
}

/* Display / Hero text */
.win98-display {
  font-family: 'VT323', monospace;
  font-size: clamp(2rem, 4vw, 3.5rem);
  font-weight: 400;
  line-height: 1.1;
}

/* Body text -- readable modern sans for comfort */
body {
  font-family: 'IBM Plex Sans', 'Roboto', 'Tahoma', 'MS Sans Serif', sans-serif;
  font-weight: 400;
  font-size: 13px;
  line-height: 1.5;
  color: var(--win98-text);
  -webkit-font-smoothing: none;
  -moz-osx-font-smoothing: grayscale;
}

/* UI labels -- small, system-like */
.win98-label {
  font-family: 'Pixelify Sans', 'IBM Plex Sans', sans-serif;
  font-weight: 400;
  font-size: 12px;
  letter-spacing: 0;
}

/* Monospace / code / status bar */
.win98-mono {
  font-family: 'IBM Plex Mono', 'Courier Prime', 'Fixedsys', monospace;
  font-weight: 400;
  font-size: 13px;
  line-height: 1.4;
}

/* Title bar text */
.win98-titlebar-text {
  font-family: 'Pixelify Sans', 'IBM Plex Sans', sans-serif;
  font-weight: 700;
  font-size: 12px;
  color: var(--win98-titlebar-text);
}
```

---

## Layout Principles

### Grid and Structure

- **Fixed-width containers** -- classic Win98 interfaces used exact pixel dimensions; web recreations typically use a max-width of 800-1024px to evoke the era's screen resolutions
- **No fractional sizing** -- all dimensions, padding, and margins should be whole pixel values; use `px` units, not `rem` or `em`, for authentic rendering
- **Window-based composition** -- the page is organized as a collection of "window" panels, each with a title bar, content area, and optional status bar
- **Nested panel hierarchy** -- windows contain toolbars, content regions, and status bars as distinct sunken or raised sub-panels
- **Taskbar anchoring** -- a fixed-position bottom bar mimics the Windows taskbar with a Start button and clock
- **Compact spacing** -- padding inside panels is typically 2-4px; spacing between elements is tight by modern standards
- **Z-index stacking** -- overlapping windows create depth through layering, with active windows on top and drop-shadow or border emphasis

### Section Organization

- **Taskbar**: Fixed bottom bar with Start button (raised bevel), quick-launch icons, and a sunken clock area on the right
- **Desktop area**: Teal background with scattered icon shortcuts arranged in a grid
- **Window panels**: Each content section is framed as a draggable window with title bar, menu bar, toolbar, content body, and status bar
- **Dialog boxes**: Centered modal panels with an icon (information, warning, error, question), message text, and a row of action buttons
- **Menu system**: Dropdown menus with beveled borders, separator lines, keyboard shortcut annotations, and disabled item states
- **Tabbed interfaces**: Folder-tab controls along the top of content areas for switching between views

### Responsive Approach

- **Desktop-first design** -- the aesthetic is inherently desktop-oriented; design for 800px+ widths first
- **Stack windows vertically on mobile** -- convert overlapping desktop windows into a single-column stacked layout on narrow screens
- **Preserve bevel integrity** -- border widths and shadow offsets must remain constant (1-2px) regardless of viewport size; do not scale them
- **Collapse menus into a single Start-style button on mobile** -- the cascading menu system maps naturally to a hamburger/Start menu pattern
- **Allow horizontal scroll for toolbars** -- toolbars with many icon buttons can scroll horizontally rather than wrapping
- **Keep the taskbar fixed** -- the bottom taskbar remains visible as a persistent navigation element at all breakpoints

---

## CSS / Design Techniques

### Window / Card Component

The fundamental building block of the Windows 95/98 aesthetic is the window panel with its characteristic beveled border system.

```css
/* Raised panel (window frame, buttons) */
.win98-window {
  background: var(--win98-surface);
  border-top: 2px solid var(--win98-border-lightest);
  border-left: 2px solid var(--win98-border-lightest);
  border-right: 2px solid var(--win98-border-darkest);
  border-bottom: 2px solid var(--win98-border-darkest);
  box-shadow:
    inset 1px 1px 0 var(--win98-border-light),
    inset -1px -1px 0 var(--win98-border-dark);
  padding: 3px;
}

/* Alternative: box-shadow-only approach for raised effect */
.win98-raised {
  background: var(--win98-surface);
  box-shadow:
    inset -1px -1px 0 var(--win98-border-darkest),
    inset 1px 1px 0 var(--win98-border-lightest),
    inset -2px -2px 0 var(--win98-border-dark),
    inset 2px 2px 0 var(--win98-border-light);
}

/* Sunken panel (text inputs, status bar fields, content wells) */
.win98-sunken {
  background: var(--win98-window-bg);
  box-shadow:
    inset -1px -1px 0 var(--win98-border-lightest),
    inset 1px 1px 0 var(--win98-border-darkest),
    inset -2px -2px 0 var(--win98-border-light),
    inset 2px 2px 0 var(--win98-border-dark);
}

/* Title bar */
.win98-titlebar {
  background: linear-gradient(to right, var(--win98-titlebar-active), var(--win98-titlebar-active-end));
  color: var(--win98-titlebar-text);
  font-weight: bold;
  font-size: 12px;
  padding: 2px 4px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  user-select: none;
}

.win98-titlebar.inactive {
  background: linear-gradient(to right, var(--win98-titlebar-inactive), var(--win98-titlebar-inactive-end));
}

/* Title bar buttons (minimize, maximize, close) */
.win98-titlebar-btn {
  width: 16px;
  height: 14px;
  min-width: 16px;
  background: var(--win98-surface);
  border-top: 1px solid var(--win98-border-lightest);
  border-left: 1px solid var(--win98-border-lightest);
  border-right: 1px solid var(--win98-border-darkest);
  border-bottom: 1px solid var(--win98-border-darkest);
  box-shadow:
    inset 1px 1px 0 var(--win98-border-light),
    inset -1px -1px 0 var(--win98-border-dark);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0;
  font-size: 10px;
  line-height: 1;
  cursor: pointer;
}
```

### Button Component

```css
/* Standard raised button */
.win98-button {
  background: var(--win98-surface);
  color: var(--win98-text);
  border: none;
  font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
  font-size: 12px;
  padding: 4px 16px;
  min-width: 75px;
  min-height: 23px;
  cursor: pointer;
  box-shadow:
    inset -1px -1px 0 var(--win98-border-darkest),
    inset 1px 1px 0 var(--win98-border-lightest),
    inset -2px -2px 0 var(--win98-border-dark),
    inset 2px 2px 0 var(--win98-border-light);
}

/* Pressed / active state -- borders invert */
.win98-button:active {
  box-shadow:
    inset -1px -1px 0 var(--win98-border-lightest),
    inset 1px 1px 0 var(--win98-border-darkest),
    inset -2px -2px 0 var(--win98-border-light),
    inset 2px 2px 0 var(--win98-border-dark);
  padding: 5px 15px 3px 17px;
}

/* Focused button -- dotted inner border */
.win98-button:focus {
  outline: none;
  box-shadow:
    inset -1px -1px 0 var(--win98-border-darkest),
    inset 1px 1px 0 var(--win98-border-lightest),
    inset -2px -2px 0 var(--win98-border-dark),
    inset 2px 2px 0 var(--win98-border-light);
}

.win98-button:focus::after {
  content: '';
  position: absolute;
  top: 4px;
  left: 4px;
  right: 4px;
  bottom: 4px;
  border: 1px dotted var(--win98-text);
  pointer-events: none;
}

/* Default (primary) button -- extra outer border */
.win98-button.default {
  border: 2px solid var(--win98-border-darkest);
  padding: 2px 14px;
}

/* Disabled button */
.win98-button:disabled {
  color: var(--win98-border-dark);
  text-shadow: 1px 1px 0 var(--win98-border-lightest);
  cursor: default;
}
```

### Navigation / Menu Bar

```css
/* Menu bar strip */
.win98-menubar {
  background: var(--win98-surface);
  display: flex;
  padding: 2px 0;
  border-bottom: 1px solid var(--win98-border-dark);
}

/* Menu bar item */
.win98-menubar-item {
  padding: 2px 8px;
  font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
  font-size: 12px;
  cursor: pointer;
  position: relative;
}

.win98-menubar-item:hover {
  box-shadow:
    inset -1px -1px 0 var(--win98-border-darkest),
    inset 1px 1px 0 var(--win98-border-lightest);
}

/* Dropdown menu */
.win98-dropdown {
  position: absolute;
  background: var(--win98-surface);
  border-top: 2px solid var(--win98-border-lightest);
  border-left: 2px solid var(--win98-border-lightest);
  border-right: 2px solid var(--win98-border-darkest);
  border-bottom: 2px solid var(--win98-border-darkest);
  box-shadow:
    inset 1px 1px 0 var(--win98-border-light),
    inset -1px -1px 0 var(--win98-border-dark);
  padding: 2px;
  min-width: 160px;
  z-index: 1000;
}

/* Menu item */
.win98-menu-item {
  padding: 3px 24px 3px 28px;
  font-size: 12px;
  cursor: pointer;
  white-space: nowrap;
}

.win98-menu-item:hover {
  background: var(--win98-selection-bg);
  color: var(--win98-selection-text);
}

/* Menu separator */
.win98-menu-separator {
  height: 1px;
  background: var(--win98-border-dark);
  border-bottom: 1px solid var(--win98-border-lightest);
  margin: 3px 2px;
}

/* Disabled menu item */
.win98-menu-item.disabled {
  color: var(--win98-border-dark);
  text-shadow: 1px 1px 0 var(--win98-border-lightest);
  cursor: default;
}

.win98-menu-item.disabled:hover {
  background: transparent;
  color: var(--win98-border-dark);
}
```

### Hero / Desktop Area

```css
/* Desktop background */
.win98-desktop {
  background: var(--win98-desktop);
  min-height: 100vh;
  padding: 8px;
  padding-bottom: 40px; /* space for taskbar */
  position: relative;
}

/* Desktop icon */
.win98-desktop-icon {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 75px;
  padding: 4px;
  cursor: pointer;
  text-align: center;
}

.win98-desktop-icon img {
  width: 32px;
  height: 32px;
  image-rendering: pixelated;
}

.win98-desktop-icon span {
  font-size: 11px;
  color: white;
  text-shadow: 1px 1px 1px black;
  margin-top: 4px;
  word-wrap: break-word;
}

.win98-desktop-icon:focus span,
.win98-desktop-icon.selected span {
  background: var(--win98-selection-bg);
  color: var(--win98-selection-text);
}
```

### Taskbar

```css
/* Taskbar */
.win98-taskbar {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 32px;
  background: var(--win98-surface);
  border-top: 2px solid var(--win98-border-lightest);
  display: flex;
  align-items: center;
  padding: 2px 4px;
  z-index: 9999;
  gap: 4px;
}

/* Start button */
.win98-start-btn {
  font-weight: bold;
  font-size: 12px;
  padding: 2px 8px;
  display: flex;
  align-items: center;
  gap: 4px;
  min-width: auto;
  height: 24px;
}

/* Taskbar window buttons area */
.win98-taskbar-windows {
  display: flex;
  flex: 1;
  gap: 2px;
  overflow: hidden;
}

.win98-taskbar-window-btn {
  font-size: 11px;
  padding: 2px 8px;
  height: 22px;
  min-width: 120px;
  max-width: 180px;
  text-align: left;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

/* System tray / notification area */
.win98-systray {
  display: flex;
  align-items: center;
  gap: 6px;
  padding: 1px 8px;
  font-size: 11px;
  box-shadow:
    inset -1px -1px 0 var(--win98-border-lightest),
    inset 1px 1px 0 var(--win98-border-dark);
  height: 22px;
}
```

### Form Inputs

```css
/* Text input */
.win98-input {
  background: var(--win98-window-bg);
  color: var(--win98-text);
  font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
  font-size: 12px;
  padding: 3px 4px;
  border: none;
  box-shadow:
    inset -1px -1px 0 var(--win98-border-lightest),
    inset 1px 1px 0 var(--win98-border-darkest),
    inset -2px -2px 0 var(--win98-border-light),
    inset 2px 2px 0 var(--win98-border-dark);
  outline: none;
}

/* Checkbox */
.win98-checkbox {
  appearance: none;
  -webkit-appearance: none;
  width: 13px;
  height: 13px;
  background: var(--win98-window-bg);
  box-shadow:
    inset -1px -1px 0 var(--win98-border-lightest),
    inset 1px 1px 0 var(--win98-border-darkest),
    inset -2px -2px 0 var(--win98-border-light),
    inset 2px 2px 0 var(--win98-border-dark);
  cursor: pointer;
  vertical-align: middle;
  position: relative;
}

.win98-checkbox:checked::after {
  content: '\\2713';
  position: absolute;
  top: -1px;
  left: 1px;
  font-size: 12px;
  font-weight: bold;
  color: var(--win98-text);
}

/* Select / dropdown */
.win98-select {
  background: var(--win98-window-bg);
  color: var(--win98-text);
  font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
  font-size: 12px;
  padding: 2px 20px 2px 4px;
  border: none;
  box-shadow:
    inset -1px -1px 0 var(--win98-border-lightest),
    inset 1px 1px 0 var(--win98-border-darkest),
    inset -2px -2px 0 var(--win98-border-light),
    inset 2px 2px 0 var(--win98-border-dark);
  outline: none;
  cursor: pointer;
}

/* Group box (fieldset) */
.win98-groupbox {
  border: none;
  padding: 12px 8px 8px;
  margin: 8px 0;
  box-shadow:
    inset 0 0 0 1px var(--win98-border-dark),
    inset 0 0 0 2px var(--win98-border-lightest);
}

.win98-groupbox legend {
  font-size: 12px;
  padding: 0 4px;
  background: var(--win98-surface);
}
```

### Tab Control

```css
/* Tab container */
.win98-tabs {
  display: flex;
  padding: 0 4px;
  position: relative;
  bottom: -2px;
  z-index: 1;
}

/* Individual tab */
.win98-tab {
  background: var(--win98-surface);
  border-top: 2px solid var(--win98-border-lightest);
  border-left: 2px solid var(--win98-border-lightest);
  border-right: 2px solid var(--win98-border-darkest);
  border-bottom: none;
  padding: 4px 16px;
  font-size: 12px;
  cursor: pointer;
  position: relative;
  margin-right: 2px;
}

.win98-tab.active {
  background: var(--win98-surface);
  padding-bottom: 6px;
  margin-bottom: -2px;
  z-index: 2;
}

/* Tab content area */
.win98-tab-content {
  background: var(--win98-surface);
  border-top: 2px solid var(--win98-border-lightest);
  border-left: 2px solid var(--win98-border-lightest);
  border-right: 2px solid var(--win98-border-darkest);
  border-bottom: 2px solid var(--win98-border-darkest);
  padding: 12px;
  position: relative;
  z-index: 0;
}
```

### Progress Bar

```css
/* Progress bar track */
.win98-progress {
  width: 100%;
  height: 18px;
  background: var(--win98-window-bg);
  box-shadow:
    inset -1px -1px 0 var(--win98-border-lightest),
    inset 1px 1px 0 var(--win98-border-darkest),
    inset -2px -2px 0 var(--win98-border-light),
    inset 2px 2px 0 var(--win98-border-dark);
  padding: 2px;
}

/* Segmented fill (classic Win98 style) */
.win98-progress-fill {
  height: 100%;
  background: repeating-linear-gradient(
    to right,
    var(--win98-selection-bg) 0px,
    var(--win98-selection-bg) 8px,
    transparent 8px,
    transparent 10px
  );
}
```

### Tooltip

```css
.win98-tooltip {
  background: var(--win98-tooltip-bg);
  color: var(--win98-text);
  border: 1px solid var(--win98-border-darkest);
  padding: 2px 6px;
  font-size: 11px;
  font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
  position: absolute;
  white-space: nowrap;
  z-index: 10000;
  pointer-events: none;
  box-shadow: 2px 2px 0 rgba(0, 0, 0, 0.15);
}
```

---

## Design Do's and Don'ts

### Do

- Use the four-tone beveled border system consistently on every interactive element (white highlight, light grey, dark grey, black shadow)
- Keep all measurements in whole pixels -- avoid sub-pixel rendering, fractional units, or anti-aliased borders
- Apply the sunken/raised border paradigm correctly: raised for clickable surfaces, sunken for input fields and status areas
- Use the exact system color palette (#C0C0C0, #808080, #FFFFFF, #000000, #000080, #008080) rather than approximations
- Include proper window chrome: title bar with gradient, control buttons (minimize, maximize, close), menu bar, and status bar
- Render text without font smoothing where possible (`-webkit-font-smoothing: none`) for authentic crispness
- Design compact, information-dense layouts that respect the low-resolution origins of the aesthetic
- Include a taskbar element with a Start button and clock to anchor the desktop metaphor
- Use `image-rendering: pixelated` on any icons or images to prevent blurring when scaled
- Ensure interactive elements have clear pressed/active states where all borders invert direction
- Add a focus indicator (dotted inner border, 1px) on keyboard-navigable elements for accessibility
- Layer windows with proper z-index stacking to create the illusion of a multi-window desktop

### Don't

- Do not use rounded corners anywhere -- the aesthetic is strictly rectangular
- Do not apply modern box-shadows, blur effects, or transparency -- the only shadows are the solid-color beveled borders
- Do not use gradients (except on title bars) -- all surfaces are flat, solid colors
- Do not over-scale the aesthetic -- huge beveled borders look wrong; keep borders at 1-2px as they were on actual 96dpi screens
- Do not mix modern UI paradigms (material ripples, glassmorphism, animated transitions) with the Win98 style
- Do not use web fonts with extensive anti-aliasing or OpenType features -- they clash with the pixel-perfect intent
- Do not center-align large blocks of text -- the original OS used left alignment almost exclusively
- Do not use vibrant, saturated accent colors beyond the system palette -- keep to the muted teal, navy, and grey scheme
- Do not forget disabled states -- greyed-out text with a white 1px offset shadow is essential for completeness
- Do not apply hover effects that change colors smoothly; state changes should be instant and binary (raised vs. sunken)
- Do not use SVG icons -- the aesthetic calls for raster/pixel art at fixed sizes (16x16, 32x32)

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **8-Bit** | Shares pixel-grid precision and bitmap rendering, but 8-Bit focuses on gaming consoles rather than desktop operating systems |
| **Early Cyber** | Both emerged from 1990s computing, but Early Cyber leans toward internet culture (animated GIFs, under-construction banners) while Win95/98 is about the OS itself |
| **Dial-Up Delight** | Overlaps in era and technology nostalgia; Dial-Up Delight focuses on the internet experience (loading bars, AOL) while Win95/98 focuses on the desktop shell |
| **Flat Design** | A philosophical descendant -- Flat Design stripped away the bevels and 3D effects that define Win95/98, replacing them with pure 2D surfaces |
| **Material Design** | Google's system inherits the structured component hierarchy and elevation concept from Win95/98 but replaces pixel borders with soft shadows and motion |
| **Frutiger Aero** | The glossy, transparent, nature-infused aesthetic that replaced the Win95/98 look in Windows Vista/7 -- a direct visual successor |
| **Skeuomorphism** | Win95/98 is proto-skeuomorphic: the beveled buttons simulate physical pushbuttons, preceding Apple's richer texture-heavy skeuomorphism |
| **Metro Design** | Microsoft's own reaction against Win95/98 chrome -- Metro stripped all bevels, borders, and ornamentation in favor of typography and flat tiles |
| **Cyberpunk** | Can borrow Win95/98 UI frames as retro-tech elements, embedding them in neon-lit dystopian compositions |
| **Mallsoft** | Shares the 1990s nostalgia angle and often uses Win95/98 interface frames as visual motifs in vaporwave-adjacent digital collage |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Windows 95/98 Aesthetic</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;500&family=IBM+Plex+Sans:wght@400;500;600&family=Pixelify+Sans:wght@400;700&family=VT323&display=swap" rel="stylesheet">
  <style>
    /* ========================================
       CSS CUSTOM PROPERTIES
    ======================================== */
    :root {
      --win98-desktop: #008080;
      --win98-surface: #C0C0C0;
      --win98-window-bg: #FFFFFF;
      --win98-tooltip-bg: #FFFFE1;

      --win98-border-lightest: #FFFFFF;
      --win98-border-light: #DFDFDF;
      --win98-border-dark: #808080;
      --win98-border-darkest: #000000;

      --win98-titlebar-active: #000080;
      --win98-titlebar-active-end: #1084D0;
      --win98-titlebar-inactive: #808080;
      --win98-titlebar-inactive-end: #B5B5B5;
      --win98-titlebar-text: #FFFFFF;

      --win98-text: #000000;
      --win98-text-disabled: #808080;
      --win98-text-link: #0000FF;
      --win98-text-visited: #800080;

      --win98-selection-bg: #000080;
      --win98-selection-text: #FFFFFF;
    }

    /* ========================================
       RESET & BASE
    ======================================== */
    *, *::before, *::after {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      height: 100%;
    }

    body {
      font-family: 'IBM Plex Sans', 'Tahoma', 'MS Sans Serif', sans-serif;
      font-size: 12px;
      line-height: 1.4;
      color: var(--win98-text);
      background: var(--win98-desktop);
      min-height: 100%;
      padding-bottom: 40px;
      -webkit-font-smoothing: none;
      -moz-osx-font-smoothing: grayscale;
    }

    /* ========================================
       RAISED & SUNKEN UTILITIES
    ======================================== */
    .raised {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-darkest),
        inset 1px 1px 0 var(--win98-border-lightest),
        inset -2px -2px 0 var(--win98-border-dark),
        inset 2px 2px 0 var(--win98-border-light);
    }

    .sunken {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
    }

    /* ========================================
       WINDOW COMPONENT
    ======================================== */
    .window {
      background: var(--win98-surface);
      box-shadow:
        inset -1px -1px 0 var(--win98-border-darkest),
        inset 1px 1px 0 var(--win98-border-lightest),
        inset -2px -2px 0 var(--win98-border-dark),
        inset 2px 2px 0 var(--win98-border-light);
      padding: 3px;
    }

    .title-bar {
      background: linear-gradient(to right, var(--win98-titlebar-active), var(--win98-titlebar-active-end));
      color: var(--win98-titlebar-text);
      font-family: 'Pixelify Sans', 'IBM Plex Sans', sans-serif;
      font-weight: 700;
      font-size: 12px;
      padding: 3px 4px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      user-select: none;
      margin-bottom: 2px;
    }

    .title-bar.inactive {
      background: linear-gradient(to right, var(--win98-titlebar-inactive), var(--win98-titlebar-inactive-end));
    }

    .title-bar-text {
      overflow: hidden;
      white-space: nowrap;
      text-overflow: ellipsis;
      letter-spacing: 0.5px;
    }

    .title-bar-controls {
      display: flex;
      gap: 2px;
    }

    .title-bar-controls button {
      width: 16px;
      height: 14px;
      min-width: 16px;
      background: var(--win98-surface);
      border: none;
      box-shadow:
        inset -1px -1px 0 var(--win98-border-darkest),
        inset 1px 1px 0 var(--win98-border-lightest),
        inset -2px -2px 0 var(--win98-border-dark),
        inset 2px 2px 0 var(--win98-border-light);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 0;
      font-size: 9px;
      font-family: 'IBM Plex Mono', monospace;
      font-weight: bold;
      line-height: 1;
      cursor: pointer;
    }

    .title-bar-controls button:active {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
    }

    .window-body {
      padding: 8px;
    }

    /* ========================================
       MENU BAR
    ======================================== */
    .menu-bar {
      display: flex;
      padding: 1px 0;
      margin-bottom: 2px;
    }

    .menu-bar span {
      padding: 2px 8px;
      cursor: pointer;
      font-size: 12px;
    }

    .menu-bar span:hover {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-darkest),
        inset 1px 1px 0 var(--win98-border-lightest);
    }

    .menu-bar span:active,
    .menu-bar span.open {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest);
    }

    /* ========================================
       BUTTONS
    ======================================== */
    button, .btn {
      background: var(--win98-surface);
      color: var(--win98-text);
      border: none;
      font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
      font-size: 12px;
      padding: 4px 16px;
      min-width: 75px;
      min-height: 23px;
      cursor: pointer;
      box-shadow:
        inset -1px -1px 0 var(--win98-border-darkest),
        inset 1px 1px 0 var(--win98-border-lightest),
        inset -2px -2px 0 var(--win98-border-dark),
        inset 2px 2px 0 var(--win98-border-light);
      position: relative;
    }

    button:active, .btn:active {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
      padding: 5px 15px 3px 17px;
    }

    button.default-btn {
      outline: 2px solid var(--win98-border-darkest);
      outline-offset: -4px;
    }

    button:disabled {
      color: var(--win98-border-dark);
      text-shadow: 1px 1px 0 var(--win98-border-lightest);
      cursor: default;
    }

    button:disabled:active {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-darkest),
        inset 1px 1px 0 var(--win98-border-lightest),
        inset -2px -2px 0 var(--win98-border-dark),
        inset 2px 2px 0 var(--win98-border-light);
      padding: 4px 16px;
    }

    /* ========================================
       FORM INPUTS
    ======================================== */
    input[type="text"],
    input[type="email"],
    input[type="password"],
    textarea,
    select {
      background: var(--win98-window-bg);
      color: var(--win98-text);
      font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
      font-size: 12px;
      padding: 3px 4px;
      border: none;
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
      outline: none;
    }

    textarea {
      resize: vertical;
      font-family: 'IBM Plex Mono', 'Courier New', monospace;
    }

    /* ========================================
       TABS
    ======================================== */
    .tabs {
      display: flex;
      padding: 0 4px;
      position: relative;
      bottom: -2px;
      z-index: 1;
    }

    .tab {
      background: var(--win98-surface);
      border-top: 2px solid var(--win98-border-lightest);
      border-left: 2px solid var(--win98-border-lightest);
      border-right: 2px solid var(--win98-border-darkest);
      border-bottom: none;
      padding: 4px 14px;
      font-size: 12px;
      cursor: pointer;
      position: relative;
      margin-right: 2px;
      box-shadow: none;
      min-width: auto;
      min-height: auto;
    }

    .tab.active {
      padding-bottom: 6px;
      margin-bottom: -2px;
      z-index: 2;
    }

    .tab-content {
      background: var(--win98-surface);
      border: 2px solid;
      border-color: var(--win98-border-lightest) var(--win98-border-darkest) var(--win98-border-darkest) var(--win98-border-lightest);
      box-shadow:
        inset 1px 1px 0 var(--win98-border-light),
        inset -1px -1px 0 var(--win98-border-dark);
      padding: 12px;
      position: relative;
    }

    /* ========================================
       PROGRESS BAR
    ======================================== */
    .progress-track {
      width: 100%;
      height: 18px;
      background: var(--win98-window-bg);
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
      padding: 2px;
    }

    .progress-fill {
      height: 100%;
      background: repeating-linear-gradient(
        to right,
        var(--win98-selection-bg) 0px,
        var(--win98-selection-bg) 8px,
        transparent 8px,
        transparent 10px
      );
    }

    /* ========================================
       STATUS BAR
    ======================================== */
    .status-bar {
      display: flex;
      gap: 2px;
      margin-top: 2px;
    }

    .status-bar-field {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-dark);
      padding: 2px 6px;
      font-size: 11px;
      flex: 1;
      overflow: hidden;
      white-space: nowrap;
      text-overflow: ellipsis;
    }

    /* ========================================
       GROUP BOX
    ======================================== */
    fieldset {
      border: none;
      padding: 12px 8px 8px;
      margin: 8px 0;
      box-shadow:
        inset 0 0 0 1px var(--win98-border-dark),
        inset 0 0 0 2px var(--win98-border-lightest);
    }

    fieldset legend {
      font-size: 12px;
      padding: 0 4px;
      background: var(--win98-surface);
    }

    /* ========================================
       TREE VIEW
    ======================================== */
    .tree-view {
      background: var(--win98-window-bg);
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
      padding: 4px;
      font-size: 12px;
      overflow: auto;
    }

    .tree-view ul {
      list-style: none;
      padding-left: 16px;
    }

    .tree-view > ul {
      padding-left: 4px;
    }

    .tree-view li {
      padding: 1px 4px;
      cursor: pointer;
      white-space: nowrap;
    }

    .tree-view li:hover {
      background: var(--win98-selection-bg);
      color: var(--win98-selection-text);
    }

    .tree-view li::before {
      content: '\1F4C4 ';
      font-size: 11px;
    }

    .tree-view li.folder::before {
      content: '\1F4C1 ';
    }

    /* ========================================
       TASKBAR
    ======================================== */
    .taskbar {
      position: fixed;
      bottom: 0;
      left: 0;
      right: 0;
      height: 32px;
      background: var(--win98-surface);
      border-top: 2px solid var(--win98-border-lightest);
      display: flex;
      align-items: center;
      padding: 2px 4px;
      z-index: 9999;
      gap: 4px;
    }

    .start-btn {
      font-weight: bold;
      font-size: 12px;
      padding: 2px 8px;
      display: flex;
      align-items: center;
      gap: 4px;
      min-width: auto;
      height: 24px;
    }

    .start-btn .start-logo {
      width: 16px;
      height: 16px;
      background: linear-gradient(135deg, #FF0000 25%, #00FF00 25%, #00FF00 50%, #0000FF 50%, #0000FF 75%, #FFFF00 75%);
      display: inline-block;
    }

    .taskbar-windows {
      display: flex;
      flex: 1;
      gap: 2px;
      overflow: hidden;
    }

    .taskbar-window-btn {
      font-size: 11px;
      padding: 2px 8px;
      height: 22px;
      min-width: 100px;
      max-width: 160px;
      text-align: left;
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
      min-height: auto;
    }

    .taskbar-window-btn.active-window {
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
      font-weight: bold;
    }

    .systray {
      display: flex;
      align-items: center;
      gap: 6px;
      padding: 1px 8px;
      font-size: 11px;
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-dark);
      height: 22px;
      font-family: 'IBM Plex Sans', 'Tahoma', sans-serif;
    }

    /* ========================================
       DESKTOP & ICONS
    ======================================== */
    .desktop {
      min-height: 100vh;
      padding: 12px;
      padding-bottom: 48px;
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .desktop-icons {
      display: flex;
      flex-direction: column;
      gap: 8px;
      position: absolute;
      top: 12px;
      left: 12px;
    }

    .desktop-icon {
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 70px;
      padding: 4px;
      cursor: pointer;
      text-align: center;
      border: 1px solid transparent;
    }

    .desktop-icon:hover {
      border: 1px dotted var(--win98-border-lightest);
    }

    .desktop-icon .icon {
      width: 32px;
      height: 32px;
      font-size: 28px;
      line-height: 32px;
      image-rendering: pixelated;
    }

    .desktop-icon span {
      font-size: 11px;
      color: white;
      text-shadow: 1px 1px 1px black;
      margin-top: 2px;
      word-wrap: break-word;
      max-width: 68px;
    }

    /* ========================================
       LAYOUT HELPERS
    ======================================== */
    .windows-container {
      display: flex;
      flex-wrap: wrap;
      gap: 16px;
      padding: 12px;
      max-width: 1024px;
      margin: 0 auto;
      position: relative;
      z-index: 1;
    }

    .window-sm { width: 320px; }
    .window-md { width: 480px; }
    .window-lg { width: 100%; max-width: 680px; }
    .window-full { width: 100%; }

    /* ========================================
       TYPOGRAPHY
    ======================================== */
    h1, h2, h3 {
      font-family: 'VT323', 'Pixelify Sans', monospace;
      font-weight: 400;
    }

    h1 { font-size: 28px; }
    h2 { font-size: 22px; }
    h3 { font-size: 18px; }

    a {
      color: var(--win98-text-link);
    }

    a:visited {
      color: var(--win98-text-visited);
    }

    .pixel-text {
      font-family: 'VT323', monospace;
    }

    .mono-text {
      font-family: 'IBM Plex Mono', 'Courier New', monospace;
    }

    /* ========================================
       SEPARATOR
    ======================================== */
    hr {
      border: none;
      border-top: 1px solid var(--win98-border-dark);
      border-bottom: 1px solid var(--win98-border-lightest);
      margin: 8px 0;
    }

    /* ========================================
       DIALOG BOX
    ======================================== */
    .dialog-content {
      display: flex;
      gap: 16px;
      align-items: flex-start;
      margin-bottom: 16px;
    }

    .dialog-icon {
      font-size: 32px;
      flex-shrink: 0;
    }

    .dialog-buttons {
      display: flex;
      justify-content: center;
      gap: 6px;
    }

    /* ========================================
       LIST VIEW
    ======================================== */
    .list-view {
      background: var(--win98-window-bg);
      box-shadow:
        inset -1px -1px 0 var(--win98-border-lightest),
        inset 1px 1px 0 var(--win98-border-darkest),
        inset -2px -2px 0 var(--win98-border-light),
        inset 2px 2px 0 var(--win98-border-dark);
    }

    .list-view-header {
      display: flex;
      border-bottom: 1px solid var(--win98-border-dark);
    }

    .list-view-header span {
      padding: 2px 8px;
      font-size: 12px;
      font-weight: 500;
      background: var(--win98-surface);
      box-shadow:
        inset -1px -1px 0 var(--win98-border-darkest),
        inset 1px 1px 0 var(--win98-border-lightest);
      cursor: pointer;
      white-space: nowrap;
    }

    .list-view-row {
      display: flex;
      padding: 1px 0;
      font-size: 12px;
    }

    .list-view-row:hover {
      background: var(--win98-selection-bg);
      color: var(--win98-selection-text);
    }

    .list-view-row span {
      padding: 1px 8px;
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
    }

    /* Column widths */
    .col-name { width: 45%; }
    .col-size { width: 15%; text-align: right; }
    .col-type { width: 20%; }
    .col-modified { width: 20%; }

    /* ========================================
       RESPONSIVE
    ======================================== */
    @media (max-width: 768px) {
      .windows-container {
        padding: 8px;
        gap: 8px;
      }

      .window-sm,
      .window-md,
      .window-lg {
        width: 100%;
      }

      .desktop-icons {
        position: relative;
        top: auto;
        left: auto;
        flex-direction: row;
        flex-wrap: wrap;
        margin-bottom: 8px;
      }

      .taskbar-windows {
        display: none;
      }
    }
  </style>
</head>
<body>

  <!-- DESKTOP ICONS -->
  <div class="desktop-icons">
    <div class="desktop-icon">
      <div class="icon">&#128187;</div>
      <span>My Computer</span>
    </div>
    <div class="desktop-icon">
      <div class="icon">&#128193;</div>
      <span>My Documents</span>
    </div>
    <div class="desktop-icon">
      <div class="icon">&#128279;</div>
      <span>Internet Explorer</span>
    </div>
    <div class="desktop-icon">
      <div class="icon">&#128225;</div>
      <span>Network Neighborhood</span>
    </div>
    <div class="desktop-icon">
      <div class="icon">&#9851;</div>
      <span>Recycle Bin</span>
    </div>
  </div>

  <!-- MAIN CONTENT -->
  <div class="windows-container">

    <!-- ==========================================
         WINDOW 1: WELCOME / ABOUT
    ========================================== -->
    <div class="window window-lg">
      <div class="title-bar">
        <span class="title-bar-text">Welcome to Windows 98</span>
        <div class="title-bar-controls">
          <button>_</button>
          <button>&#9633;</button>
          <button>X</button>
        </div>
      </div>
      <div class="menu-bar">
        <span>File</span>
        <span>Edit</span>
        <span>View</span>
        <span>Help</span>
      </div>
      <div class="window-body">
        <h1 class="pixel-text" style="margin-bottom: 12px;">Welcome to Windows 98</h1>
        <p style="margin-bottom: 10px;">
          Thank you for choosing Microsoft Windows 98, the most exciting and powerful
          version of Windows yet. Windows 98 brings you faster system performance,
          easier ways to use your computer, and seamless integration with the Internet.
        </p>
        <p style="margin-bottom: 16px;">
          This page demonstrates the classic Windows 95/98 visual aesthetic recreated
          entirely with modern HTML and CSS. Every beveled border, grey panel, and
          pixel-perfect detail has been faithfully reproduced using box-shadow
          techniques and the original system color palette.
        </p>

        <!-- Tabs -->
        <div class="tabs">
          <div class="tab active">General</div>
          <div class="tab">Features</div>
          <div class="tab">Support</div>
        </div>
        <div class="tab-content">
          <fieldset>
            <legend>System Information</legend>
            <div style="display: grid; grid-template-columns: auto 1fr; gap: 4px 12px; font-size: 12px;">
              <strong>OS:</strong> <span>Microsoft Windows 98 Second Edition</span>
              <strong>Version:</strong> <span>4.10.2222 A</span>
              <strong>Registered to:</strong> <span>Home User</span>
              <strong>Product ID:</strong> <span>12345-OEM-6789012-34567</span>
              <strong>Processor:</strong> <span>Intel Pentium II 350 MHz</span>
              <strong>Memory:</strong> <span>64.0 MB RAM</span>
              <strong>Display:</strong> <span>800 x 600, 256 Colors</span>
            </div>
          </fieldset>
        </div>
      </div>
      <div class="status-bar">
        <div class="status-bar-field">Ready</div>
        <div class="status-bar-field" style="flex: 0 0 120px;">My Computer</div>
      </div>
    </div>

    <!-- ==========================================
         WINDOW 2: FILE EXPLORER
    ========================================== -->
    <div class="window window-lg">
      <div class="title-bar">
        <span class="title-bar-text">C:\My Documents</span>
        <div class="title-bar-controls">
          <button>_</button>
          <button>&#9633;</button>
          <button>X</button>
        </div>
      </div>
      <div class="menu-bar">
        <span>File</span>
        <span>Edit</span>
        <span>View</span>
        <span>Favorites</span>
        <span>Tools</span>
        <span>Help</span>
      </div>
      <div class="window-body" style="padding: 4px;">
        <!-- Address bar -->
        <div style="display: flex; align-items: center; gap: 4px; margin-bottom: 4px;">
          <span style="font-size: 12px;">Address</span>
          <input type="text" value="C:\My Documents" style="flex: 1; font-size: 12px;" readonly>
          <button style="min-width: auto; padding: 2px 8px; min-height: 20px;">Go</button>
        </div>

        <div style="display: flex; gap: 0;">
          <!-- Tree view sidebar -->
          <div class="tree-view" style="width: 180px; min-height: 200px; flex-shrink: 0;">
            <ul>
              <li class="folder">Desktop
                <ul>
                  <li class="folder">My Computer
                    <ul>
                      <li class="folder">C:</li>
                      <li class="folder">D:</li>
                    </ul>
                  </li>
                  <li class="folder" style="background: var(--win98-selection-bg); color: var(--win98-selection-text);">My Documents</li>
                  <li class="folder">Network</li>
                  <li class="folder">Recycle Bin</li>
                </ul>
              </li>
            </ul>
          </div>

          <!-- File list -->
          <div class="list-view" style="flex: 1;">
            <div class="list-view-header">
              <span class="col-name">Name</span>
              <span class="col-size">Size</span>
              <span class="col-type">Type</span>
              <span class="col-modified">Modified</span>
            </div>
            <div class="list-view-row">
              <span class="col-name">&#128193; My Pictures</span>
              <span class="col-size"></span>
              <span class="col-type">File Folder</span>
              <span class="col-modified">3/15/1999</span>
            </div>
            <div class="list-view-row">
              <span class="col-name">&#128193; My Music</span>
              <span class="col-size"></span>
              <span class="col-type">File Folder</span>
              <span class="col-modified">6/02/1999</span>
            </div>
            <div class="list-view-row">
              <span class="col-name">&#128196; Budget.xls</span>
              <span class="col-size">45 KB</span>
              <span class="col-type">Excel File</span>
              <span class="col-modified">11/23/1998</span>
            </div>
            <div class="list-view-row">
              <span class="col-name">&#128196; Letter.doc</span>
              <span class="col-size">12 KB</span>
              <span class="col-type">Word File</span>
              <span class="col-modified">1/08/1999</span>
            </div>
            <div class="list-view-row">
              <span class="col-name">&#128196; Notes.txt</span>
              <span class="col-size">2 KB</span>
              <span class="col-type">Text File</span>
              <span class="col-modified">4/17/1999</span>
            </div>
            <div class="list-view-row">
              <span class="col-name">&#127912; Wallpaper.bmp</span>
              <span class="col-size">1.4 MB</span>
              <span class="col-type">Bitmap Image</span>
              <span class="col-modified">8/30/1998</span>
            </div>
            <div class="list-view-row">
              <span class="col-name">&#128196; README.txt</span>
              <span class="col-size">1 KB</span>
              <span class="col-type">Text File</span>
              <span class="col-modified">9/12/1998</span>
            </div>
          </div>
        </div>
      </div>
      <div class="status-bar">
        <div class="status-bar-field">7 object(s)</div>
        <div class="status-bar-field" style="flex: 0 0 100px;">1.46 MB</div>
        <div class="status-bar-field" style="flex: 0 0 120px;">My Computer</div>
      </div>
    </div>

    <!-- ==========================================
         WINDOW 3: CONTROL PANEL / SETTINGS
    ========================================== -->
    <div class="window window-md">
      <div class="title-bar">
        <span class="title-bar-text">Display Properties</span>
        <div class="title-bar-controls">
          <button>X</button>
        </div>
      </div>
      <div class="window-body">
        <div class="tabs">
          <div class="tab">Background</div>
          <div class="tab">Screen Saver</div>
          <div class="tab active">Appearance</div>
          <div class="tab">Settings</div>
        </div>
        <div class="tab-content">
          <!-- Preview box -->
          <div class="sunken" style="background: var(--win98-desktop); padding: 16px; margin-bottom: 12px; min-height: 120px; display: flex; align-items: center; justify-content: center;">
            <div class="window" style="width: 200px;">
              <div class="title-bar" style="font-size: 10px; padding: 2px 3px;">
                <span class="title-bar-text">Active Window</span>
                <div class="title-bar-controls">
                  <button style="width: 12px; height: 10px; font-size: 7px;">X</button>
                </div>
              </div>
              <div class="window-body" style="padding: 6px; font-size: 10px;">
                Window Text Sample
              </div>
            </div>
          </div>

          <div style="display: flex; gap: 8px; align-items: center; margin-bottom: 8px;">
            <label style="font-size: 12px;">Scheme:</label>
            <select style="flex: 1;">
              <option>Windows Standard</option>
              <option>High Contrast Black</option>
              <option>Desert</option>
              <option>Eggplant</option>
              <option>Lilac</option>
              <option>Maple</option>
              <option>Marine</option>
              <option>Rainy Day</option>
              <option>Rose</option>
              <option>Slate</option>
              <option>Teal</option>
            </select>
          </div>

          <div style="display: flex; gap: 8px; align-items: center;">
            <label style="font-size: 12px;">Item:</label>
            <select style="flex: 1;">
              <option>Desktop</option>
              <option>Active Title Bar</option>
              <option>Inactive Title Bar</option>
              <option>Menu</option>
              <option>Message Box</option>
              <option>Scrollbar</option>
              <option>Window</option>
            </select>
          </div>
        </div>

        <div style="display: flex; justify-content: flex-end; gap: 6px; margin-top: 12px;">
          <button>OK</button>
          <button>Cancel</button>
          <button>Apply</button>
        </div>
      </div>
    </div>

    <!-- ==========================================
         WINDOW 4: NOTEPAD
    ========================================== -->
    <div class="window window-md">
      <div class="title-bar">
        <span class="title-bar-text">Untitled - Notepad</span>
        <div class="title-bar-controls">
          <button>_</button>
          <button>&#9633;</button>
          <button>X</button>
        </div>
      </div>
      <div class="menu-bar">
        <span>File</span>
        <span>Edit</span>
        <span>Search</span>
        <span>Help</span>
      </div>
      <div class="window-body" style="padding: 0;">
        <textarea rows="10" style="width: 100%; border: none; box-shadow: none; padding: 4px; font-size: 13px; resize: vertical;">Dear Diary,

Today I finally got Windows 98 installed. It only
took three floppy disks and two hours. The new
desktop looks amazing with that teal wallpaper.

I discovered you can right-click on things now
and a little menu pops up. The future is here.

Also found something called "The Internet" --
it makes a loud screeching noise when connecting
but then you can look at web pages. Amazing.

- Me, 1998</textarea>
      </div>
    </div>

    <!-- ==========================================
         WINDOW 5: DIALOG BOX
    ========================================== -->
    <div class="window window-sm">
      <div class="title-bar">
        <span class="title-bar-text">Windows</span>
        <div class="title-bar-controls">
          <button>X</button>
        </div>
      </div>
      <div class="window-body">
        <div class="dialog-content">
          <div class="dialog-icon">&#9432;</div>
          <div>
            <p style="margin-bottom: 4px; font-size: 12px;">
              This page has been designed using the authentic Windows 95/98
              visual language, including beveled borders, grey panels, and
              pixel-precise typography.
            </p>
            <p style="font-size: 12px;">
              Do you want to continue exploring?
            </p>
          </div>
        </div>
        <div class="dialog-buttons">
          <button class="default-btn">Yes</button>
          <button>No</button>
        </div>
      </div>
    </div>

    <!-- ==========================================
         WINDOW 6: DOWNLOAD PROGRESS
    ========================================== -->
    <div class="window window-sm">
      <div class="title-bar">
        <span class="title-bar-text">Downloading...</span>
        <div class="title-bar-controls">
          <button>X</button>
        </div>
      </div>
      <div class="window-body">
        <p style="font-size: 12px; margin-bottom: 8px;">
          Downloading file from the Internet...
        </p>
        <div style="display: flex; gap: 8px; align-items: center; margin-bottom: 12px; font-size: 24px;">
          <span>&#128196;</span>
          <span style="font-size: 12px;">&#10132;&#10132;&#10132;</span>
          <span>&#128187;</span>
        </div>

        <div class="progress-track" style="margin-bottom: 8px;">
          <div class="progress-fill" style="width: 68%;"></div>
        </div>

        <div style="display: grid; grid-template-columns: auto 1fr; gap: 2px 12px; font-size: 11px; margin-bottom: 12px;">
          <span>Saving:</span>
          <span class="mono-text">setup.exe from ftp.microsoft.com</span>
          <span>Estimated time:</span>
          <span>47 min 23 sec (28.8 Kbps)</span>
          <span>Downloaded:</span>
          <span>342 KB of 502 KB</span>
        </div>

        <div style="display: flex; justify-content: flex-end; gap: 6px;">
          <button>Cancel</button>
        </div>
      </div>
    </div>

    <!-- ==========================================
         WINDOW 7: FORM / SIGN-UP
    ========================================== -->
    <div class="window window-sm">
      <div class="title-bar">
        <span class="title-bar-text">Internet Connection Wizard</span>
        <div class="title-bar-controls">
          <button>X</button>
        </div>
      </div>
      <div class="window-body">
        <p style="font-size: 12px; margin-bottom: 12px;">
          Enter your information to set up your Internet connection.
        </p>

        <fieldset style="margin-bottom: 8px;">
          <legend>Account Information</legend>
          <div style="display: grid; grid-template-columns: 80px 1fr; gap: 6px 8px; align-items: center;">
            <label style="font-size: 12px; text-align: right;">Name:</label>
            <input type="text" value="John Smith" style="width: 100%;">
            <label style="font-size: 12px; text-align: right;">Email:</label>
            <input type="email" value="john@geocities.com" style="width: 100%;">
            <label style="font-size: 12px; text-align: right;">Password:</label>
            <input type="password" value="password" style="width: 100%;">
          </div>
        </fieldset>

        <fieldset>
          <legend>Connection Type</legend>
          <div style="display: flex; flex-direction: column; gap: 4px; font-size: 12px;">
            <label><input type="radio" name="conn" checked> 28.8 Kbps Modem</label>
            <label><input type="radio" name="conn"> 56 Kbps Modem</label>
            <label><input type="radio" name="conn"> ISDN</label>
            <label><input type="radio" name="conn" disabled> Cable Modem</label>
          </div>
        </fieldset>

        <hr>

        <div style="display: flex; justify-content: flex-end; gap: 6px;">
          <button>&lt; Back</button>
          <button class="default-btn">Next &gt;</button>
          <button>Cancel</button>
        </div>
      </div>
    </div>

  </div>

  <!-- ==========================================
       TASKBAR
  ========================================== -->
  <div class="taskbar">
    <button class="start-btn raised">
      <span class="start-logo"></span>
      Start
    </button>

    <div class="taskbar-windows">
      <button class="taskbar-window-btn active-window">&#128187; Welcome to Windows 98</button>
      <button class="taskbar-window-btn raised">&#128193; C:\My Documents</button>
      <button class="taskbar-window-btn raised">&#128196; Untitled - Notepad</button>
    </div>

    <div class="systray">
      <span>&#128264;</span>
      <span>3:14 PM</span>
    </div>
  </div>

</body>
</html>
```
