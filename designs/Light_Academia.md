# Light Academia -- Design Reference

Light Academia is a warm, optimistic aesthetic rooted in the romantic pursuit of knowledge, classical art, and literary culture. It is the sunlit counterpart to Dark Academia, replacing moody shadows and gothic undertones with honey-gold light, cream-colored pages, and the quiet joy of a morning spent reading poetry in a sun-drenched library. The visual language draws from Neoclassical and Beaux-Arts architecture, Renaissance painting, vintage bookshops, and the soft patina of aged paper and linen. Where Dark Academia dwells in candlelit intensity, Light Academia celebrates the warmth of golden hour streaming through tall arched windows, the texture of hand-stitched journals, and the gentle abundance of botanical illustrations and pressed flowers. Its palette centers on ivory, warm sand, honey, dusty rose, and muted sage -- tones that evoke sun-bleached marble, chamomile tea, and well-loved paperbacks. In web design, the aesthetic translates to refined serif typography, generous whitespace, soft textures, classical ornament used sparingly, and an overall atmosphere of unhurried intellectual warmth that invites lingering and contemplation.

---

## Visual Characteristics

### Core Design Traits

- **Warm, sunlit color foundation** -- creams, ivories, honey golds, and soft tans form the base, evoking the warmth of natural light on aged paper and limestone
- **Classical typographic hierarchy** -- elegant serif typefaces for headings paired with clean, readable body text create a scholarly yet approachable tone
- **Textured backgrounds and surfaces** -- subtle paper grain, linen weave, parchment, and watercolor wash textures add tactile warmth without visual noise
- **Generous whitespace and breathing room** -- layouts favor openness and calm, reflecting the unhurried pace of reading and reflection
- **Botanical and literary imagery** -- pressed flowers, vintage illustrations, open books, handwritten marginalia, and classical artwork serve as decorative motifs
- **Soft, diffused shadows** -- light drop shadows and gentle elevation mimic the softness of natural daylight rather than harsh artificial contrast
- **Classical ornamental details** -- thin rules, delicate borders, small flourishes, and drop caps reference historical book design and typographic tradition
- **Muted, desaturated accent colors** -- dusty rose, sage green, lavender, and terracotta appear as accents, always softened and never garish
- **Natural material references** -- linen, cotton, marble, aged wood, brass, and dried botanicals inform color and texture choices
- **Rounded, approachable forms** -- soft corners, gentle curves, and organic shapes replace hard geometric edges

### Design Principles

- Lead with warmth -- every design decision should contribute to an atmosphere of welcoming, golden-hour comfort
- Treat typography as the primary design element; the beauty of well-set text is central to the scholarly aesthetic
- Use texture to add depth, but keep it subtle enough that it never competes with content
- Embrace asymmetry and organic layout over rigid mechanical grids -- think curated bookshelf, not spreadsheet
- Honor the tradition of book design: meaningful margins, considered leading, and hierarchy through scale rather than weight alone
- Let natural light be a design principle -- use luminous backgrounds, warm gradients, and light-to-dark progressions that mimic sunlight
- Apply ornamentation with restraint; a single well-placed flourish is more powerful than decoration everywhere
- Prefer photography and illustration with soft, warm toning -- golden hour, overexposed highlights, and gentle bokeh
- Create quiet moments of delight through hover animations, subtle transitions, and thoughtful micro-interactions
- Maintain accessibility by ensuring warm tones still meet contrast requirements for body text and interactive elements

---

## Color Palette

