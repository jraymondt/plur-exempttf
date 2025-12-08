# initial blocks of spam, punched through a re-tooled reality tunnel for semester 2 of our summer of love experiments

Creating a WordPress block theme from scratch involves building a theme that leverages the Full Site Editing (FSE) capabilities of WordPress, primarily relying on blocks and the theme.json file for configuration and styling.
Steps to create a blank block theme

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

Here's a rewritten version that's current and in your voice for the next team:

***

# WordPress Block Theme Implementation Notes

Look, I'm going to be straight with you. We built this thing using WordPress Full Site Editing (FSE) block theme architecture. It works, it looks good, Keith likes it. But here's the reality: FSE is probably not what you learned in your WordPress classes, and that's going to make your life harder than it needs to be.

## What We Actually Built

This is a custom block theme called "the-exemplar" that uses WordPress's FSE capabilities. The entire site is built using blocks and the theme.json configuration file instead of traditional PHP templates.

**Current Status:**

- Theme is live and functional at theexemplar.com.au
- Basic page structure complete (home, restaurant, spa, events, facilities, attractions)
- Styling system implemented with CSS custom properties
- Login link to Laravel application working
- Mobile responsive

**What's Not Done:**

- Some content still needs Keith's final approval
- Images not fully optimized
- No caching plugin installed
- Accessibility not comprehensively tested
- Performance optimization needed
- linking front and backend


## The FSE Situation - What You Need to Know

### Why This Might Be a Problem

Traditional WordPress development uses PHP template files (header.php, footer.php, etc.) and the theme customizer. That's probably what you learned.

FSE uses:

- HTML template files instead of PHP
- theme.json for configuration instead of functions.php
- Site Editor interface instead of theme customizer
- Block patterns instead of template parts

If this sounds unfamiliar, that's because it's newer WordPress tech that hasn't made it into most TAFE coursework yet.

### Your Options

You've got three legitimate paths here:

**1. Keep the FSE Theme**

- Means teaching yourself FSE concepts outside of class
- WordPress documentation exists but it's learning curve is real
- Everything works currently, so maintenance is the main concern

**2. Convert to Classic Theme**

- Use something like Astra Pro, OceanWP, or Hotel WP
- Aligns with what you learned in class
- Way more documentation and support available
- Would take 2-3 weeks to rebuild to current state

**3. Add a Page Builder**

- Chuck Elementor on top of what's there
- Visual editing, no code needed
- Makes content updates way easier
- Your call on complexity vs ease of use

**My Take:** If FSE is making things harder instead of easier, change it. Keith cares about the end result, not the technical implementation. Do what works for your team's skillset and timeline.

## Current Theme Structure

```
/wp-content/themes/the-exemplar
├── style.css              # Theme info and base styles
├── theme.json             # Core configuration (this is the big one)
├── functions.php          # Limited functions (not like classic themes)
├── templates/             # HTML template files
│   ├── index.html
│   ├── page.html
│   └── single.html
└── parts/                 # Reusable template parts
    ├── header.html
    └── footer.html
```


## The Styling System

All styling uses CSS custom properties. This actually makes things easier once you understand it - change a variable, change it everywhere.

### Brand Colors

```css
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
  
  /* UI feedback colours - use sparingly */
  --accent: #e67e22;         /* Orange */
  --success: #2ecc71;        /* Green */
  --warning: #f1c40f;        /* Yellow */
  --danger: #e74c3c;         /* Red */
  --info: #3498db;           /* Blue */
}
```

These colors came from Keith's spec: "upper echelon four-star, Claremont kids" aesthetic. Think Smith Beach resort vibes.

### Spacing System

Responsive spacing using viewport units (vmin):

```css
:root {
  --space-xxs: calc(0.125rem + 0.1vmin); /* 2px base */
  --space-xs: calc(0.25rem + 0.2vmin);   /* 4px base */
  --space-sm: calc(0.5rem + 0.3vmin);    /* 8px base */
  --space-md: calc(1rem + 0.5vmin);      /* 16px base */
  --space-lg: calc(1.5rem + 0.7vmin);    /* 24px base */
  --space-xl: calc(2rem + 1vmin);        /* 32px base */
  --space-2xl: calc(3rem + 1.5vmin);     /* 48px base */
}
```

Yeah, the naming is a bit abstract. Feel free to rename these to something that makes more sense to you. They're just variables.

### Typography Scale

Also responsive using vmin:

```css
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
}

h1 {
  font-size: var(--font-size-3xl);
  font-weight: 700;
}

h2 { font-size: var(--font-size-2xl); }
h3 { font-size: var(--font-size-xl); }
```

**Fonts:**

- Body and headings: Montserrat (Google Fonts)
- Logo: Pristina, MS Sans Serif

Originally considered Playfair Display for feature headings but ended up sticking with Montserrat for consistency.

### Navigation Styling

```css
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
    color: var(--copper-gold) !important;
    text-decoration: underline;
}

/* Logo styling */
.custom-logo {
    max-height: 60px;
    width: auto;
    height: auto;
    vertical-align: middle;
    transition: all 0.3s ease;
}

/* Smaller on mobile */
@media (max-width: 767.98px) {
    .custom-logo {
        max-height: 40px;
    }
}
```


## Logo Assets

Current logo files in `/assets/img/`:

- `exemplar-logo-vig.svg` - Vector format, scales perfectly
- `exemplar-logo-vig.webp` - Web format for compatibility

**What's Missing:**
We talked about having multiple logo variations but only have the one. If you need monochrome or white versions for dark backgrounds, you'll need to create them or ask Keith.

## File Organization Standards

These matter for maintainability:

**Folder Structure:**

- Group by type: `/css` `/js` `/images` `/fonts` `/includes`
- Keep it flat, don't nest too deep (affects URLs)
- Use kebab-case for folder names

**File Naming:**

- Always kebab-case: `perth-sunset-beach.jpg`
- No spaces, no special characters
- All lowercase
- Date prefix for chronological files: `20251209-meeting-notes.pdf`
- Version suffixes: `policy-v1.pdf`, `policy-v2.pdf`
- Descriptive names for SEO: `margaret-river-winery.jpg` not `IMG_1234.jpg`

This isn't just being pedantic - it affects SEO, accessibility, and whether you can find shit six months from now.

## Core Brand Guidelines

From Keith's brief and our interpretation:

**Brand Values:**

- Excellence
- Hospitality
- Growth
- Elegance
- Professionalism

**Design Aesthetic:**
"Upper echelon four-star, Claremont kids" - sophisticated but approachable. Not budget resort, not ultra-luxury. Think nice Margaret River accommodation.

**Site Purpose:**
This is a fictional resort website that provides realistic context for the document management system. It needs to look professional enough that people believe it's real (they tried to book rooms during testing), but forms intentionally don't work to prevent confusion.

## What Actually Needs Doing

### Before This Goes Live

**Critical:**

- Finalize content with Keith (some pages still have placeholder text)
- Optimize all images (many are way too large)
- Install and configure caching plugin (WP Super Cache or W3 Total Cache)
- Test all booking forms redirect to "unavailable" messages correctly
- Accessibility audit and fixes (WCAG 2.1 compliance)
- Set up proper backup system with off-site storage

**Important:**

- Performance testing and optimization
- Mobile testing on actual devices
- Cross-browser testing (Chrome, Firefox, Safari, Edge)
- Verify login link to Laravel works smoothly
- Security scan and hardening

**Nice to Have:**

- Minify CSS/JS
- Implement lazy loading for images
- Consider CDN if performance becomes issue


### Ongoing Maintenance

**Weekly:**

- Check for WordPress/plugin updates
- Verify backups are running

**Monthly:**

- Test backup restoration
- Review performance metrics
- Check error logs

**Quarterly:**

- Security audit
- Content review with Keith
- User feedback evaluation


## Things That Will Trip You Up

**Forms Are Intentionally Broken:**
All booking forms are designed to look functional but redirect to "not accepting bookings" messages. Keith specifically requested this because people tried to book actual holidays during testing. Don't "fix" them - they're working as intended.

**WordPress and Laravel Are Separate:**
The login link in the header goes to the Laravel app at `/intranet`. WordPress users and Laravel users are completely separate databases. Logging into WordPress admin doesn't give you Laravel access.

**Search Engine Visibility:**
Currently set to discourage search engines. This is intentional during development but needs to be changed before going live if Keith wants public visibility.

**ScreenCraft Hosting Limits:**
We're on a student hosting package with limited bandwidth and storage. If this goes into real production use, you'll need to request increases from Adrian Gould at ScreenCraft.

## If You Need to Modify Things

### Changing Colors

Edit the CSS variables in theme.json or your custom CSS:

```css
--midnight-navy: #YourNewColor;
```

That's it. Changes everywhere that variable is used.

### Adding Pages

Use the WordPress block editor like normal. The FSE theme provides the structure, blocks provide the content.

### Modifying Templates

Templates are in `/templates/` as HTML files. Edit them in the Site Editor (Appearance → Editor in WordPress admin). This is the part that's different from traditional WordPress.

### Custom CSS

Add to style.css in the theme folder or use WordPress customizer's additional CSS section.

## Resources If You're Sticking With FSE

**WordPress Documentation:**

- Block themes: wordpress.org/documentation/article/block-themes/
- FSE handbook: developer.wordpress.org/block-editor/
- Theme.json reference: developer.wordpress.org/block-editor/reference-guides/theme-json-reference/

**Reality Check:**
FSE documentation is less comprehensive than classic theme docs. You'll be figuring some things out through trial and error. That's frustrating but not unusual with newer WordPress tech.

## Resources If You're Converting Away From FSE

**Hotel Themes to Consider:**

- Astra Pro - Highly customizable, good docs
- OceanWP - Fast, has hotel demos
- Hotel WP - Purpose-built for hospitality
- Bellevue - Resort-focused

**Page Builders:**

- Elementor Pro - Most popular, drag-and-drop
- Beaver Builder - Clean code
- WPBakery - Large community

All of these align better with what you learned in class and have way more support resources.

## My Honest Assessment

The site looks good. Keith's happy with it. It does what it's supposed to do - provides a realistic hotel website facade for the document management system.

The FSE implementation was a choice that seemed reasonable during development but creates a knowledge gap for typical TAFE WordPress coursework. That's a real issue.

If maintaining this in FSE becomes a pain in the ass because it doesn't match what you learned in class, you should change it. Convert to a classic theme, add a page builder, do whatever makes it maintainable for your team.

Keith cares about the result working for students, not about preserving any particular technical architecture. Make the decision that's right for your situation and timeline.

## Contact

If you've got questions about why things were done a certain way or need clarification:

**James Thompson**

- j344988@tafe.wa.edu.au
- flatlinejim@jraymondt.com

Available for handover questions via email. Can't do long-term maintenance for you, but happy to explain decisions and help troubleshoot the handover period.

***

**Bottom Line:** This works, but FSE might not be the right long-term solution for a student-maintained project. Evaluate your team's skills and available support, then make the call that works for you. There's no ego here about keeping things a certain way - just get it working in a sustainable manner for the people who'll actually be maintaining it.

