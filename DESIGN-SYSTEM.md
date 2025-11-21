# Minor Hotels Design System - EDS Implementation

This document describes the design system implementation for the Minor Hotels website, based on analysis of minorhotels.com.

## Quick Start

The global styles are implemented in `/styles/styles.css` following EDS (Edge Delivery Services) conventions.

## Color Palette

### Primary Brand Colors
- **Navy Blue**: `#13213C` - Primary brand color, used for headers, buttons, navigation
- **Black**: `#111111` - Body text and secondary elements
- **White**: `#FFFFFF` - Backgrounds and contrast

### Gray Scale
- **Light Gray**: `#EBEEEE` - Subtle backgrounds
- **Light Gray 2**: `#F1EFF0` - Alternative background
- **Light Gray 3**: `#F8F8F9` - Very light backgrounds
- **Medium Gray**: `#9E9E9E` - Secondary text, disabled states
- **Dark Gray**: `#333333` - Secondary headings

### Accent Colors
- **Light Blue**: `#98D0EF` - Newsletter sections, call-to-actions
- **Red**: `#E00000` - Error states, alerts

### Overlay Colors
- **Dark Overlay**: `rgba(32, 31, 31, 0.95)` - Modal backgrounds
- **White 28%**: `rgba(255, 255, 255, 0.28)` - Image overlays
- **White 20%**: `rgba(255, 255, 255, 0.2)` - Card overlays
- **White 60%**: `rgba(255, 255, 255, 0.6)` - Text protection overlays

## Typography

### Font Families

#### Headings
**Primary**: Manuka (custom brand font)
**Fallbacks**: Impact, Haettenschweiler, "Franklin Gothic Bold", Charcoal, "Helvetica Inserat", "Bitstream Vera Sans Bold", "Arial Black", sans-serif

#### Body Text
**Primary**: "Sitka Text" (elegant serif)
**Fallbacks**: Palatino, "Palatino Linotype", "Palatino LT STD", "Book Antiqua", Georgia, serif

#### UI Elements (Buttons, Navigation)
**Primary**: "Helvetica Neue"
**Fallbacks**: Helvetica, Arial, sans-serif

### Heading Sizes

| Element | Desktop | Tablet (≤900px) | Mobile (≤600px) |
|---------|---------|-----------------|-----------------|
| H1      | 57.6px  | 42px            | 28px            |
| H2      | 57.6px  | 38px            | 24px            |
| H3      | 64px    | 32px            | 20px            |
| H4      | 32px    | 28px            | 20px            |
| H5      | 24px    | 22px            | 18px            |
| H6      | 20px    | 18px            | 16px            |

### Letter Spacing
- H1: `1.152px` (desktop), `0.84px` (tablet), `0.8px` (mobile)
- H2: `1.152px` (desktop), `0.76px` (tablet), `0.7px` (mobile)
- H3: `2px` (desktop), `1.28px` (tablet), `1px` (mobile)
- Buttons: `0.7px`

### Body Text
- Desktop: 16px
- Mobile: 15px
- Line Height: 1.6

## Buttons

### Default Button (Primary)
```html
<a href="#" class="button">Book Now</a>
```
- Background: Navy Blue (#13213C)
- Text: White
- Padding: 10px 20px
- Border Radius: 5px
- Font: Helvetica Neue, 14px, bold
- Text Transform: UPPERCASE
- Letter Spacing: 0.7px

### Secondary Button
```html
<a href="#" class="button secondary">Learn More</a>
```
- Background: Transparent
- Text: White
- Border: 2px solid white
- Hover: Black background

### Button Sizes
```html
<a href="#" class="button small">Small</a>
<a href="#" class="button large">Large</a>
<a href="#" class="button full-width">Full Width</a>
```

## Layout Components

### Hero Sections
```html
<div class="hero">
  <img src="hero-image.jpg" alt="Hero">
  <div>
    <h1>Welcome to Minor Hotels</h1>
    <p>Experience luxury worldwide</p>
    <a href="#" class="button">Explore</a>
  </div>
</div>
```
- Full-width background images
- Semi-transparent overlay (28% white)
- Centered content
- Minimum height: 500px (desktop), 300px (mobile)

### Section Variants

#### Dark Background Section
```html
<div class="section dark-bg">
  <div>
    <h2>Premium Experiences</h2>
    <p>Content here...</p>
  </div>
</div>
```

#### Light Background Section
```html
<div class="section light-bg">
  <div>
    <h2>Newsletter Signup</h2>
    <p>Stay connected...</p>
  </div>
</div>
```

### Image with Overlay
```html
<div class="image-wrapper">
  <img src="image.jpg" alt="Description">
  <div class="image-overlay"></div>
  <div class="image-content">
    <h3>Card Title</h3>
    <p>Card description</p>
  </div>
</div>
```

## CSS Variables Reference

All design tokens are available as CSS custom properties in `styles.css`:

### Colors
```css
--color-navy-primary: #13213C
--color-black: #111
--color-white: #fff
--color-gray-light: #EBEEEE
--color-blue-light: #98D0EF
```

### Typography
```css
--heading-font-family: Manuka, Impact, ...
--body-font-family: "Sitka Text", Palatino, ...
--heading-font-size-xxl: 57.6px
--letter-spacing-h1: 1.152px
```

### Spacing
```css
--spacing-xs: 5px
--spacing-sm: 10px
--spacing-md: 15px
--spacing-lg: 20px
--spacing-xl: 40px
--spacing-xxl: 60px
```

### Buttons
```css
--button-border-radius: 5px
--button-padding: 10px 20px
--letter-spacing-button: 0.7px
```

## Utility Classes

### Text Utilities
- `.text-white` - White text color
- `.text-center` - Center aligned text
- `.text-uppercase` - Uppercase with button letter spacing

### Spacing Utilities
- `.mt-sm`, `.mt-md`, `.mt-lg`, `.mt-xl` - Margin top
- `.mb-sm`, `.mb-md`, `.mb-lg`, `.mb-xl` - Margin bottom
- `.pt-sm`, `.pt-md`, `.pt-lg`, `.pt-xl` - Padding top
- `.pb-sm`, `.pb-md`, `.pb-lg`, `.pb-xl` - Padding bottom

## Design Principles

1. **Luxury Branding** - Premium serif fonts and large-scale photography
2. **Navy Blue Identity** - #13213C as signature brand color
3. **Typography First** - Bold Manuka headings with wide letter spacing
4. **Image-Centric** - Full-width photography with subtle overlays
5. **Minimal UI** - Clean interfaces letting content shine
6. **High Contrast** - Strong navy/black on white
7. **Sharp Edges** - Minimal border radius (5px max)

## Responsive Breakpoints

- **Desktop**: 900px and above
- **Tablet**: 601px to 900px
- **Mobile**: 600px and below

## Browser Support

Modern browsers with CSS custom properties support:
- Chrome/Edge 88+
- Firefox 85+
- Safari 14+

## Resources

- Full design analysis: `/workspace/design-system-analysis.md`
- Homepage screenshot: `/tmp/playwright/minorhotels-homepage.png`
- Offers page screenshot: `/tmp/playwright/minorhotels-offers.png`