| Color Name | Hex | Role / Usage |
|---|---|---|
| **Parchment Cream** | `#FAF6F0` | Primary background, page canvas |
| **Warm Ivory** | `#F5EDE3` | Secondary background, card surfaces |
| **Antique Linen** | `#EBE1D4` | Tertiary surface, sidebar backgrounds |
| **Honey Gold** | `#D4A853` | Primary accent, links, call-to-action highlights |
| **Burnished Brass** | `#B8923A` | Active states, strong accent, button backgrounds |
| **Dusty Rose** | `#C9A09A` | Secondary accent, decorative elements, tags |
| **Sage Mist** | `#A8B5A0` | Tertiary accent, success states, botanical motifs |
| **Faded Lavender** | `#B8A9C9` | Subtle accent, hover tints, decorative borders |
| **Terracotta Blush** | `#C07C5A` | Warm emphasis, notification badges, highlights |
| **Aged Walnut** | `#5C4033` | Primary text, headings, strong foreground |
| **Sepia Ink** | `#3E2C1C` | Display text, darkest foreground, high-contrast elements |
| **Warm Taupe** | `#8C7B6B` | Secondary text, captions, metadata |
| **Sandstone** | `#D2C4B0` | Borders, dividers, subtle UI lines |
| **Morning Fog** | `#E8E2DA` | Disabled states, placeholder backgrounds |
| **Marble White** | `#FFFFFF` | Maximum light, overlays, modal backgrounds |
| **Deep Mahogany** | `#2E1A0E` | Footer backgrounds, inverse surface |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --la-bg-primary: #FAF6F0;
  --la-bg-secondary: #F5EDE3;
  --la-bg-tertiary: #EBE1D4;
  --la-bg-inverse: #2E1A0E;
  --la-bg-white: #FFFFFF;

  /* Text */
  --la-text-primary: #3E2C1C;
  --la-text-secondary: #5C4033;
  --la-text-muted: #8C7B6B;
  --la-text-on-accent: #FAF6F0;
  --la-text-on-inverse: #F5EDE3;

  /* Accents */
  --la-accent-gold: #D4A853;
  --la-accent-gold-dark: #B8923A;
  --la-accent-rose: #C9A09A;
  --la-accent-sage: #A8B5A0;
  --la-accent-lavender: #B8A9C9;
  --la-accent-terracotta: #C07C5A;

  /* UI Elements */
  --la-border: #D2C4B0;
  --la-border-light: #EBE1D4;
  --la-divider: #E8E2DA;
  --la-shadow-color: rgba(92, 64, 51, 0.08);
  --la-shadow-strong: rgba(92, 64, 51, 0.15);

  /* Gradients */
  --la-gradient-warmth: linear-gradient(135deg, #FAF6F0 0%, #F5EDE3 50%, #EBE1D4 100%);
  --la-gradient-golden: linear-gradient(135deg, #D4A853 0%, #B8923A 100%);
  --la-gradient-sunrise: linear-gradient(180deg, #FAF6F0 0%, #F5EDE3 60%, #EBE1D4 100%);

  /* Typography */
  --la-font-display: 'Playfair Display', Georgia, 'Times New Roman', serif;
  --la-font-heading: 'Cormorant Garamond', Garamond, 'Times New Roman', serif;
  --la-font-body: 'Libre Baskerville', Baskerville, Georgia, serif;
  --la-font-sans: 'Lato', 'Gill Sans', Calibri, sans-serif;
  --la-font-accent: 'EB Garamond', Garamond, serif;

  /* Spacing */
  --la-space-xs: 0.25rem;
  --la-space-sm: 0.5rem;
  --la-space-md: 1rem;
  --la-space-lg: 2rem;
  --la-space-xl: 4rem;
  --la-space-2xl: 6rem;

  /* Border Radius */
  --la-radius-sm: 4px;
  --la-radius-md: 8px;
  --la-radius-lg: 16px;
  --la-radius-pill: 9999px;

  /* Transitions */
  --la-transition-gentle: 0.3s ease;
  --la-transition-slow: 0.5s ease;
}
```

---

## Typography

### Typeface Characteristics

Light Academia typography channels the elegance of classical book design. Serif typefaces dominate, drawing from the tradition of Aldine, Garamond, and Baskerville -- typefaces born in the golden age of printing. Headings favor high-contrast serifs with elegant swash details and refined stroke modulation. Body text uses sturdy, readable serifs designed for sustained reading, with generous line-height and comfortable measure. Sans-serif type is used sparingly -- for UI labels, navigation, or captions -- and should be warm and humanist rather than cold and geometric. Display type may incorporate italic or small-cap variants to echo the typographic conventions of title pages and chapter openings in fine editions. Letter-spacing is generally tight for headings and normal for body, with careful attention to optical sizing.

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|---|---|---|
| **Playfair Display** | High-contrast transitional serif with elegant hairlines | Display headings, hero titles, pull quotes |
| **Cormorant Garamond** | Refined Garamond revival with graceful italics | Subheadings, section titles, literary passages |
| **Libre Baskerville** | Sturdy and readable Baskerville optimized for screen | Body text, article content, long-form reading |
| **EB Garamond** | Faithful Claude Garamond revival with old-style figures | Block quotes, accent text, scholarly citations |
| **Lato** | Warm humanist sans-serif with semi-rounded details | Navigation, UI labels, captions, metadata |
| **Spectral** | Serif designed specifically for screen reading | Alternative body text, responsive-friendly content |
| **Crimson Pro** | Elegant book-weight serif with extensive weight range | Versatile body or heading use across weight spectrum |

### Font Pairing Suggestions

| Heading Font | Body Font | Mood |
|---|---|---|
| Playfair Display | Libre Baskerville | Grand and scholarly, classical library |
| Cormorant Garamond | Lato | Refined elegance with modern readability |
| Playfair Display | Lato | Dramatic contrast, editorial magazine feel |
| Crimson Pro | Spectral | Quiet sophistication, all-serif harmony |
| Cormorant Garamond | Libre Baskerville | Deep literary tradition, old-world warmth |

### Typography CSS Example

```css
/* Light Academia Typography Scale */

/* Display -- Title pages, hero sections */
.la-display {
  font-family: var(--la-font-display);
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 700;
  line-height: 1.1;
  letter-spacing: -0.02em;
  color: var(--la-text-primary);
}

/* Heading 1 -- Page titles */
.la-h1 {
  font-family: var(--la-font-heading);
  font-size: clamp(2rem, 4vw, 3rem);
  font-weight: 600;
  line-height: 1.2;
  letter-spacing: -0.01em;
  color: var(--la-text-primary);
}

/* Heading 2 -- Section titles */
.la-h2 {
  font-family: var(--la-font-heading);
  font-size: clamp(1.5rem, 3vw, 2.25rem);
  font-weight: 500;
  line-height: 1.25;
  color: var(--la-text-secondary);
}

/* Heading 3 -- Subsection titles */
.la-h3 {
  font-family: var(--la-font-heading);
  font-size: clamp(1.25rem, 2vw, 1.5rem);
  font-weight: 600;
  line-height: 1.3;
  color: var(--la-text-secondary);
}

/* Body -- Primary reading text */
.la-body {
  font-family: var(--la-font-body);
  font-size: 1.0625rem;
  font-weight: 400;
  line-height: 1.75;
  letter-spacing: 0.01em;
  color: var(--la-text-primary);
}

/* Small / Caption */
.la-caption {
  font-family: var(--la-font-sans);
  font-size: 0.8125rem;
  font-weight: 400;
  line-height: 1.5;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  color: var(--la-text-muted);
}

/* Block Quote */
.la-blockquote {
  font-family: var(--la-font-accent);
  font-size: 1.25rem;
  font-style: italic;
  line-height: 1.7;
  color: var(--la-text-secondary);
  border-left: 3px solid var(--la-accent-gold);
  padding-left: var(--la-space-lg);
  margin: var(--la-space-xl) 0;
}

/* Drop Cap */
.la-dropcap::first-letter {
  font-family: var(--la-font-display);
  font-size: 3.5em;
  float: left;
  line-height: 0.8;
  margin-right: 0.08em;
  margin-top: 0.05em;
  color: var(--la-accent-gold-dark);
}
```

---

## Layout Principles

### Grid and Structure

- Use a soft, content-centered layout with a maximum width of 720--900px for body text to maintain a comfortable reading measure of 60--75 characters per line
- Employ a 12-column grid for full-page layouts, but allow content to break free of rigid columns for an organic, editorial feel
- Generous margins on both sides (at least 10--15% of viewport width on desktop) frame the content like the margins of a well-designed book
- Vertical rhythm should follow the body line-height as a baseline unit, creating harmonious spacing between elements
- Use golden ratio proportions (1:1.618) for key dimensional relationships -- sidebar widths, image aspect ratios, section padding
- Allow for asymmetric layouts where a narrower column holds marginalia, pull quotes, or decorative elements alongside the main content

### Section Organization

- Open with a quiet, spacious hero -- a warm background with elegant typography and perhaps a single classical image
- Use horizontal rules or thin ornamental dividers (not heavy bars) to separate major sections
- Alternate between full-width and narrow-measure sections to create visual rhythm and prevent monotony
- Pull quotes and featured passages should break out of the text column, drawing the eye like annotations in a margin
- Image sections should use generous padding and soft rounded corners, presented as if mounted on a gallery wall or pressed into a journal
- Footer should feel like the endpapers of a book -- a quiet, slightly darker surface with understated typography
- Navigation should be minimal and refined, positioned to be accessible without dominating the scholarly atmosphere

### Responsive Approach

- On mobile, collapse to a single column with increased vertical spacing to preserve the sense of breathing room
- Scale typography fluidly using clamp() to maintain readability and proportional hierarchy across screen sizes
- On smaller screens, reduce margin width but increase padding within content blocks to keep text comfortably inset
- Images should scale gracefully, shifting from side-by-side arrangements on desktop to stacked layouts on mobile
- Navigation transforms from a horizontal serif-styled menu into a simple, warm-toned hamburger menu on mobile
- Maintain the warm textured background on all breakpoints; do not flatten to pure white on mobile
- Touch targets should be generously sized (minimum 44px) and styled with soft, visible boundaries

---

## CSS / Design Techniques

### Card Component

```css
.la-card {
  background: var(--la-bg-white);
  border: 1px solid var(--la-border);
  border-radius: var(--la-radius-md);
  padding: var(--la-space-lg);
  box-shadow:
    0 1px 3px var(--la-shadow-color),
    0 4px 12px var(--la-shadow-color);
  transition: box-shadow var(--la-transition-gentle),
              transform var(--la-transition-gentle);
}

.la-card:hover {
  box-shadow:
    0 2px 8px var(--la-shadow-strong),
    0 8px 24px var(--la-shadow-color);
  transform: translateY(-2px);
}

.la-card__image {
  width: 100%;
  border-radius: var(--la-radius-sm);
  margin-bottom: var(--la-space-md);
  object-fit: cover;
  aspect-ratio: 4 / 3;
}

.la-card__category {
  font-family: var(--la-font-sans);
  font-size: 0.75rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--la-accent-gold-dark);
  margin-bottom: var(--la-space-sm);
}

.la-card__title {
  font-family: var(--la-font-heading);
  font-size: 1.375rem;
  font-weight: 600;
  line-height: 1.3;
  color: var(--la-text-primary);
  margin-bottom: var(--la-space-sm);
}

.la-card__excerpt {
  font-family: var(--la-font-body);
  font-size: 0.9375rem;
  line-height: 1.7;
  color: var(--la-text-muted);
}
```

### Button Component

```css
/* Primary button -- warm gold */
.la-button {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  font-family: var(--la-font-sans);
  font-size: 0.875rem;
  font-weight: 600;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--la-text-on-accent);
  background: var(--la-accent-gold-dark);
  border: none;
  border-radius: var(--la-radius-sm);
  padding: 0.75rem 1.75rem;
  cursor: pointer;
  transition: background var(--la-transition-gentle),
              box-shadow var(--la-transition-gentle);
}

