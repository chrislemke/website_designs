# Avant Basic

An aesthetic characterized by pastel colors, retro-psychedelic patterns, and a combination of clean and curved lines. It represents maximalism as a deliberate contrast to minimalism, popularized via Instagram and TikTok. The term was coined in December 2020 by Emma Hope Allwood, describing it as "extravagance in the age of mechanical reproduction."

---

## Color Palette

- **Primary palette:** Pastel blues, pinks, greens, and oranges
- **Background tones:** Neutral whites and off-whites
- **Overall feel:** Light hues dominate; colors are soft but saturated enough to feel playful
- **Contrast strategy:** Vibrant pastels placed against clean white or neutral backdrops to let the color pop without becoming overwhelming

### Suggested CSS Color Tokens

| Role            | Description          | Suggested Value     |
|-----------------|----------------------|---------------------|
| Background      | Neutral white        | `#FFFFFF` / `#F8F5F0` |
| Primary         | Pastel pink          | `#F4A7BB` / `#FFB6C1` |
| Secondary       | Pastel blue          | `#A8D8EA` / `#89CFF0` |
| Accent 1        | Pastel green         | `#B5EAD7` / `#98D8AA` |
| Accent 2        | Pastel orange        | `#FFCBA4` / `#FFD3A3` |
| Accent 3        | Pastel lavender      | `#C3B1E1` / `#D4BBFF` |
| Text            | Soft dark            | `#2D2D2D` / `#3A3A3A` |

---

## Typography

- **Lettering style:** Playful, rounded, and organic; avoiding rigid or corporate typefaces
- **Suggested font families:**
  - Display/headings: Rounded sans-serifs (e.g., Nunito, Quicksand, Comfortaa, Fredoka One)
  - Body: Clean sans-serifs with soft geometry (e.g., Poppins, DM Sans, Inter with rounded alternates)
  - Accent/decorative: Retro-inspired or hand-drawn faces for emphasis
- **Weight usage:** Bold and extra-bold for headings; regular or medium for body text
- **Sizing:** Generous and confident; large headings with comfortable line spacing

---

## Visual Characteristics

### Shapes and Forms

- **Curved and rounded elements** are central -- rounded corners, pill shapes, blob forms
- **Wavy and squiggly lines** used as dividers, borders, and decorative accents
- **Organic geometry:** Freeform shapes that feel hand-drawn but structured
- **No sharp edges:** Everything softened; border-radius values are generous

### Patterns and Textures

- **Checkerboard patterns** -- a signature motif, used at various scales
- **Abstract florals** -- natural forms rendered in unnatural/pastel colors
- **Animal prints** -- used sparingly as accent patterns
- **Organic swirls** -- retro-psychedelic flowing forms
- **Geometric patterns** -- Memphis-influenced repeating shapes
- **Gradient washes** -- subtle pastel-to-pastel gradients

### Key Decorative Motifs

- Wiggly/freeform mirror shapes (translate to irregular containers or frames in web design)
- Bubbly, rounded accents
- Statement lighting effects (translate to glows, soft shadows, or highlight effects)
- Gallery-wall layouts with mixed-scale graphic art

---

## Layout Principles

- **Maximalist but organized:** Lots of visual elements, but arranged with intentional rhythm
- **White space as backdrop:** Neutral backgrounds act as a canvas for colorful, patterned elements
- **Mixed scales:** Repeat colors and patterns at different sizes to create visual cohesion
- **Asymmetric balance:** Not rigidly symmetrical; balance achieved through color weight and visual density rather than strict alignment
- **Gallery-wall composition:** Grid-breaking layouts where items are arranged in an organic, curated cluster
- **Layering:** Elements overlap and stack to create depth and visual richness
- **Playful hierarchy:** Important elements are emphasized through color, scale, and shape rather than strict typographic hierarchy alone

---

## CSS / Web Design Techniques

### Border Radius and Soft Shapes

```css
/* Generous rounding on all interactive elements */
.card { border-radius: 24px; }
.button { border-radius: 999px; } /* pill shape */
.container { border-radius: 16px; }
```

### Checkerboard Pattern (CSS)

```css
.checkerboard {
  background-image:
    linear-gradient(45deg, #F4A7BB 25%, transparent 25%),
    linear-gradient(-45deg, #F4A7BB 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, #F4A7BB 75%),
    linear-gradient(-45deg, transparent 75%, #F4A7BB 75%);
  background-size: 40px 40px;
  background-position: 0 0, 0 20px, 20px -20px, -20px 0;
}
```

### Wavy Dividers (SVG/CSS)

```css
.wavy-divider {
  background: url("data:image/svg+xml,...") repeat-x;
  /* Or use clip-path for wavy section edges */
  clip-path: polygon(
    0% 0%, 100% 0%, 100% 85%,
    75% 100%, 50% 85%, 25% 100%, 0% 85%
  );
}
```

### Soft Shadows and Glows

```css
.card {
  box-shadow: 0 8px 32px rgba(244, 167, 187, 0.2);
}
.highlight {
  box-shadow: 0 0 20px rgba(168, 216, 234, 0.4);
}
```

### Blob / Organic Shapes

```css
.blob {
  border-radius: 60% 40% 50% 70% / 50% 60% 40% 60%;
  /* Irregular border-radius creates organic blob forms */
}
```

### Pastel Gradients

```css
.gradient-bg {
  background: linear-gradient(135deg, #A8D8EA 0%, #F4A7BB 50%, #FFCBA4 100%);
}
```

---

## Design Influences

- **Memphis Design** -- the primary visual ancestor; bold geometry, clashing patterns, bright pastels
- **1960s and 1970s design** -- retro color palettes, psychedelic swirls, organic forms
- **Psychedelia** -- flowing, melting shapes; saturated but dreamy color relationships
- **Mid-Century Modern** -- clean structure underlying the maximalist surface layer

---

## Related Aesthetics

- Danish Pastel
- Dopamine (Dopamine Dressing)
- Gen Z Maximalism
- Indie Kid
- Kidcore
- Maximalism
- Memphis Design
- Mid-Century Modern
- Neubrutalism
- Psychedelia
- Vaporwave

---

## Associated Brands and Visual References

- Lisa Says Gah!
- House of Sunny (Day Tripper cardigan, Hockney dress)
- Paloma Wool
- Gimaguas
- Ganni
- Stine Goya
- Baum und Pferdgarten
- Coming Soon (NYC design store)
- Holiday the Label (checkerboard-print pajamas)

---

## Key Design Values

- **Playfulness** -- every element should feel joyful and approachable
- **Maximalism** -- more is more; embrace visual density with intention
- **Kitsch** -- deliberately fun, unserious, and colorful
- **Creativity** -- handmade feel, organic irregularity, anti-corporate sensibility
- **Inclusivity** -- emphasizes work from female, queer, non-binary, and minority-owned businesses
