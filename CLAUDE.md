# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a modern portfolio website for Jesus Heredia (JesusHered.github.io), showcasing expertise as a Tech Lead in Data Engineering, AI specialist, and cloud architect. The site features a contemporary blue-themed design with animated elements, highlighting data science projects, AI solutions, and cloud infrastructure experience.

## Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (jQuery-based)
- **CSS Framework**: Bootstrap 4
- **JavaScript Libraries**: 
  - jQuery 3.5.1
  - Isotope (grid filtering)
  - Owl Carousel (testimonials carousel)
  - WOW.js (scroll animations)
  - Fancybox (image lightbox)
  - Perfect Scrollbar
  - Nice Select
- **Hosting**: GitHub Pages
- **Template**: Based on "Virtual Folio" theme by MACode ID

## Architecture

### File Structure
- `index.html` - Main portfolio page (Spanish content)
- `index-2.html` - Alternative layout variant
- `blog-*.html` - Blog layout variants (topbar/minibar)
- `assets/` - Static assets directory
  - `css/` - Stylesheets (Bootstrap, theme, icons)
  - `js/` - JavaScript files and vendor libraries
  - `img/` - Images, logos, portfolio screenshots
  - `vendor/` - Third-party library assets

### Key Components
- **Single Page Layout**: All content sections (home, about, portfolio, contact) in one HTML file
- **Portfolio Grid**: Isotope-powered filterable project showcase
- **Responsive Design**: Bootstrap-based responsive layout
- **Animation System**: WOW.js for scroll-triggered animations

## Development Workflow

### Local Development
Since this is a static site, simply open `index.html` in a browser for local development. No build process required.

### Deployment
The site is automatically deployed via GitHub Pages from the `master` branch. Any push to master will trigger deployment.

### Content Updates
- Portfolio projects: Update the `.grid-item` sections in `index.html:370-431`
- Personal information: Update the about section in `index.html:102-303`
- Contact details: Update footer section in `index.html:437-468`
- Skills/experience: Update timeline sections in `index.html:160-302`

## Key Features

### Modern Design System
- Blue color scheme with CSS variables for consistency
- Gradient backgrounds and modern card designs
- Animated skill cards and progress bars with shimmer effects
- Floating elements animation in hero section

### AI Projects Section
- Dedicated section highlighting LangChain and RAG projects
- Tech stack tags for each project
- Hover animations and modern card layouts

### Enhanced Skills Dashboard
- Interactive skill cards with percentage displays
- Separate sections for Data/AI vs Development skills
- Modern progress bars with gradient fills and animations

### Portfolio Grid System
- Isotope library for filtering and layout
- New filter categories: Data & IA, Web & Apps, Automatización
- Updated project descriptions emphasizing data and AI work
- Images stored in `assets/img/work/`

### Professional Timeline
- Enhanced timeline with modern styling
- Tech stack tags for each position
- Emphasis on data engineering and cloud experience

### Certification Display
- Visual badges for GCP certifications
- Grouped by category (Cloud, Development, Management)

## Important Notes

- All content is in Spanish (target audience: Mexico/Latin America)
- Google Maps integration with hardcoded API key in `index.html:496`
- External template attribution should be maintained (lines 50-53)
- Profile image: `profile-image.jpeg` in root directory
- Contact information is real and should be handled carefully

## Common Tasks

### Adding New Portfolio Items
1. Add new image to `assets/img/work/`
2. Create new `.grid-item` div in the gridder section
3. Follow existing pattern with data-src, data-caption attributes
4. Ensure proper class assignments for filtering

### Updating Personal Information
- Skills percentages: Update progress-bar style widths in `index.html:131-155`
- Experience timeline: Add new `<li>` elements to timeline sections
- Contact details: Update footer section and ensure consistency

### Theme Customization
- Primary theme color controlled by `.fg-theme` CSS class
- Main theme file: `assets/css/virtual.css`
- Color scheme defined by `body.theme-red` class