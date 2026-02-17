# Solarpunk Design Reference

Solarpunk is a utopian green-futures aesthetic that envisions a world where technology and nature coexist in harmony. It blends Art Nouveau curves, living architecture, warm sunlight, and lush botanical technology into a vision of sustainable abundance. Unlike the dystopian warnings of Cyberpunk or the ironic nostalgia of Vaporwave, Solarpunk is earnestly optimistic -- it imagines communities powered by renewable energy, buildings wrapped in climbing plants, and technology that serves ecological well-being. In web design, Solarpunk translates to warm sunlit color palettes, organic curves, botanical illustrations, glass-and-greenery textures, and a design language that feels simultaneously natural and futuristic.

---

## Visual Characteristics

### Core Design Traits

- **Warm golden sunlight** -- amber, honey, and golden yellow tones pervade, suggesting perpetual late-afternoon light
- **Lush green vegetation** -- rich emeralds, sage greens, and botanical motifs are omnipresent, reflecting living architecture
- **Art Nouveau curves** -- flowing, organic lines inspired by Mucha and Gaudi replace rigid geometric grids
- **Living architecture** -- buildings integrated with climbing vines, rooftop gardens, and solar panels
- **Glass and transparency** -- translucent panels, greenhouse structures, and light-filled spaces
- **Botanical illustrations** -- detailed plant drawings, leaf patterns, and floral borders
- **Terracotta and natural materials** -- earth-toned surfaces suggesting clay, wood, and stone
- **Solar and wind motifs** -- sun rays, solar panels, wind turbines, and energy flow diagrams
- **Community and abundance** -- imagery of shared gardens, communal spaces, and cooperative technology
- **Stained glass and mosaic elements** -- colorful translucent panels with organic leading patterns

### Design Principles

- Design with genuine optimism -- Solarpunk is hopeful about the future, not ironic or dystopian
- Blend organic and technological elements seamlessly -- technology should feel like it grew naturally
- Use warm, sunlit color temperatures -- the dominant light source is always the sun
- Embrace curves and flowing lines over rigid grids -- nature does not build in straight lines
- Green is the primary color family, supported by warm golds and earth tones
- Transparency and lightness suggest openness, sustainability, and nothing to hide
- Every design choice should feel sustainable -- avoid excess, embrace elegant sufficiency
- Reference Art Nouveau as the historical foundation, updating it with futuristic optimism
- Community and collaboration are core values -- design should feel welcoming and inclusive

---

## Color Palette

### Sunlit Garden Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Sunbeam Gold** | `#F0A830` | Primary accent, CTAs, energy motifs |
| **Honey Amber** | `#D4922A` | Hover states, warm emphasis |
| **Solar Orange** | `#E8762B` | Secondary warm accent, highlights |
| **Living Green** | `#3A8C3F` | Primary green, success states, botanical accents |
| **Sage** | `#6B9E6B` | Secondary green, softer plant tones |
| **Deep Canopy** | `#1E5631` | Dark green accent, text on light backgrounds |
| **Fresh Leaf** | `#8BC34A` | Bright accent, growth indicators, badges |
| **Sky Blue** | `#5DADE2` | Water motifs, secondary cool accent |
| **Terracotta** | `#C67A4B` | Earth-toned accent, warm surfaces |
| **Warm Cream** | `#FFF9ED` | Primary light background |
| **Sunlit Linen** | `#F5ECD7` | Secondary background, card surfaces |
| **Greenhouse Glass** | `#E8F0E0` | Tinted background, translucent panels |
| **Rich Earth** | `#3E2F23` | Dark text, footer background |
| **Bark Brown** | `#5C4033` | Secondary text, headers on light backgrounds |
| **Warm Gray** | `#8A7E72` | Muted text, captions, borders |

### CSS Custom Properties

```css
:root {
  /* Warm accents */
  --solar-gold: #f0a830;
  --solar-amber: #d4922a;
  --solar-orange: #e8762b;
  --solar-terracotta: #c67a4b;

  /* Greens */
  --solar-green: #3a8c3f;
  --solar-sage: #6b9e6b;
  --solar-canopy: #1e5631;
  --solar-leaf: #8bc34a;

  /* Cool accent */
  --solar-sky: #5dade2;

  /* Backgrounds */
  --solar-bg-cream: #fff9ed;
  --solar-bg-linen: #f5ecd7;
  --solar-bg-glass: #e8f0e0;
  --solar-bg-dark: #3e2f23;

  /* Text */
  --solar-text-dark: #3e2f23;
  --solar-text-brown: #5c4033;
  --solar-text-muted: #8a7e72;
  --solar-text-light: #fff9ed;

  /* Gradients */
  --solar-gradient-sunrise: linear-gradient(135deg, #f0a830 0%, #e8762b 30%, #c67a4b 60%, #3a8c3f 100%);
  --solar-gradient-canopy: linear-gradient(180deg, #e8f0e0 0%, #6b9e6b 50%, #1e5631 100%);
  --solar-gradient-glass: linear-gradient(135deg, rgba(232, 240, 224, 0.8), rgba(255, 249, 237, 0.6));
}
```

