# Web 2.0 Design Reference

Web 2.0 is the glossy, gradient-heavy visual aesthetic that defined startup and social-media web design from approximately **2005 to 2010**. Born alongside the explosion of user-generated content platforms -- Flickr, del.icio.us, Digg, early Twitter, Basecamp -- it signaled a shift from the gray, utilitarian interfaces of Web 1.0 to bright, bubbly, inviting pages that made the web feel approachable and exciting. The style is instantly recognizable by its **oversized glossy buttons with specular reflections**, generous drop shadows, rounded-everything, saturated color gradients, "Beta" badges, starburst callouts, reflective-floor logo treatments, and large friendly sans-serif typography rendered almost exclusively in lowercase. As a deliberate retro style today, Web 2.0 carries strong nostalgic appeal for the optimism of the mid-2000s tech boom, evoking the era when "tagging," "sharing," and "social bookmarking" were revolutionary concepts and every startup appended a cheerful gradient badge to announce its perpetual beta status.

---

## Visual Characteristics

### Core Design Traits

- **Glossy / "Wet" buttons** -- the signature element; buttons feature a vertical gradient from light to dark with a white-to-transparent specular highlight across the top half, simulating a convex, lacquered plastic surface
- **Ubiquitous gradients** -- virtually every surface uses a linear gradient, from navigation bars to content panels to footer sections; flat solid fills are avoided
- **Rounded corners everywhere** -- generous `border-radius` on buttons, cards, input fields, navigation bars, and badges; sharp 90-degree corners are rare
- **Prominent drop shadows** -- medium-weight box-shadows on panels, cards, and buttons create a layered, floating appearance above the background
- **Reflective floor / mirror effect** -- logos and hero elements cast a fading, vertically-flipped reflection below them, simulating a polished surface
- **Starburst / badge callouts** -- star-shaped or circular badges (often rotated) containing short text like "New!", "Free!", "Beta", or "2.0" in bold white type, inspired by retail price stickers
- **"Beta" labels** -- small, brightly-colored rounded-rectangle tags appended to logos, signaling perpetual development and startup culture
- **Saturated, friendly color palette** -- bright greens, sky blues, hot pinks, and warm oranges; muted or desaturated tones are almost never used
- **Large call-to-action buttons** -- oversized, brightly-colored action buttons with strong contrast against the page background, drawing immediate attention
- **Simple iconography over stock photography** -- clean, glossy vector icons and screenshots replace traditional corporate stock imagery

### Design Principles

- **Simplicity and focus** -- reduce page elements to essentials; clean, uncluttered layouts with a single primary action per screen
- **Centered, narrow content columns** -- content is typically constrained to a centered 760-960px column with generous side margins
- **Casual, conversational tone** -- friendly, lowercase, informal copy and typography that feel personal rather than corporate
- **Visual hierarchy through size and color** -- large headings, bold colors for key actions, and muted tones for secondary information
- **Generous whitespace and line-height** -- airy layouts with ample breathing room between elements for a crisp, fresh feel
- **Invite participation** -- design communicates openness, community, and collaboration; sign-up forms and social features are prominently placed
- **Progressive disclosure** -- reveal complexity gradually; the homepage is a simple pitch with a single prominent call-to-action

---

## Color Palette

The canonical Web 2.0 palette draws from the branded colors of era-defining services. These are saturated, optimistic, and unapologetically vivid.

| Swatch Name | Hex | Role / Usage |
|-------------|-----|-------------|
| **Flickr Pink** | `#FF0084` | Primary accent, logo highlights, attention-grabbing links |
| **Digg Blue** | `#356AA0` | Navigation backgrounds, header bars, trust-conveying surfaces |
| **Flock Blue** | `#4096EE` | Primary buttons, links, interactive elements, sky tones |
| **RSS Orange** | `#FF7400` | Call-to-action buttons, RSS icons, warm highlights |
| **Techcrunch Green** | `#008C00` | Success states, "Go" buttons, positive indicators |
| **Basecamp Green** | `#6BBA70` | Secondary buttons, muted success, friendly accents |
| **Qoop Mint** | `#CDEB8B` | Light accent backgrounds, tag backgrounds, highlights |
| **Gmail Blue** | `#C3D9FF` | Soft backgrounds, selected-row highlights, info panels |
| **43 Things Gold** | `#C79810` | Premium badges, star ratings, warm accents |
| **Rollyo Red** | `#CC0000` | Error states, alerts, destructive action buttons |
| **Last.fm Crimson** | `#D01F3C` | Bold accent, notifications, badges |
| **Etsy Vermillion** | `#D15600` | Warm secondary CTA, hover states on orange elements |
| **Magnolia Cream** | `#F9F7ED` | Page backgrounds, off-white content areas |
| **Shiny Silver** | `#EEEEEE` | Card backgrounds, border colors, subtle dividers |
| **Shadows Grey** | `#36393D` | Body text, footer backgrounds, dark UI elements |

### CSS Custom Properties

```css
:root {
  /* Primary accents */
  --web2-flickr-pink: #ff0084;
  --web2-flock-blue: #4096ee;
  --web2-digg-blue: #356aa0;
  --web2-rss-orange: #ff7400;
  --web2-techcrunch-green: #008c00;
  --web2-basecamp-green: #6bba70;

  /* Secondary accents */
  --web2-gmail-blue: #c3d9ff;
  --web2-qoop-mint: #cdeb8b;
  --web2-43things-gold: #c79810;
  --web2-etsy-vermillion: #d15600;
  --web2-rollyo-red: #cc0000;
  --web2-lastfm-crimson: #d01f3c;

  /* Neutrals */
  --web2-magnolia: #f9f7ed;
  --web2-silver: #eeeeee;
  --web2-grey: #36393d;
  --web2-white: #ffffff;
  --web2-light-grey: #f5f5f5;
  --web2-mid-grey: #999999;
  --web2-border-grey: #cccccc;

  /* Functional mappings */
  --web2-bg-primary: var(--web2-white);
  --web2-bg-secondary: var(--web2-magnolia);
  --web2-bg-surface: var(--web2-silver);
  --web2-text-primary: var(--web2-grey);
  --web2-text-secondary: var(--web2-mid-grey);
  --web2-accent: var(--web2-flock-blue);
  --web2-accent-secondary: var(--web2-basecamp-green);
  --web2-cta: var(--web2-rss-orange);
  --web2-shadow: rgba(0, 0, 0, 0.25);
  --web2-shadow-light: rgba(0, 0, 0, 0.12);
  --web2-gloss: rgba(255, 255, 255, 0.6);
  --web2-gloss-subtle: rgba(255, 255, 255, 0.3);
}
```

