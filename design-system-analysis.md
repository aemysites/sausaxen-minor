# Minor Hotels Design System Analysis

## Color Palette

### Primary Colors
- **Navy Blue (Primary)**: `rgb(19, 33, 60)` / `#13213C`
  - Used for headers, primary buttons, navigation
  - Main brand color throughout the site

- **Black**: `rgb(17, 17, 17)` / `#111111`
  - Body text and headings
  - Secondary UI elements

- **White**: `rgb(255, 255, 255)` / `#FFFFFF`
  - Background color
  - Button text on dark backgrounds
  - Contrast element

### Secondary Colors
- **Light Gray**: `rgb(235, 238, 238)` / `#EBEEEE`
  - Subtle backgrounds
  - Section dividers

- **Light Gray 2**: `rgb(241, 239, 240)` / `#F1EFF0`
  - Alternative background shade

- **Light Gray 3**: `rgb(248, 248, 249)` / `#F8F8F9`
  - Very light backgrounds

- **Medium Gray**: `rgb(158, 158, 158)` / `#9E9E9E`
  - Secondary text
  - Disabled states

- **Dark Gray**: `rgb(51, 51, 51)` / `#333333`
  - Secondary headings

### Accent Colors
- **Light Blue**: `rgb(152, 208, 239)` / `#98D0EF`
  - Newsletter section backgrounds
  - Call-to-action sections

- **Red**: `rgb(224, 0, 0)` / `#E00000`
  - Error states
  - Urgent notifications

### Overlay/Modal Colors
- **Dark Overlay**: `rgba(32, 31, 31, 0.95)`
  - Popup backgrounds

- **White Overlay (28% opacity)**: `rgba(255, 255, 255, 0.28)`
  - Subtle overlays on images

- **White Overlay (20% opacity)**: `rgba(255, 255, 255, 0.2)`
  - Card overlays

- **White Overlay (60% opacity)**: `rgba(255, 255, 255, 0.6)`
  - Text overlays on images

## Typography

### Font Families

#### Headings Font
- **Primary**: `Manuka` (custom font)
- **Fallbacks**: Impact, Haettenschweiler, "Franklin Gothic Bold", Charcoal, "Helvetica Inserat", "Bitstream Vera Sans Bold", "Arial Black", sans-serif

#### Body Font
- **Primary**: `"Sitka Text"` (custom font)
- **Fallbacks**: Palatino, "Palatino Linotype", "Palatino LT STD", "Book Antiqua", Georgia, serif

#### UI Font (Buttons, Navigation)
- **Primary**: `"Helvetica Neue"`
- **Fallbacks**: Helvetica, Arial, sans-serif

### Heading Styles

#### H1
- **Font Family**: Manuka
- **Font Size**: `57.6px` (3.6rem)
- **Font Weight**: `700` (Bold)
- **Line Height**: `72px` (1.25)
- **Letter Spacing**: `1.152px`
- **Color**: `#13213C` (Navy Blue)

#### H2
- **Font Family**: Manuka
- **Font Size**: `57.6px` (3.6rem)
- **Font Weight**: `700` (Bold)
- **Line Height**: `72px` (1.25)
- **Letter Spacing**: `1.152px`
- **Color**: `#13213C` (Navy Blue)

#### H3
- **Font Family**: Manuka
- **Font Size**: `64px` (4rem)
- **Font Weight**: `700` (Bold)
- **Line Height**: `64px` (1)
- **Letter Spacing**: `2px`
- **Color**: `#111111` (Black)

### Body Text
- **Font Size**: `16px` (1rem)
- **Font Weight**: `400` (Regular)
- **Line Height**: `normal`
- **Color**: `#111111` (Black)

## Button Styles

### Primary Button ("Book Now" style)
- **Background**: `#13213C` (Navy Blue)
- **Color**: `#FFFFFF` (White)
- **Padding**: `10px 20px`
- **Font Size**: `14px`
- **Font Weight**: `700` (Bold)
- **Border Radius**: `5px`
- **Border**: None
- **Text Transform**: `UPPERCASE`
- **Letter Spacing**: `0.7px`

### Secondary Button (Circular +/- buttons)
- **Background**: `#13213C` (Navy Blue)
- **Color**: `#FFFFFF` (White)
- **Padding**: `1px 6px`
- **Font Size**: `10px`
- **Border Radius**: `50%` (Circular)
- **Border**: None

### Button Variants (CSS Variables)
- **Default Button Background**: `#FFFFFF` (White)
- **Default Button Text**: `#111111` (Black)
- **Default Button Hover Background**: `#111111` (Black)
- **Default Button Hover Text**: `#FFFFFF` (White)
- **Revert Button Background**: `transparent`
- **Revert Button Text**: `#FFFFFF` (White)
- **Revert Button Border**: `#FFFFFF` (White)
- **Revert Button Hover Background**: `#111111` (Black)
- **Button Text Size**: `12px`

## Links
- **Color**: `#111111` (Black)
- **Text Decoration**: None
- **Font Weight**: `400` (Regular)
- **Hover State**: Typically white text (`#FFFFFF`)

## Layout & Spacing

### Container
- **Main Padding**: `0px` (tight to edges)
- **Max Width**: None (full width)

### Cards/Offer Items
- **Background**: Transparent or image-based
- **Border Radius**: `0px` (sharp corners)
- **Box Shadow**: None
- **Padding**: `0px`
- **Margin**: `0px 15px 0px 0px` (right margin for spacing)
- **Display**: `inline-flex`

### Grid System
- **Display**: Block-based with inline-flex cards
- **Gap**: Normal (not using CSS gap property)

## Design Patterns

### Visual Style
- **Modern luxury aesthetic** with bold typography
- **Large hero images** with text overlays
- **Sharp corners** (no border radius on cards)
- **High contrast** between navy/black and white
- **Minimal shadows** - focus on photography and typography

### Component Hierarchy
1. Large hero sections with full-width images
2. Card-based offer displays with image backgrounds
3. Text overlays with semi-transparent backgrounds
4. Clean, structured footer with multi-column layout
5. Sticky navigation bar with booking widget

### Spacing Philosophy
- Tight margins on cards
- Generous whitespace around sections
- Compact buttons and UI elements
- Focus on image-first design

## CSS Custom Properties Used

```css
--button-default-bgcolor: #ffffff
--button-default-textcolor: #111111
--button-default-hover-bg-color: #111
--button-default-hover-text-color: #ffffff
--button-default-hover-border-color: transparent
--button-revert-bgcolor: transparent
--button-revert-textcolor: #FFF
--button-revert-border-color: #111
--button-revert-border-white: #fff
--button-revert-hover-bg-color: #111
--button-revert-hover-text-color: #FFFFFF
--button-text-size: 12px
--textColor: #ffffff
--titleColor: #ffffff
--textLinkColor: #FFFFFF
--white: #ffffff
--popup_backgroup_color: rgba(32, 31, 31, 0.95)
--popup_overlay_color: #000000
```

## Responsive Considerations
- Mobile-first approach with hamburger menu
- Full-width images scale responsively
- Card grids adjust for different screen sizes
- Fixed booking bar at bottom on mobile

## Key Design Takeaways
1. **Luxury branding** through premium serif fonts and large-scale photography
2. **Navy blue (#13213C)** is the signature brand color
3. **Manuka** font family for impactful headings
4. **Sitka Text** for elegant body copy
5. **Minimal UI chrome** - letting content shine
6. **High-quality imagery** as primary design element
7. **Clear CTAs** with uppercase, bold button text
