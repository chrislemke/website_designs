# Expressionism Reference

Expressionism is an art-driven design aesthetic rooted in the early 20th-century movement that prioritized emotional truth over visual accuracy. Applied to digital design, it uses vivid, often clashing colors, distorted forms, heavy contrast, and raw brushstroke textures to convey intensity and subjective experience. The style rejects polished perfection in favor of visible human gesture -- jagged edges, uneven compositions, and dramatic tonal shifts that make the viewer feel something visceral before they think anything rational.

---

## Visual Characteristics

### Core Design Traits

- **Vivid, emotionally charged colors** -- deep reds, electric blues, acid yellows, and heavy blacks used for psychological impact
- **Distorted, angular forms** -- shapes are stretched, skewed, and fragmented to create tension and unease
- **Heavy contrast** -- extreme light/dark juxtapositions that create drama and focal intensity
- **Visible texture and brushwork** -- surfaces feel hand-painted with rough edges, grain, and impasto-like digital textures
- **Bold, thick outlines** -- dark contour lines around elements reminiscent of woodcut prints and expressionist painting
- **Asymmetric, unstable compositions** -- layouts that feel deliberately off-balance and emotionally charged
- **Raw, unpolished elements** -- imperfect edges, smeared colors, and visible artifacts as aesthetic choices
- **Dark, moody backgrounds** -- deep tones that ground the vivid foreground elements
- **Dramatic scale contrast** -- oversized elements paired with small details for visual tension
- **Hand-drawn and organic** -- curves, strokes, and shapes that feel human-made, not machine-generated

### Design Principles

- Emotion first: every design decision should amplify the intended feeling
- Color is not decorative but expressive -- choose hues for their psychological impact
- Imperfection is intentional: rough edges and visible texture convey authenticity
- Contrast creates drama: push light against dark, large against small, calm against chaotic
- Composition should feel dynamic and slightly unstable to maintain tension
- Typography is expressive, not merely functional -- letterforms carry emotion
- Break conventional design rules deliberately: overlap, misalign, and distort with purpose
- The viewer should have a visceral, gut-level response before an intellectual one

---

## Color Palette

### Expressionism Core Palette

Colors drawn from the canvases of Kirchner, Munch, Kandinsky, and Nolde: emotionally raw, psychologically intense, and unapologetically bold.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Blood Red** | `#B91C1C` | Primary emotional accent, passion, danger, urgency |
| **Vermillion** | `#DC2626` | Active states, CTAs, intense highlights |
| **Cadmium Yellow** | `#EAB308` | Warmth, anxiety, attention, distortion highlights |
| **Chrome Yellow** | `#FACC15` | Secondary warm accent, illumination |
| **Prussian Blue** | `#1E3A5F` | Deep melancholy, night scenes, somber backgrounds |
| **Cobalt Blue** | `#2563EB` | Cool accent, introspection, contrast to warm |
| **Ultramarine** | `#3730A3` | Deep blue, spiritual depth, dark accents |
| **Viridian** | `#166534` | Organic, nature-as-threat, environmental tension |
| **Sap Green** | `#15803D` | Secondary green, life force, organic accent |
| **Ivory Black** | `#1A1A1A` | Primary dark, outlines, text, grounding |
| **Lamp Black** | `#0D0D0D` | Deepest dark, page backgrounds |
| **Raw Umber** | `#78350F` | Earth tone, aging, decay, textured surfaces |
| **Bone White** | `#FFFBEB` | Light text on dark, highlight areas |
| **Ash** | `#A8A29E` | Muted text, secondary information |
| **Parchment** | `#FEF3C7` | Warm light backgrounds, paper texture tint |

### CSS Custom Properties

```css
:root {
  /* Primaries */
  --expr-blood-red: #b91c1c;
  --expr-vermillion: #dc2626;
  --expr-cadmium-yellow: #eab308;
  --expr-chrome-yellow: #facc15;
  --expr-prussian-blue: #1e3a5f;
  --expr-cobalt-blue: #2563eb;
  --expr-ultramarine: #3730a3;

  /* Organics */
  --expr-viridian: #166534;
  --expr-sap-green: #15803d;
  --expr-raw-umber: #78350f;

  /* Darks */
  --expr-ivory-black: #1a1a1a;
  --expr-lamp-black: #0d0d0d;

  /* Lights */
  --expr-bone-white: #fffbeb;
  --expr-ash: #a8a29e;
  --expr-parchment: #fef3c7;

  /* Text */
  --expr-text-primary: #fffbeb;
  --expr-text-secondary: #a8a29e;
  --expr-text-dark: #1a1a1a;

  /* Backgrounds */
  --expr-bg-dark: #0d0d0d;
  --expr-bg-deep: #1a1a1a;
  --expr-bg-warm: #fef3c7;
}
```

