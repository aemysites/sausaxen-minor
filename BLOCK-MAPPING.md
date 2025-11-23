# Minor Hotels - EDS Block Mapping

This document maps the components from minorhotels.com to EDS out-of-box blocks.

## Block Mapping

### 1. Hero Section
**Original**: Large full-width hero with background image and centered text overlay
**EDS Block**: `hero`
**Location**: Homepage top section
**Features**:
- Full-width background image
- Centered white text overlay
- Semi-transparent overlay (28% white)
- CTA button
- Minimum height: 500px

### 2. Brand/Hotel Cards Carousel
**Original**: Horizontal scrolling brand logos with descriptions
**EDS Block**: `cards` (carousel variant)
**Location**: Homepage - "Explore the world with Minor Hotels" section
**Features**:
- Brand logos with names
- Expandable descriptions
- Horizontal scroll
- Navigation arrows

### 3. Destination Cards
**Original**: Grid of destination cards with images
**EDS Block**: `cards`
**Location**: Homepage - "Destinations" section
**Features**:
- Image cards with location names
- Grid layout (responsive)
- Linked cards

### 4. Promotional Slider/Carousel
**Original**: Full-width image slider with promotional offers
**EDS Block**: `carousel`
**Location**: Homepage - offers slider
**Features**:
- Full-width images
- Text overlay
- Dot navigation
- Auto-rotate

### 5. Feature Sections (More to Explore)
**Original**: Three feature blocks with images and descriptions
**EDS Block**: `columns` (with images)
**Location**: Homepage - "More to Explore" section
**Features**:
- 3-column layout
- Images on alternating sides
- Text content with CTAs
- Responsive stack on mobile

### 6. Offer Cards Grid
**Original**: Grid of offer cards with images and text
**EDS Block**: `cards`
**Location**: Offers page - main content
**Features**:
- 2-column grid (desktop)
- Image background with text overlay
- CTA buttons
- Stacks to 1 column on mobile

### 7. CTA/Promo Banner
**Original**: Full-width promotional section with background
**EDS Block**: `hero` (compact variant) or `section` with metadata
**Location**: Offers page - loyalty program section
**Features**:
- Background image/color
- Centered text
- CTA button

### 8. FAQ/Accordion
**Original**: Expandable FAQ items
**EDS Block**: `accordion`
**Location**: Offers page - bottom section
**Features**:
- Expandable/collapsible items
- Click to expand
- Arrow indicators

### 9. Header/Navigation
**Original**: Sticky header with logo, navigation, and booking widget
**EDS Block**: `header` (custom)
**Location**: Top of all pages
**Features**:
- Logo
- Main navigation
- User actions (Login/Signup)
- Language/Currency selector
- Booking widget (collapsible)

### 10. Footer
**Original**: Multi-column footer with links and newsletter signup
**EDS Block**: `footer` (custom)
**Location**: Bottom of all pages
**Features**:
- Newsletter signup
- Brand logos grid
- Multi-column link sections
- Social media links
- App download badges
- Legal links

### 11. Breadcrumb
**Original**: Simple breadcrumb navigation
**EDS Block**: Built into page structure
**Location**: Offers page top
**Features**:
- Text-based navigation path
- Separator characters

## Block Priority for Implementation

1. **hero** - Most prominent block
2. **cards** - Used for offers and destinations
3. **header** - Navigation and branding
4. **footer** - Site-wide information
5. **carousel** - Promotional content
6. **columns** - Feature sections
7. **accordion** - FAQ section

## Notes

- All blocks should maintain the navy blue (#13213C) brand color
- Images should be full-width with proper aspect ratios
- Text overlays need 28% white overlay for readability
- Buttons should use uppercase styling with 0.7px letter spacing
- Mobile breakpoint at 600px, tablet at 900px