---

## Typography

### Typeface Characteristics

Web 2.0 typography is **clean, rounded, sans-serif, and friendly**. Lowercase is strongly preferred over uppercase. Headings are large and bold, often in a contrasting color to the body. The hallmark fonts of the era -- Lucida Grande, Helvetica, and Verdana -- prioritize screen readability at a time when anti-aliasing and font rendering were still maturing.

### Recommended Google Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Nunito** | Rounded humanist sans | Headlines, logos -- captures the bubbly Web 2.0 warmth |
| **Cabin** | Slightly rounded humanist | Body text, navigation -- clean and modern |
| **Open Sans** | Neutral humanist sans | Body text, paragraphs -- the workhorse readable font |
| **Lato** | Warm semi-rounded sans | Headlines, subheadings -- professional yet friendly |
| **Quicksand** | Rounded geometric sans | Display text, badges, taglines -- playful and bubbly |
| **Varela Round** | Rounded grotesque | Logos, buttons, labels -- the closest to Lucida Grande feel |
| **Source Sans 3** | Adobe humanist sans | Body text, UI labels -- clean Frutiger-like proportions |
| **Rubik** | Rounded geometric-humanist | Headlines, buttons -- chunky and friendly |
| **Ubuntu** | Humanist rounded | Headlines, navigation -- distinctive and warm |
| **PT Sans** | Transitional humanist | Body text, long-form content -- excellent readability |

### Font Pairing Suggestions

| Heading Font | Body Font | Mood / Use Case |
|-------------|-----------|-----------------|
| **Nunito (700)** | **Open Sans (400)** | Classic Web 2.0 feel; bubbly headlines with clean body text |
| **Rubik (700)** | **Source Sans 3 (400)** | Bold, chunky headers with refined, readable body |
| **Varela Round (400)** | **Cabin (400)** | Soft, approachable logos and navigation with crisp content |
| **Quicksand (600)** | **PT Sans (400)** | Playful display text paired with serious readability |
| **Ubuntu (700)** | **Lato (400)** | Distinctive, personality-rich headings with warm body text |

### CSS Example

```css
/* Google Fonts import */
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Open+Sans:wght@400;600&family=Varela+Round&family=Quicksand:wght@500;600;700&display=swap');

/* Headlines */
h1, h2, h3 {
  font-family: 'Nunito', 'Trebuchet MS', 'Lucida Grande', sans-serif;
  font-weight: 700;
  color: var(--web2-grey);
  letter-spacing: -0.01em;
}

/* Display / hero text */
.web2-display {
  font-family: 'Nunito', 'Trebuchet MS', sans-serif;
  font-size: clamp(2rem, 5vw, 3.5rem);
  font-weight: 800;
  line-height: 1.2;
  color: var(--web2-digg-blue);
}

/* Body text */
body {
  font-family: 'Open Sans', 'Lucida Grande', 'Lucida Sans Unicode', Verdana, Helvetica, Arial, sans-serif;
  font-size: 14px;
  font-weight: 400;
  line-height: 1.7;
  color: var(--web2-grey);
  -webkit-font-smoothing: antialiased;
}

/* Logo / brand text */
.web2-logo {
  font-family: 'Varela Round', 'Nunito', 'Lucida Grande', sans-serif;
  font-size: 1.75rem;
  font-weight: 400;
  letter-spacing: -0.02em;
  text-transform: lowercase;
  color: var(--web2-digg-blue);
}

/* Badge / label text */
.web2-label {
  font-family: 'Quicksand', 'Nunito', 'Helvetica Neue', sans-serif;
  font-size: 0.7rem;
  font-weight: 700;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: var(--web2-white);
}

/* Navigation links */
.web2-nav-link {
  font-family: 'Nunito', 'Lucida Grande', sans-serif;
  font-size: 0.875rem;
  font-weight: 600;
  color: var(--web2-white);
  text-decoration: none;
  text-transform: lowercase;
}
```

---

## Layout Principles

- **Fixed-width, centered layout** -- the classic 960px (or 760px) centered container with equal left/right margins; fluid/responsive layouts were not yet common
- **Top navigation bar** -- a horizontal gradient bar spanning the full viewport width, containing the logo on the left and navigation links on the right
- **Prominent hero/pitch section** -- a large area immediately below the nav with a headline, tagline, and oversized call-to-action button
- **Three-column feature grid** -- three side-by-side columns below the hero, each with an icon, heading, and short description
- **Generous vertical spacing** -- sections are separated by ample padding (40-80px) and sometimes thin horizontal rules
- **Footer with utility links** -- a darker-toned footer containing secondary navigation, copyright, and the ubiquitous "About / Blog / Contact / Terms" links
- **Sidebar patterns** -- on interior pages, a right sidebar for secondary navigation, tag clouds, or social widgets
- **Single-column sign-up flow** -- registration and login forms are centered, minimal, and visually prominent
- **Content width: 600-700px for text** -- body text columns are kept narrow for readability, even within the wider 960px container
- **Clear visual hierarchy** -- the page reads top-to-bottom with decreasing visual weight: logo > headline > CTA > features > footer

---

## CSS / Design Techniques

