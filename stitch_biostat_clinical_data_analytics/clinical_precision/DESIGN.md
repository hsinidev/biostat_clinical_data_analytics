---
name: Clinical Precision
colors:
  surface: '#f7f9fe'
  surface-dim: '#d8dade'
  surface-bright: '#f7f9fe'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f8'
  surface-container: '#eceef2'
  surface-container-high: '#e6e8ed'
  surface-container-highest: '#e0e2e7'
  on-surface: '#191c1f'
  on-surface-variant: '#424752'
  inverse-surface: '#2d3134'
  inverse-on-surface: '#eff1f5'
  outline: '#727783'
  outline-variant: '#c2c6d4'
  surface-tint: '#005db6'
  primary: '#00478d'
  on-primary: '#ffffff'
  primary-container: '#005eb8'
  on-primary-container: '#c8daff'
  inverse-primary: '#a9c7ff'
  secondary: '#5d5e5f'
  on-secondary: '#ffffff'
  secondary-container: '#e0dfdf'
  on-secondary-container: '#626363'
  tertiary: '#244971'
  on-tertiary: '#ffffff'
  tertiary-container: '#3e618b'
  on-tertiary-container: '#c3dbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d6e3ff'
  primary-fixed-dim: '#a9c7ff'
  on-primary-fixed: '#001b3d'
  on-primary-fixed-variant: '#00468c'
  secondary-fixed: '#e3e2e2'
  secondary-fixed-dim: '#c6c6c6'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#464747'
  tertiary-fixed: '#d2e4ff'
  tertiary-fixed-dim: '#a6c9f8'
  on-tertiary-fixed: '#001c37'
  on-tertiary-fixed-variant: '#244871'
  background: '#f7f9fe'
  on-background: '#191c1f'
  surface-variant: '#e0e2e7'
typography:
  h1:
    fontFamily: Public Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  h2:
    fontFamily: Public Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  h3:
    fontFamily: Public Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: '0'
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: '0'
  data-tabular:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
    letterSpacing: 0.01em
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
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
  container-max: 1440px
---

## Brand & Style

The brand personality of this design system is authoritative, sterile, and hyper-logical. It is designed for high-stakes environments where data integrity and clarity are non-negotiable, such as clinical trial monitoring and regulatory auditing. The UI must evoke a sense of absolute reliability and medical-grade accuracy.

The visual style follows a **Corporate/Modern** approach with a heavy emphasis on structural functionalism. It prioritizes information density without sacrificing legibility. By utilizing a "clean-room" aesthetic, the design system removes all unnecessary decorative flourishes, ensuring that the user's cognitive load is dedicated entirely to data analysis and compliance workflows.

## Colors

The color palette is derived from clinical and laboratory environments. **Laboratory Blue** serves as the primary action color, signaling professionalism and trust. **Sterile White** is the foundational background color to maintain a high-contrast, clean environment. **Silver** and neutral greys are used for structural elements, borders, and secondary information.

Functional colors (Success, Warning, Error) must follow international medical standards: a precise emerald for success, a technical amber for warnings, and a high-visibility crimson for critical errors. This ensures that alerts are immediately distinguishable from the primary blue brand accents.

## Typography

This design system utilizes a dual-font approach to balance institutional authority with technical utility. **Public Sans** is used for headings and top-level navigation to provide an accessible, official tone. **Inter** is the primary typeface for all technical data, body copy, and interface labels due to its exceptional legibility in high-density layouts and its "tall" x-height which aids in reading long strings of alphanumeric clinical data.

Tabular data should always utilize Inter with tabular lining figures to ensure vertical alignment of numerical values across rows.

## Layout & Spacing

The layout is built on a **12-column fluid grid** with a strict 4px baseline rhythm. This ensures that every element—from the height of an input field to the padding within a data cell—is mathematically consistent. 

A high-density information layout is achieved by using the `sm` (8px) unit for internal component padding, while `lg` (24px) units are reserved for external margins to provide "breathing room" between major logical sections. This intentional use of whitespace prevents the technical data from feeling overwhelming while maintaining a compact, professional footprint.

## Elevation & Depth

To maintain a sterile and clinical aesthetic, this design system avoids heavy, organic shadows. Instead, it utilizes **low-contrast outlines** and **tonal layers** to define hierarchy.

1.  **Level 0 (Base):** Sterile White (#FFFFFF) background.
2.  **Level 1 (Containers):** Defined by a 1px solid Silver (#C0C0C0) border. No shadow.
3.  **Level 2 (Interactive/Floating):** A subtle, highly diffused shadow (0px 4px 12px rgba(0, 0, 0, 0.05)) is permitted only for temporary elements like dropdown menus or tooltips to lift them slightly from the analytical plane.
4.  **Emphasis:** Section headers use a subtle grey fill (#F8F9FA) to ground the information within a white container.

## Shapes

The shape language is conservative and precise. A **Soft (0.25rem)** border radius is applied to buttons, input fields, and containers. This slight rounding prevents the UI from feeling aggressive while maintaining a sharp, professional edge that aligns with medical equipment interfaces. Smaller components like tags or status indicators should maintain this same radius for system-wide cohesion.

## Components

### Buttons
Primary buttons use Laboratory Blue with white text. Secondary buttons use a Silver border with Laboratory Blue text. All buttons have a fixed height of 36px for a compact, technical feel.

### Data Tables
Tables are the core component of the design system. They feature 1px Silver horizontal dividers, no vertical lines, and a subtle hover state (#F8F9FA). Column headers use the `label-caps` typography style for clear distinction from data.

### Input Fields
Inputs are rectangular with 1px Silver borders. Focus states transition the border to Laboratory Blue with a 1px inset glow. Labels are always persistent; placeholder text should only be used for formatting examples.

### Medical-Grade Iconography
Icons must be "outline" style with a consistent 1.5px stroke weight. They should be literal and functional (e.g., a microscope for "Analysis," a document for "Protocol," a shield for "Compliance").

### Status Chips
Chips use a de-saturated background of the status color (e.g., light green) with a high-contrast dark text of the same hue. They are used for trial status (e.g., "Active," "Recruiting," "Completed").

### Clinical Cards
Analytical modules are housed in cards with 1px Silver borders and 16px internal padding. They should always have a clear title bar to separate metadata from the primary data visualization or content.