---

## Typography

### Typeface Characteristics

Solarpunk typography is:

- **Organic and flowing** -- typefaces that echo Art Nouveau curves and natural growth patterns
- **Warm and readable** -- inviting, friendly faces that encourage extended reading
- **Mix of serif and sans-serif** -- elegant serif headings paired with clean sans-serif body text
- **Slightly rounded** -- soft terminals and curves that avoid harsh mechanical rigidity
- **Medium weights preferred** -- neither too thin (fragile) nor too heavy (industrial)
- **Generous line-height and spacing** -- airy and open, reflecting the abundance of space and light

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Fraunces** | Soft serif, old-style | Headlines, display text, warm editorial |
| **Cormorant Garamond** | Elegant, high-contrast serif | Headlines, refined display text |
| **Lora** | Contemporary serif, brushed curves | Body text, readable long-form content |
| **Nunito** | Rounded sans-serif | Body text, friendly interfaces |
| **Quicksand** | Rounded geometric sans | Subheadings, labels, soft UI elements |
| **Josefin Sans** | Elegant geometric, Art Deco touch | Headlines, navigation, display |
| **DM Serif Display** | Refined serif display | Large headlines, hero text |
| **Atkinson Hyperlegible** | Maximum legibility sans | Body text, accessibility-focused content |
| **Cabin** | Humanist sans, warm | Body text, versatile UI |
| **Merriweather** | Screen-optimized serif | Body text, content-heavy layouts |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Fraunces** (700) | **Nunito** (400) | Warm organic heading, friendly rounded body |
| **DM Serif Display** (400) | **Cabin** (400) | Elegant serif display, humanist sans body |
| **Cormorant Garamond** (600) | **Quicksand** (400) | Art Nouveau elegance, soft geometric body |
| **Josefin Sans** (600) | **Lora** (400) | Clean geometric heading, warm serif body |
| **Fraunces** (700) | **Atkinson Hyperlegible** (400) | Accessible, inclusive, legible at all sizes |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500;9..144,700;9..144,900&family=Nunito:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Fraunces', 'DM Serif Display', serif;
  font-weight: 700;
  color: var(--solar-text-dark);
  line-height: 1.2;
}

/* Display / Hero text */
.solar-display {
  font-family: 'Fraunces', serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 900;
  color: var(--solar-canopy);
  line-height: 1.1;
}

/* Body text */
body {
  font-family: 'Nunito', 'Cabin', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.8;
  color: var(--solar-text-brown);
}

/* Labels and accents */
.solar-label {
  font-family: 'Nunito', sans-serif;
  font-weight: 600;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--solar-text-muted);
}