.la-button:hover {
  background: var(--la-accent-gold);
  box-shadow: 0 4px 12px rgba(184, 146, 58, 0.3);
}

.la-button:active {
  background: #9F7E30;
  transform: translateY(1px);
}

/* Secondary button -- outlined */
.la-button--secondary {
  background: transparent;
  color: var(--la-accent-gold-dark);
  border: 1.5px solid var(--la-accent-gold-dark);
}

.la-button--secondary:hover {
  background: rgba(212, 168, 83, 0.08);
  box-shadow: none;
}

/* Ghost button -- text only */
.la-button--ghost {
  background: transparent;
  color: var(--la-text-secondary);
  border: none;
  padding: 0.5rem 0.75rem;
  text-transform: none;
  letter-spacing: normal;
  font-family: var(--la-font-body);
  font-style: italic;
}

.la-button--ghost:hover {
  color: var(--la-accent-gold-dark);
  background: transparent;
  box-shadow: none;
}
```

### Navigation Bar

```css
.la-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: var(--la-space-md) var(--la-space-xl);
  background: var(--la-bg-primary);
  border-bottom: 1px solid var(--la-border-light);
}

.la-nav__logo {
  font-family: var(--la-font-display);
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--la-text-primary);
  text-decoration: none;
  letter-spacing: -0.02em;
}

.la-nav__links {
  display: flex;
  gap: var(--la-space-lg);
  list-style: none;
  margin: 0;
  padding: 0;
}

.la-nav__link {
  font-family: var(--la-font-sans);
  font-size: 0.8125rem;
  font-weight: 400;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--la-text-muted);
  text-decoration: none;
  padding: var(--la-space-xs) 0;
  border-bottom: 1.5px solid transparent;
  transition: color var(--la-transition-gentle),
              border-color var(--la-transition-gentle);
}

