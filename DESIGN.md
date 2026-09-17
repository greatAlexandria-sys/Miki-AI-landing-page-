---
name: Precision Intelligence
colors:
  surface: '#f9f9ff'
  surface-dim: '#d1daf1'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f3ff'
  surface-container: '#e8eeff'
  surface-container-high: '#e0e8ff'
  surface-container-highest: '#dae2f9'
  on-surface: '#131c2c'
  on-surface-variant: '#44474d'
  inverse-surface: '#283042'
  inverse-on-surface: '#ecf0ff'
  outline: '#75777e'
  outline-variant: '#c5c6ce'
  surface-tint: '#505e7f'
  primary: '#00081e'
  on-primary: '#ffffff'
  primary-container: '#10203d'
  on-primary-container: '#7988aa'
  inverse-primary: '#b7c6ec'
  secondary: '#415e95'
  on-secondary: '#ffffff'
  secondary-container: '#a4c1ff'
  on-secondary-container: '#304e84'
  tertiary: '#000b17'
  on-tertiary: '#ffffff'
  tertiary-container: '#00233a'
  on-tertiary-container: '#098fd9'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#b7c6ec'
  on-primary-fixed: '#0a1b38'
  on-primary-fixed-variant: '#384766'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a41'
  on-secondary-fixed-variant: '#27467b'
  tertiary-fixed: '#cde5ff'
  tertiary-fixed-dim: '#95ccff'
  on-tertiary-fixed: '#001d32'
  on-tertiary-fixed-variant: '#004a75'
  background: '#f9f9ff'
  on-background: '#131c2c'
  surface-variant: '#dae2f9'
  bg-marketing: '#FAFAF9'
  surface-product: '#0B1424'
  surface-product-elevated: '#111C30'
  border-product: '#1E2D4A'
  text-muted-light: '#6B7280'
  text-primary-dark: '#F1F5F9'
  text-muted-dark: '#94A3B8'
  signal-accent: '#3FA9F5'
  status-success: '#2FA36B'
  status-warning: '#D9A441'
  status-danger: '#D9534F'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '500'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 28px
    letterSpacing: -0.01em
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
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
  code-md:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-lg: 1.5rem
  margin: 1.25rem
  margin-md: 2rem
  margin-lg: 4rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

# Miki AI Design System

## Visual Personality & Brand Principles
- **Aesthetic**: Premium enterprise security & intelligence, disciplined, restrained (reminiscent of Linear, Space, Vercel).
- **Core Philosophy**: "Marketing claim vs. actual product" separation. Light off-white marketing background (`#FAFAF9`), ultra-deep navy/near-black for product UI surfaces (`#0B1424`).
- **Signature Motif**: Node/network geometry converging camera feed and POS stream into one verified answer.
- **Negative Constraints**: Strictly no purple, no neon green, no decorative gradients, no ALL-CAPS eyebrow labels, no arrow suffixes (`→`) on buttons/links, no stock photography, no fabricated percentages.

## Color Palette
- **Primary / Brand**: `#10203D` (Logo, headlines, primary buttons, nav)
- **Secondary**: `#2E4C82` (Supporting UI elements, subtle borders)
- **Marketing Background**: `#FAFAF9` (Nav, marketing sections, footer)
- **Product Surface (Dark Mode)**: `#0B1424` (Product interface panels and close-ups)
- **Product Surface Elevated**: `#111C30`
- **Product Border**: `#1E2D4A`
- **Text Primary (Light BG)**: `#0B1424`
- **Text Muted (Light BG)**: `#6B7280`
- **Text Primary (Dark BG)**: `#F1F5F9`
- **Text Muted (Dark BG)**: `#94A3B8`
- **Accent / Signal**: `#3FA9F5` (Reserved strictly for detected/flagged mismatch states)
- **Success**: `#2FA36B` (Cleared/resolved states)
- **Warning**: `#D9A441` (Reviewing states)
- **Danger**: `#D9534F` (High-severity flags)

## Typography
- **Headlines / Display**: "Söhne", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; font-weight: 500; tight line-height; slight negative letter-spacing (-0.02em).
- **Body / Interface**: "Inter", sans-serif; font-weight: 400, 500, 600.
- **Data & Metadata**: "JetBrains Mono", monospace; strictly for timestamps, transaction IDs, confidence scores, currency values. Never decorative.

## UI Patterns & Structure
- **Buttons**: Clean solid pill/rounded rectangle, padding `10px 20px`, no arrows (`→`), sharp subtle hover.
- **Data Rows & Pills**: Precision stroke borders (`1px solid`), crisp contrast, clear status chips (`#3FA9F5` tinted background with clean borders).
