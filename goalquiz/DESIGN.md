---
name: GoalQuiz
colors:
  surface: '#faf9f8'
  surface-dim: '#dadad9'
  surface-bright: '#faf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f3f2'
  surface-container: '#eeeeed'
  surface-container-high: '#e9e8e7'
  surface-container-highest: '#e3e2e1'
  on-surface: '#1a1c1c'
  on-surface-variant: '#554240'
  inverse-surface: '#2f3130'
  inverse-on-surface: '#f1f0ef'
  outline: '#887270'
  outline-variant: '#dbc1be'
  surface-tint: '#98443e'
  primary: '#98443e'
  on-primary: '#ffffff'
  primary-container: '#f28b82'
  on-primary-container: '#6d2420'
  inverse-primary: '#ffb3ac'
  secondary: '#635d5d'
  on-secondary: '#ffffff'
  secondary-container: '#eae0e0'
  on-secondary-container: '#696363'
  tertiary: '#735858'
  on-tertiary: '#ffffff'
  tertiary-container: '#c1a0a0'
  on-tertiary-container: '#4f3737'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad6'
  primary-fixed-dim: '#ffb3ac'
  on-primary-fixed: '#3f0204'
  on-primary-fixed-variant: '#7a2e29'
  secondary-fixed: '#eae0e0'
  secondary-fixed-dim: '#cdc4c4'
  on-secondary-fixed: '#1f1b1b'
  on-secondary-fixed-variant: '#4b4546'
  tertiary-fixed: '#ffdada'
  tertiary-fixed-dim: '#e1bebe'
  on-tertiary-fixed: '#2a1617'
  on-tertiary-fixed-variant: '#594041'
  background: '#faf9f8'
  on-background: '#1a1c1c'
  surface-variant: '#e3e2e1'
typography:
  display-xl:
    fontFamily: Lexend
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Lexend
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  headline-md:
    fontFamily: Lexend
    fontSize: 22px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
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
  lg: 40px
  xl: 64px
  gutter: 16px
  margin-mobile: 20px
---

## Brand & Style

This design system is built to evoke a sense of friendly competition and athletic focus without the aggressive visual weight typical of sports apps. The brand personality is welcoming, energetic, and clean. 

The aesthetic follows a **Modern Minimalist** approach with a focus on high-quality typography and soft tonal transitions. By utilizing a pastel red rather than a vibrant primary red, the interface remains comfortable for long periods of focus during quiz sessions. Surfaces are kept airy and light, ensuring that the content—the football trivia—remains the central hero of the experience.

## Colors

The palette revolves around a "Soft Stadium Red," a muted pastel tone that provides brand recognition without causing eye fatigue. 

- **Primary:** A soft, desaturated red used for primary actions, progress indicators, and key branding.
- **Surface:** A light off-white ("Bone White") serves as the primary canvas, providing a warmer, more sophisticated feel than pure white.
- **Accents:** Tertiary and secondary reds are used for subtle backgrounds, hover states, and container fills to create a cohesive "blush" effect across the UI.
- **Neutral:** A deep chocolate-grey is used for text to maintain high legibility while harmonizing with the warm red tones.

## Typography

This design system utilizes **Lexend** for headlines to leverage its athletic, highly-readable, and modern character. It communicates momentum and clarity, essential for a timed quiz environment. 

**Plus Jakarta Sans** is used for body copy and UI labels. Its soft, rounded terminals complement the overall shape language of the app and maintain an approachable, friendly tone. Letter spacing is slightly tightened for large displays to maintain impact, while labels use slightly increased tracking for better legibility at small sizes.

## Layout & Spacing

The layout philosophy follows a **Fluid Grid** model optimized for mobile devices. The system is built on an 8px rhythmic scale to ensure consistent vertical and horizontal alignment.

- **Margins:** A 20px safe area is maintained on mobile devices.
- **Gutter:** 16px gutters are used between cards and grid elements to allow the soft shadows and red accents room to breathe.
- **Rhythm:** Use the `md` (24px) spacing for vertical separation between distinct sections, and `sm` (12px) for elements within a group (e.g., a question and its multiple-choice answers).

## Elevation & Depth

This design system uses **Tonal Layers** combined with **Ambient Shadows** to create depth. Instead of traditional grey shadows, shadows are slightly tinted with the primary red color (e.g., a hex like `#B85C5C` at 8-12% opacity) to maintain the warmth of the palette.

- **Level 0 (Floor):** The off-white surface.
- **Level 1 (Cards):** Low elevation, used for answer choices and secondary navigation. 
- **Level 2 (Active/Primary):** Medium elevation with a more pronounced soft red glow, used for the current active question or primary call-to-action buttons.
- **Interaction:** Buttons should appear to "sink" (reduce elevation) upon press, reinforcing the tactile nature of the UI.

## Shapes

The shape language is defined by **Rounded** geometry (Level 2). This level of curvature balances the "blocky" nature of traditional sports grids with the softness of the pastel color scheme.

- **Standard Elements:** Buttons and input fields use a 0.5rem (8px) radius.
- **Containers:** Large cards and modals use the `rounded-lg` (1rem / 16px) or `rounded-xl` (1.5rem / 24px) setting to create a friendly, "pocketable" feel.
- **Selection Indicators:** Small indicators (like category tags) may utilize pill-shaped rounding to distinguish them from interactive buttons.

## Components

### Buttons
Primary buttons use the soft red fill with white text. Secondary buttons use a light red tint (`#FCE8E6`) with primary red text. All buttons feature high-radius corners and subtle red-tinted shadows.

### Quiz Cards
Cards should have no border, instead relying on the `neutral_color_hex` surface and a Level 1 shadow for definition. When a user selects an answer, the card border should animate to a 2px stroke of the primary pastel red.

### Input Fields
Inputs use the `neutral_color_hex` background with a subtle 1px border in a darker tint of the off-white. On focus, the border transitions to the soft red brand color with a subtle outer glow.

### Progress Bars
The "Quiz Timer" and "Level Progress" bars should use a rounded track with the `tertiary_color_hex` as the background and the `primary_color_hex` as the fill, ensuring a smooth, non-aliased animation.

### Chips & Tags
Used for football leagues or difficulty levels. These use a "Pill" shape and the `secondary_color_hex` background to keep them distinct from actionable buttons.

### Modals
Modals appear from the bottom (drawer-style) on mobile, using `rounded-xl` top corners and a dark semi-transparent backdrop to focus the user on the feedback (e.g., "Correct Answer!").