.la-nav__link:hover,
.la-nav__link--active {
  color: var(--la-text-primary);
  border-bottom-color: var(--la-accent-gold);
}
```

### Hero Section

```css
.la-hero {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  min-height: 80vh;
  padding: var(--la-space-2xl) var(--la-space-xl);
  background: var(--la-gradient-sunrise);
  overflow: hidden;
}

.la-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23d2c4b0' fill-opacity='0.15'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
  opacity: 0.5;
  pointer-events: none;
}

.la-hero__overline {
  font-family: var(--la-font-sans);
  font-size: 0.75rem;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--la-accent-gold-dark);
  margin-bottom: var(--la-space-md);
}

.la-hero__title {
  font-family: var(--la-font-display);
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  line-height: 1.08;
  color: var(--la-text-primary);
  max-width: 14ch;
  margin-bottom: var(--la-space-lg);
}

.la-hero__subtitle {
  font-family: var(--la-font-accent);
  font-size: clamp(1.125rem, 2vw, 1.375rem);
  font-style: italic;
  line-height: 1.6;
  color: var(--la-text-muted);
  max-width: 42ch;
  margin-bottom: var(--la-space-xl);
}

.la-hero__ornament {
  width: 60px;
  height: 1px;
  background: var(--la-accent-gold);
  margin: var(--la-space-lg) auto;
  position: relative;
}

.la-hero__ornament::before {
  content: '\2726';
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  font-size: 0.875rem;
  color: var(--la-accent-gold);
  background: var(--la-bg-primary);
  padding: 0 0.5rem;
}
```

### Blockquote / Pull Quote

```css
.la-pullquote {
  position: relative;
  max-width: 640px;
  margin: var(--la-space-2xl) auto;
  padding: var(--la-space-xl) var(--la-space-xl) var(--la-space-xl) var(--la-space-2xl);
  font-family: var(--la-font-accent);
  font-size: 1.375rem;
  font-style: italic;
  line-height: 1.7;
  color: var(--la-text-secondary);
  border-left: 3px solid var(--la-accent-gold);
}

.la-pullquote::before {
  content: '\201C';
  position: absolute;
  top: -0.2em;
  left: 0.5rem;
  font-family: var(--la-font-display);
  font-size: 4rem;
  font-style: normal;
  color: var(--la-accent-gold);
  line-height: 1;
  opacity: 0.4;
}

.la-pullquote__attribution {
  display: block;
  margin-top: var(--la-space-md);
  font-family: var(--la-font-sans);
  font-size: 0.8125rem;
  font-style: normal;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--la-text-muted);
}

.la-pullquote__attribution::before {
  content: '\2014\00a0';
}
```

### Ornamental Divider

```css
.la-divider {
  display: flex;
  align-items: center;
  gap: var(--la-space-md);
  margin: var(--la-space-xl) 0;
  color: var(--la-border);
}

.la-divider::before,
.la-divider::after {
  content: '';
  flex: 1;
  height: 1px;
  background: var(--la-border);
}

.la-divider__ornament {
  font-size: 1rem;
  color: var(--la-accent-gold);
  opacity: 0.6;
  line-height: 1;
}
```

### Form Input

```css
.la-input-group {
  display: flex;
  flex-direction: column;
  gap: var(--la-space-xs);
  margin-bottom: var(--la-space-lg);
}

.la-input-group__label {
  font-family: var(--la-font-sans);
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--la-text-muted);
}

.la-input {
  font-family: var(--la-font-body);
  font-size: 1rem;
  color: var(--la-text-primary);
  background: var(--la-bg-white);
  border: 1.5px solid var(--la-border);
  border-radius: var(--la-radius-sm);
  padding: 0.75rem 1rem;
  transition: border-color var(--la-transition-gentle),
              box-shadow var(--la-transition-gentle);
}

.la-input::placeholder {
  color: var(--la-border);
  font-style: italic;
}

.la-input:focus {
  outline: none;
  border-color: var(--la-accent-gold);
  box-shadow: 0 0 0 3px rgba(212, 168, 83, 0.15);
}
```

### Tag / Badge

```css
.la-tag {
  display: inline-block;
  font-family: var(--la-font-sans);
  font-size: 0.6875rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--la-accent-gold-dark);
  background: rgba(212, 168, 83, 0.1);
  border: 1px solid rgba(212, 168, 83, 0.25);
  border-radius: var(--la-radius-pill);
  padding: 0.3rem 0.75rem;
}

.la-tag--rose {
  color: #9E7571;
  background: rgba(201, 160, 154, 0.12);
  border-color: rgba(201, 160, 154, 0.3);
}

