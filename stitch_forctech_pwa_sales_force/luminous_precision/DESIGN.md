---
name: Luminous Precision
colors:
  surface: '#111317'
  surface-dim: '#111317'
  surface-bright: '#37393e'
  surface-container-lowest: '#0c0e12'
  surface-container-low: '#1a1c20'
  surface-container: '#1e2024'
  surface-container-high: '#282a2e'
  surface-container-highest: '#333539'
  on-surface: '#e2e2e8'
  on-surface-variant: '#bac9cc'
  inverse-surface: '#e2e2e8'
  inverse-on-surface: '#2f3035'
  outline: '#849396'
  outline-variant: '#3b494c'
  surface-tint: '#00daf3'
  primary: '#c3f5ff'
  on-primary: '#00363d'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#006875'
  secondary: '#b6c4ff'
  on-secondary: '#002780'
  secondary-container: '#0050ee'
  on-secondary-container: '#d4dbff'
  tertiary: '#ffeac0'
  on-tertiary: '#3e2e00'
  tertiary-container: '#fec931'
  on-tertiary-container: '#6f5500'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#dce1ff'
  secondary-fixed-dim: '#b6c4ff'
  on-secondary-fixed: '#001550'
  on-secondary-fixed-variant: '#003ab3'
  tertiary-fixed: '#ffdf96'
  tertiary-fixed-dim: '#f3bf26'
  on-tertiary-fixed: '#251a00'
  on-tertiary-fixed-variant: '#594400'
  background: '#111317'
  on-background: '#e2e2e8'
  surface-variant: '#333539'
typography:
  headline-lg:
    fontFamily: Outfit
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Outfit
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Outfit
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  headline-lg-mobile:
    fontFamily: Outfit
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 20px
---

## Brand & Style

The design system is engineered for high-performance sales professionals who require speed, clarity, and a sense of "technological edge" while in the field. The brand personality is authoritative yet frictionless, combining the depth of a premium dark-mode interface with the tactical feedback of modern interaction design.

The aesthetic merges **Glassmorphism** for information hierarchy and **Neomorphism** for interactive affordance. Semi-transparent, blurred layers signify secondary data surfaces, while soft, extruded shapes identify actionable touchpoints. This hybrid approach creates a UI that feels both physically present and digitally sophisticated. The emotional response is one of confidence, precision, and futuristic efficiency.

## Colors

The palette is anchored in a deep "Obsidian" neutral foundation to maximize contrast and reduce eye strain during extended field use. 

- **Primary & Secondary:** A vibrant "Electric Cyan" to "Deep Cobalt" gradient is used exclusively for primary actions, progress indicators, and brand-critical moments.
- **Surface Logic:** Dark surfaces use subtle tonal shifts rather than pure black to maintain depth. `surface_dark` is for the base canvas, while `surface_light` is for raised neomorphic containers.
- **Functional Colors:** Status colors are high-chroma to ensure immediate recognition against the dark background.
- **Glass Effects:** Overlays utilize a 40% opacity of the neutral palette with a high saturation boost to prevent a "muddy" appearance.

## Typography

This design system employs a dual-font strategy. **Outfit** is used for headlines to provide a modern, geometric character that feels premium and tech-forward. **Inter** is utilized for all body copy and UI labels to ensure maximum legibility and functional clarity in data-dense sales environments.

Maintain tight tracking on larger headlines to emphasize the "bold" brand character. For small labels and captions, increase letter spacing slightly to prevent character blurring on low-brightness mobile screens.

## Layout & Spacing

This design system follows a 4px soft-grid system to ensure mathematical harmony across all components. 

- **Mobile Philosophy:** As a mobile-first PWA, the layout prioritizes the "thumb-zone." Interactive elements are clustered in the lower two-thirds of the screen.
- **Safe Areas:** A 20px horizontal margin is mandatory for all primary content containers.
- **Grids:** Use a 4-column fluid grid for mobile. Elements should snap to the grid, but internal component padding should remain generous (16px minimum) to maintain the "airy" feel of glassmorphism.
- **Vertical Rhythm:** Use the `md` (16px) unit as the standard separator between logical content blocks.

## Elevation & Depth

Depth is conveyed through a sophisticated layering system:

1.  **Level 0 (Background):** `neutral_color_hex` (#0F1115).
2.  **Level 1 (Neomorphic Base):** Uses `surface_dark` with two shadows. A "light" shadow (top-left) at 10% opacity white and a "dark" shadow (bottom-right) at 40% opacity black. This creates an extruded, tactile look for physical buttons and static cards.
3.  **Level 2 (Glass Overlays):** Used for modals, navigation bars, and floating action buttons. These use a backdrop-blur of 12px–20px and a 1px semi-transparent border (top and left edges only) to simulate a light-catching glass edge.
4.  **Interaction:** Upon press, neomorphic elements should transition from "extruded" to "inset" using internal shadows, while glass elements should slightly scale down (98%) and increase blur intensity.

## Shapes

The design system uses **Rounded (0.5rem / 8px)** as the base radius. This provides a balance between the precision of professional software and the approachability of modern mobile apps.

- **Standard Elements:** 8px radius (Cards, Input fields).
- **Large Elements:** 16px radius (Modals, Bottom sheets).
- **Pill Elements:** 100px radius (Search bars, Chips, Primary action buttons).
- **Borders:** Glass elements must feature a 1px stroke at 15% white opacity to define their boundaries against complex backgrounds.

## Components

### Buttons
- **Primary:** High-vibrancy gradient background. No shadow, but a subtle outer glow using the primary color at 20% opacity. Scale down on tap.
- **Secondary (Neomorphic):** Match the surface color with extruded shadows. Text uses the primary color.
- **Tertiary:** Ghost style with glass stroke.

### Input Fields
- **Style:** Inset neomorphic wells. The "sunken" look clearly distinguishes them from "raised" buttons. 
- **Focus State:** 1px border using the primary gradient.

### Cards & Panels
- **Data Cards:** Neomorphic (raised).
- **Contextual Overlays:** Glassmorphic (blurred background).

### Chips
- Small, pill-shaped elements with a subtle glass blur and a 1px border. Used for filtering sales leads or status tags.

### Feedback Elements
- **Haptics:** Every button press should trigger a light haptic tap to reinforce the tactile visual style.
- **Loading:** A shimmering "glass-sweep" skeleton loader that moves diagonally across the cards.