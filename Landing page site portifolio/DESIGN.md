---
name: Obsidian Flux
colors:
  surface: '#13121b'
  surface-dim: '#13121b'
  surface-bright: '#393842'
  surface-container-lowest: '#0e0d16'
  surface-container-low: '#1b1b24'
  surface-container: '#201f28'
  surface-container-high: '#2a2932'
  surface-container-highest: '#35343d'
  on-surface: '#e5e0ed'
  on-surface-variant: '#c8c4d7'
  inverse-surface: '#e5e0ed'
  inverse-on-surface: '#312f39'
  outline: '#928ea1'
  outline-variant: '#474555'
  surface-tint: '#c5c0ff'
  primary: '#c5c0ff'
  on-primary: '#2600a1'
  primary-container: '#6d5ef7'
  on-primary-container: '#fffeff'
  inverse-primary: '#5543de'
  secondary: '#5de6ff'
  on-secondary: '#00363e'
  secondary-container: '#00cbe6'
  on-secondary-container: '#00515d'
  tertiary: '#ffb785'
  on-tertiary: '#502500'
  tertiary-container: '#b85d00'
  on-tertiary-container: '#fffeff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e4dfff'
  primary-fixed-dim: '#c5c0ff'
  on-primary-fixed: '#140067'
  on-primary-fixed-variant: '#3c23c6'
  secondary-fixed: '#a2eeff'
  secondary-fixed-dim: '#2fd9f4'
  on-secondary-fixed: '#001f25'
  on-secondary-fixed-variant: '#004e5a'
  tertiary-fixed: '#ffdcc6'
  tertiary-fixed-dim: '#ffb785'
  on-tertiary-fixed: '#301400'
  on-tertiary-fixed-variant: '#713700'
  background: '#13121b'
  on-background: '#e5e0ed'
  surface-variant: '#35343d'
typography:
  display-xl:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: '800'
    lineHeight: 72px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
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
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  code-snippet:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 22px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 0.5rem
  sm: 1rem
  md: 1.5rem
  lg: 2.5rem
  xl: 4rem
  container-max: 1200px
  gutter: 24px
---

## Brand & Style

The design system is engineered for a high-end personal portfolio that balances technical rigor with creative fluidity. It targets tech-forward recruiters and fellow engineers, evoking an emotional response of competence, precision, and modern sophistication.

The aesthetic leans heavily into **Modern Minimalism** with a **Tech-Focused** edge, drawing inspiration from industry leaders like Vercel and Stripe. The visual language utilizes vast negative space to frame code snippets and projects as artifacts. Interactivity is key: every surface should feel reactive through subtle micro-interactions, utilizing backdrop filters and high-performance transitions to imply a "state-of-the-art" development environment.

## Colors

The palette is strictly dark-mode, rooted in a deep, void-like blue (`#0B0F1A`) to ensure high contrast for the neon-inspired accents. 

- **Primary Accent (#6D5EF7):** Used for primary calls-to-action, active states, and brand-critical highlights.
- **Secondary Accent (#22D3EE):** Used for technical callouts, "success" indicators, and secondary data visualizations.
- **Surface Strategy:** Backgrounds transition from the base void to `#111827` for elevated containers. Text hierarchy is maintained through a stark white for headers and a muted zinc for descriptions, ensuring readability without eye strain in low-light environments.

## Typography

This design system utilizes **Inter** for all UI and prose elements to maintain a neutral, systematic appearance that doesn't distract from the content. **JetBrains Mono** is introduced for labels, badges, and code blocks to reinforce the developer-centric narrative.

Large headings should use "Tight" or "Tighter" letter spacing to create a dense, impactful visual weight. Body text uses a generous line height (1.5x) to ensure long-form project case studies are easily digestible. Use semantic weighting: bold for clarity in headers and medium for labels.

## Layout & Spacing

The layout follows a **Fixed-Fluid hybrid grid**. Content is centered within a 1200px max-width container for desktop, utilizing a 12-column grid. 

- **Desktop:** 12 columns / 24px gutters / 80px margins.
- **Tablet:** 8 columns / 16px gutters / 40px margins.
- **Mobile:** 4 columns / 16px gutters / 20px margins.

Spacing follows an 8pt rhythm, emphasizing "breathing room" around project cards and section transitions. Vertical rhythm is expansive; sections should be separated by `xl` spacing units to allow the glassmorphism effects to stand out against the dark background.

## Elevation & Depth

Hierarchy is achieved through **Glassmorphism** and **Tonal Layering**. Instead of heavy shadows, depth is communicated through:

1.  **Backdrop Blurs:** High-level floating elements (like Navbars or Modals) use `backdrop-filter: blur(12px)` with a semi-transparent `background-secondary` fill.
2.  **Inner Glows:** Use a 1px solid top-border (white, 10% opacity) on cards to simulate a "rim light" effect from above.
3.  **Soft Shadows:** Use large, diffused shadows with low opacity (`rgba(0, 0, 0, 0.5)`) and a slight color tint matching the primary accent for active elements.
4.  **Gradient Borders:** High-priority cards use a subtle linear gradient border (Primary to Secondary accent) at 15% opacity to separate from the background.

## Shapes

The design system utilizes **Rounded (0.5rem)** as the base radius. This provides a modern, approachable feel while maintaining the structural integrity of a technical product. 

- **Standard Elements:** 0.5rem (Buttons, Input fields).
- **Cards/Containers:** 1rem (rounded-lg) to soften large surface areas.
- **Badges/Chips:** 1.5rem (rounded-xl) or Pill-shaped to distinguish them as discrete interactive meta-data.

## Components

### Buttons
- **Primary:** Solid `#6D5EF7` with white text. Hover state: slight scale up (1.02x) and an outer glow.
- **Secondary:** Outline variant with a 1px border of `border_subtle`. Hover state: background fills with `rgba(255, 255, 255, 0.05)`.
- **Tertiary:** Text-only with an arrow icon. Interaction: Arrow slides 4px to the right on hover.

### Glass Cards
Project cards feature a subtle `1px` border. On hover, the border opacity increases, and the `backdrop-blur` intensifies. Content inside uses `text_secondary` for metadata and `text_primary` for titles.

### Skill Badges
Small, pill-shaped containers using `JetBrains Mono`. Background is a 10% opacity tint of the secondary accent (`#22D3EE`), with the text in the full-saturation accent color.

### Inputs
Dark backgrounds (`#0B0F1A`) with a subtle border. Focus state: border color changes to the primary accent with a soft 2px outer glow.

### Interactive Patterns
- **Hover States:** All interactive elements must have a transition-duration of `200ms` with a `cubic-bezier(0.4, 0, 0.2, 1)` easing.
- **Scroll Reveals:** Sections should fade in and slide up slightly as they enter the viewport to reinforce the premium, polished feel.