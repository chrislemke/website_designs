# Avantropop

**Named by:** Evan Collins
**Term origin:** Portmanteau of "avant-garde" and "electropop"
**Alternative name:** Avant Garde Prefuse
**Era:** Late 2000s -- mid 2010s

Avantropop refers to a graphic design style of Recession Pop, seen in media during the late 2000s and early 2010s, such as the "Noods" (2008--2010) and "CHECK it" (2010--2016) eras of Cartoon Network. It blends avant-garde graphic sensibilities with the glossy futurism of electropop music culture. The overall feel is high-energy, experimental, optimistic yet edgy -- sleek digital simplicity combined with vivid, neon-saturated compositions.

---

## Visual Characteristics

- Asymmetrical geometric shapes and diagonal lines dominate compositions
- CMYK color palettes with soft gradients
- Triangular and square patterns; colorful polygonal designs
- Vector-based graphics as the foundational technique
- Striped patterns, commonly in black and white
- Abstract digital overlays and neon backdrops
- High-contrast, eye-catching color combinations
- Smooth gradient transitions between vibrant hues
- Glossy, futuristic surfaces and textures
- Dynamic visual flow prioritized over rigid grids

---

## Color Palette

### Primary Neon Colors

| Color   | Suggested Hex | Role                    |
|---------|---------------|-------------------------|
| Magenta | `#FF00FF`     | Primary accent          |
| Purple  | `#9B30FF`     | Primary accent          |
| Red     | `#FF2D55`     | Primary accent          |
| Blue    | `#007AFF`     | Primary accent          |
| Green   | `#00FF7F`     | Primary accent          |
| Yellow  | `#FFFF00`     | Primary accent          |
| Orange  | `#FF8C00`     | Secondary accent        |

### Supporting Neutrals

| Color | Suggested Hex | Role              |
|-------|---------------|-------------------|
| Black | `#000000`     | Background / text |
| White | `#FFFFFF`     | Background / text |

### Palette Principles

- Neon-saturated hues at full intensity
- High contrast between neon accents and dark or white backgrounds
- CMYK-inspired combinations (cyan, magenta, yellow, key/black)
- Soft gradients blending two or more neon colors together
- Use black and white for structure; neon for energy

---

## Typography

| Typeface               | Role           | Notes                                                             |
|------------------------|----------------|-------------------------------------------------------------------|
| ITC Avant Garde Gothic | Primary        | Geometric, modern letterforms; clean lines; futuristic appeal     |
| Lot                    | Display / Alt  | Used for variety in headlines and display contexts                 |
| Val                    | Display / Alt  | Used for variety in headlines and display contexts                 |

### Typographic Principles

- Geometric sans-serif letterforms
- Clean lines, even stroke weights
- Futuristic and modern feel
- Bold weights for headlines; regular/light for body
- Uppercase or title case for maximum graphic impact
- Letter-spacing can be expanded for display use

---

## Key Design Elements and Motifs

1. **Asymmetrical geometric shapes** -- triangles, squares, polygons placed off-grid for dynamic tension
2. **Diagonal lines** -- create movement, energy, and directional flow across the composition
3. **Soft gradients** -- smooth color transitions between neon hues (e.g., magenta to blue, green to yellow)
4. **Vector graphics** -- clean, scalable shapes with hard edges and flat fills
5. **Black-and-white stripes** -- structural contrast element used alongside neon color
6. **Neon glow effects** -- subtle outer glows or bloom on text and shapes
7. **Polygonal patterns** -- tessellated triangles or faceted surfaces as background textures
8. **Abstract digital overlays** -- layered transparent shapes, light leaks, or bokeh-style circles
9. **CMYK registration marks and print artifacts** -- used decoratively as design accents
10. **Colorblocking** -- large areas of flat, saturated color placed adjacent for maximum impact

---

## Layout Principles

