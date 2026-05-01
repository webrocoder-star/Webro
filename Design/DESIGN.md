---
name: Kinetic Noir
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1b1b1b'
  surface-container: '#1f1f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#c7c4d7'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#303030'
  outline: '#908fa0'
  outline-variant: '#464554'
  surface-tint: '#c0c1ff'
  primary: '#c0c1ff'
  on-primary: '#1000a9'
  primary-container: '#8083ff'
  on-primary-container: '#0d0096'
  inverse-primary: '#494bd6'
  secondary: '#ffa9fd'
  on-secondary: '#590061'
  secondary-container: '#7f0f89'
  on-secondary-container: '#fd90ff'
  tertiary: '#c2c6d3'
  on-tertiary: '#2c313a'
  tertiary-container: '#8c919c'
  on-tertiary-container: '#252a33'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#07006c'
  on-primary-fixed-variant: '#2f2ebe'
  secondary-fixed: '#ffd6fa'
  secondary-fixed-dim: '#ffa9fd'
  on-secondary-fixed: '#37003c'
  on-secondary-fixed-variant: '#7c0986'
  tertiary-fixed: '#dee2ef'
  tertiary-fixed-dim: '#c2c6d3'
  on-tertiary-fixed: '#171c25'
  on-tertiary-fixed-variant: '#424751'
  background: '#131313'
  on-background: '#e2e2e2'
  surface-variant: '#353535'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1440px
  gutter: 24px
  margin-x: 64px
  stack-sm: 16px
  stack-md: 32px
  stack-lg: 80px
---

## Brand & Style

The brand personality is defined by technical precision and high-end sophistication. This design system targets elite tech enterprises and innovative startups, evoking an emotional response of trust, luxury, and "next-generation" capability. 

The aesthetic is a hybrid of **Minimalism** and **Glassmorphism**. It utilizes a deep, nocturnal foundation to allow content to emerge through translucent layers and luminous accents. Motion is not an afterthought but a core structural element—transitions should be fluid, utilizing easing functions that mimic organic physics to reinforce a premium, high-touch feel.

## Colors

The palette is anchored in a sophisticated "True Black" (#000000) to ensure maximum contrast and visual depth. The primary Indigo (#6366F1) serves as the digital heartbeat of the UI, used for interactive states and primary brand signals. The secondary Magenta (#86198F) is reserved for high-impact accents and subtle gradient stops.

Neutral tones leverage the off-white lavender (#EEF2FF) for secondary text and borders, creating a softer alternative to pure white that feels more intentional and premium. Gradients should be used sparingly, primarily as background "auras" or soft glows behind glass layers.

## Typography

This design system employs a dual-font strategy to balance technical innovation with readability. **Space Grotesk** is used for headlines; its geometric and slightly unconventional letterforms signal a cutting-edge tech focus. Negative letter-spacing is applied to larger display sizes to create a compact, high-impact editorial feel.

**Manrope** handles all body and functional text. Its modern, refined proportions ensure legibility across dense technical specifications and long-form agency manifestos. Labels and micro-copy utilize uppercase Manrope with generous tracking to provide a structural, "architectural" quality to the layout.

## Layout & Spacing

The layout philosophy follows a **fixed grid** model to maintain a controlled, premium presentation on larger displays. A 12-column system is used with a generous 1440px maximum container width. 

Margins are intentionally wide (64px+) to create "breathable" luxury, pushing content toward the center to focus the eye. Vertical rhythm is established through a 8px base unit, with large "stack" spacing (80px) used to clearly delineate high-level sections and services. Layouts should favor asymmetrical balance to create visual interest and dynamic movement.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and backdrop filters rather than traditional heavy shadows. Surfaces are treated as semi-transparent panes with a `blur` effect (12px to 20px) and a subtle 1px border using a low-opacity version of the tertiary color.

When depth is required for interactive elements, use **ambient shadows**—diffused, wide-spread glows that utilize the primary indigo color at very low opacity (5-10%). This creates the illusion that the UI elements are emitting light onto the dark canvas below, reinforcing the tech-centric theme.

## Shapes

The shape language is consistently **Rounded**, using a 0.5rem (8px) base radius. This provides a modern, approachable feel that softens the high-contrast dark palette. 

Larger containers and cards should use the `rounded-xl` (1.5rem/24px) setting to emphasize the "glass pane" aesthetic. Interactive elements like buttons should maintain the base roundedness to feel precise and mechanical, avoiding the "pill" shape which can feel too casual for a high-end agency.

## Components

### Buttons
Primary buttons use a subtle gradient transition from the Primary Indigo to the Secondary Magenta. On hover, the element should slightly scale (1.02x) with a soft outer glow. Secondary buttons use a "ghost" style with a 1px border and high-blur backdrop filter.

### Cards
Cards are the primary container for portfolio items and services. They must feature a `backdrop-filter: blur()` and a subtle top-to-bottom linear gradient (from 5% white to 0% white). Hover states should reveal a primary-colored border glow.

### Input Fields
Inputs are minimalist: a single bottom border that expands from the center upon focus. Backgrounds should be a dark "surface" color slightly lighter than the pure black page background (#121212).

### Motion Design
All components must support high-quality motion. Use `cubic-bezier(0.23, 1, 0.32, 1)` for all transitions—this "expo-out" curve ensures animations feel snappy yet smooth. Lists should reveal items with a staggered "fade-and-slide" effect to emphasize the agency's attention to detail.

### Chips & Tags
Small, monochromatic tags using the Tertiary color at 10% opacity for the background and 100% for the text. These provide categorization without distracting from the main visual hierarchy.