### Glossy Card Component

```css
/* The classic Web 2.0 content card with gradient and shadow */
.web2-card {
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #f5f5f5 60%,
    #eeeeee 100%
  );
  border: 1px solid #cccccc;
  border-radius: 12px;
  padding: 1.5rem 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 3px 8px rgba(0, 0, 0, 0.15),
    0 1px 2px rgba(0, 0, 0, 0.08);
  transition: box-shadow 0.2s ease, transform 0.2s ease;
}

/* Upper gloss highlight */
.web2-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.8) 0%,
    rgba(255, 255, 255, 0.2) 50%,
    transparent 100%
  );
  border-radius: 12px 12px 0 0;
  pointer-events: none;
}

.web2-card:hover {
  transform: translateY(-2px);
  box-shadow:
    0 6px 16px rgba(0, 0, 0, 0.18),
    0 2px 4px rgba(0, 0, 0, 0.08);
}

.web2-card h3 {
  margin: 0 0 0.75rem;
  font-size: 1.15rem;
  color: var(--web2-digg-blue);
}

.web2-card p {
  margin: 0;
  font-size: 0.9rem;
  color: #666666;
  line-height: 1.6;
}
```

### Glossy Button Component (The Iconic Web 2.0 Button)

```css
/* The quintessential Web 2.0 glossy button */
.web2-button {
  display: inline-block;
  padding: 0.65rem 1.75rem;
  border-radius: 8px;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-bottom: 2px solid rgba(0, 0, 0, 0.25);
  background: linear-gradient(
    180deg,
    #5aabf0 0%,
    #4096ee 45%,
    #2a7ad5 100%
  );
  color: #ffffff;
  font-family: 'Nunito', 'Lucida Grande', sans-serif;
  font-size: 0.95rem;
  font-weight: 700;
  text-shadow: 0 -1px 1px rgba(0, 0, 0, 0.3);
  cursor: pointer;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 2px 6px rgba(0, 0, 0, 0.2),
    inset 0 1px 0 rgba(255, 255, 255, 0.35);
  transition: all 0.15s ease;
  text-decoration: none;
}

/* Glossy specular highlight across top half */
.web2-button::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.5) 0%,
    rgba(255, 255, 255, 0.1) 100%
  );
  border-radius: 7px 7px 0 0;
  pointer-events: none;
}

.web2-button:hover {
  background: linear-gradient(
    180deg,
    #6ab8f7 0%,
    #4da3f5 45%,
    #3585e0 100%
  );
  box-shadow:
    0 3px 10px rgba(0, 0, 0, 0.25),
    inset 0 1px 0 rgba(255, 255, 255, 0.4);
  transform: translateY(-1px);
}

.web2-button:active {
  background: linear-gradient(
    180deg,
    #3585e0 0%,
    #2a7ad5 45%,
    #1e6ac0 100%
  );
  box-shadow:
    0 1px 3px rgba(0, 0, 0, 0.2),
    inset 0 2px 4px rgba(0, 0, 0, 0.15);
  transform: translateY(0);
}

/* Green CTA variant */
.web2-button--green {
  background: linear-gradient(180deg, #5fbf6f 0%, #3da84d 45%, #2a8e3a 100%);
  border-color: rgba(0, 80, 0, 0.3);
}

.web2-button--green:hover {
  background: linear-gradient(180deg, #72cc80 0%, #4db85d 45%, #359945 100%);
}

/* Orange CTA variant */
.web2-button--orange {
  background: linear-gradient(180deg, #ff9933 0%, #ff7400 45%, #e06000 100%);
  border-color: rgba(100, 50, 0, 0.3);
}

.web2-button--orange:hover {
  background: linear-gradient(180deg, #ffad55 0%, #ff8822 45%, #f07010 100%);
}

/* Large "Sign Up Free" CTA variant */
.web2-button--large {
  padding: 1rem 2.5rem;
  font-size: 1.2rem;
  border-radius: 10px;
}
```

### Navigation Bar

```css
/* Classic Web 2.0 gradient navigation bar */
.web2-nav {
  background: linear-gradient(
    180deg,
    #5a6c80 0%,
    #3d4f63 50%,
    #2c3e50 100%
  );
  border-bottom: 1px solid #1a2a3a;
  padding: 0 2rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 48px;
  position: relative;
  box-shadow:
    0 2px 8px rgba(0, 0, 0, 0.25),
    inset 0 1px 0 rgba(255, 255, 255, 0.12);
}

/* Top-edge gloss on nav bar */
.web2-nav::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.15) 0%,
    rgba(255, 255, 255, 0.02) 100%
  );
  pointer-events: none;
}

.web2-nav__logo {
  font-family: 'Varela Round', 'Nunito', sans-serif;
  font-size: 1.35rem;
  color: #ffffff;
  text-decoration: none;
  text-transform: lowercase;
  position: relative;
  z-index: 1;
}

.web2-nav__links {
  display: flex;
  gap: 0.25rem;
  list-style: none;
  margin: 0;
  padding: 0;
  position: relative;
  z-index: 1;
}

.web2-nav__links a {
  display: block;
  padding: 0.4rem 0.9rem;
  border-radius: 4px;
  font-family: 'Nunito', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  color: rgba(255, 255, 255, 0.85);
  text-decoration: none;
  transition: all 0.15s ease;
}

.web2-nav__links a:hover,
.web2-nav__links a.active {
  background: rgba(255, 255, 255, 0.12);
  color: #ffffff;
}
```

### Hero Section