- **Asymmetrical composition** over centered or symmetric layouts
- **Diagonal axes** as primary compositional structure (elements tilted 15--45 degrees)
- **Overlapping layers** of shapes, text, and imagery create depth
- **Dynamic visual flow** -- the eye moves along diagonal lines and color transitions rather than a standard grid
- **Generous use of whitespace** (or blackspace on dark backgrounds) to let neon elements breathe
- **Off-center focal points** for visual tension
- **Mixed scale** -- large shapes or type juxtaposed with small geometric details
- **Foreground/background interplay** using transparency and gradients

---

## CSS / Design Techniques

### Gradients

```css
/* Neon gradient backgrounds */
background: linear-gradient(135deg, #FF00FF, #007AFF);
background: linear-gradient(45deg, #00FF7F, #FFFF00);
```

### Neon Glow Effects

```css
/* Neon text glow */
text-shadow:
  0 0 7px #FF00FF,
  0 0 10px #FF00FF,
  0 0 21px #FF00FF,
  0 0 42px #FF00FF;

/* Neon box glow */
box-shadow:
  0 0 5px rgba(255, 0, 255, 0.5),
  0 0 20px rgba(255, 0, 255, 0.3);
```

### Diagonal Lines and Skewed Elements

```css
/* Diagonal stripe background */
background: repeating-linear-gradient(
  45deg,
  #000 0px,
  #000 10px,
  #FFF 10px,
  #FFF 20px
);

/* Skewed container for diagonal energy */
transform: skewY(-5deg);
```

### Geometric Shapes with CSS

```css
/* Triangle using clip-path */
clip-path: polygon(50% 0%, 0% 100%, 100% 100%);

/* Polygonal clipping */
clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
```

### Colorblocking

```css
/* Large flat color areas */
.block-magenta { background: #FF00FF; }
.block-blue    { background: #007AFF; }
.block-green   { background: #00FF7F; }
```

### Transparency and Overlays

```css
/* Semi-transparent overlay shapes */
background: rgba(255, 0, 255, 0.3);
mix-blend-mode: screen;
```

### Vector / SVG Styling

```css
/* Clean vector shapes */
svg { fill: #FF00FF; stroke: none; }
svg:hover { filter: drop-shadow(0 0 10px #FF00FF); }
```

### Dark Background Base

```css
/* Dark base for neon contrast */
body {
  background: #0A0A0A;
  color: #FFFFFF;
  font-family: 'ITC Avant Garde Gothic', 'Avant Garde', 'Century Gothic', sans-serif;
}
```

---

## Fashion Elements

- Neon-colored accessories
- Geometric prints on clothing
- Digital and holographic textures
- Electropop-inspired streetwear
- Leggings with bold patterns
- Graphic tees with vector artwork
- Colorblocked pieces
- Futuristic metallic fabrics and finishes

---

## Media and Cultural References

### Television Branding

- Cartoon Network "Noods" era (2008--2010)
- Cartoon Network "CHECK it" era (2010--2016)
- Cartoon Network "Let's Go!/Prefuse" bumpers
- Boomerang Latin American branding (2010--2014)
- Nickelodeon Kids' Choice Awards 2010 graphics
- Big Brother (UK) Series 17 set design and icons
- MTV Acesso opening graphics

### Music

- m-flo album "COSMICOLOR" (2007)
- Electropop and dance-pop music videos with neon backdrops, vector overlays, and abstract digital shapes

### Other Media

- Malhacao season 18 opening (2010--2011)
- Gatchaman Crowds (2013)
- Funky Panda wallpaper (2013, combined with Superflat Pop)
- Tech product advertising, mobile carrier branding, app store graphics
- Youth-oriented social platform design

---

## Related Aesthetics

- Avant-garde
- Bright Tertiaries
- Dark Aero
- Flat Design
- Frutiger Aero
- Internet Awesomesauce
- McBling
- Memphis Design
- Memphis Lite
- Monochrome Luxe
- Shibuya Punk
- Superflat Pop
- UrBling
- Vectordelia
- Y2K Futurism