.la-tag--sage {
  color: #6E7F67;
  background: rgba(168, 181, 160, 0.12);
  border-color: rgba(168, 181, 160, 0.3);
}
```

---

## Design Do's and Don'ts

### Do

- Use warm-toned photography with soft lighting, golden highlights, and natural settings (libraries, gardens, cafes)
- Pair high-contrast serif headings with readable serif or humanist sans-serif body text
- Add subtle texture overlays (paper grain, linen) at very low opacity (5--15%) for tactile warmth
- Employ generous line-height (1.6--1.8) for body text to create a relaxed, book-like reading experience
- Use ornamental dividers, drop caps, and thin rules sparingly to honor typographic tradition
- Apply soft, warm-toned shadows using brown-based rgba values rather than pure black
- Include botanical motifs, classical illustration, or vintage engraving-style imagery as decorative accents
- Maintain warm tones even in neutral grays by mixing in subtle brown or gold undertones
- Use italic serif type for captions, attributions, and secondary information to add personality
- Provide ample padding within cards and content blocks -- content should never feel cramped

### Don't

- Use cold, blue-tinted grays or stark pure white (#FFFFFF) as the primary background -- always warm it
- Apply heavy, dark drop shadows that create harsh contrast incompatible with the soft aesthetic
- Choose geometric sans-serif typefaces (Futura, Montserrat, Bebas) as primary display fonts -- they feel too modernist
- Saturate accent colors to full vibrancy -- Light Academia colors are always muted, dusty, and desaturated
- Use neon, fluorescent, or high-chroma colors anywhere in the design
- Clutter the layout with too many decorative elements -- restraint is essential to the scholarly atmosphere
- Apply aggressive animations, bounce effects, or flashy transitions that break the contemplative mood
- Use stock photography with harsh flash, cool color grading, or overly corporate subjects
- Neglect contrast ratios -- warm palettes can easily produce text that fails accessibility checks
- Mix too many serif typefaces in a single design; two is elegant, four is chaotic

---

## Related Aesthetics

| Aesthetic | Relationship |
|---|---|
| **Dark Academia** | Direct sibling -- shares the scholarly, literary foundation but replaces warmth with gothic moodiness, candlelight, and autumnal darkness |
| **Cottagecore** | Overlapping warmth and botanical motifs, but Cottagecore leans rural, handmade, and pastoral rather than intellectual and classical |
| **Old Money** | Shares the refined, preppy palette and classical taste, but Old Money emphasizes wealth signaling and exclusivity over intellectual pursuit |
| **Romantic Academia** | A softer, more emotionally expressive variant that amplifies the poetry, flowers, and sentimentality within Light Academia |
| **Grandmillennial** | Both embrace tradition, pattern, and warmth; Grandmillennial adds chintz, needlepoint, and maximalist layering that Light Academia avoids |
| **Wes Anderson** | Shares the warm, curated color palette and whimsical attention to detail, but Wes Anderson is more playful, symmetric, and self-consciously stylized |
| **Japandi** | Both value natural materials and calm, but Japandi strips away ornamentation and warmth in favor of minimalist restraint and cool neutrals |
| **Art Nouveau** | Shares organic forms, classical beauty, and fine craftsmanship, but Art Nouveau features bolder curves, richer color, and more elaborate ornamentation |
| **Editorial / Magazine** | Light Academia borrows editorial layout conventions -- pull quotes, asymmetric grids, strong typography -- but softens the bold, high-contrast approach |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Gilded Page -- A Light Academia Journal</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&family=EB+Garamond:ital,wght@0,400;0,500;1,400&family=Lato:wght@300;400;700&family=Playfair+Display:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
  <style>
    /* ===========================
       CSS Custom Properties
       =========================== */
    :root {
      --la-bg-primary: #FAF6F0;
      --la-bg-secondary: #F5EDE3;
      --la-bg-tertiary: #EBE1D4;
      --la-bg-inverse: #2E1A0E;
      --la-bg-white: #FFFFFF;

      --la-text-primary: #3E2C1C;
      --la-text-secondary: #5C4033;
      --la-text-muted: #8C7B6B;
      --la-text-on-accent: #FAF6F0;
      --la-text-on-inverse: #F5EDE3;

      --la-accent-gold: #D4A853;
      --la-accent-gold-dark: #B8923A;
      --la-accent-rose: #C9A09A;
      --la-accent-sage: #A8B5A0;
      --la-accent-lavender: #B8A9C9;
      --la-accent-terracotta: #C07C5A;

      --la-border: #D2C4B0;
      --la-border-light: #EBE1D4;
      --la-divider: #E8E2DA;
      --la-shadow-color: rgba(92, 64, 51, 0.08);
      --la-shadow-strong: rgba(92, 64, 51, 0.15);

      --la-font-display: 'Playfair Display', Georgia, serif;
      --la-font-heading: 'Cormorant Garamond', Garamond, serif;
      --la-font-body: 'EB Garamond', Georgia, serif;
      --la-font-sans: 'Lato', 'Gill Sans', sans-serif;
      --la-font-accent: 'EB Garamond', Garamond, serif;

      --la-radius-sm: 4px;
      --la-radius-md: 8px;
      --la-radius-lg: 16px;
      --la-radius-pill: 9999px;
    }

    /* ===========================
       Reset & Base
       =========================== */
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    html {
      scroll-behavior: smooth;
      font-size: 16px;
    }

    body {
      font-family: var(--la-font-body);
      font-size: 1.0625rem;
      line-height: 1.75;
      color: var(--la-text-primary);
      background-color: var(--la-bg-primary);
      -webkit-font-smoothing: antialiased;
    }

    img { max-width: 100%; height: auto; display: block; }
    a { color: var(--la-accent-gold-dark); text-decoration: none; transition: color 0.3s ease; }
    a:hover { color: var(--la-accent-gold); }

    /* ===========================
       Navigation
       =========================== */
    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1.25rem 4rem;
      background: var(--la-bg-primary);
      border-bottom: 1px solid var(--la-border-light);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav__logo {
      font-family: var(--la-font-display);
      font-size: 1.375rem;
      font-weight: 700;
      color: var(--la-text-primary);
      text-decoration: none;
      letter-spacing: -0.02em;
    }

    .nav__links {
      display: flex;
      gap: 2rem;
      list-style: none;
    }

    .nav__links a {
      font-family: var(--la-font-sans);
      font-size: 0.75rem;
      font-weight: 400;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--la-text-muted);
      text-decoration: none;
      padding-bottom: 2px;
      border-bottom: 1.5px solid transparent;
      transition: color 0.3s ease, border-color 0.3s ease;
    }

    .nav__links a:hover,
    .nav__links a.active {
      color: var(--la-text-primary);
      border-bottom-color: var(--la-accent-gold);
    }

    /* ===========================
       Hero Section
       =========================== */
    .hero {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 85vh;
      padding: 6rem 2rem;
      background: linear-gradient(180deg, var(--la-bg-primary) 0%, var(--la-bg-secondary) 70%, var(--la-bg-tertiary) 100%);
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg width='80' height='80' viewBox='0 0 80 80' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='%23d2c4b0' fill-opacity='0.1'%3E%3Cpath d='M40 0L40 80M0 40L80 40' stroke='%23d2c4b0' stroke-opacity='0.07' stroke-width='0.5' fill='none'/%3E%3C/g%3E%3C/svg%3E");
      pointer-events: none;
    }

    .hero__overline {
      font-family: var(--la-font-sans);
      font-size: 0.6875rem;
      letter-spacing: 0.25em;
      text-transform: uppercase;
      color: var(--la-accent-gold-dark);
      margin-bottom: 1.5rem;
      position: relative;
    }

    .hero__title {
      font-family: var(--la-font-display);
      font-size: clamp(2.75rem, 6vw, 5rem);
      font-weight: 700;
      line-height: 1.08;
      color: var(--la-text-primary);
      max-width: 16ch;
      margin-bottom: 2rem;
      position: relative;
    }

    .hero__ornament {
      width: 80px;
      height: 1px;
      background: var(--la-accent-gold);
      margin: 0 auto 2rem;
      position: relative;
    }

    .hero__ornament::before {
      content: '\2726';
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      font-size: 0.75rem;
      color: var(--la-accent-gold);
      background: var(--la-bg-secondary);
      padding: 0 0.75rem;
    }

    .hero__subtitle {
      font-family: var(--la-font-accent);
      font-size: clamp(1.125rem, 2vw, 1.375rem);
      font-style: italic;
      line-height: 1.65;
      color: var(--la-text-muted);
      max-width: 44ch;
      margin-bottom: 2.5rem;
      position: relative;
    }

    /* ===========================
       Buttons
       =========================== */
    .btn {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      font-family: var(--la-font-sans);
      font-size: 0.8125rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      text-decoration: none;
      border-radius: var(--la-radius-sm);
      padding: 0.875rem 2rem;
      cursor: pointer;
      transition: all 0.3s ease;
      border: 1.5px solid transparent;
    }

    .btn--primary {
      color: var(--la-text-on-accent);
      background: var(--la-accent-gold-dark);
      border-color: var(--la-accent-gold-dark);
    }

    .btn--primary:hover {
      background: var(--la-accent-gold);
      border-color: var(--la-accent-gold);
      box-shadow: 0 4px 16px rgba(184, 146, 58, 0.3);
      color: var(--la-text-on-accent);
    }

    .btn--secondary {
      color: var(--la-accent-gold-dark);
      background: transparent;
      border-color: var(--la-accent-gold-dark);
    }

    .btn--secondary:hover {
      background: rgba(212, 168, 83, 0.08);
      color: var(--la-accent-gold-dark);
    }

    /* ===========================
       Section Utilities
       =========================== */
    .section {
      padding: 5rem 2rem;
    }

    .section--warm {
      background: var(--la-bg-secondary);
    }

    .section__container {
      max-width: 1100px;
      margin: 0 auto;
    }

    .section__header {
      text-align: center;
      margin-bottom: 3rem;
    }

    .section__overline {
      font-family: var(--la-font-sans);
      font-size: 0.6875rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--la-accent-gold-dark);
      margin-bottom: 0.75rem;
    }

    .section__title {
      font-family: var(--la-font-heading);
      font-size: clamp(1.75rem, 3.5vw, 2.75rem);
      font-weight: 500;
      line-height: 1.2;
      color: var(--la-text-primary);
      margin-bottom: 0.75rem;
    }

    .section__desc {
      font-family: var(--la-font-accent);
      font-size: 1.0625rem;
      font-style: italic;
      color: var(--la-text-muted);
      max-width: 48ch;
      margin: 0 auto;
      line-height: 1.7;
    }

    /* ===========================
       Ornamental Divider
       =========================== */
    .divider {
      display: flex;
      align-items: center;
      gap: 1rem;
      max-width: 300px;
      margin: 0 auto 3rem;
    }

    .divider::before,
    .divider::after {
      content: '';
      flex: 1;
      height: 1px;
      background: var(--la-border);
    }

    .divider__icon {
      font-size: 0.875rem;
      color: var(--la-accent-gold);
      opacity: 0.6;
    }

    /* ===========================
       Cards Grid
       =========================== */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 2rem;
    }

    .card {
      background: var(--la-bg-white);
      border: 1px solid var(--la-border-light);
      border-radius: var(--la-radius-md);
      overflow: hidden;
      box-shadow: 0 1px 3px var(--la-shadow-color), 0 4px 12px var(--la-shadow-color);
      transition: box-shadow 0.3s ease, transform 0.3s ease;
    }

    .card:hover {
      box-shadow: 0 2px 8px var(--la-shadow-strong), 0 8px 28px var(--la-shadow-color);
      transform: translateY(-3px);
    }

    .card__img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      border-bottom: 1px solid var(--la-border-light);
    }

    .card__body {
      padding: 1.75rem;
    }

    .card__tag {
      display: inline-block;
      font-family: var(--la-font-sans);
      font-size: 0.625rem;
      font-weight: 700;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--la-accent-gold-dark);
      background: rgba(212, 168, 83, 0.1);
      border: 1px solid rgba(212, 168, 83, 0.2);
      border-radius: var(--la-radius-pill);
      padding: 0.25rem 0.625rem;
      margin-bottom: 1rem;
    }

    .card__tag--rose {
      color: #9E7571;
      background: rgba(201, 160, 154, 0.12);
      border-color: rgba(201, 160, 154, 0.25);
    }

    .card__tag--sage {
      color: #6E7F67;
      background: rgba(168, 181, 160, 0.12);
      border-color: rgba(168, 181, 160, 0.25);
    }

    .card__title {
      font-family: var(--la-font-heading);
      font-size: 1.375rem;
      font-weight: 600;
      line-height: 1.3;
      color: var(--la-text-primary);
      margin-bottom: 0.5rem;
    }

    .card__excerpt {
      font-family: var(--la-font-body);
      font-size: 0.9375rem;
      line-height: 1.7;
      color: var(--la-text-muted);
      margin-bottom: 1.25rem;
    }

    .card__link {
      font-family: var(--la-font-sans);
      font-size: 0.75rem;
      font-weight: 700;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      color: var(--la-accent-gold-dark);
    }

    .card__link:hover {
      color: var(--la-accent-gold);
    }

    /* ===========================
       Pull Quote
       =========================== */
    .pullquote {
      max-width: 700px;
      margin: 0 auto;
      padding: 3rem 3rem 3rem 4rem;
      position: relative;
      text-align: center;
    }

    .pullquote::before {
      content: '\201C';
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
      font-family: var(--la-font-display);
      font-size: 6rem;
      color: var(--la-accent-gold);
      opacity: 0.2;
      line-height: 1;
    }

    .pullquote__text {
      font-family: var(--la-font-accent);
      font-size: clamp(1.25rem, 2.5vw, 1.625rem);
      font-style: italic;
      line-height: 1.7;
      color: var(--la-text-secondary);
      position: relative;
    }

    .pullquote__attribution {
      display: block;
      margin-top: 1.25rem;
      font-family: var(--la-font-sans);
      font-size: 0.75rem;
      font-style: normal;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--la-text-muted);
    }

    /* ===========================
       Article Prose
       =========================== */
    .prose {
      max-width: 680px;
      margin: 0 auto;
    }

    .prose p {
      margin-bottom: 1.5rem;
    }

    .prose p:first-of-type::first-letter {
      font-family: var(--la-font-display);
      font-size: 3.5em;
      float: left;
      line-height: 0.8;
      margin-right: 0.06em;
      margin-top: 0.07em;
      color: var(--la-accent-gold-dark);
    }

    .prose h2 {
      font-family: var(--la-font-heading);
      font-size: 1.75rem;
      font-weight: 500;
      color: var(--la-text-primary);
      margin: 3rem 0 1rem;
    }

    /* ===========================
       Newsletter Form
       =========================== */
    .newsletter {
      max-width: 520px;
      margin: 0 auto;
      text-align: center;
    }

    .newsletter__form {
      display: flex;
      gap: 0.75rem;
      margin-top: 1.5rem;
    }

    .newsletter__input {
      flex: 1;
      font-family: var(--la-font-body);
      font-size: 0.9375rem;
      color: var(--la-text-primary);
      background: var(--la-bg-white);
      border: 1.5px solid var(--la-border);
      border-radius: var(--la-radius-sm);
      padding: 0.75rem 1rem;
      transition: border-color 0.3s ease, box-shadow 0.3s ease;
    }

    .newsletter__input::placeholder {
      color: var(--la-border);
      font-style: italic;
    }

    .newsletter__input:focus {
      outline: none;
      border-color: var(--la-accent-gold);
      box-shadow: 0 0 0 3px rgba(212, 168, 83, 0.15);
    }

    /* ===========================
       Footer
       =========================== */
    .footer {
      background: var(--la-bg-inverse);
      color: var(--la-text-on-inverse);
      padding: 4rem 2rem 2rem;
      text-align: center;
    }

    .footer__logo {
      font-family: var(--la-font-display);
      font-size: 1.25rem;
      font-weight: 700;
      color: var(--la-text-on-inverse);
      margin-bottom: 1rem;
    }

    .footer__tagline {
      font-family: var(--la-font-accent);
      font-style: italic;
      font-size: 0.9375rem;
      color: rgba(245, 237, 227, 0.5);
      margin-bottom: 2rem;
    }

    .footer__links {
      display: flex;
      justify-content: center;
      gap: 2rem;
      list-style: none;
      margin-bottom: 2.5rem;
    }

    .footer__links a {
      font-family: var(--la-font-sans);
      font-size: 0.75rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: rgba(245, 237, 227, 0.5);
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .footer__links a:hover {
      color: var(--la-accent-gold);
    }

    .footer__divider {
      width: 60px;
      height: 1px;
      background: rgba(245, 237, 227, 0.15);
      margin: 0 auto 1.5rem;
    }

    .footer__copy {
      font-family: var(--la-font-sans);
      font-size: 0.6875rem;
      letter-spacing: 0.04em;
      color: rgba(245, 237, 227, 0.3);
    }

    /* ===========================
       Responsive
       =========================== */
    @media (max-width: 768px) {
      .nav {
        padding: 1rem 1.5rem;
      }

      .nav__links {
        display: none; /* Would become hamburger menu in production */
      }

      .hero {
        min-height: 70vh;
        padding: 4rem 1.5rem;
      }

      .section {
        padding: 3.5rem 1.5rem;
      }

      .cards {
        grid-template-columns: 1fr;
        gap: 1.5rem;
      }

      .newsletter__form {
        flex-direction: column;
      }

      .footer__links {
        flex-wrap: wrap;
        gap: 1rem 1.5rem;
      }
    }
  </style>
</head>
<body>

  <!-- ===========================
       Navigation
       =========================== -->
  <nav class="nav">
    <a href="#" class="nav__logo">The Gilded Page</a>
    <ul class="nav__links">
      <li><a href="#" class="active">Journal</a></li>
      <li><a href="#">Library</a></li>
      <li><a href="#">Poetry</a></li>
      <li><a href="#">Letters</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <!-- ===========================
       Hero Section
       =========================== -->
  <header class="hero">
    <span class="hero__overline">A journal of quiet wonder</span>
    <h1 class="hero__title">Where Sunlight Meets the Written Word</h1>
    <div class="hero__ornament"></div>
    <p class="hero__subtitle">Reflections on literature, philosophy, and the gentle art of living thoughtfully among books, tea, and afternoon light.</p>
    <div style="display: flex; gap: 1rem; flex-wrap: wrap; justify-content: center;">
      <a href="#latest" class="btn btn--primary">Begin Reading</a>
      <a href="#subscribe" class="btn btn--secondary">Subscribe</a>
    </div>
  </header>

  <!-- ===========================
       Latest Essays
       =========================== -->
  <section id="latest" class="section">
    <div class="section__container">
      <div class="section__header">
        <p class="section__overline">Latest Essays</p>
        <h2 class="section__title">From the Writing Desk</h2>
        <div class="divider"><span class="divider__icon">&#10086;</span></div>
        <p class="section__desc">Meditations on the books we carry, the rooms we inhabit, and the ideas that stay with us long after the page is turned.</p>
      </div>

      <div class="cards">
        <!-- Card 1 -->
        <article class="card">
          <img class="card__img" src="https://images.unsplash.com/photo-1507842217343-583bb7270b66?w=600&h=400&fit=crop" alt="Sunlit library with arched windows and rows of aged books">
          <div class="card__body">
            <span class="card__tag">Literature</span>
            <h3 class="card__title">On the Pleasure of Rereading</h3>
            <p class="card__excerpt">There is a particular kind of solace in returning to a familiar novel. The words have not changed, but we have, and in the distance between those two readings lies a quiet autobiography.</p>
            <a href="#" class="card__link">Continue Reading &rarr;</a>
          </div>
        </article>

        <!-- Card 2 -->
        <article class="card">
          <img class="card__img" src="https://images.unsplash.com/photo-1481627834876-b7833e8f5570?w=600&h=400&fit=crop" alt="Stack of well-loved books beside a window with warm light">
          <div class="card__body">
            <span class="card__tag card__tag--rose">Philosophy</span>
            <h3 class="card__title">The Stoic Morning Ritual</h3>
            <p class="card__excerpt">Marcus Aurelius began each day with an act of philosophical preparation. In our own hurried mornings, there may be wisdom in pausing, even briefly, to set the mind before the world rushes in.</p>
            <a href="#" class="card__link">Continue Reading &rarr;</a>
          </div>
        </article>

        <!-- Card 3 -->
        <article class="card">
          <img class="card__img" src="https://images.unsplash.com/photo-1513475382585-d06e58bcb0e0?w=600&h=400&fit=crop" alt="Botanical illustration of pressed wildflowers on aged paper">
          <div class="card__body">
            <span class="card__tag card__tag--sage">Nature</span>
            <h3 class="card__title">A Herbarium of Small Wonders</h3>
            <p class="card__excerpt">The Victorians understood something we have largely forgotten: that pressing a flower between the pages of a heavy book is a way of pressing time itself into something you can hold.</p>
            <a href="#" class="card__link">Continue Reading &rarr;</a>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- ===========================
       Pull Quote Section
       =========================== -->
  <section class="section section--warm">
    <div class="pullquote">
      <p class="pullquote__text">One must always be careful of books, and what is inside them, for words have the power to change us.</p>
      <span class="pullquote__attribution">Cassandra Clare</span>
    </div>
  </section>

  <!-- ===========================
       Featured Article
       =========================== -->
  <section class="section">
    <div class="section__container">
      <div class="section__header">
        <p class="section__overline">Featured</p>
        <h2 class="section__title">The Architecture of Contemplation</h2>
        <div class="divider"><span class="divider__icon">&#10087;</span></div>
      </div>

      <div class="prose">
        <p>There exists, in the great reading rooms of the world, a particular quality of silence that cannot be manufactured. It is not merely the absence of noise but the presence of concentrated thought, centuries of it, absorbed into limestone walls and vaulted ceilings. The Bodleian, the Sainte-Genevieve, the Long Room at Trinity College -- these spaces were designed not simply to store books but to elevate the act of reading into something approaching the sacred.</p>

        <p>The architects understood that light matters. Not the clinical fluorescence of a modern office, but the warm, angled light that falls through tall windows and shifts across a desk throughout the afternoon, marking the passage of hours in slow golden increments. It is this quality of light -- honeyed, unhurried, almost tangible -- that defines the atmosphere we now call Light Academia.</p>

        <h2>On the Relationship Between Space and Thought</h2>

        <p>Consider how differently the mind behaves in a sun-filled room lined with books compared to, say, a windowless conference room. The presence of accumulated knowledge, the warmth of aged wood, the faint scent of old paper -- these are not mere decorations but active participants in the process of thinking. The room itself becomes a collaborator, gently encouraging the kind of slow, associative thought that produces genuine insight rather than mere productivity.</p>
      </div>
    </div>
  </section>

  <!-- ===========================
       Newsletter
       =========================== -->
  <section id="subscribe" class="section section--warm">
    <div class="section__container">
      <div class="newsletter">
        <p class="section__overline">Stay Connected</p>
        <h2 class="section__title" style="font-size: clamp(1.5rem, 3vw, 2.25rem);">Letters from the Reading Room</h2>
        <p class="section__desc">A fortnightly letter on books worth savoring, ideas worth considering, and the quiet pleasures of an attentive life.</p>
        <form class="newsletter__form" onsubmit="event.preventDefault()">
          <input type="email" class="newsletter__input" placeholder="Your email address..." aria-label="Email address">
          <button type="submit" class="btn btn--primary" style="white-space: nowrap;">Subscribe</button>
        </form>
      </div>
    </div>
  </section>

  <!-- ===========================
       Footer
       =========================== -->
  <footer class="footer">
    <div class="footer__logo">The Gilded Page</div>
    <p class="footer__tagline">Where sunlight meets the written word</p>
    <ul class="footer__links">
      <li><a href="#">Journal</a></li>
      <li><a href="#">Library</a></li>
      <li><a href="#">Poetry</a></li>
      <li><a href="#">Letters</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">RSS</a></li>
    </ul>
    <div class="footer__divider"></div>
    <p class="footer__copy">&copy; 2026 The Gilded Page. Crafted with care and chamomile tea.</p>
  </footer>

</body>
</html>
```