```css
/* Web 2.0 hero section with gradient background */
.web2-hero {
  background: linear-gradient(
    180deg,
    #e8f4fd 0%,
    #c3d9ff 40%,
    #a8c8f0 100%
  );
  border-bottom: 1px solid #a0b8d0;
  text-align: center;
  padding: 4rem 2rem 5rem;
  position: relative;
  overflow: hidden;
}

/* Subtle inner shadow at bottom */
.web2-hero::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 40px;
  background: linear-gradient(
    180deg,
    transparent,
    rgba(0, 0, 0, 0.04)
  );
  pointer-events: none;
}

.web2-hero h1 {
  font-family: 'Nunito', 'Trebuchet MS', sans-serif;
  font-size: clamp(2rem, 5vw, 3.2rem);
  font-weight: 800;
  color: var(--web2-grey);
  margin-bottom: 0.75rem;
  text-shadow: 0 1px 0 rgba(255, 255, 255, 0.7);
}

.web2-hero p {
  font-family: 'Open Sans', sans-serif;
  font-size: 1.15rem;
  color: #555555;
  max-width: 600px;
  margin: 0 auto 2rem;
  line-height: 1.6;
}
```

### Beta Badge

```css
/* The iconic Web 2.0 "Beta" badge */
.web2-beta-badge {
  display: inline-block;
  padding: 0.15rem 0.55rem;
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-size: 0.6rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: #ffffff;
  background: linear-gradient(
    180deg,
    #ff5a9e 0%,
    #ff0084 50%,
    #d4006d 100%
  );
  border-radius: 6px;
  border: 1px solid rgba(0, 0, 0, 0.15);
  box-shadow:
    0 1px 3px rgba(0, 0, 0, 0.2),
    inset 0 1px 0 rgba(255, 255, 255, 0.35);
  position: relative;
  overflow: hidden;
  vertical-align: super;
  margin-left: 0.3rem;
  line-height: 1;
}

/* Glossy top highlight */
.web2-beta-badge::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.45) 0%,
    rgba(255, 255, 255, 0.05) 100%
  );
  pointer-events: none;
}
```

### Starburst / Callout Badge

```css
/* Web 2.0 starburst callout -- the "New!", "Free!", "Sale!" badge */
.web2-starburst {
  position: relative;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 80px;
  height: 80px;
  font-family: 'Nunito', sans-serif;
  font-size: 0.85rem;
  font-weight: 800;
  color: #ffffff;
  text-transform: uppercase;
  text-shadow: 0 -1px 1px rgba(0, 0, 0, 0.3);
  z-index: 1;
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.25));
}

/* Star shape built from rotated squares */
.web2-starburst::before,
.web2-starburst::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    180deg,
    #ff5a5a 0%,
    #cc0000 100%
  );
  z-index: -1;
}

.web2-starburst::before {
  border-radius: 4px;
  transform: rotate(0deg);
}

.web2-starburst::after {
  border-radius: 4px;
  transform: rotate(45deg);
}

/* Third layer via a wrapper for full starburst (use an inner span) */
.web2-starburst span {
  position: relative;
  z-index: 2;
}

/* Alternate approach: CSS clip-path starburst */
.web2-starburst--clip {
  width: 90px;
  height: 90px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(
    180deg,
    #ff5a5a 0%,
    #cc0000 100%
  );
  clip-path: polygon(
    50% 0%, 63% 25%, 90% 10%, 78% 38%,
    100% 50%, 78% 63%, 90% 90%, 63% 78%,
    50% 100%, 38% 78%, 10% 90%, 23% 63%,
    0% 50%, 23% 38%, 10% 10%, 38% 25%
  );
  font-family: 'Nunito', sans-serif;
  font-size: 0.8rem;
  font-weight: 800;
  color: #ffffff;
  text-transform: uppercase;
  text-shadow: 0 -1px 1px rgba(0, 0, 0, 0.3);
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.25));
}
```

### Reflective Floor Effect

```css
/* The classic Web 2.0 reflective floor / mirror effect */
.web2-reflection-container {
  display: inline-block;
  position: relative;
}

.web2-reflection-container img,
.web2-reflection-container .web2-reflected-text {
  display: block;
}

/* The reflection is an inverted, fading copy placed below the original */
.web2-reflection {
  transform: scaleY(-1);
  -webkit-mask-image: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0.25) 0%,
    transparent 60%
  );
  mask-image: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0.25) 0%,
    transparent 60%
  );
  opacity: 0.4;
  pointer-events: none;
  margin-top: -2px;
}

/* Reflective floor surface beneath hero elements */
.web2-reflective-floor {
  position: relative;
  padding-bottom: 3rem;
}

.web2-reflective-floor::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(0, 0, 0, 0.08),
    transparent
  );
}
```

### Glossy Panel / Content Box

```css
/* Glossy raised panel -- the Web 2.0 content container */
.web2-panel {
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #f8f8f8 100%
  );
  border: 1px solid #cccccc;
  border-top: 1px solid #dddddd;
  border-radius: 10px;
  padding: 1.5rem 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 3px 10px rgba(0, 0, 0, 0.12),
    inset 0 1px 0 rgba(255, 255, 255, 0.9);
}

/* Gradient header bar on panel */
.web2-panel__header {
  background: linear-gradient(
    180deg,
    #5a8cbf 0%,
    #356aa0 50%,
    #2a5580 100%
  );
  margin: -1.5rem -2rem 1.5rem;
  padding: 0.75rem 2rem;
  border-radius: 10px 10px 0 0;
  border-bottom: 1px solid #1e3f5f;
  position: relative;
  overflow: hidden;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.2);
}

/* Gloss on panel header */
.web2-panel__header::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.2) 0%,
    rgba(255, 255, 255, 0.02) 100%
  );
  pointer-events: none;
}

.web2-panel__header h3 {
  margin: 0;
  font-size: 0.95rem;
  font-weight: 700;
  color: #ffffff;
  text-shadow: 0 -1px 1px rgba(0, 0, 0, 0.3);
}
```

### Tag Cloud