---

## Typography

### Typeface Characteristics

Expressionist typography is:

- **Bold, angular, and emotionally charged** -- letterforms that look carved or brushstroked
- **Irregular and imperfect** -- slightly uneven baselines, varied stroke widths, hand-drawn quality
- **High contrast weight** -- extremely bold headings against regular-weight body text
- **Serif or slab-serif for drama** -- serifs add gravitas and historical weight
- **Display fonts with character** -- condensed, distorted, or woodcut-inspired faces for headlines
- **Readable body text** -- the body must still be legible despite the expressive headings

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Playfair Display** | High-contrast serif, dramatic | Headlines, hero text -- classical drama |
| **Abril Fatface** | Bold display serif | Hero headlines, maximum emotional impact |
| **Oswald** | Condensed sans, bold | Section headings, compressed intensity |
| **Bitter** | Slab serif, sturdy | Body text, grounded readability |
| **Zilla Slab** | Mechanical slab serif | Headlines, structured intensity |
| **DM Serif Display** | Elegant display serif | Headlines, refined drama |
| **Cormorant Garamond** | Classical high-contrast serif | Body text, literary elegance |
| **Libre Baskerville** | Traditional serif, readable | Body text, editorial expressionist pages |
| **Anton** | Condensed, impact-style | Display text, bold statements |
| **Vollkorn** | Organic serif, warm | Body text, warm expressive layouts |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Abril Fatface** (400) | **Libre Baskerville** (400) | Maximum drama meets readable classicism |
| **Playfair Display** (700) | **Bitter** (400) | High-contrast serif meets sturdy slab |
| **Anton** (400) | **Vollkorn** (400) | Condensed impact with warm organic body |
| **Oswald** (600) | **Cormorant Garamond** (400) | Compressed tension with elegant body |
| **Zilla Slab** (700) | **Bitter** (400) | Mechanical intensity, grounded reading |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700;800;900&family=Bitter:wght@400;500;700&display=swap');

h1, h2, h3, h4, h5, h6 {
  font-family: 'Playfair Display', serif;
  font-weight: 800;
  color: var(--expr-text-primary);
  line-height: 1.1;
  letter-spacing: -0.02em;
}

.expr-display {
  font-family: 'Playfair Display', serif;
  font-size: clamp(3rem, 7vw, 6rem);
  font-weight: 900;
  letter-spacing: -0.03em;
  line-height: 0.95;
  text-transform: uppercase;
}

body {
  font-family: 'Bitter', serif;
  font-weight: 400;
  font-size: 1.05rem;
  line-height: 1.75;
  color: var(--expr-text-secondary);
}

.expr-label {
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  font-size: 0.8rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--expr-cadmium-yellow);
}

.expr-caption {
  font-family: 'Bitter', serif;
  font-weight: 400;
  font-size: 0.9rem;
  font-style: italic;
  color: var(--expr-ash);
}
```

---

## Layout Principles

### Grid and Structure

- **Deliberately unbalanced compositions** -- elements are off-center, overlapping, and at varied scales
- **Broken grid layouts** -- columns of unequal width, elements that break out of containers
- **Dramatic scale contrast** -- tiny details next to massive headlines for visual tension
- **Layered elements** -- text over images, shapes overlapping cards, creating depth and collision
- **Dark, weighted backgrounds** -- heavy dark sections anchor the vivid color bursts
- **Irregular spacing** -- vary padding and margins intentionally to create uneven visual rhythm
- **Full-bleed imagery** -- images and textures extend to edges without polite containment

### Section Organization

- **Navigation**: Dark bar with bold serif logo; minimal links with dramatic hover color shifts
- **Hero**: Oversized dramatic headline on dark textured background, vivid accent color slash or stroke
- **Content**: Asymmetric two-column layouts with text and imagery at conflicting scales
- **Gallery/Feature**: Overlapping cards with rough borders, varied sizes, dramatic color backgrounds
- **Quote/Statement**: Large italic text on solid color block, full-width, emotionally charged
- **CTA**: Dark background with vivid red or yellow accent, bold serif headline
- **Footer**: Deepest dark with minimal, muted text

### Responsive Approach

- Single column on mobile with maintained dramatic scale contrasts
- Overlapping elements simplify to stacked on small screens
- Textures and brushstroke effects remain at all sizes for consistent mood
- Typography scale reduces but maintains bold weight contrast
- Color intensity and dark backgrounds work well on all screen sizes

---

## CSS / Design Techniques

### Expressionist Card Component

```css
.expr-card {
  background: var(--expr-bg-deep);
  border: 3px solid var(--expr-ivory-black);
  padding: 32px;
  position: relative;
  transition: transform 0.3s ease;
}

