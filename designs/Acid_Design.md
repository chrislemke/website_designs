# Acid Design

A visual aesthetic rooted in 1990s Acid House and rave flyer art, revived in mid-2010s
Instagram design communities. It expresses visual dissonance and confusion to convey
subjective emotions and unique, individualized identity. The mood is anti-utopian or
dystopian, reflecting contemporary anxieties and digital culture with ironic, darkly
humorous, or cynical perspectives.

---

## Color Palette

- **Primary base:** Dark / black backgrounds
- **Accent colors:** Highly saturated neon and fluorescent colors layered over the dark base
- **Core technique -- "Colorful Black":** Use black as the dominant background color so that saturated, fluorescent accent colors appear significantly more vibrant through contrast
- **Suggested neon accents for web implementation:**
  - Electric green: `#39FF14`
  - Hot magenta / neon pink: `#FF00FF` or `#FF1493`
  - Acid yellow: `#CCFF00` or `#DFFF00`
  - Cyan / electric blue: `#00FFFF` or `#0FF0FC`
  - Neon orange: `#FF6600`
  - Ultraviolet purple: `#BF00FF`
- **Background:** Near-black or pure black (`#000000`, `#0A0A0A`, `#111111`)
- **Avoid:** Pastels, muted tones, earth tones, or large expanses of white

## Typography

- **Letterform style:** Experimental, geometric, jagged, and distorted
- **Surface treatment:** Chrome, liquid metal, and iridescent textures applied to type
- **Overall feel:** Futuristic and tactile -- text should look like it has physical materiality
- **Implementation techniques:**
  - Use bold, condensed, or display typefaces with angular geometry
  - Apply CSS `background-clip: text` with metallic or gradient fills
  - Use `text-shadow` with neon glow colors (multiple layered shadows for bloom effect)
  - Consider SVG filters for chrome / distortion effects
  - Animate text with subtle glitch, flicker, or warp effects
- **Example CSS glow effect:**
  ```css
  .acid-text {
    color: #39FF14;
    text-shadow:
      0 0 7px #39FF14,
      0 0 10px #39FF14,
      0 0 21px #39FF14,
      0 0 42px #0fa,
      0 0 82px #0fa;
  }
  ```

## Key Design Elements and Motifs

- **Psychedelic and Op-Art patterns:** Checkerboards, warped stripes, moire patterns, spiral distortions
- **Wireframe models:** 3D wireframe globes, geometric solids, grid planes receding into perspective
- **Chrome and liquid metal surfaces:** Reflective, mercurial textures on text and shapes
- **Glass and plastic renderings:** Translucent, refractive materials with specular highlights
- **Laser effects:** Sharp beams of colored light cutting across compositions
- **Smiley faces:** The iconic 90s rave smiley, often distorted or deconstructed
- **World globes:** Rendered as wireframes or with technological overlays
- **Technological symbols:** Circuit-like patterns, data visualization motifs, HUD-style overlays

## Composition and Layout Principles

- **Horror vacui (fear of empty space):** Fill the entire composition; avoid large areas of negative space
- **Dense, layered arrangements:** Elements should overlap and stack, appearing random or chaotic but creating continuous visual flow
- **Fragmented geometric patterns:** Break layouts into angular, overlapping sections rather than clean grids
- **Dynamic disorder:** The composition should feel energetic and restless, not calm or orderly
- **Overlapping elements:** Text over images, shapes over text, layers upon layers
- **Implementation approach:**
  - Use CSS Grid or absolute positioning for overlapping element placement
  - Apply `mix-blend-mode` (screen, overlay, difference) for layered color interactions
  - Use `clip-path` with polygon values for angular, fragmented sections
  - Apply `transform: rotate()` and `skew()` to break rigid alignment
  - Use `z-index` stacking to create depth through overlapping layers

## Textures and Surface Effects

- **Chrome / metallic:** Linear gradients alternating between white, gray, and dark gray simulate reflective metal
  ```css
  .chrome {
    background: linear-gradient(
      135deg,
      #333 0%, #fff 10%, #333 20%,
      #fff 30%, #666 40%, #fff 50%,
      #333 60%, #fff 70%, #333 80%,
      #fff 90%, #333 100%
    );
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  ```
- **Iridescent / holographic:** Use `hue-rotate` animations on gradient backgrounds for color-shifting effects
  ```css
  .iridescent {
    background: linear-gradient(135deg, #ff00ff, #00ffff, #ff00ff, #ffff00);
    background-size: 400% 400%;
    animation: holo-shift 3s ease infinite;
  }
  @keyframes holo-shift {
    0% { background-position: 0% 50%; filter: hue-rotate(0deg); }
    50% { background-position: 100% 50%; filter: hue-rotate(45deg); }
    100% { background-position: 0% 50%; filter: hue-rotate(0deg); }
  }
  ```
- **Noise / grain:** Overlay SVG noise filters or CSS pseudo-elements with repeating grain textures to add analog texture
- **Scanlines:** Thin repeating horizontal lines via `repeating-linear-gradient` to simulate CRT displays

## Animation and Motion

- **Glitch effects:** Rapid, short-duration shifts in position, color channels, or clip regions
- **Flicker:** Intermittent opacity changes on text or decorative elements
- **Rotation and drift:** Slow, continuous rotation on geometric decorative elements
- **Distortion waves:** CSS or SVG filter-based displacement effects
- **Scrolling patterns:** Infinite scrolling background patterns using `@keyframes` with `background-position` or `transform: translate()`

## CSS Techniques Summary

| Technique | CSS Property / Approach |
|-----------|------------------------|
| Neon glow | Multiple `text-shadow` or `box-shadow` with same-hue colors at increasing blur |
| Chrome text | `background-clip: text` with metallic linear gradient |
| Overlapping layout | CSS Grid with overlapping `grid-row` / `grid-column`, or absolute positioning |
| Color blending | `mix-blend-mode: screen`, `difference`, `overlay` |
| Angular clipping | `clip-path: polygon(...)` |
| Warped patterns | SVG `feTurbulence` + `feDisplacementMap` filters |
| Scanlines | `repeating-linear-gradient(0deg, transparent, transparent 2px, rgba(0,0,0,0.3) 2px, rgba(0,0,0,0.3) 4px)` |
| Noise grain | SVG filter with `feTurbulence` as overlay |
| Holographic shift | Animated `hue-rotate` filter on gradient background |
| Geometric rotation | `transform: rotate()` with `animation` |

## Notable Designers and Influences

- **David Rudnick** -- typographic and identity work with distorted, chrome-treated letterforms
- **Jonathan Castro** -- dense, layered compositions with rave and cyberpunk motifs
- **GUCCIMAZE** -- jagged, angular custom typography with metallic textures
- **Origin era:** 1990s Acid House and rave flyer art
- **Revival:** Mid-2010s Instagram design communities

## Related Aesthetics

- Acid House
- Barber Beats
- Cyberdelia
- Cyberpunk
- Neo-Vectorheart
- Neubrutalism
- New Beat
- Psychedelia
- Rave
- Retrofuturism
- Vectorheart
- Y2K Futurism
