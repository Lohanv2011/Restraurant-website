---
name: Haute Gastronomy
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#d1c5b4'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#9a8f80'
  outline-variant: '#4e4639'
  surface-tint: '#e9c176'
  primary: '#e9c176'
  on-primary: '#412d00'
  primary-container: '#c5a059'
  on-primary-container: '#4e3700'
  inverse-primary: '#775a19'
  secondary: '#d7c3b0'
  on-secondary: '#3a2e21'
  secondary-container: '#544738'
  on-secondary-container: '#c8b5a3'
  tertiary: '#c8c6c5'
  on-tertiary: '#313030'
  tertiary-container: '#a7a5a5'
  on-tertiary-container: '#3b3b3b'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdea5'
  primary-fixed-dim: '#e9c176'
  on-primary-fixed: '#261900'
  on-primary-fixed-variant: '#5d4201'
  secondary-fixed: '#f4dfcb'
  secondary-fixed-dim: '#d7c3b0'
  on-secondary-fixed: '#241a0e'
  on-secondary-fixed-variant: '#524436'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474746'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: Noto Serif
    fontSize: 64px
    fontWeight: '400'
    lineHeight: 72px
    letterSpacing: -0.02em
  display-lg:
    fontFamily: Noto Serif
    fontSize: 48px
    fontWeight: '400'
    lineHeight: 56px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Noto Serif
    fontSize: 32px
    fontWeight: '400'
    lineHeight: 40px
  headline-md:
    fontFamily: Noto Serif
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
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
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.08em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base-unit: 8px
  container-max-width: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  stack-sm: 8px
  stack-md: 24px
  stack-lg: 48px
  section-gap: 120px
---

## Brand & Style

This design system is built to evoke the atmosphere of an exclusive, high-end culinary establishment. The brand personality is rooted in the "New Luxury" movement—moving away from stuffy traditionalism toward a sophisticated, modern, and welcoming minimalism. 

The visual style leverages a dark-mode-first approach to create an intimate, evening-inspired aesthetic. We utilize heavy whitespace (negative space) to allow high-quality photography of signature dishes and architectural interiors to breathe. The emotional response should be one of anticipation and prestige, positioning the service as a curated experience rather than a simple transaction.

## Colors

The palette is designed to mirror the physical materials found in fine dining: obsidian stone, warm linen, and brushed brass. 

- **Neutral (Deep Black):** Used for the primary canvas to create depth and focus.
- **Secondary (Warm Beige):** Used for secondary text and subtle UI borders to soften the interface and provide a "warm" welcome.
- **Primary (Sophisticated Gold):** Reserved for high-value actions, accents, and celebratory markers. It must be used sparingly to maintain its premium status.
- **Tertiary (Layered Grey):** Used for surface containers and card backgrounds to create subtle separation from the pure black backdrop.

## Typography

This design system employs a classic typographic contrast. The serif font (**Noto Serif**) provides an authoritative and literary tone for headlines, suggesting a heritage of craft. The sans-serif (**Inter**) provides a functional, highly legible counterpoint for menus, descriptions, and functional UI elements.

All labels and navigation items should use the `label` styles with uppercase transformations to enhance the "luxury directory" feel. Large display sizes should utilize slightly tighter letter-spacing to appear more composed and "designed."

## Layout & Spacing

The layout philosophy follows a **fixed grid** for desktop resolutions to ensure the "curated" feel of a physical menu, transitioning to a fluid layout for mobile. 

We prioritize generous vertical spacing (`section-gap`) to separate different courses of information. Content should be centered or elegantly asymmetrical to avoid the rigid, utilitarian feel of standard SaaS products. Use the 8px rhythm to define internal component padding, but allow for expansive margins at the edges of the screen to create a sense of exclusivity.

## Elevation & Depth

Hierarchy in this design system is established through **tonal layering** and **ambient shadows**. 

- **Level 0 (Background):** Pure #0A0A0A.
- **Level 1 (Cards/Surfaces):** A slightly lighter #1A1A1A with a 1px border of #D9C5B2 at 10% opacity.
- **Shadows:** Use extremely soft, large-radius shadows (e.g., 40px blur) with a very low opacity black or a subtle gold tint (#C5A059 at 5% alpha). This creates a "glow" effect rather than a harsh drop shadow.
- **Interactive Depth:** On hover, elements should subtly lift by increasing shadow spread and slightly lightening the surface color.

## Shapes

The design system utilizes **Rounded** (0.5rem base) geometry to soften the interface and make it feel more approachable and "welcoming" despite the dark palette. 

Cards and high-quality image containers use `rounded-xl` (1.5rem) to create a modern, chic frame for food photography. Smaller interactive elements like inputs and tags use the base `rounded` (0.5rem) to maintain a crisp, professional edge. Avoid sharp corners entirely to maintain the brand's sophisticated but gentle personality.

## Components

### Buttons
Primary buttons use a solid Gold (#C5A059) fill with dark text. Secondary buttons are "Ghost" style—transparent with a Warm Beige border and text. All buttons should have a generous horizontal padding (32px+) to emphasize a premium feel.

### Cards
Cards are the primary vehicle for menu items and gallery features. They feature a Level 1 surface, 1.5rem corner radius, and must always prioritize the image. Text within cards should be center-aligned or elegantly tucked into a corner with high contrast.

### Input Fields
Inputs are minimalist: a simple bottom border in Warm Beige or a very subtle filled container. Focus states are indicated by the border turning Gold.

### Lists & Menus
For the digital menu, use wide-spaced lists with the Noto Serif font for item names and Inter for prices. Prices should not use currency symbols where possible to emphasize the premium "fine dining" experience.

### Imagery
Images are considered a core component. Use a slight desaturation or a subtle dark overlay on hero images to ensure typography remains legible while maintaining a cinematic quality.