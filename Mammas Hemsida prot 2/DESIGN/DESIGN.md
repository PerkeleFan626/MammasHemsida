---
name: Split Kawaii
colors:
  surface: '#fdf7ff'
  surface-dim: '#ded8e0'
  surface-bright: '#fdf7ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f8f2fa'
  surface-container: '#f2ecf4'
  surface-container-high: '#ece6ee'
  surface-container-highest: '#e6e0e9'
  on-surface: '#1d1b20'
  on-surface-variant: '#494551'
  inverse-surface: '#322f35'
  inverse-on-surface: '#f5eff7'
  outline: '#7a7582'
  outline-variant: '#cbc4d2'
  surface-tint: '#6750a4'
  primary: '#4f378a'
  on-primary: '#ffffff'
  primary-container: '#6750a4'
  on-primary-container: '#e0d2ff'
  inverse-primary: '#cfbcff'
  secondary: '#63597c'
  on-secondary: '#ffffff'
  secondary-container: '#e1d4fd'
  on-secondary-container: '#645a7d'
  tertiary: '#765b00'
  on-tertiary: '#ffffff'
  tertiary-container: '#c9a74d'
  on-tertiary-container: '#503d00'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#cfbcff'
  on-primary-fixed: '#22005d'
  on-primary-fixed-variant: '#4f378a'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#cdc0e9'
  on-secondary-fixed: '#1f1635'
  on-secondary-fixed-variant: '#4b4263'
  tertiary-fixed: '#ffdf93'
  tertiary-fixed-dim: '#e7c365'
  on-tertiary-fixed: '#241a00'
  on-tertiary-fixed-variant: '#594400'
  background: '#fdf7ff'
  on-background: '#1d1b20'
  surface-variant: '#e6e0e9'
typography:
  headline-xl:
    fontFamily: Spline Sans
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Spline Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.6'
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 16px
  margin: 24px
---

## Brand & Style

This design system centers on a dualistic aesthetic narrative, bridging the gap between "mischievous gothic" and "soft sweetness." It is designed for high-engagement social and lifestyle platforms catering to an audience that values expressive, character-driven interfaces. The emotional response is one of playful nostalgia combined with modern, high-fidelity polish.

The style is a hybrid of **Glassmorphism** and **Tactile Modernism**. The dark theme utilizes depth through translucent layers and vibrant gradients, while the light theme employs soft, voluminous surfaces. Both themes are unified by a "sparkle" motif—micro-interactions and decorative elements that shimmer, ensuring the UI feels alive and reactive.

## Colors

The color palette is anchored by a unified bright pink accent that bridges the two distinct themes. 

**Theme 1 (Kuromi):** A "Night-Mode" palette built on deep purple gradients. It uses high-saturation hot pinks for interactive states and black for structural grounding. Sparkle effects should be rendered in white or neon pink to pop against the dark background.

**Theme 2 (My Melody):** A "Day-Mode" palette characterized by low-contrast pastel pinks and pure white surfaces. It prioritizes legibility and a "cloud-like" feel, using soft pinks for secondary information rather than harsh greys.

## Typography

This design system uses a typographic "handshake" between two distinct typefaces to mirror the dual themes. 

**Spline Sans** is utilized for headlines and primary headers. In the dark theme, it should lean into its "Bold" and "Black" weights to provide an energetic, rebellious punch. **Plus Jakarta Sans** serves as the body and UI font, providing a soft, rounded, and welcoming feel that excels in the light theme and remains highly legible in the dark theme. Use tight letter spacing for large headlines and generous line heights for body text to maintain a modern, breathable UI.

## Layout & Spacing

The layout follows a 12-column fluid grid system with generous outer margins to emphasize the "card-based" nature of the content. Spacing is governed by an 8px base unit, but decorative elements (like sparkles and ribbons) are allowed to break the grid, overlapping container edges to create a sense of depth and playfulness. 

Container padding should be oversized—typically `md` (24px) or higher—to ensure that the rounded corners do not clip content and to maintain the "clean" aesthetic requested.

## Elevation & Depth

Hierarchy is handled differently across the two themes to maximize the strengths of each palette:

- **The Light Theme (My Melody)** uses **Ambient Shadows**. Shadows are tinted with a hint of pink (#FF4FA3 at 10-15% opacity) and feature large blur radii to make white cards appear as if they are floating softly over the pastel background.
- **The Dark Theme (Kuromi)** uses **Tonal Layers & Glassmorphism**. Depth is achieved through semi-transparent dark surfaces (Background Blur: 20px) and thin, high-contrast inner borders (1px) that mimic a neon or glass edge. 

In both themes, the "Sparkle" iconography sits at the highest Z-index, often accompanied by a small outer glow to simulate light emission.

## Shapes

The shape language is dominated by soft, organic curves. Primary containers use `rounded-lg` (1rem), while smaller interactive elements like buttons and chips utilize `rounded-full` (pill-shaped) for a friendly, approachable feel. 

Unique to this design system are "Decorative Corner Overlays." Certain cards should feature a small ribbon or heart-shaped notch in the top-right or top-left corner, reinforcing the character-driven inspiration without compromising the clean UI layout.

## Components

### Buttons
Buttons are pill-shaped. In the Kuromi theme, use a dark-to-purple gradient with a hot pink "inner glow" on hover. In the My Melody theme, use solid bright pink with a soft shadow. Use heart icons as prefix or suffix elements.

### Cards
Cards are the primary container. Light theme cards are pure white with soft, tinted shadows. Dark theme cards are semi-transparent purple with a 1px border of #FF4FA3 at 30% opacity.

### Input Fields
Inputs should be highly rounded (pill-style). The focus state is a 2px bright pink border accompanied by a subtle sparkle icon appearing at the end of the field.

### Chips & Tags
Small, pill-shaped elements. Use ribbons or star icons within the chip to denote special categories.

### Checkboxes & Radios
Standard checkboxes are replaced by heart-shaped toggles. When selected, the heart fills with the unified accent pink and triggers a micro-animation of "sparkles" bursting outward.

### Lists
List items are separated by generous spacing rather than divider lines. Hover states involve a slight scale-up effect (1.02x) and a soft glow, making the list feel tactile and responsive.