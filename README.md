# Hash it Out Website

A professional marketing website for the Hash it Out debate application.

## Overview

This website serves as the main marketing and support hub for Hash it Out, featuring:
- **Home Page** (`index.html`) - Marketing page with features, pricing, and download CTAs
- **Support Page** (`support.html`) - FAQs and contact information
- **Privacy Policy** (`privacy.html`) - Comprehensive privacy policy

## Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Modern, responsive styling with CSS Grid and Flexbox
- **Vanilla JavaScript** - Interactive elements (mobile menu, FAQ accordion, animations)
- **No dependencies** - Pure HTML/CSS/JS for fast loading and easy hosting

## File Structure

```
HashItOut-Site/
├── index.html          # Main marketing page
├── support.html        # Support and FAQ page
├── privacy.html        # Privacy policy page
├── styles.css          # Main stylesheet
├── script.js           # JavaScript for interactivity
├── images/             # Image assets directory
│   └── README.md       # List of required images
└── README.md           # This file
```

## Required Images

The website currently has placeholders for the following images. Replace these with actual assets:

### Logo and Branding
- `logo.png` (40x40px) - App logo for navigation

### App Store Badges
- `app-store-badge.png` - Apple App Store download badge
- `google-play-badge.png` - Google Play Store download badge

### Hero Section
- `hero-mockup.png` - Main hero image showing app interface

### Feature Icons (60x60px recommended)
- `icon-turn-based.png` - Turn-based debates icon
- `icon-ai.png` - AI analysis icon
- `icon-evidence.png` - Evidence-based icon
- `icon-voting.png` - Voting system icon
- `icon-community.png` - Community icon
- `icon-notifications.png` - Notifications icon

### How It Works Steps
- `step-1.png` - Create/join debate screenshot
- `step-2.png` - Present argument screenshot
- `step-3.png` - Turn-based exchange screenshot
- `step-4.png` - Debate conclusion screenshot

### Support Page Icons
- `icon-email.png` - Email support icon
- `icon-bug.png` - Bug report icon
- `icon-feedback.png` - Feedback icon

### Social Media Icons
- `icon-twitter.png` - Twitter/X logo
- `icon-facebook.png` - Facebook logo
- `icon-linkedin.png` - LinkedIn logo

## Color Scheme

The website uses the following color palette:

- **Primary**: #2563eb (Blue)
- **Secondary**: #10b981 (Green)
- **Accent**: #f59e0b (Orange)
- **Text Primary**: #1f2937 (Dark Gray)
- **Text Secondary**: #6b7280 (Medium Gray)
- **Background**: #ffffff (White)
- **Background Light**: #f9fafb (Light Gray)

## Email Addresses

The following email addresses are used throughout the site (configured for hashitout.net domain):

- **support@hashitout.net** - General support inquiries
- **bugs@hashitout.net** - Bug reports
- **feedback@hashitout.net** - User feedback and suggestions
- **privacy@hashitout.net** - Privacy-related inquiries

## Responsive Design

The website is fully responsive with breakpoints at:
- **Desktop**: 992px and above
- **Tablet**: 768px - 991px
- **Mobile**: 767px and below

## Features

### Navigation
- Sticky header with smooth scroll
- Mobile-responsive hamburger menu
- Active page highlighting

### Hero Section
- Gradient background
- App mockup display
- Clear call-to-action buttons
- App store badges

### Features Grid
- 6 key features with icons
- Hover animations
- Responsive grid layout

### How It Works
- 4-step process with alternating layout
- Step numbers with gradient backgrounds
- Screenshot placeholders

### Pricing
- 3-tier pricing cards
- "Most Popular" badge on mid-tier
- Hover effects and animations

### Support Page
- Contact information cards
- Comprehensive FAQ with accordion functionality
- 6 categories of questions

### Privacy Policy
- Professional legal page layout
- Sidebar navigation (desktop)
- GDPR and CCPA compliance sections

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Deployment

This is a static website and can be hosted on:
- **Netlify** - Drop the folder or connect to Git
- **Vercel** - Deploy via CLI or Git integration
- **GitHub Pages** - Push to a GitHub repo
- **Any web server** - Upload via FTP/SFTP

### Recommended: Netlify Deployment

1. Sign up for a free Netlify account
2. Drag and drop the `HashItOut-Site` folder
3. Configure custom domain (hashitout.net)
4. Enable HTTPS (automatic with Netlify)

## Customization

### Updating Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-color: #2563eb;
    --secondary-color: #10b981;
    /* etc. */
}
```

### Updating Content
- Main marketing copy: `index.html`
- FAQs: `support.html`
- Privacy policy: `privacy.html`

### Adding New Pages
1. Create new HTML file
2. Copy header and footer from existing pages
3. Link stylesheet and script
4. Add navigation link

## Performance

The website is optimized for performance:
- No external dependencies
- Minimal CSS and JavaScript
- Images are placeholders (optimize when adding real images)
- Lazy loading can be added for images if needed

## SEO

The website includes:
- Meta descriptions on all pages
- Semantic HTML structure
- Proper heading hierarchy
- Alt text placeholders for images

## Accessibility

- Semantic HTML elements
- ARIA labels where appropriate
- Keyboard navigation support
- Sufficient color contrast
- Responsive text sizing

## Testing Checklist

Before going live, test:
- [ ] All navigation links work
- [ ] Mobile menu opens and closes
- [ ] FAQ accordions expand/collapse
- [ ] Smooth scrolling works
- [ ] All email links are correct
- [ ] Responsive design on mobile, tablet, desktop
- [ ] Images display correctly (when added)
- [ ] App store links point to correct locations (when published)

## Future Enhancements

Consider adding:
- Terms of Service page
- Blog section for debate tips and updates
- User testimonials/reviews
- Press/media kit section
- Analytics integration (Google Analytics, Plausible)
- Newsletter signup form
- Live chat support widget

## Support

For questions about the website:
- Email: support@hashitout.net
- Issues: Create an issue in the project repository

## License

© 2025 Hash it Out. All rights reserved.

---

**Last Updated**: October 22, 2025
**Version**: 1.0
