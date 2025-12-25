# Project Structure

This document describes the organization of the BlackVoxel website project.

## Directory Structure

```
BlackVoxel/
├── assets/           # Static assets (images, icons, etc.)
│   └── color.gif     # Color palette reference image
├── css/              # Stylesheets
│   └── styles.css    # Main stylesheet with all CSS
├── js/               # JavaScript files
│   └── main.js       # Main JavaScript with all functionality
├── .do/              # DigitalOcean deployment configuration
│   ├── app.yaml
│   └── deploy.template.yaml
├── .github/          # GitHub configuration
│   └── dependabot.yaml
├── index.html        # Main HTML file
├── README.md         # Project documentation
├── .npmignore        # NPM ignore configuration
└── STRUCTURE.md      # This file
```

## File Descriptions

### HTML Files
- **index.html** - Main entry point for the website. Contains the semantic HTML structure for the BlackVoxel landing page.

### CSS Files
- **css/styles.css** - Contains all styling for the website including:
  - CSS variables for theme colors
  - Navigation styles
  - Hero section with animated voxel background
  - Game showcase cards
  - Technology stack grid
  - Features section
  - Footer styles
  - Responsive design for mobile devices
  - Custom animations (glitch effect, pixel float, scanlines)
  - Custom cursor styles

### JavaScript Files
- **js/main.js** - Contains all client-side functionality including:
  - Smooth scrolling for navigation links
  - Parallax effect on hero section
  - Scroll-based animations for sections and cards
  - Dynamic page title with current time

### Assets
- **assets/color.gif** - Visual asset used in the project

## Design Principles

The project follows these web development best practices:

1. **Separation of Concerns** - HTML structure, CSS presentation, and JavaScript behavior are kept in separate files
2. **Maintainability** - Each file has a single, clear responsibility making it easier to update and debug
3. **Performance** - External CSS and JavaScript files can be cached by browsers
4. **Scalability** - The modular structure makes it easy to add new features or pages
5. **Clean Code** - Reduced the main HTML file from 675 lines to 165 lines

## Making Changes

### To modify styles:
Edit `css/styles.css`

### To modify functionality:
Edit `js/main.js`

### To modify content or structure:
Edit `index.html`

### To add new assets:
Place them in the `assets/` directory and reference them in HTML or CSS

## Development

To test the website locally:
```bash
# Using Python 3
python3 -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## Deployment

The website is configured for deployment on DigitalOcean App Platform using the configuration in `.do/` directory.