```css
/* Web 2.0 tag cloud -- the iconic sidebar widget */
.web2-tag-cloud {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem;
  padding: 1rem;
}

.web2-tag {
  display: inline-block;
  padding: 0.2rem 0.6rem;
  background: linear-gradient(
    180deg,
    #f0f0f0 0%,
    #e0e0e0 100%
  );
  border: 1px solid #cccccc;
  border-radius: 4px;
  font-family: 'Open Sans', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  color: var(--web2-digg-blue);
  text-decoration: none;
  box-shadow:
    0 1px 2px rgba(0, 0, 0, 0.08),
    inset 0 1px 0 rgba(255, 255, 255, 0.8);
  transition: all 0.15s ease;
}

.web2-tag:hover {
  background: linear-gradient(
    180deg,
    #4da3f5 0%,
    #356aa0 100%
  );
  color: #ffffff;
  border-color: #2a5580;
  text-shadow: 0 -1px 1px rgba(0, 0, 0, 0.2);
}

/* Size variations for cloud weighting */
.web2-tag--sm { font-size: 0.65rem; }
.web2-tag--md { font-size: 0.8rem; }
.web2-tag--lg { font-size: 1rem; font-weight: 700; }
.web2-tag--xl { font-size: 1.2rem; font-weight: 800; }
```

---

## Design Do's and Don'ts

### Do's

- **Do** use vertical gradients on every interactive surface -- buttons, nav bars, panels, and badges all get the light-to-dark treatment
- **Do** add a `::before` pseudo-element with a white-to-transparent gradient on the top half of glossy elements for the specular highlight
- **Do** use `inset` box-shadows with white for inner glow and standard box-shadows for depth beneath elements
- **Do** round your corners generously -- `border-radius: 6px` to `12px` for containers, full pill shapes for tags and small badges
- **Do** keep typography lowercase, friendly, and casual; use large font sizes for headings (24-36px)
- **Do** embrace bold, saturated brand colors -- bright greens, vivid blues, punchy oranges
- **Do** include signature Web 2.0 furniture: a "Beta" badge, a tag cloud, a starburst callout, a reflective logo
- **Do** separate sections with gradient backgrounds, alternating between light (white/cream) and soft blue/green tinted bands
- **Do** text-shadow your white button text with `0 -1px 1px rgba(0,0,0,0.3)` for the classic engraved/letterpress look
- **Do** use a centered, fixed-width layout (960px) for authenticity

### Don'ts

- **Don't** use flat, solid-color fills without gradients -- that belongs to the Flat Design era that replaced Web 2.0
- **Don't** use dark mode or dark backgrounds as the primary theme; Web 2.0 is overwhelmingly light, bright, and airy
- **Don't** use modern CSS features like `backdrop-filter` or glassmorphism -- Web 2.0 predates these; use opaque gradients and solid shadows instead
- **Don't** use CSS Grid or Flexbox-based complex layouts for an authentic retro feel -- float-based or simple centered columns are period-accurate
- **Don't** use thin, ultralight font weights -- Web 2.0 fonts are regular (400) to bold (700), never hairline
- **Don't** use uppercase headings or all-caps navigation -- lowercase is the Web 2.0 way
- **Don't** use desaturated, muted, or pastel color palettes -- Web 2.0 colors are vivid and unapologetically bright
- **Don't** overcomplicate the page with too many columns or competing CTAs -- simplicity and focus are core principles
- **Don't** use realistic photography as primary imagery -- prefer vector icons, screenshots, and simple illustrations
- **Don't** forget the drop shadow -- nearly every raised element casts a soft shadow onto the surface below it

---

## Related Aesthetics

