---
name: Obsidian Portfolio System
colors:
  surface: '#051424'
  surface-dim: '#051424'
  surface-bright: '#2c3a4c'
  surface-container-lowest: '#010f1f'
  surface-container-low: '#0d1c2d'
  surface-container: '#122131'
  surface-container-high: '#1c2b3c'
  surface-container-highest: '#273647'
  on-surface: '#d4e4fa'
  on-surface-variant: '#c6c6cd'
  inverse-surface: '#d4e4fa'
  inverse-on-surface: '#233143'
  outline: '#909097'
  outline-variant: '#46464c'
  surface-tint: '#c0c6de'
  primary: '#c0c6de'
  on-primary: '#2a3043'
  primary-container: '#020617'
  on-primary-container: '#72778d'
  inverse-primary: '#585e73'
  secondary: '#bec6e0'
  on-secondary: '#283044'
  secondary-container: '#3f465c'
  on-secondary-container: '#adb4ce'
  tertiary: '#c0c1ff'
  on-tertiary: '#1000a9'
  tertiary-container: '#01002e'
  on-tertiary-container: '#6467f2'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dce1fb'
  primary-fixed-dim: '#c0c6de'
  on-primary-fixed: '#151b2d'
  on-primary-fixed-variant: '#40465a'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#e1e0ff'
  tertiary-fixed-dim: '#c0c1ff'
  on-tertiary-fixed: '#07006c'
  on-tertiary-fixed-variant: '#2f2ebe'
  background: '#051424'
  on-background: '#d4e4fa'
  surface-variant: '#273647'
typography:
  display-xl:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.75'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-max: 1280px
  gutter: 2rem
  margin-mobile: 1rem
  stack-sm: 0.5rem
  stack-md: 1.5rem
  stack-lg: 4rem
  section-padding: 8rem
---

## Brand & Style

The design system is rooted in **Minimalism** with a **Corporate/Modern** technical edge. It is tailored for high-end professional portfolios, emphasizing precision, technical mastery, and content clarity. The aesthetic prioritizes deep, monochromatic foundations paired with high-energy accents to guide the eye toward key achievements and calls to action.

The emotional response should be one of quiet confidence—professional, focused, and premium. By utilizing expansive whitespace (or "dark space") and a strict adherence to a grid, the system allows the user's work to take center stage without visual clutter.

## Colors

This design system utilizes a tiered dark-mode hierarchy to create depth without relying on heavy shadows.

- **Primary (#020617):** The "Rich Black" base for page backgrounds.
- **Secondary (#0f172a):** The "Deep Slate" used for surface containers, cards, and section blocks.
- **Tertiary (#6366f1):** A "Refined Violet" used sparingly for interactive states, high-contrast buttons, and focus indicators.
- **Neutral (#94a3b8):** A muted slate used for secondary text, borders, and icons to maintain a low-friction visual experience.
- **Foreground:** Pure white (#ffffff) is reserved for primary headings, while (#e2e8f0) is used for standard body text to reduce eye strain.

## Typography

The typography system is built on **Inter** for its neutral, highly legible characteristics. For technical labels and metadata, **Geist** is introduced to provide a subtle developer-centric feel.

Generous line heights (1.6 to 1.75) are mandatory for body text to ensure readability against the dark background. Display and Headline styles use tighter letter spacing and heavier weights to create a commanding presence. Section headers should use the `label-sm` style with increased letter spacing to clearly demarcate content transitions.

## Layout & Spacing

The design system employs a **Fixed Grid** model for desktop, centered within the viewport.

- **Grid:** A 12-column grid with a 32px (2rem) gutter.
- **Sectioning:** Content sections are separated by significant vertical rhythm (`section-padding`) to create a gallery-like experience. 
- **Mobile Adaptivity:** On mobile devices, the 12-column grid collapses to a single-column layout with 16px margins. 
- **Consistency:** Use the `stack` variables for vertical spacing between elements within a component (e.g., `stack-sm` between a label and a title, `stack-md` between a title and description).

## Elevation & Depth

This design system rejects traditional heavy shadows in favor of **Tonal Layers** and **Low-contrast Outlines**.

1.  **Base Layer:** The deepest value (#020617) defines the global background.
2.  **Surface Layer:** Cards and containers use the secondary color (#0f172a).
3.  **Borders:** Rather than shadows, depth is defined by a 1px solid border (#1e293b) on all containers.
4.  **Interaction Depth:** Upon hover, borders transition to the tertiary violet (#6366f1) or a lighter slate (#334155), and the background may subtly brighten.

## Shapes

The shape language is "Soft" and controlled. Elements use a 0.25rem (4px) base radius to maintain a professional, architectural feel. 

- **Buttons & Tags:** Use `rounded-lg` (8px) to provide a tactile point of interaction.
- **Cards:** Use the base `rounded` (4px) or `rounded-lg` (8px) depending on size.
- **Media/Images:** Always match the container roundedness to maintain alignment.

## Components

### Buttons
- **Primary:** High-contrast background (#6366f1) with white text. No shadow; sharp transitions.
- **Secondary:** Transparent background with a 1px border (#334155). Text in white.
- **Tertiary/Ghost:** No background or border; text uses the tertiary color.

### Cards
- **Style:** Background (#0f172a), 1px border (#1e293b), 8px corner radius.
- **Spacing:** 2rem internal padding.
- **Hover:** Border color shifts to violet (#6366f1); slight Y-axis translation (-4px).

### Chips/Tags
- **Style:** Small, `label-sm` typography, background (#1e293b), rounded-full. Used for skill listing and project categories.

### Inputs
- **Style:** Dark fill (#020617), subtle border (#334155). Focus state triggers a 1px violet border and a soft violet outer glow (0px 0px 0px 2px).

### Section Headers
- **Composition:** A `label-sm` category name in violet, followed by a `headline-md` title in white, underlined by a 2px thick, short horizontal rule (32px wide).