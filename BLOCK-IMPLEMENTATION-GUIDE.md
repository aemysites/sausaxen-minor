# Block Implementation Guide - Minor Hotels

This guide shows how to use the styled EDS blocks for the Minor Hotels website.

## Available Blocks

All blocks are styled to match the Minor Hotels brand with navy blue (#13213C), Manuka headings, and Sitka Text body font.

### 1. Hero Block

**Use for**: Large promotional sections, homepage hero, landing pages

**Location**: `/blocks/hero/`

**Basic Usage**:
```
| Hero |
|---|
| ![Hero Image](hero.jpg) |
| # Welcome to Minor Hotels<br>Experience luxury worldwide<br>[Explore](/destinations) |
```

**Variants**:
- Add `(compact)` for shorter hero: `| Hero (compact) |`
- Add `(dark)` for darker overlay: `| Hero (dark) |`

**Features**:
- Full-width background images
- 28% white overlay for readability
- Centered white text
- Responsive (500px desktop → 300px mobile)

---

### 2. Cards Block

**Use for**: Offers grid, destinations, hotel listings, feature showcases

**Location**: `/blocks/cards/`

**Basic Usage**:
```
| Cards |
|---|---|
| ![Offer 1](offer1.jpg) | ![Offer 2](offer2.jpg) |
| ### Black Friday Sale<br>Save up to 45%<br>[Book Now](/offers/black-friday) | ### Exclusive Deals<br>Plan ahead and save<br>[Book Now](/offers/exclusive) |
```

**Variants**:
- `| Cards (2-cols) |` - Force 2 columns
- `| Cards (3-cols) |` - Force 3 columns
- `| Cards (4-cols) |` - Force 4 columns
- `| Cards (image-overlay) |` - Text overlays on images
- `| Cards (horizontal-scroll) |` - Carousel-like scrolling
- `| Cards (compact) |` - Smaller cards with less padding

**Features**:
- Auto-responsive grid
- Hover animations (lift + image scale)
- Image aspect ratio: 3:2 default
- Navy headings, clean layout

---

### 3. Columns Block

**Use for**: Feature sections, "More to Explore" type content, services

**Location**: `/blocks/columns/`

**Basic Usage**:
```
| Columns |
|---|---|
| ![Restaurants](restaurants.jpg) | ![Spa](spa.jpg) |
| ### Restaurants & Bars<br>Dine for any occasion...<br>[Discover More](/restaurants) | ### Spa & Wellness<br>Restore your mind...<br>[Discover More](/spa) |
```

**Variants**:
- `| Columns (2) |` - 2 columns
- `| Columns (3) |` - 3 columns
- `| Columns (4) |` - 4 columns
- `| Columns (image-left) |` - Image on left, text on right
- `| Columns (image-right) |` - Image on right, text on left
- `| Columns (alternating) |` - Alternate image sides
- `| Columns (centered) |` - Center-aligned content
- `| Columns (dark-bg) |` - Navy background

**Features**:
- Flexible layouts
- Responsive stacking
- Image hover zoom effect

---

### 4. Carousel Block

**Use for**: Promotional sliders, featured offers, image galleries

**Location**: `/blocks/carousel/`

**Basic Usage**:
```
| Carousel |
|---|
| ![Slide 1](promo1.jpg) |
| ## Festive Celebrations<br>Glittering occasions worldwide<br>[Discover More](/offers/festive) |
| ![Slide 2](promo2.jpg) |
| ## Black Friday Sale<br>Save up to 45%<br>[Shop Now](/offers/black-friday) |
```

**Variants**:
- `| Carousel (compact) |` - Shorter height

**Features**:
- Full-width slides
- Arrow navigation
- Dot indicators
- Auto-rotate capability
- 28% white overlay

---

### 5. Accordion Block

**Use for**: FAQs, expandable content sections

**Location**: `/blocks/accordion/`

**Basic Usage**:
```
| Accordion |
|---|---|
| Frequently Asked Questions | |
| **Are there special offers available?** | Yes, Minor Hotels offers exclusive deals for members... |
| **What benefits do members enjoy?** | Members receive priority check-in, room upgrades... |
| **How can I become a member?** | Sign up online at our membership portal... |
```

**Variants**:
- `| Accordion (compact) |` - Smaller padding
- `| Accordion (dark-bg) |` - Navy background

**Features**:
- Expandable/collapsible items
- Arrow indicators
- Smooth transitions
- Navy headings

---

### 6. Header Block

**Use for**: Site navigation (auto-loaded)

**Location**: `/blocks/header/`

**Features**:
- Sticky positioning
- Logo on left
- Main navigation center
- Actions (Login/Signup) on right
- Mobile hamburger menu
- Language/Currency selector

**Customization**: Edit `/blocks/header/header.js` for navigation items

---

### 7. Footer Block

**Use for**: Site footer (auto-loaded)

**Location**: `/blocks/footer/`

**Features**:
- Navy background (#13213C)
- Newsletter signup (light blue section)
- Brand logos grid
- Multi-column link sections
- Social media icons
- App download badges
- Legal links
- Responsive layout

**Customization**: Edit `/blocks/footer/footer.js` for footer content

---

## Section Metadata

Add section styling using metadata:

### Dark Background Section
```
---
# Section Metadata

style: dark-bg
---
```

### Light Background Section
```
---
# Section Metadata

style: light-bg
---
```

### Hero Section
```
---
# Section Metadata

style: hero-section
---
```

---

## Color Usage Guide

### When to use Navy Blue (#13213C):
- Primary buttons
- Headings (H1, H2)
- Navigation links (hover)
- Footer background
- Brand elements

### When to use White:
- Text on dark backgrounds
- Button text on navy buttons
- Hero text overlays
- Footer text

### When to use Light Blue (#98D0EF):
- Newsletter sections
- Call-to-action backgrounds
- Accent highlights

### When to use Black (#111):
- Body text
- H3 headings
- Secondary elements

---

## Responsive Breakpoints

- **Desktop**: 900px and above
- **Tablet**: 601px - 900px
- **Mobile**: 600px and below

All blocks automatically adapt to these breakpoints.

---

## Typography Examples

### Headings
```
# Main Page Title (H1)
## Section Title (H2)
### Card/Feature Title (H3)
```

### Buttons
```
[Primary Button](/link)
[Secondary Button](/link){.secondary}
[Small Button](/link){.small}
[Large Button](/link){.large}
```

### Text Styles
Use section metadata for special text styling:
- White text: add `text-white` class
- Centered text: add `text-center` class
- Uppercase: add `text-uppercase` class

---

## Example Page Structure

### Homepage
```
| Hero |
|---|
| ![Hero](hero.jpg) |
| # Explore the world with Minor Hotels<br>Luxury hotels worldwide<br>[Book Now](/book) |

---

| Carousel |
|---|
| ![Promo 1](promo1.jpg) |
| ## Black Friday Sale<br>Save up to 45%<br>[Discover More](/offers/black-friday) |

---

| Cards (3-cols) |
|---|---|---|
| ![Destination 1](dest1.jpg) | ![Destination 2](dest2.jpg) | ![Destination 3](dest3.jpg) |
| ### Thailand<br>[Explore](/destinations/thailand) | ### Maldives<br>[Explore](/destinations/maldives) | ### Dubai<br>[Explore](/destinations/dubai) |

---
# Section Metadata

style: dark-bg
---

| Columns (alternating) |
|---|---|
| ![Restaurants](rest.jpg) | ![Spa](spa.jpg) |
| ### Restaurants & Bars<br>Description<br>[Discover More](/restaurants) | ### Spa & Wellness<br>Description<br>[Discover More](/spa) |
```

### Offers Page
```
| Hero (compact) |
|---|
| ![Offers Hero](offers-hero.jpg) |
| # Hotel Offers and Promotional Packages<br>[View All Offers](#offers) |

---

| Cards (2-cols, image-overlay) |
|---|---|
| ![Offer 1](offer1.jpg) | ![Offer 2](offer2.jpg) |
| ### Black Friday<br>Save up to 45%<br>[Explore More](/offers/black-friday) | ### Exclusive Deals<br>Plan ahead<br>[Explore More](/offers/exclusive) |

---

| Accordion |
|---|---|
| Frequently Asked Questions | |
| **Are there special offers?** | Yes, we have seasonal offers... |
| **What are the booking terms?** | Booking terms vary by offer... |
```

---

## Tips for Best Results

1. **Images**: Use high-quality images (min 1920px wide for heroes)
2. **Alt Text**: Always provide descriptive alt text
3. **Aspect Ratios**:
   - Hero: 16:9 or wider
   - Cards: 3:2 works best
   - Columns: 4:3 or square
4. **Text Length**: Keep card titles under 60 characters
5. **CTAs**: Always include clear call-to-action buttons
6. **Contrast**: Ensure text is readable on images (use overlays)

---

## Browser Support

All blocks support:
- Chrome/Edge 88+
- Firefox 85+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## Need Help?

- Full design system: See `/workspace/DESIGN-SYSTEM.md`
- Block mappings: See `/workspace/BLOCK-MAPPING.md`
- Design analysis: See `/workspace/design-system-analysis.md`