.expr-card:hover {
  transform: rotate(-1deg) translateY(-4px);
}

/* Rough, hand-painted border effect */
.expr-card::before {
  content: '';
  position: absolute;
  inset: -3px;
  border: 3px solid var(--expr-blood-red);
  transform: rotate(0.5deg);
  pointer-events: none;
}

.expr-card--warm {
  background: var(--expr-blood-red);
  color: var(--expr-bone-white);
  border-color: var(--expr-vermillion);
}

.expr-card--cool {
  background: var(--expr-prussian-blue);
  color: var(--expr-bone-white);
  border-color: var(--expr-cobalt-blue);
}
```

### Expressionist Button

```css
.expr-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--expr-blood-red);
  color: var(--expr-bone-white);
  border: 3px solid var(--expr-ivory-black);
  padding: 14px 36px;
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  font-size: 1rem;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  cursor: pointer;
  transition: transform 0.2s ease, background 0.2s ease;
  text-decoration: none;
  position: relative;
}

.expr-button:hover {
  background: var(--expr-vermillion);
  transform: rotate(-1deg) scale(1.02);
}

.expr-button:active {
  transform: rotate(0.5deg) scale(0.98);
}

.expr-button--yellow {
  background: var(--expr-cadmium-yellow);
  color: var(--expr-ivory-black);
}

.expr-button--blue {
  background: var(--expr-prussian-blue);
  color: var(--expr-bone-white);
}

/* Rough edge variant */
.expr-button--raw {
  border: none;
  box-shadow: 4px 4px 0px var(--expr-ivory-black);
}

.expr-button--raw:hover {
  box-shadow: 2px 2px 0px var(--expr-ivory-black);
}
```

### Navigation Bar

```css
.expr-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 24px 40px;
  border-bottom: 3px solid var(--expr-blood-red);
}

.expr-nav__logo {
  font-family: 'Playfair Display', serif;
  font-weight: 900;
  font-size: 1.5rem;
  color: var(--expr-bone-white);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.expr-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.expr-nav__links a {
  font-family: 'Bitter', serif;
  font-weight: 500;
  font-size: 0.95rem;
  color: var(--expr-ash);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  transition: color 0.2s ease;
}

.expr-nav__links a:hover {
  color: var(--expr-cadmium-yellow);
}
```

### Hero Section

```css
.expr-hero {
  min-height: 80vh;
  display: flex;
  align-items: center;
  padding: 80px 40px;
  position: relative;
  overflow: hidden;
  background: var(--expr-bg-dark);
}

.expr-hero::before {
  content: '';
  position: absolute;
  top: -20%;
  right: -10%;
  width: 60%;
  height: 140%;
  background: var(--expr-blood-red);
  transform: rotate(-12deg);
  opacity: 0.15;
}

.expr-hero__content {
  max-width: 700px;
  position: relative;
  z-index: 1;
}

.expr-hero h1 {
  font-size: clamp(3rem, 8vw, 6rem);
  font-weight: 900;
  line-height: 0.95;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
}

.expr-hero h1 .accent {
  color: var(--expr-vermillion);
  display: block;
  transform: rotate(-2deg);
  transform-origin: left;
}

.expr-hero p {
  font-size: 1.15rem;
  margin-bottom: 2.5rem;
  max-width: 500px;
  line-height: 1.8;
}
```

### Textured Background

```css
.expr-texture {
  position: relative;
}

.expr-texture::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.05'/%3E%3C/svg%3E");
  pointer-events: none;
  opacity: 0.4;
}
```

### Dramatic Divider

```css
.expr-divider {
  height: 6px;
  background: var(--expr-blood-red);
  border: none;
  margin: 60px 0;
  transform: rotate(-0.5deg);
}

