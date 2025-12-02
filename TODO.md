# TOFU LIST

1. Get buttons to work /dining/beauty/
2. Front hero image resorty
3. Footer tweaks
4. Dining Pic Tweaks (hotpocket)
5. return to top / and/or menu sticky
6. footer details
7. Content for Events/Dining(menu)

```html
<div class="back-to-top-box">
  <button class="back-to-top" aria-label="Back to top">
	<svg class="back-to-topicon" aria-hidden="true" focusable="false" width="28" height="47" viewBox="0 0 28 47" fill="none" xmlns="http://www.w3.org/2000/svg">
		<path d="M6 8.82715L14 1.00106" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">				</path>
		<path d="M22 8.82715L14 1.00106" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
		</path>
		<path d="M14 21L14 1" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
		</path>
		<path d="M2.94 41V33.41H0.36V31.25H8.1V33.41H5.52V41H2.94ZM13.2027 41.18C12.5227 41.18 11.9027 41.065 11.3427 40.835C10.7927 40.605 10.3177 40.275 9.9177 39.845C9.5277 39.405 9.2227 38.87 9.0027 38.24C8.7827 37.6 8.6727 36.88 8.6727 36.08C8.6727 35.28 8.7827 34.57 9.0027 33.95C9.2227 33.32 9.5277 32.795 9.9177 32.375C10.3177 31.945 10.7927 31.62 11.3427 31.4C11.9027 31.18 12.5227 31.07 13.2027 31.07C13.8727 31.07 14.4877 31.18 15.0477 31.4C15.6077 31.62 16.0827 31.945 16.4727 32.375C16.8727 32.805 17.1827 33.33 17.4027 33.95C17.6227 34.57 17.7327 35.28 17.7327 36.08C17.7327 36.88 17.6227 37.6 17.4027 38.24C17.1827 38.87 16.8727 39.405 16.4727 39.845C16.0827 40.275 15.6077 40.605 15.0477 40.835C14.4877 41.065 13.8727 41.18 13.2027 41.18ZM13.2027 38.96C13.7927 38.96 14.2527 38.705 14.5827 38.195C14.9227 37.675 15.0927 36.97 15.0927 36.08C15.0927 35.19 14.9227 34.505 14.5827 34.025C14.2527 33.535 13.7927 33.29 13.2027 33.29C12.6127 33.29 12.1477 33.535 11.8077 34.025C11.4777 34.505 11.3127 35.19 11.3127 36.08C11.3127 36.97 11.4777 37.675 11.8077 38.195C12.1477 38.705 12.6127 38.96 13.2027 38.96ZM19.4784 41V31.25H23.0484C23.5784 31.25 24.0834 31.305 24.5634 31.415C25.0434 31.515 25.4634 31.695 25.8234 31.955C26.1834 32.205 26.4684 32.54 26.6784 32.96C26.8984 33.37 27.0084 33.88 27.0084 34.49C27.0084 35.09 26.8984 35.605 26.6784 36.035C26.4684 36.465 26.1834 36.82 25.8234 37.1C25.4634 37.37 25.0484 37.575 24.5784 37.715C24.1084 37.845 23.6184 37.91 23.1084 37.91H22.0584V41H19.4784ZM22.0584 35.87H22.9884C23.4984 35.87 23.8734 35.75 24.1134 35.51C24.3634 35.27 24.4884 34.93 24.4884 34.49C24.4884 34.05 24.3534 33.74 24.0834 33.56C23.8134 33.38 23.4284 33.29 22.9284 33.29H22.0584V35.87Z" fill="white">
		</path>
	</svg>      
  </button>
</div>
```
can think of a better way to implement such things and maybe give us a step by step on how you would tackle these from a custom(twentytwentyfive) FSE block theme perspective.
Here's a step-by-step checklist for tackling your website polish, along with practical guides and suggestions for each item—focused on a custom Twenty Twenty-Five Full Site Editing (FSE) block theme. I'll prioritise actionable advice so you can efficiently finish before your presentation.

## Polish Checklist \& Practical Steps

### 1. **Get Buttons to Work (/dining/, /beauty/)**

- **Check Block Assignment**: Are your "Dining" and "Beauty" buttons made with the Button block in the FSE editor? Double-check that their URLs are correctly set (`/dining/`, `/beauty/`).
- **Test Button Functionality**: Publish and test each button in a live/preview environment, checking that navigation works.
- **Troubleshooting FSE Issues**
- If links aren’t working, ensure your menu or button block is inside a Navigation or Groupblock,and check for custom JS that might interfere.
- In some FSE builds, `Button` blocks require explicit URL settings in the sidebar—double-check there.

### 2. **Front Hero Image: "Resorty" Look**

- **Add Hero via Cover Block**:
    - In FSE, choose the Cover block and set your hero image. For a resort look: use high-quality, bright images (palms, pools, open skies).
- **Theme Branding**: Follow your brand style guide (theexemplar.com.au colors: gold, blue, white, slight resort tropical vibes).[^2]
- **Styling Tips**:
    - Overlay heading text with an accent color.
    - Add padding/margin using block settings.
    - Use block patterns to easily swap out hero images if reviewing with clients.