/* Decorative botanical caption */
.solar-caption {
  font-family: 'Fraunces', serif;
  font-weight: 500;
  font-size: 0.9rem;
  font-style: italic;
  color: var(--solar-sage);
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, medium-width containers** -- max-width 1000-1200px with generous padding, suggesting open garden spaces
- **Organic, curved section transitions** -- use `border-radius`, SVG wave dividers, and curved clip-paths instead of straight horizontal lines
- **Asymmetric, flowing compositions** -- content arranged in organic patterns rather than rigid grids
- **Glass-panel card layouts** -- translucent cards with subtle backdrop blur, suggesting greenhouse walls
- **Botanical border and frame elements** -- leaf patterns, vine lines, and floral corners
- **Warm gradient backgrounds** -- sunrise/sunset gradients that shift from gold to green
- **Generous breathing room** -- ample whitespace representing the abundance and openness of the solarpunk ethos

### Section Organization

- **Navigation**: Clean, light bar with organic logo mark, warm-toned links, leaf or sun icon accents
- **Hero**: Warm gradient or sunlit background with large serif headline, botanical illustration, rounded CTA
- **Features**: Glass-panel cards on a light greenhouse background, plant-themed icons
- **Content rows**: Flowing organic layouts with curved dividers between sections
- **Statistics**: Warm gold numbers with green accents, suggesting growth and abundance
- **Community section**: Warm photography or illustration of gardens, buildings, people
- **CTA section**: Deep green or warm gold background with rounded button
- **Footer**: Rich earth-brown background, organized links, botanical decorations

### Responsive Approach

- Maintain warm, sunlit backgrounds across all breakpoints
- Curved dividers and organic shapes simplify on mobile but retain softness
- Stack content vertically with generous spacing on small screens
- Glass-panel cards maintain translucency but reduce blur for mobile performance
- Typography scales smoothly; serif headings remain prominent at all sizes

---

## CSS / Design Techniques

### Solarpunk Card Component

```css
.solar-card {
  background: rgba(255, 249, 237, 0.75);
  border: 1px solid rgba(107, 158, 107, 0.25);
  border-radius: 16px;
  padding: 32px;
  backdrop-filter: blur(8px);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.solar-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 12px 32px rgba(30, 86, 49, 0.1);
}

/* Leaf accent */
.solar-card__icon {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  background: var(--solar-bg-glass);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 16px;
  font-size: 1.5rem;
}

/* Card grid */
.solar-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
}
```

### Solarpunk Button

```css
.solar-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--solar-green);
  color: #ffffff;
  border: none;
  border-radius: 50px;
  padding: 14px 36px;
  font-family: 'Nunito', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  cursor: pointer;
  transition: all 0.2s ease;
  text-decoration: none;
  box-shadow: 0 4px 12px rgba(58, 140, 63, 0.25);
}

.solar-button:hover {
  background: var(--solar-canopy);
  box-shadow: 0 6px 20px rgba(30, 86, 49, 0.3);
  transform: translateY(-2px);
}

.solar-button:active {
  transform: translateY(0);
  box-shadow: 0 2px 8px rgba(30, 86, 49, 0.2);
}

/* Gold variant */
.solar-button--gold {
  background: var(--solar-gold);
  color: var(--solar-text-dark);
  box-shadow: 0 4px 12px rgba(240, 168, 48, 0.3);
}

.solar-button--gold:hover {
  background: var(--solar-amber);
  box-shadow: 0 6px 20px rgba(212, 146, 42, 0.35);
}

/* Glass variant */
.solar-button--glass {
  background: rgba(255, 249, 237, 0.6);
  color: var(--solar-canopy);
  border: 1px solid rgba(107, 158, 107, 0.3);
  box-shadow: none;
  backdrop-filter: blur(6px);
}

.solar-button--glass:hover {
  background: rgba(255, 249, 237, 0.85);
  box-shadow: 0 4px 12px rgba(30, 86, 49, 0.1);
}
```

### Navigation Bar

```css
.solar-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
}

.solar-nav__logo {
  font-family: 'Fraunces', serif;
  font-weight: 900;
  font-size: 1.4rem;
  color: var(--solar-canopy);
  text-decoration: none;
}

.solar-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.solar-nav__links a {
  font-family: 'Nunito', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  color: var(--solar-text-muted);
  text-decoration: none;
  transition: color 0.2s;
}

.solar-nav__links a:hover {
  color: var(--solar-green);
}

.solar-nav__links a.active {
  color: var(--solar-green);
}
```

### Hero Section

```css
.solar-hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
  gap: 60px;
}

.solar-hero__content {
  flex: 1;
  max-width: 540px;
}

.solar-hero__content h1 {
  font-size: clamp(2.5rem, 5vw, 4rem);
  color: var(--solar-canopy);
  margin-bottom: 1rem;
  line-height: 1.1;
}

.solar-hero__content p {
  font-size: 1.1rem;
  color: var(--solar-text-muted);
  margin-bottom: 2rem;
  line-height: 1.8;
}

.solar-hero__visual {
  flex: 1;
  display: flex;
  justify-content: center;
}

@media (max-width: 768px) {
  .solar-hero {
    flex-direction: column-reverse;
    text-align: center;
    padding: 40px 20px;
    gap: 40px;
  }
}
```

### Curved Section Divider

```css
.solar-wave {
  width: 100%;
  height: 80px;
  overflow: hidden;
  position: relative;
}

.solar-wave svg {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 100%;
}

/* Usage: place between sections */
/* <div class="solar-wave">
  <svg viewBox="0 0 1440 80" preserveAspectRatio="none">
    <path d="M0,40 C360,80 720,0 1440,40 L1440,80 L0,80 Z" fill="#e8f0e0"/>
  </svg>
</div> */
```

### Glass Panel Component

```css
.solar-glass {
  background: rgba(232, 240, 224, 0.5);
  border: 1px solid rgba(107, 158, 107, 0.2);
  border-radius: 20px;
  padding: 40px;
  backdrop-filter: blur(12px);
  box-shadow: 0 8px 32px rgba(30, 86, 49, 0.06);
}
```

### Growth Metric Display

```css
.solar-metric {
  text-align: center;
  padding: 24px;
}

.solar-metric__number {
  font-family: 'Fraunces', serif;
  font-size: 3rem;
  font-weight: 900;
  color: var(--solar-gold);
  line-height: 1.1;
  margin-bottom: 4px;
}

.solar-metric__label {
  font-family: 'Nunito', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--solar-text-muted);
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.solar-metric__trend {
  font-family: 'Nunito', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  color: var(--solar-green);
  margin-top: 4px;
}
```

### Feature Grid with Botanical Icons

```css
.solar-features {
  padding: 80px 0;
}

.solar-features__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 28px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px;
}

.solar-feature {
  text-align: center;
  padding: 32px 24px;
}

.solar-feature__icon {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  background: var(--solar-bg-glass);
  margin: 0 auto 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.75rem;
  border: 1px solid rgba(107, 158, 107, 0.2);
}

.solar-feature h3 {
  font-family: 'Fraunces', serif;
  font-size: 1.15rem;
  font-weight: 700;
  color: var(--solar-text-dark);
  margin-bottom: 0.5rem;
}

.solar-feature p {
  font-size: 0.95rem;
  color: var(--solar-text-muted);
  line-height: 1.7;
}
```

---

## Design Do's and Don'ts

### Do

- Use warm, sunlit color palettes dominated by greens and golds
- Apply organic curves and rounded shapes to cards, buttons, and section dividers
- Include botanical motifs: leaves, vines, flowers, and plant patterns
- Use Art Nouveau as a design reference for curves, borders, and ornamentation
- Create glass-panel effects with `backdrop-filter: blur()` and translucent backgrounds
- Design with genuine optimism and warmth -- this is a hopeful aesthetic
- Reference sustainable technology: solar panels, wind energy, living architecture
- Make typography feel warm and inviting with serif headings and rounded sans-serif body text

### Don't

- Use cold, clinical color palettes -- avoid sterile blues, grays, and stark whites
- Apply rigid, mechanical grid layouts -- Solarpunk favors organic flow
- Use dark, dystopian backgrounds -- the dominant mood is light, warm, and sunlit
- Include industrial or corporate imagery that suggests exploitation or pollution
- Use angular, harsh typefaces -- nothing should feel aggressive or mechanical
- Over-decorate with Art Nouveau flourishes to the point of visual clutter
- Forget functionality -- Solarpunk values practical sustainability, not just decoration
- Mix in neon or electric lighting effects -- the light source is the sun, not LEDs

---

## Related Aesthetics

| Aesthetic | Relationship to Solarpunk |
|-----------|--------------------------|
| **Art Nouveau** | Primary historical influence; Solarpunk inherits its flowing organic curves, botanical motifs, and integration of art with function |
| **Cottagecore** | Shares the pastoral, nature-positive values; Cottagecore is nostalgic and rural, Solarpunk is futuristic and urban-green |
| **Cyberpunk** | Philosophical opposite; both imagine technology-rich futures, but Cyberpunk is dystopian while Solarpunk is utopian |
| **Biophilic Design** | Architectural sibling; both integrate living plants into built environments and prioritize human-nature connection |
| **Scandinavian Design** | Shares values of functionality, sustainability, and clean living; Scandinavian is minimalist, Solarpunk is more ornamental |
| **Studio Ghibli** | Shares the warm, nature-harmonious, hopeful worldview; Ghibli's visual language is a direct aesthetic cousin |
| **Lunarpunk** | Sister aesthetic; applies Solarpunk values with a nocturnal, bioluminescent, and mystical twist |
| **Goblincore** | Shares appreciation for nature but celebrates the messy, decomposing, mushroom-and-moss side rather than curated gardens |
| **Arts and Crafts** | Historical parallel; both reject industrialism in favor of handmade quality and natural materials |

---

## Quick-Start: Minimal Solarpunk Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Solarpunk Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500;9..144,700;9..144,900&family=Nunito:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --solar-gold: #f0a830;
      --solar-amber: #d4922a;
      --solar-orange: #e8762b;
      --solar-green: #3a8c3f;
      --solar-sage: #6b9e6b;
      --solar-canopy: #1e5631;
      --solar-leaf: #8bc34a;
      --solar-sky: #5dade2;
      --solar-terracotta: #c67a4b;
      --solar-bg-cream: #fff9ed;
      --solar-bg-linen: #f5ecd7;
      --solar-bg-glass: #e8f0e0;
      --solar-bg-dark: #3e2f23;
      --solar-text-dark: #3e2f23;
      --solar-text-brown: #5c4033;
      --solar-text-muted: #8a7e72;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--solar-bg-cream);
      color: var(--solar-text-brown);
      font-family: 'Nunito', sans-serif;
      font-size: 1rem;
      line-height: 1.8;
    }

    h1, h2, h3 {
      font-family: 'Fraunces', serif;
      font-weight: 700;
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
    }

    nav a.logo {
      font-family: 'Fraunces', serif;
      font-weight: 900;
      font-size: 1.3rem;
      color: var(--solar-canopy);
      text-decoration: none;
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'Nunito', sans-serif;
      font-weight: 600;
      font-size: 0.9rem;
      color: var(--solar-text-muted);
      text-decoration: none;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--solar-green); }

    /* Hero */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 80px 40px;
      gap: 60px;
    }

    .hero-content { flex: 1; max-width: 540px; }

    .hero h1 {
      font-size: clamp(2.5rem, 5vw, 4rem);
      color: var(--solar-canopy);
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.1rem;
      color: var(--solar-text-muted);
      margin-bottom: 2rem;
    }

    .hero-visual {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    .btn {
      display: inline-block;
      background: var(--solar-green);
      color: #fff;
      border: none;
      border-radius: 50px;
      padding: 14px 36px;
      font-family: 'Nunito', sans-serif;
      font-weight: 600;
      font-size: 0.95rem;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 0 4px 12px rgba(58, 140, 63, 0.25);
      transition: all 0.2s;
    }

    .btn:hover {
      background: var(--solar-canopy);
      box-shadow: 0 6px 20px rgba(30, 86, 49, 0.3);
      transform: translateY(-2px);
    }

    /* Wave divider */
    .wave {
      width: 100%;
      overflow: hidden;
      line-height: 0;
    }

    .wave svg { width: 100%; height: 60px; }

    /* Features */
    .features {
      padding: 60px 0 80px;
      background: var(--solar-bg-glass);
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--solar-text-dark);
      margin-bottom: 8px;
    }

    .features .subtitle {
      text-align: center;
      font-size: 0.9rem;
      color: var(--solar-text-muted);
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: rgba(255, 249, 237, 0.75);
      border: 1px solid rgba(107, 158, 107, 0.2);
      border-radius: 16px;
      padding: 32px;
      text-align: center;
      backdrop-filter: blur(6px);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .feature:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 24px rgba(30, 86, 49, 0.08);
    }

    .feature-icon {
      width: 56px;
      height: 56px;
      border-radius: 50%;
      background: var(--solar-bg-glass);
      border: 1px solid rgba(107, 158, 107, 0.2);
      margin: 0 auto 16px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
    }

    .feature h3 { font-size: 1.1rem; margin-bottom: 0.5rem; color: var(--solar-canopy); }
    .feature p { color: var(--solar-text-muted); font-size: 0.95rem; }

    /* CTA */
    .cta {
      background: var(--solar-canopy);
      text-align: center;
      padding: 80px 40px;
    }

    .cta h2 {
      font-size: 2rem;
      color: var(--solar-gold);
      margin-bottom: 1rem;
    }

    .cta p {
      color: rgba(255, 249, 237, 0.8);
      font-size: 1.05rem;
      margin-bottom: 2rem;
    }

    .cta .btn {
      background: var(--solar-gold);
      color: var(--solar-bg-dark);
      box-shadow: 0 4px 12px rgba(240, 168, 48, 0.3);
    }

    .cta .btn:hover {
      background: var(--solar-amber);
    }

    /* Footer */
    footer {
      background: var(--solar-bg-dark);
      text-align: center;
      padding: 30px 40px;
      color: var(--solar-text-muted);
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .hero {
        flex-direction: column-reverse;
        text-align: center;
        padding: 40px 20px;
        gap: 40px;
      }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Luminos</a>
    <ul>
      <li><a href="#">Gardens</a></li>
      <li><a href="#">Energy</a></li>
      <li><a href="#">Community</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Growing futures, together</h1>
      <p>Sustainable technology rooted in community. We build living systems that power neighborhoods, nourish ecosystems, and brighten every day.</p>
      <a href="#" class="btn">Explore</a>
    </div>
    <div class="hero-visual">
      <svg width="400" height="320" viewBox="0 0 400 320" fill="none" xmlns="http://www.w3.org/2000/svg">
        <!-- Building with plants -->
        <rect x="120" y="80" width="160" height="200" rx="8" fill="#e8f0e0" stroke="#6b9e6b" stroke-width="2"/>
        <!-- Windows -->
        <rect x="140" y="100" width="40" height="30" rx="4" fill="#fff9ed" stroke="#8a7e72" stroke-width="1"/>
        <rect x="220" y="100" width="40" height="30" rx="4" fill="#fff9ed" stroke="#8a7e72" stroke-width="1"/>
        <rect x="140" y="150" width="40" height="30" rx="4" fill="#fff9ed" stroke="#8a7e72" stroke-width="1"/>
        <rect x="220" y="150" width="40" height="30" rx="4" fill="#fff9ed" stroke="#8a7e72" stroke-width="1"/>
        <!-- Solar panels on roof -->
        <rect x="130" y="65" width="55" height="15" rx="2" fill="#5dade2" stroke="#3a8c3f" stroke-width="1"/>
        <rect x="215" y="65" width="55" height="15" rx="2" fill="#5dade2" stroke="#3a8c3f" stroke-width="1"/>
        <!-- Climbing vines -->
        <path d="M120 280 Q115 240 125 200 Q120 160 130 120" stroke="#3a8c3f" stroke-width="3" fill="none"/>
        <circle cx="125" cy="200" r="6" fill="#8bc34a"/>
        <circle cx="130" cy="160" r="5" fill="#6b9e6b"/>
        <circle cx="125" cy="130" r="4" fill="#8bc34a"/>
        <!-- Ground garden -->
        <ellipse cx="200" cy="290" rx="160" ry="15" fill="#6b9e6b" opacity="0.3"/>
        <!-- Sun -->
        <circle cx="330" cy="50" r="30" fill="#f0a830" opacity="0.4"/>
        <circle cx="330" cy="50" r="20" fill="#f0a830" opacity="0.6"/>
        <!-- Trees -->
        <circle cx="60" cy="240" r="25" fill="#3a8c3f" opacity="0.5"/>
        <rect x="57" y="260" width="6" height="25" rx="2" fill="#5c4033" opacity="0.5"/>
        <circle cx="340" cy="230" r="20" fill="#6b9e6b" opacity="0.5"/>
        <rect x="337" y="245" width="6" height="30" rx="2" fill="#5c4033" opacity="0.5"/>
      </svg>
    </div>
  </section>

  <div class="wave">
    <svg viewBox="0 0 1440 60" preserveAspectRatio="none">
      <path d="M0,30 C240,60 480,0 720,30 C960,60 1200,0 1440,30 L1440,60 L0,60 Z" fill="#e8f0e0"/>
    </svg>
  </div>

  <section class="features">
    <h2>What we cultivate</h2>
    <p class="subtitle">Technology that grows with the world, not against it</p>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon">&#127793;</div>
        <h3>Living Rooftops</h3>
        <p>Transform unused rooftop space into thriving gardens that feed communities and cool buildings naturally.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#9728;&#65039;</div>
        <h3>Solar Commons</h3>
        <p>Community-owned solar arrays that distribute clean energy equitably across neighborhoods.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#127795;</div>
        <h3>Urban Forests</h3>
        <p>Dense pocket forests planted using Miyawaki method, creating biodiversity hotspots in city centers.</p>
      </div>
    </div>
  </section>

  <div class="wave" style="transform: scaleY(-1);">
    <svg viewBox="0 0 1440 60" preserveAspectRatio="none">
      <path d="M0,30 C240,60 480,0 720,30 C960,60 1200,0 1440,30 L1440,60 L0,60 Z" fill="#e8f0e0"/>
    </svg>
  </div>

  <section class="cta">
    <h2>Join the garden</h2>
    <p>Every seed planted is a vote for the future we want. Start growing with us today.</p>
    <a href="#" class="btn">Get started</a>
  </section>

  <footer>
    <p>Luminos Collective -- Building solarpunk futures since 2024</p>
  </footer>
</body>
</html>
```