.expr-divider--yellow {
  background: var(--expr-cadmium-yellow);
}

.expr-divider--brush {
  height: 12px;
  background: linear-gradient(90deg,
    transparent 0%,
    var(--expr-blood-red) 5%,
    var(--expr-blood-red) 30%,
    var(--expr-vermillion) 50%,
    var(--expr-blood-red) 70%,
    var(--expr-blood-red) 95%,
    transparent 100%
  );
  border-radius: 6px;
}
```

---

## Design Do's and Don'ts

### Do

- Use vivid, emotionally charged colors with high contrast
- Apply bold, thick outlines and borders to evoke woodcut print aesthetics
- Let compositions feel deliberately off-balance and asymmetric
- Use serif or slab-serif fonts with dramatic weight contrast
- Add texture and grain to surfaces for a hand-made, painted quality
- Create dramatic scale differences between headings and body text
- Let elements overlap, rotate, and break out of containers
- Design for emotional impact: the viewer should feel something immediately

### Don't

- Use pastel or muted color palettes -- Expressionism demands intensity
- Make layouts symmetrical and perfectly balanced -- tension requires imbalance
- Use lightweight, delicate sans-serif fonts for headings -- they lack the required gravitas
- Polish away all imperfections -- rough edges and visible texture are essential
- Apply minimalist whitespace rules -- Expressionism fills space with drama
- Use flat, shadowless design -- depth and contrast drive the aesthetic
- Ignore readability entirely: body text still needs to be legible despite the expressive context
- Confuse chaos with expression: every "broken" rule should serve an emotional purpose

---

## Related Aesthetics

| Aesthetic | Relationship to Expressionism |
|-----------|------------------------------|
| **Neubrutalism** | Contemporary digital cousin; shares raw edges, bold outlines, and anti-polish attitude |
| **DIY Punk** | Shares handmade, anti-establishment energy; rougher and more collage-oriented |
| **Graffiti Pop** | Shares bold color and urban raw energy; more street-culture and spray-paint influenced |
| **New Wave** | 1980s design movement that channeled expressionist energy through punk and postmodern typography |
| **Art Nouveau** | Historical contrast; organic curves vs. angular distortion, both reject industrial standardization |
| **Art Deco** | Structural opposite; geometric precision and luxury vs. emotional rawness and distortion |
| **Plakatstil** | Early poster art ancestor; bold, flat color and simplified forms but more commercial and restrained |
| **Polish Poster School** | Direct descendant; mid-century poster art that channeled expressionist intensity into cultural commentary |
| **Maximalism** | Shares the more-is-more philosophy; Expressionism focuses emotion while Maximalism embraces abundance |
| **Corporate Grunge** | Shares rough texture and anti-corporate energy but applied to commercial design contexts |
| **Ligne Claire** | Opposite approach; clean, uniform outlines and flat color vs. heavy, varied strokes and raw emotion |
| **Heroic Realism** | Shares dramatic intensity but channels it toward idealized, propagandistic imagery rather than subjective emotion |

---

## Quick-Start: Minimal Expressionism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Expressionism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700;800;900&family=Bitter:wght@400;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --expr-blood-red: #b91c1c;
      --expr-vermillion: #dc2626;
      --expr-cadmium-yellow: #eab308;
      --expr-chrome-yellow: #facc15;
      --expr-prussian-blue: #1e3a5f;
      --expr-cobalt-blue: #2563eb;
      --expr-ultramarine: #3730a3;
      --expr-viridian: #166534;
      --expr-ivory-black: #1a1a1a;
      --expr-lamp-black: #0d0d0d;
      --expr-bone-white: #fffbeb;
      --expr-ash: #a8a29e;
      --expr-parchment: #fef3c7;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--expr-lamp-black);
      color: var(--expr-ash);
      font-family: 'Bitter', serif;
      font-weight: 400;
      font-size: 1.05rem;
      line-height: 1.75;
    }

    h1, h2, h3 {
      font-family: 'Playfair Display', serif;
      font-weight: 800;
      color: var(--expr-bone-white);
      line-height: 1.1;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 24px 40px;
      border-bottom: 3px solid var(--expr-blood-red);
    }

    nav a.logo {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      font-size: 1.5rem;
      color: var(--expr-bone-white);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.05em;
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      color: var(--expr-ash);
      text-decoration: none;
      font-weight: 500;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--expr-cadmium-yellow); }

    /* Hero */
    .hero {
      min-height: 80vh;
      display: flex;
      align-items: center;
      padding: 80px 40px;
      position: relative;
      overflow: hidden;
      max-width: 1200px;
      margin: 0 auto;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: -20%;
      right: -10%;
      width: 50%;
      height: 140%;
      background: var(--expr-blood-red);
      transform: rotate(-12deg);
      opacity: 0.12;
    }

    .hero-content { max-width: 700px; position: relative; z-index: 1; }

    .hero h1 {
      font-size: clamp(3rem, 8vw, 5.5rem);
      font-weight: 900;
      text-transform: uppercase;
      margin-bottom: 1.5rem;
      line-height: 0.95;
    }

    .hero h1 .accent {
      color: var(--expr-vermillion);
      display: block;
      transform: rotate(-2deg);
      transform-origin: left;
    }

    .hero p {
      font-size: 1.15rem;
      margin-bottom: 2.5rem;
      max-width: 500px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      background: var(--expr-blood-red);
      color: var(--expr-bone-white);
      border: 3px solid var(--expr-ivory-black);
      padding: 14px 36px;
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 1rem;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      cursor: pointer;
      text-decoration: none;
      transition: transform 0.2s, background 0.2s;
      box-shadow: 4px 4px 0px var(--expr-ivory-black);
    }

    .btn:hover {
      background: var(--expr-vermillion);
      transform: rotate(-1deg) scale(1.02);
      box-shadow: 2px 2px 0px var(--expr-ivory-black);
    }

    /* Divider */
    .divider {
      height: 6px;
      background: var(--expr-blood-red);
      border: none;
      max-width: 1200px;
      margin: 0 auto;
      transform: rotate(-0.3deg);
    }

    /* Features */
    .features {
      padding: 80px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .features h2 {
      font-size: 2.5rem;
      text-transform: uppercase;
      margin-bottom: 48px;
    }

    .features h2 .yellow { color: var(--expr-cadmium-yellow); }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
    }

    .feature-card {
      background: var(--expr-ivory-black);
      border: 3px solid currentColor;
      padding: 32px;
      position: relative;
      transition: transform 0.3s;
    }

    .feature-card:hover { transform: rotate(-1deg) translateY(-4px); }

    .feature-card:nth-child(1) { color: var(--expr-vermillion); border-color: var(--expr-blood-red); }
    .feature-card:nth-child(2) { color: var(--expr-cobalt-blue); border-color: var(--expr-prussian-blue); }
    .feature-card:nth-child(3) { color: var(--expr-cadmium-yellow); border-color: var(--expr-cadmium-yellow); }

    .feature-card::before {
      content: '';
      position: absolute;
      inset: -3px;
      border: 3px solid currentColor;
      transform: rotate(0.5deg);
      pointer-events: none;
      opacity: 0.3;
    }

    .card-icon {
      width: 48px;
      height: 48px;
      margin-bottom: 20px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .feature-card h3 {
      font-size: 1.3rem;
      margin-bottom: 0.75rem;
      text-transform: uppercase;
      color: var(--expr-bone-white);
    }

    .feature-card p { font-size: 0.95rem; line-height: 1.7; color: var(--expr-ash); }

    /* Quote section */
    .quote {
      background: var(--expr-prussian-blue);
      padding: 80px 40px;
      text-align: center;
    }

    .quote blockquote {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: clamp(1.5rem, 3vw, 2.5rem);
      font-style: italic;
      color: var(--expr-bone-white);
      max-width: 800px;
      margin: 0 auto;
      line-height: 1.3;
    }

    .quote cite {
      display: block;
      margin-top: 24px;
      font-family: 'Bitter', serif;
      font-style: normal;
      font-size: 1rem;
      color: var(--expr-ash);
    }

    /* CTA */
    .cta {
      padding: 80px 40px;
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      gap: 60px;
    }

    .cta-text { flex: 1; }
    .cta h2 { font-size: 2.5rem; text-transform: uppercase; margin-bottom: 1rem; }
    .cta p { margin-bottom: 2rem; max-width: 500px; }

    .cta-visual {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    /* Footer */
    footer {
      border-top: 3px solid var(--expr-blood-red);
      text-align: center;
      padding: 40px;
      font-size: 0.9rem;
      color: var(--expr-ash);
    }

    @media (max-width: 768px) {
      .hero { min-height: 60vh; padding: 60px 20px; }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
      .cta { flex-direction: column; gap: 40px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Sturm</a>
    <ul>
      <li><a href="#">Works</a></li>
      <li><a href="#">Manifesto</a></li>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Feel before<br><span class="accent">you think</span></h1>
      <p>Design that speaks to the gut, not the mind. Raw emotion translated into vivid color, distorted form, and uncompromising visual truth.</p>
      <a href="#" class="btn">Enter the Gallery</a>
    </div>
  </section>

  <hr class="divider">

  <section class="features">
    <h2>The inner <span class="yellow">vision</span></h2>
    <div class="features-grid">
      <div class="feature-card">
        <div class="card-icon">
          <svg width="32" height="32" viewBox="0 0 32 32"><path d="M16 2L4 28h24L16 2z" fill="none" stroke="#dc2626" stroke-width="3" stroke-linejoin="round"/></svg>
        </div>
        <h3>Raw Emotion</h3>
        <p>Every color choice, every distorted form serves the emotional truth of the message. Nothing is decorative; everything is expressive.</p>
      </div>
      <div class="feature-card">
        <div class="card-icon">
          <svg width="32" height="32" viewBox="0 0 32 32"><circle cx="16" cy="16" r="12" fill="none" stroke="#2563eb" stroke-width="3"/><path d="M10 16 L16 10 L22 16 L16 22 Z" fill="none" stroke="#2563eb" stroke-width="2"/></svg>
        </div>
        <h3>Bold Distortion</h3>
        <p>Shapes stretch and break. Typography angles and collides. The viewer is pulled into a world where form follows feeling.</p>
      </div>
      <div class="feature-card">
        <div class="card-icon">
          <svg width="32" height="32" viewBox="0 0 32 32"><rect x="4" y="4" width="24" height="24" fill="none" stroke="#eab308" stroke-width="3" transform="rotate(5 16 16)"/><line x1="4" y1="16" x2="28" y2="16" stroke="#eab308" stroke-width="2"/></svg>
        </div>
        <h3>Vivid Contrast</h3>
        <p>Light crashes against dark. Warm battles cool. The palette is a battlefield where every hue fights for attention.</p>
      </div>
    </div>
  </section>

  <section class="quote">
    <blockquote>"The artist must train not only his eye but also his soul."</blockquote>
    <cite>-- Wassily Kandinsky</cite>
  </section>

  <section class="cta">
    <div class="cta-text">
      <h2>Create with<br>intensity</h2>
      <p>Join a community of artists and designers who believe that great design must first be felt.</p>
      <a href="#" class="btn">Begin Now</a>
    </div>
    <div class="cta-visual">
      <svg width="300" height="300" viewBox="0 0 300 300" fill="none">
        <rect x="40" y="60" width="120" height="180" fill="#b91c1c" transform="rotate(-8 100 150)"/>
        <rect x="100" y="40" width="140" height="160" fill="#1e3a5f" transform="rotate(5 170 120)"/>
        <circle cx="180" cy="200" r="60" fill="#eab308" opacity="0.7"/>
        <line x1="20" y1="280" x2="280" y2="250" stroke="#dc2626" stroke-width="4"/>
        <rect x="200" y="100" width="80" height="120" fill="none" stroke="#fffbeb" stroke-width="3" transform="rotate(-3 240 160)"/>
      </svg>
    </div>
  </section>

  <footer>
    <p>Built with Expressionism principles. Vivid, distorted, emotionally true.</p>
  </footer>
</body>
</html>
```
