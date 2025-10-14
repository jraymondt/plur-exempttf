# initial blocks of spam, punched through a re-tooled reality tunnel for semester 2 of our summer of love experiments

Creating a WordPress block theme from scratch involves building a theme that leverages the Full Site Editing (FSE) capabilities of WordPress, primarily relying on blocks and the theme.json file for configuration and styling.
Steps to create a blank block theme

## Set up your development environment

Ensure you have a local WordPress installation running.

- create a new folder for your theme (e.g., my-block-theme)
- Add style.css: Inside your theme folder, basic theme information

```css

/*
    Theme Name: bloxemplar
    Description: A custom WordPress block theme.
    Version: 0.1
    Author: A-Team
    Text Domain: bloxemplar
*/

```

## Create theme.json

This is the core configuration file for your block theme, defining global styles, settings, and block-specific configurations.

```json

    {
        "version": 2,
        "settings": {
            "color": {
                "palette": [
                    {
                        "slug": "primary",
                        "color": "#007cba",
                        "name": "Primary"
                    }
                ]
            },
            "typography": {
                "fontFamilies": [
                    {
                        "fontFamily": "sans-serif",
                        "name": "Sans Serif",
                        "slug": "sans-serif"
                    }
                ]
            }
        },
        "styles": {
            "color": {
                "text": "var(--wp--preset--color--primary)",
                "background": "#ffffff"
            }
        }
    }
```

## Create template files

Block themes use HTML files for templates. Common templates include:

- index.html: The main template for displaying posts.
- page.html: For static pages.
- single.html: For single posts.
- header.html, footer.html: For reusable header and footer parts (often placed in a parts folder).

## Create a templates folder and place these HTML files inside

These files will primarily contain block markup.

## Activate the theme

In your WordPress admin dashboard, navigate to Appearance > Themes and activate your newly created theme.

## Start building with blocks (punch them through those holes)

Use the WordPress Block Editor (Full Site Editing interface) to design your site by adding and arranging blocks within your templates. The theme.json settings will influence the available styles and options within the editor.

## HERE IS SOME STYLE

This document outlines the official style guide for The Exemplar WordPress theme. It provides comprehensive guidelines for maintaining brand consistency across all visual and written communications.

## Core Values

- Excellence
- Hospitality
- Growth
- Elegance
- Professionalism

## Brand Identity

- Logo
- The Exemplar's logo embodies elegance and professionalism.

## Logo Variations

This is the hand we have

![logo](assets/img/exemplar-logo-vig.svg)

![webp logo](assets/img/exemplar-logo-vig.webp)

For compatibility sake we may need to consider:

- Primary logo (full colour)
- Monochrome (black)
- Reverse (white for dark backgrounds)
- Compact/favicon version

## CSS

```SCSS
:root {
    
}
  

/* Navigation */

.navbar {
    background-color: var(--midnight-navy);
    color: var(--soft-white);
}

.nav-link {
    color: var(--soft-white) !important;
    text-decoration: none;
    font-weight: 500;
    margin: 0 10px;
    transition: all 0.3s;
}

.nav-link:hover {
    color:  var(--copper-gold) !important;
    text-decoration: underline;
}

/* Logo styling */
.custom-logo-link {
    display: inline-block;
    padding: 0;
    margin: 0;
}

.custom-logo {
    max-height: 60px; /* Adjust this value as needed */
    width: auto;
    height: auto;
    vertical-align: middle;
    transition: all 0.3s ease;
}

/* For small screens */
@media (max-width: 767.98px) {
    .custom-logo {
        max-height: 40px; /* Smaller on mobile */
    }
}

/* For the navbar brand container */
.site-branding.navbar-brand {
    display: flex;
    align-items: center;
    padding: 0;
}

/*******************************************************
 * custom styles for the wp hotel website
 *******************************************************/

```

### colours

```SCSS
:root {
    /* Primary colours */
  --midnight-navy: #2C3E50;  /* Professional, trustworthy */
  --copper-gold: #B08D57;    /* Excellence, prestige */
  
  /* Secondary colours */
  --warm-sand: #F4E1C1;      /* Comfort, hospitality */
  --sage-green: #A8C3A0;     /* Growth, learning */
  
  /* Neutral colours */
  --soft-white: #FAFAFA;     /* Clean, modern background */
  --dark-text: #212529;
  --grey-text: #818285;      /* Primary text colour */
  
  /* UI feedback colours */
  --accent: #e67e22;         /* Orange (use sparingly) */
  --success: #2ecc71;        /* Green */
  --warning: #f1c40f;        /* Yellow */
  --danger: #e74c3c;         /* Red */
  --info: #3498db;           /* Blue */
  }
  ```

### spacing

```SCSS
:root {
  --space-xxs: calc(0.125rem + 0.1vmin); /* 2px+ */
  --space-xs: calc(0.25rem + 0.2vmin);  /* 4px+ */
  --space-sm: calc(0.5rem + 0.3vmin);   /* 8px+ */
  --space-md: calc(1rem + 0.5vmin);     /* 16px+ */
  --space-lg: calc(1.5rem + 0.7vmin);   /* 24px+ */
  --space-xl: calc(2rem + 1vmin);       /* 32px+ */
  --space-2xl: calc(3rem + 1.5vmin);    /* 48px+ */
}
```

## fonts

```SCSS
:root {
/* Base font sizes with vmin for better responsiveness */
  --font-size-xs: calc(0.75rem + 0.2vmin);   /* Small text */
  --font-size-sm: calc(0.875rem + 0.3vmin);  /* Secondary text */
  --font-size-base: calc(1rem + 0.4vmin);    /* Body text */
  --font-size-lg: calc(1.25rem + 0.5vmin);   /* Small headings */
  --font-size-xl: calc(1.5rem + 0.7vmin);    /* H3 */
  --font-size-2xl: calc(2rem + 0.9vmin);     /* H2 */
  --font-size-3xl: calc(2.5rem + 1.1vmin);   /* H1 */
}

body {
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  font-size: var(--font-size-base);
  color: var(--dark-text);
  background-color: var(--soft-white);
  line-height: 1.6;
}

h1, h2, h3, h4, h5 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  color: var(--copper-gold);
  line-height: 1.2;
  margin-bottom: 0.8em;
  text-shadow: var(--space-xxs) var(--space-xxs) 0 rgba(24, 3, 3, 0.213);
}

h1 {
  font-size: var(--font-size-3xl);
  font-weight: 700;
}

h2 {
  font-size: var(--font-size-2xl);
}

h3 {
  font-size: var(--font-size-xl);
}

.feature-heading {
  font-weight: 700;
}

.small-text {
  font-size: var(--font-size-sm);
}

.xsmall-text {
  font-size: var(--font-size-xs);
}

.divider {
    width: 80px;
    height: 3px;
    background-color: var(--soft-white);
    margin: 1.5rem auto;
}

.accordion-header {
    font-family: 'Lato', sans-serif;
}

```

### Secondary Font: Playfair Display

Feature headings: Playfair Display Bold (700)
Quotes: Playfair Display Italic (400)

### Logo fonts

- Pristina
- MS Sans Serif

## Folder Structure

- Group assets by type /css /js /images /fonts /includes
- *no spaces* use `kebab-case`
- Do not nest directories too deep, avoid long URLs

## File naming

- *No spaces* use `kebab-case`
- Machine readable
- no special characters
- lower case for consistancy
- Date `YYYYMMDD` for automatic file sorting chronology
- version append `example-v1.file`
- Descriptive keywords for SEO and accessibility `(perth-skyline-sunset.jpg instead of IMG_1234.jpg)`