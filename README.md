# Popy Website

A minimalist, responsive marketing website for Popy - a home for all the misfits.

## Project Structure

```
popy-website/
├── index.html              # Main landing page
├── manifesto.html          # Full manifesto/story page
├── privacy.html            # Privacy policy
├── support.html            # FAQ and support page
├── css/
│   └── styles.css          # All styles (responsive, optimized)
├── js/
│   └── main.js             # Animations and interactions
├── public/
│   └── images/
│       ├── logo.png        # Popy logo (add your logo here)
│       ├── favicon.png     # Favicon (add your favicon here)
│       └── illustrations/  # SVG illustrations (optional)
└── ref_docs/               # Reference documentation
    ├── base_reference.html
    ├── privacy.md
    └── website_idea.md
```

## Features

- **Minimalist Design**: Clean, calm aesthetic with generous whitespace
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Teal Brand Color**: Subtle use of #0F766E throughout the design
- **Stacked Card Animation**: Smooth scroll-triggered card reveal on homepage
- **Local-First Philosophy**: Emphasizes privacy and local data storage
- **Performance Optimized**: No external dependencies, minimal JavaScript

## Pages

### 1. Homepage (index.html)
- Hero section with tagline "A home for all the misfits"
- Download section (macOS primary, Chrome extension secondary)
- Feature cards with scroll animation (Reads, Finds, Notes, Meetings, Voice, Tasks)
- "Misfits" section explaining the problem
- Privacy highlight
- Final CTA

### 2. Manifesto (manifesto.html)
- Full story and philosophy
- Product explanation
- Privacy commitment
- Download CTA

### 3. Privacy Policy (privacy.html)
- Comprehensive privacy policy
- Local-first architecture explanation
- Data handling transparency
- Summary table

### 4. Support (support.html)
- FAQ section (12 common questions)
- Contact support form link
- Email: hello@getpopy.com

## Brand Colors

```css
--color-teal: #0F766E;          /* Primary brand color */
--color-teal-dark: #0d6660;     /* Hover states */
--color-teal-light: #14b8a6;    /* Accents */
--color-teal-subtle: rgba(15, 118, 110, 0.1); /* Backgrounds */
```

## Setup Instructions

### 1. Add Your Logo
Place your Popy logo file in:
- `public/images/logo.png` (recommended: 200-300px width, transparent background)
- `public/images/favicon.png` (recommended: 32x32px or 64x64px)

### 2. Update Download Links
In `index.html`, replace the placeholder download links:
```html
<!-- Line ~55 and ~339 -->
<a href="#" class="btn btn-primary">Download for macOS</a>
```
Update `href="#"` with your actual download URL.

### 3. Optional: Add Support Form
In `support.html`, you can replace the email link with a form service:
- Tally: https://tally.so
- Typeform: https://typeform.com
- Google Forms
- ConvertKit

### 4. Test Responsive Design
Open the website in a browser and test:
- Desktop (1200px+)
- Tablet (800px - 1200px)
- Mobile (< 800px)
- Small mobile (< 550px)

### 5. Deploy
Upload all files to your web hosting service, maintaining the folder structure.

## Development

### No Build Process Required
This is a static website with no build tools needed. Just open `index.html` in a browser.

### Live Server (Optional)
For development with live reload:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve

# Using VS Code
# Install "Live Server" extension and click "Go Live"
```

Then visit: `http://localhost:8000`

## Customization

### Colors
All colors are defined as CSS variables in `css/styles.css` (lines 14-23). Modify these to match your brand.

### Typography
Font stack is defined in `--font-stack` variable. Currently using system fonts for performance.

### Animations
Card stacking animation parameters can be adjusted in `js/main.js` (lines 50-80).

## Browser Support

- Chrome/Edge (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Mobile Safari (iOS 12+)
- Chrome Mobile (Android 8+)

## Performance

- **No external dependencies**: Pure HTML/CSS/JS
- **Optimized animations**: Uses CSS transforms and `requestAnimationFrame`
- **Responsive images**: Images with fallbacks
- **Minimal JavaScript**: ~150 lines of vanilla JS

## Accessibility

- Semantic HTML structure
- Proper heading hierarchy
- Focus states on interactive elements
- Alt text for images
- Keyboard navigation support

## Contact

For questions or support:
- Email: hello@getpopy.com
- Website: [Your website URL]

## License

[Add your license information here]

---

**Made with care for people who save things.**