### 3. **Footer Tweaks**

- **Edit in Site Editor**:
    - Go to Appearance → Editor (Site Editor), select Footer template part.
- **Content \& Styling**:
    - Insert footer navigation, contact info, copyright.
    - Adjust font sizes, spacing, and colors using settings from your style guide (try soft-white backgrounds, gold or navy text).
- **Custom Block**:
    - Use a Columns block for multi-section footers (menu links, contact, legal, socials).
    - Use the Social Icons block for quick links.


### 4. **Dining Pic Tweaks ("hotpocket")**

- **Image Block Enhancements**:
    - Place dining images in relevant sections using Image, Gallery, or Media \& Text blocks.
    - Ensure images have appropriate alt text for accessibility.
    - Crop and resize images inside WordPress for sharper presentation.
    - Use border-radius to create rounded corners for a modern effect.

***

### 5. **Return to Top / Sticky Menu**

#### **Back-to-Top Button (HTML/JS Approach)**

Use your provided markup, then add simple JavaScript:

```html
<button class="back-to-top" aria-label="Back to top">
  <!-- SVG -->
</button>
<script>
document.querySelector(".back-to-top").onclick = function() {
  window.scrollTo({ top: 0, behavior: "smooth" });
};
</script>
```

- **Placement**: Put the block at the end of your template (footer) or use FSE's Group block to float it on all pages.
- **FSE Integration**: Make a custom block pattern containing your button and SVG for reuse.


#### **Sticky Menu (CSS Only)**

```css
.site-header {
  position: sticky;
  top: 0;
  background: var(--soft-white);
  z-index: 99;
}
```

- **In the FSE Editor**: Add custom CSS via Appearance → Editor → Styles → Additional CSS.
- Works best on the main header/navigation.

***

### 6. **Footer Details**

- **Double-check Content**: Ensure all legal, contact info, and social links are correct.
- **Style Consistency**: Reference your brand's color variables (see style guide).
- **Accessibility**: Check contrast and font sizes.

***

### 7. **Content for Events/Dining (Menu)**

#### **Gathering Content**

- **Events**: List sample events for the hotel or dining (e.g., weddings, conferences, wine nights).
- **Dining Menu**: Add a sample menu for OBriens Restaurant (see Solution Report \& meeting notes).
    - Example:
        - Starters: Garlic Bread, Oysters Kilpatrick
        - Mains: Grilled Barramundi, Filet Mignon
        - Desserts: Tiramisu, Pavlova
- **Block Recommendations**:
    - For Menus: Use the List block for menu items, with bold headings for sections.
    - For Events: Use the Query Loop block to show upcoming events or featured items.

***

### 8. **Back-to-Top Button Implementation (improvement)**

- **Consider a Core Pattern**: In Twenty Twenty-Five, make a pattern for your back-to-top button so editors can insert/remove on any page.
- **Accessible SVG**: Confirm your SVG uses `aria-hidden="true"` for icons, and your button includes an accessible label.
- **Style Button**:
    - Use your color variables from the style guide.
    - Add focus/hover states for accessibility.

***

### 9. **General FSE Polish Workflow**

#### **Step-by-Step for Polish in FSE Block Theme**

1. **Review major sections in Site Editor (Header, Footer, Page Templates)**
2. **Add/adjust blocks as needed (Button, Cover, Image, List, Query Loop)**
3. **Consistency check with style guide (colors, spacings, fonts)**
4. **Test navigation and functionality in preview mode**
5. **Mobile responsiveness**: Use WordPress's preview toggle for different screen sizes.
6. **Accessibility check**: Ensure buttons have labels, images have alt text, and keyboard navigation works.

***

## Suggestions for Custom FSE Block Themes

- **Custom Patterns**: Use patterns for reusable sections (hero, footer, menu).
- **Style Variations**: Take advantage of FSE's global styles; apply your branding system (soft whites, copper gold, navy, resort imagery).[^2]
- **Block-based Approach**:
    - Stick to core blocks unless truly necessary; custom blocks can be added but require careful style matching.
- **Accommodate Non-Tech Editors**: Make patterns easy to find and edit. Name them intuitively.
- **Accessibility**: FSE makes it easy to add ARIA labels, alt text, and keyboard focus.

***

## References

1. [Virtual Block Style Guide] Style variables, recommended colors and block patterns (see *styleshit.md*).
2. [Wireframe Meeting Notes] General page flow, hotel sections, events suggestions (see *20250505wireframes-monday1031.txt*).
3. [Hotel Solution Report] Brand, content for dining/events, page suggestions, technical recommendations (see *Solutions-Report-C.pdf*).

***

## Final Advice

- Start by ticking off each item in preview mode, making small changes and saving as you go.
- Use your theme’s FSE tools for layout and patterns.
- Lean on your style guide for consistency.
- Test everything in a real browser—including mobile.
- Confirm accessibility basics before handover.

If you need a more concrete example or code sample (like a reusable back-to-top block, sticky header CSS, or a sample dining menu block), let me know exactly which section you’d like a detailed walk-through for!




