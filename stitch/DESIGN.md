---
name: Precision Ops
colors:
  surface: '#faf8ff'
  surface-dim: '#d2d9f4'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f3ff'
  surface-container: '#eaedff'
  surface-container-high: '#e2e7ff'
  surface-container-highest: '#dae2fd'
  on-surface: '#131b2e'
  on-surface-variant: '#434654'
  inverse-surface: '#283044'
  inverse-on-surface: '#eef0ff'
  outline: '#737685'
  outline-variant: '#c3c6d6'
  surface-tint: '#0c56d0'
  primary: '#003d9b'
  on-primary: '#ffffff'
  primary-container: '#0052cc'
  on-primary-container: '#c4d2ff'
  inverse-primary: '#b2c5ff'
  secondary: '#505f76'
  on-secondary: '#ffffff'
  secondary-container: '#d0e1fb'
  on-secondary-container: '#54647a'
  tertiary: '#7b2600'
  on-tertiary: '#ffffff'
  tertiary-container: '#a33500'
  on-tertiary-container: '#ffc6b2'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b2c5ff'
  on-primary-fixed: '#001848'
  on-primary-fixed-variant: '#0040a2'
  secondary-fixed: '#d3e4fe'
  secondary-fixed-dim: '#b7c8e1'
  on-secondary-fixed: '#0b1c30'
  on-secondary-fixed-variant: '#38485d'
  tertiary-fixed: '#ffdbcf'
  tertiary-fixed-dim: '#ffb59b'
  on-tertiary-fixed: '#380d00'
  on-tertiary-fixed-variant: '#812800'
  background: '#faf8ff'
  on-background: '#131b2e'
  surface-variant: '#dae2fd'
typography:
  display:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin: 24px
---

## Brand & Style

This design system is engineered for high-stakes operational environments where clarity and efficiency are paramount. The brand personality is **authoritative, analytical, and resilient**. It avoids decorative fluff in favor of a **Corporate Modern** aesthetic with **Industrial** undertones, ensuring that users can process dense information without cognitive fatigue.

The visual language communicates reliability through structured alignment, high-density data views, and a "mechanical" precision. Every element exists to serve a functional purpose, evoking the feeling of a sophisticated control room or a high-performance flight deck.

## Colors

The palette is anchored by **Deep Slate Grays** and **Ink Navy** to provide a grounded, professional foundation. 

- **Primary (Professional Blue):** Reserved strictly for primary actions, active states, and critical wayfinding. It is high-contrast against white to ensure immediate recognition.
- **Secondary (Slate):** Used for metadata, icons, and secondary information hierarchies to prevent visual clutter.
- **Surface Strategy:** The system utilizes a "layered white" approach. The base background is a very light cool gray (`#F8FAFC`), while active work surfaces and cards are pure white (`#FFFFFF`) to create subtle but clear separation.
- **Status Tints:** Success, Warning, and Error colors use desaturated backgrounds with high-chroma text for legibility within data grids.

## Typography

The system utilizes **Inter** for its exceptional legibility and neutral tone. It is optimized for high-density screens where small font sizes must remain crisp.

- **Scale:** A tight typographic scale is used to maximize information density. 14px is the standard body size, while 13px is used for dense data tables.
- **Technical Accents:** **JetBrains Mono** is introduced for IDs, timestamps, and coordinates to provide a distinct "data" feel and ensure character alignment in columns.
- **Rhythm:** Line heights are kept tight (1.2x to 1.5x) to maintain the industrial, compact aesthetic.

## Layout & Spacing

The design system employs a **4px baseline grid** for rigid vertical rhythm. 

- **Grid System:** A 12-column fluid grid is used for main dashboards, but internal workspaces often utilize a **Fixed Sidebar + Fluid Content** model.
- **Density:** High-density spacing is the default. Gutters are kept at a strict 16px to allow more data columns to be visible simultaneously.
- **Breakpoints:**
  - **Desktop (1440px+):** Full multi-pane view with persistent sidebars.
  - **Tablet (768px - 1439px):** Collapsed sidebars (icons only), transition to stacked card views for data rows.
  - **Mobile:** Minimalist view focusing on critical status alerts and single-column lists.

## Elevation & Depth

This design system prioritizes **Low-contrast outlines** over heavy shadows to maintain a clean, "flat-industrial" look. 

- **Depth Levels:**
  - **Level 0 (Base):** Background surface (`#F8FAFC`).
  - **Level 1 (Card/Surface):** Pure white with a 1px border (`#E2E8F0`). No shadow.
  - **Level 2 (Dropdown/Popover):** Pure white with a subtle 4px blur, 5% opacity black shadow to differentiate from the work surface.
- **Interactive States:** Hovering over a clickable row or card should change the background to a subtle blue-tinted gray (`#F1F5F9`) rather than raising its elevation.

## Shapes

The shape language is **Soft (0.25rem)**. This provides just enough curvature to feel modern and accessible while maintaining the structural integrity of an industrial tool. 

- **Standard Radius:** 4px (Buttons, Inputs, Checkboxes).
- **Large Radius:** 8px (Cards, Modals).
- **Interactive Elements:** Strict rectangular forms are avoided to ensure hit areas are visually distinct from the background grid lines.

## Components

- **Buttons:** Primary buttons use a solid `#0052CC` fill. Secondary buttons use a white fill with a `#E2E8F0` border. Text is always bold and centered.
- **Input Fields:** Robust 1px borders. Active states use a 2px Primary Blue border. Labels are always persistent (never placeholder-only) and set in `body-sm`.
- **Status Indicators (Chips):** Small, rectangular badges with 2px border-radius. Use a semantic color background at 10% opacity with 100% opacity text (e.g., Success = Light Green BG / Dark Green Text).
- **Data Tables:** The core of the system. Rows have 1px bottom borders only. Header cells use `label-caps` typography with a subtle slate background.
- **Action Bars:** Persistent toolbars at the top of data modules containing filters, search, and bulk actions, separated by a vertical divider.
- **Lists:** High-density vertical stacks with clear dividers. Each list item should have a defined "active" state using a left-hand 4px primary-colored accent bar.