| Aesthetic | Relationship to Web 2.0 |
|-----------|------------------------|
| **Frutiger Aero** | Sibling aesthetic; shares the same era and glossy techniques but focuses on nature imagery, eco-optimism, and Aero Glass transparency rather than startup culture |
| **Light Skeuomorphism** | Modern descendant; revives subtle depth cues (soft shadows, gentle gradients) without the full glossy excess |
| **Flat Design** | Direct successor and reaction; stripped away all of Web 2.0's gradients, gloss, and shadows starting around 2012-2013 with iOS 7 and Metro |
| **Material Design** | Google's structured evolution; reintroduced shadows and layers to Flat Design using Web 2.0-era depth principles |
| **Glassmorphism** | Spiritual grandchild; revives translucency and gloss in a contemporary context |
| **Claymorphism** | Modern playful cousin; shares the bubbly, rounded, colorful sensibility but with inflated 3D clay-like surfaces |
| **Metro Design** | Contemporary rival that emerged at the end of Web 2.0; Microsoft's sharp-cornered, typography-first reaction to glossy excess |
| **8-Bit** | Shares the playful, nostalgic tone but draws from an earlier pixel-art era rather than mid-2000s startup culture |
| **Dopamine Design** | Modern spiritual successor; matches Web 2.0's bold, saturated, optimistic color energy in a contemporary context |
| **Y2K Futurism** | Predecessor; shares techno-optimism but with a chrome, metallic, angular language rather than rounded bubbly gloss |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>shareify -- share anything, anywhere</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Open+Sans:wght@400;600&family=Varela+Round&family=Quicksand:wght@500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --web2-flickr-pink: #ff0084;
      --web2-flock-blue: #4096ee;
      --web2-digg-blue: #356aa0;
      --web2-rss-orange: #ff7400;
      --web2-basecamp-green: #6bba70;
      --web2-gmail-blue: #c3d9ff;
      --web2-qoop-mint: #cdeb8b;
      --web2-magnolia: #f9f7ed;
      --web2-silver: #eeeeee;
      --web2-grey: #36393d;
      --web2-white: #ffffff;
      --web2-border: #cccccc;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--web2-magnolia);
      color: var(--web2-grey);
      font-family: 'Open Sans', 'Lucida Grande', Verdana, Helvetica, Arial, sans-serif;
      font-size: 14px;
      line-height: 1.7;
      -webkit-font-smoothing: antialiased;
    }

    /* ── Navigation Bar ── */
    .nav {
      background: linear-gradient(180deg, #5a6c80 0%, #3d4f63 50%, #2c3e50 100%);
      border-bottom: 1px solid #1a2a3a;
      padding: 0 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 48px;
      position: relative;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.25), inset 0 1px 0 rgba(255, 255, 255, 0.12);
    }

    .nav::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0;
      height: 50%;
      background: linear-gradient(180deg, rgba(255,255,255,0.15), rgba(255,255,255,0.02));
      pointer-events: none;
    }

    .nav-logo {
      font-family: 'Varela Round', 'Nunito', sans-serif;
      font-size: 1.35rem;
      color: #fff;
      text-decoration: none;
      text-transform: lowercase;
      position: relative; z-index: 1;
    }

    .nav-logo .beta {
      display: inline-block;
      padding: 0.1rem 0.45rem;
      font-family: 'Quicksand', sans-serif;
      font-size: 0.55rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: #fff;
      background: linear-gradient(180deg, #ff5a9e, #ff0084, #d4006d);
      border-radius: 5px;
      border: 1px solid rgba(0,0,0,0.15);
      box-shadow: 0 1px 2px rgba(0,0,0,0.2), inset 0 1px 0 rgba(255,255,255,0.3);
      position: relative; overflow: hidden;
      vertical-align: super;
      margin-left: 0.2rem;
      line-height: 1;
    }

    .nav-logo .beta::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 50%;
      background: linear-gradient(180deg, rgba(255,255,255,0.4), rgba(255,255,255,0));
      pointer-events: none;
    }

    .nav-links {
      display: flex;
      gap: 0.25rem;
      list-style: none;
      position: relative; z-index: 1;
    }

    .nav-links a {
      display: block;
      padding: 0.4rem 0.9rem;
      border-radius: 4px;
      font-family: 'Nunito', sans-serif;
      font-size: 0.85rem;
      font-weight: 600;
      color: rgba(255,255,255,0.85);
      text-decoration: none;
      text-transform: lowercase;
      transition: all 0.15s ease;
    }

    .nav-links a:hover, .nav-links a.active {
      background: rgba(255,255,255,0.12);
      color: #ffffff;
    }

    /* ── Hero Section ── */
    .hero {
      background: linear-gradient(180deg, #e8f4fd 0%, #c3d9ff 40%, #a8c8f0 100%);
      border-bottom: 1px solid #a0b8d0;
      text-align: center;
      padding: 4rem 2rem 5rem;
      position: relative;
      overflow: hidden;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: 0; left: 0; right: 0;
      height: 40px;
      background: linear-gradient(180deg, transparent, rgba(0,0,0,0.04));
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Nunito', 'Trebuchet MS', sans-serif;
      font-size: clamp(2rem, 5vw, 3.2rem);
      font-weight: 800;
      color: var(--web2-grey);
      margin-bottom: 0.75rem;
      text-shadow: 0 1px 0 rgba(255,255,255,0.7);
    }

    .hero p {
      font-size: 1.15rem;
      color: #555;
      max-width: 600px;
      margin: 0 auto 2rem;
      line-height: 1.6;
    }

    /* ── Glossy Button ── */
    .btn {
      display: inline-block;
      padding: 0.75rem 2rem;
      border-radius: 8px;
      border: 1px solid rgba(0,0,0,0.2);
      border-bottom: 2px solid rgba(0,0,0,0.25);
      color: #fff;
      font-family: 'Nunito', sans-serif;
      font-size: 1rem;
      font-weight: 700;
      text-shadow: 0 -1px 1px rgba(0,0,0,0.3);
      cursor: pointer;
      position: relative;
      overflow: hidden;
      transition: all 0.15s ease;
      text-decoration: none;
    }

    .btn::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 50%;
      background: linear-gradient(180deg, rgba(255,255,255,0.5), rgba(255,255,255,0.1));
      border-radius: 7px 7px 0 0;
      pointer-events: none;
    }

    .btn:hover { transform: translateY(-1px); }
    .btn:active { transform: translateY(0); }

    .btn--blue {
      background: linear-gradient(180deg, #5aabf0, #4096ee 45%, #2a7ad5);
      box-shadow: 0 2px 6px rgba(0,0,0,0.2), inset 0 1px 0 rgba(255,255,255,0.35);
    }

    .btn--blue:hover {
      background: linear-gradient(180deg, #6ab8f7, #4da3f5 45%, #3585e0);
      box-shadow: 0 3px 10px rgba(0,0,0,0.25), inset 0 1px 0 rgba(255,255,255,0.4);
    }

    .btn--green {
      background: linear-gradient(180deg, #5fbf6f, #3da84d 45%, #2a8e3a);
      box-shadow: 0 2px 6px rgba(0,80,0,0.2), inset 0 1px 0 rgba(255,255,255,0.35);
    }

    .btn--green:hover {
      background: linear-gradient(180deg, #72cc80, #4db85d 45%, #359945);
    }

    .btn--orange {
      background: linear-gradient(180deg, #ff9933, #ff7400 45%, #e06000);
      box-shadow: 0 2px 6px rgba(100,50,0,0.2), inset 0 1px 0 rgba(255,255,255,0.35);
    }

    .btn--large {
      padding: 1rem 2.75rem;
      font-size: 1.2rem;
      border-radius: 10px;
    }

    /* ── Main Container ── */
    .container {
      max-width: 960px;
      margin: 0 auto;
      padding: 0 2rem;
    }

    /* ── Feature Cards Section ── */
    .features {
      padding: 3rem 0;
    }

    .features h2 {
      font-family: 'Nunito', sans-serif;
      font-size: 1.6rem;
      font-weight: 700;
      color: var(--web2-digg-blue);
      text-align: center;
      margin-bottom: 2rem;
    }

    .feature-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1.5rem;
    }

    .card {
      background: linear-gradient(180deg, #ffffff 0%, #f5f5f5 60%, #eee 100%);
      border: 1px solid var(--web2-border);
      border-radius: 12px;
      padding: 1.75rem 1.5rem;
      text-align: center;
      position: relative;
      overflow: hidden;
      box-shadow: 0 3px 8px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.06);
      transition: box-shadow 0.2s ease, transform 0.2s ease;
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 50%;
      background: linear-gradient(180deg, rgba(255,255,255,0.8), rgba(255,255,255,0.15), transparent);
      border-radius: 12px 12px 0 0;
      pointer-events: none;
    }

    .card:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 16px rgba(0,0,0,0.15), 0 2px 4px rgba(0,0,0,0.06);
    }

    .card-icon {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 56px;
      height: 56px;
      border-radius: 14px;
      font-size: 1.5rem;
      margin-bottom: 1rem;
      position: relative;
      overflow: hidden;
      box-shadow: 0 3px 8px rgba(0,0,0,0.2), inset 0 1px 0 rgba(255,255,255,0.4);
    }

    .card-icon::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 50%;
      background: linear-gradient(180deg, rgba(255,255,255,0.5), rgba(255,255,255,0.05));
      pointer-events: none;
    }

    .card-icon--blue {
      background: linear-gradient(180deg, #5aabf0, #356aa0);
    }

    .card-icon--green {
      background: linear-gradient(180deg, #72cc80, #2a8e3a);
    }

    .card-icon--orange {
      background: linear-gradient(180deg, #ffad55, #e06000);
    }

    .card h3 {
      font-family: 'Nunito', sans-serif;
      font-size: 1.1rem;
      font-weight: 700;
      color: var(--web2-digg-blue);
      margin-bottom: 0.5rem;
    }

    .card p {
      font-size: 0.85rem;
      color: #666;
      line-height: 1.6;
    }

    /* ── Starburst Badge ── */
    .starburst {
      position: absolute;
      top: -8px;
      right: -8px;
      width: 70px;
      height: 70px;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(180deg, #ff5a5a, #cc0000);
      clip-path: polygon(
        50% 0%, 63% 25%, 90% 10%, 78% 38%,
        100% 50%, 78% 63%, 90% 90%, 63% 78%,
        50% 100%, 38% 78%, 10% 90%, 23% 63%,
        0% 50%, 23% 38%, 10% 10%, 38% 25%
      );
      font-family: 'Nunito', sans-serif;
      font-size: 0.65rem;
      font-weight: 800;
      color: #fff;
      text-transform: uppercase;
      text-shadow: 0 -1px 1px rgba(0,0,0,0.3);
      filter: drop-shadow(0 2px 3px rgba(0,0,0,0.25));
      z-index: 2;
      transform: rotate(12deg);
    }

    /* ── Glossy Panel with Header ── */
    .panel {
      background: linear-gradient(180deg, #fff, #f8f8f8);
      border: 1px solid var(--web2-border);
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1), inset 0 1px 0 rgba(255,255,255,0.9);
      margin-top: 2rem;
    }

    .panel-header {
      background: linear-gradient(180deg, #5a8cbf, #356aa0 50%, #2a5580);
      padding: 0.75rem 1.5rem;
      border-bottom: 1px solid #1e3f5f;
      position: relative;
      overflow: hidden;
      box-shadow: inset 0 1px 0 rgba(255,255,255,0.2);
    }

    .panel-header::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 50%;
      background: linear-gradient(180deg, rgba(255,255,255,0.2), rgba(255,255,255,0.02));
      pointer-events: none;
    }

    .panel-header h3 {
      font-family: 'Nunito', sans-serif;
      font-size: 0.95rem;
      font-weight: 700;
      color: #fff;
      text-shadow: 0 -1px 1px rgba(0,0,0,0.3);
      position: relative;
      z-index: 1;
    }

    .panel-body {
      padding: 1.5rem;
    }

    /* ── Tag Cloud ── */
    .tag-cloud {
      display: flex;
      flex-wrap: wrap;
      gap: 0.4rem;
    }

    .tag {
      display: inline-block;
      padding: 0.2rem 0.6rem;
      background: linear-gradient(180deg, #f0f0f0, #e0e0e0);
      border: 1px solid #ccc;
      border-radius: 4px;
      font-family: 'Open Sans', sans-serif;
      font-weight: 600;
      color: var(--web2-digg-blue);
      text-decoration: none;
      box-shadow: 0 1px 2px rgba(0,0,0,0.08), inset 0 1px 0 rgba(255,255,255,0.8);
      transition: all 0.15s ease;
    }

    .tag:hover {
      background: linear-gradient(180deg, #4da3f5, #356aa0);
      color: #fff;
      border-color: #2a5580;
    }

    .tag--sm { font-size: 0.6rem; }
    .tag--md { font-size: 0.75rem; }
    .tag--lg { font-size: 0.9rem; font-weight: 700; }
    .tag--xl { font-size: 1.05rem; font-weight: 800; }

    /* ── Reflective Logo ── */
    .logo-reflect {
      text-align: center;
      padding: 3rem 0 2rem;
    }

    .logo-reflect h2 {
      font-family: 'Varela Round', 'Nunito', sans-serif;
      font-size: 3rem;
      font-weight: 400;
      color: var(--web2-digg-blue);
      text-transform: lowercase;
      line-height: 1;
      margin-bottom: 0;
    }

    .logo-reflect .reflection {
      font-family: 'Varela Round', 'Nunito', sans-serif;
      font-size: 3rem;
      font-weight: 400;
      color: var(--web2-digg-blue);
      text-transform: lowercase;
      line-height: 1;
      transform: scaleY(-1);
      -webkit-mask-image: linear-gradient(180deg, rgba(0,0,0,0.2) 0%, transparent 55%);
      mask-image: linear-gradient(180deg, rgba(0,0,0,0.2) 0%, transparent 55%);
      opacity: 0.35;
      pointer-events: none;
      user-select: none;
      margin-top: -4px;
    }

    .logo-reflect .floor-line {
      width: 200px;
      height: 1px;
      background: linear-gradient(90deg, transparent, rgba(0,0,0,0.08), transparent);
      margin: 0 auto;
    }

    /* ── CTA Section ── */
    .cta-section {
      text-align: center;
      padding: 3rem 0;
    }

    .cta-section h2 {
      font-family: 'Nunito', sans-serif;
      font-size: 1.5rem;
      font-weight: 700;
      color: var(--web2-grey);
      margin-bottom: 0.5rem;
    }

    .cta-section p {
      color: #777;
      margin-bottom: 1.5rem;
    }

    /* ── Footer ── */
    .footer {
      background: linear-gradient(180deg, #3d4f63, #2c3e50);
      border-top: 1px solid #556b7f;
      padding: 2rem;
      text-align: center;
      position: relative;
      box-shadow: inset 0 1px 0 rgba(255,255,255,0.08);
    }

    .footer::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 1px;
      background: rgba(255,255,255,0.1);
    }

    .footer-links {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      list-style: none;
      margin-bottom: 1rem;
    }

    .footer-links a {
      font-family: 'Nunito', sans-serif;
      font-size: 0.8rem;
      font-weight: 600;
      color: rgba(255,255,255,0.65);
      text-decoration: none;
      text-transform: lowercase;
      transition: color 0.15s ease;
    }

    .footer-links a:hover {
      color: #ffffff;
    }

    .footer p {
      font-size: 0.75rem;
      color: rgba(255,255,255,0.4);
    }

    /* ── Responsive adjustments ── */
    @media (max-width: 768px) {
      .feature-grid {
        grid-template-columns: 1fr;
        gap: 1rem;
      }

      .nav {
        flex-direction: column;
        height: auto;
        padding: 0.75rem 1.5rem;
        gap: 0.5rem;
      }

      .nav-links { gap: 0.15rem; }

      .hero { padding: 2.5rem 1.5rem 3.5rem; }
    }
  </style>
</head>
<body>

  <!-- Navigation Bar -->
  <nav class="nav">
    <a href="#" class="nav-logo">shareify<span class="beta">beta</span></a>
    <ul class="nav-links">
      <li><a href="#" class="active">home</a></li>
      <li><a href="#">features</a></li>
      <li><a href="#">pricing</a></li>
      <li><a href="#">blog</a></li>
      <li><a href="#">sign up</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <h1>share anything, with anyone, anywhere.</h1>
    <p>the simple way to bookmark, tag, and share your favorite links with the world. it's fast, free, and ridiculously easy.</p>
    <a href="#" class="btn btn--green btn--large">get started free &raquo;</a>
  </section>

  <!-- Features Section -->
  <div class="container">
    <section class="features">
      <h2>why you'll love shareify</h2>

      <div class="feature-grid">

        <!-- Card 1 -->
        <div class="card">
          <div class="starburst">new!</div>
          <div class="card-icon card-icon--blue">&#9733;</div>
          <h3>smart tagging</h3>
          <p>organize your bookmarks with tags that actually make sense. find anything in seconds, not minutes.</p>
        </div>

        <!-- Card 2 -->
        <div class="card">
          <div class="card-icon card-icon--green">&#9829;</div>
          <h3>social sharing</h3>
          <p>see what your friends are bookmarking. discover trending links from the community in real-time.</p>
        </div>

        <!-- Card 3 -->
        <div class="card">
          <div class="card-icon card-icon--orange">&#9889;</div>
          <h3>instant sync</h3>
          <p>your bookmarks follow you everywhere. access them from any browser, any device, any time.</p>
        </div>

      </div>
    </section>

    <!-- Reflective Logo Demo -->
    <section class="logo-reflect">
      <h2>shareify</h2>
      <div class="floor-line"></div>
      <div class="reflection" aria-hidden="true">shareify</div>
    </section>

    <!-- Panel with Tag Cloud -->
    <div class="panel">
      <div class="panel-header">
        <h3>popular tags</h3>
      </div>
      <div class="panel-body">
        <div class="tag-cloud">
          <a href="#" class="tag tag--xl">javascript</a>
          <a href="#" class="tag tag--lg">web 2.0</a>
          <a href="#" class="tag tag--lg">ajax</a>
          <a href="#" class="tag tag--md">ruby on rails</a>
          <a href="#" class="tag tag--xl">css</a>
          <a href="#" class="tag tag--sm">microformats</a>
          <a href="#" class="tag tag--md">api</a>
          <a href="#" class="tag tag--lg">mashup</a>
          <a href="#" class="tag tag--sm">rss</a>
          <a href="#" class="tag tag--md">folksonomy</a>
          <a href="#" class="tag tag--lg">social</a>
          <a href="#" class="tag tag--sm">tagging</a>
          <a href="#" class="tag tag--md">widgets</a>
          <a href="#" class="tag tag--xl">design</a>
          <a href="#" class="tag tag--sm">podcasting</a>
          <a href="#" class="tag tag--lg">startups</a>
          <a href="#" class="tag tag--md">flickr</a>
          <a href="#" class="tag tag--sm">digg</a>
        </div>
      </div>
    </div>

    <!-- CTA Section -->
    <section class="cta-section">
      <h2>ready to start sharing?</h2>
      <p>join 127,483 people who are already using shareify to organize the web.</p>
      <a href="#" class="btn btn--orange btn--large">sign up for free &raquo;</a>
    </section>
  </div>

  <!-- Footer -->
  <footer class="footer">
    <ul class="footer-links">
      <li><a href="#">about</a></li>
      <li><a href="#">blog</a></li>
      <li><a href="#">api</a></li>
      <li><a href="#">terms</a></li>
      <li><a href="#">privacy</a></li>
      <li><a href="#">contact</a></li>
    </ul>
    <p>&copy; 2007 shareify, inc. all rights reserved. made with &hearts; in san francisco.</p>
  </footer>

</body>
</html>
```
