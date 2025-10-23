# Image Assets Required for Hash it Out Website

This document outlines all image assets needed for the website to function properly.

## Website Pages

The Hash it Out website consists of the following pages:
- `index.html` - Main landing page
- `privacy.html` - Privacy Policy
- `terms.html` - Terms of Service
- `support.html` - Support/Help Center
- `delete-account.html` - Account Deletion Instructions (required for Google Play/App Store compliance)

---

## Image Specifications

### 1. Logo and Branding

#### logo.jpg
- **Size**: 40x40px (or higher resolution for retina displays: 80x80px)
- **Format**: PNG with transparency
- **Usage**: Navigation bar logo
- **Description**: Hash it Out app logo/icon

---

### 2. App Store Badges

#### app-store-badge.svg
- **Size**: 120x40px (standard badge size)
- **Format**: PNG
- **Usage**: Hero section and download section
- **Description**: Official Apple App Store download badge
- **Download from**: https://developer.apple.com/app-store/marketing/guidelines/#downloadOnAppstore

#### google-play-badge.png
- **Size**: 135x40px (standard badge size)
- **Format**: PNG
- **Usage**: Hero section and download section
- **Description**: Official Google Play Store badge
- **Download from**: https://play.google.com/intl/en_us/badges/

---

### 3. Hero Section

#### hero-mockup.jpg
- **Size**: 800x1000px (or higher)
- **Format**: PNG
- **Usage**: Main hero section showcasing the app
- **Description**: Mockup of the Hash it Out app interface, preferably showing:
  - Multiple phones with different screens (debate list, debate view, profile)
  - Professional presentation on gradient or transparent background
  - High-quality rendering
- **Alternative**: Create using tools like Figma, Sketch, or online mockup generators

---

### 4. Feature Icons

All feature icons should be:
- **Size**: 60x60px minimum (or SVG for scalability)
- **Format**: PNG with transparency or SVG
- **Style**: Consistent, minimal, monochrome (will be colored via CSS filter)

#### icon-turn-based.svg
- **Description**: Icon representing turn-based debates
- **Suggestions**: Clock with arrows, alternating arrows, timer icon

#### icon-ai.svg
- **Description**: AI/machine learning icon
- **Suggestions**: Brain with circuit, robot head, neural network pattern

#### icon-evidence.svg
- **Description**: Evidence-based discussion icon
- **Suggestions**: Document with checkmark, magnifying glass over document, citation symbol

#### icon-voting.svg
- **Description**: Voting/rating system icon
- **Suggestions**: Thumbs up/down, star rating, slider scale

#### icon-community.svg
- **Description**: Community engagement icon
- **Suggestions**: Group of people, connected users, forum/discussion icon

#### icon-notifications.svg
- **Description**: Push notifications icon
- **Suggestions**: Bell, notification badge, alert symbol

**Free Icon Resources**:
- Heroicons: https://heroicons.com/
- Font Awesome: https://fontawesome.com/
- Feather Icons: https://feathericons.com/
- Lucide: https://lucide.dev/

---

### 5. How It Works Section

Screenshots should show actual app functionality:
- **Size**: 375x812px (iPhone size) or 600x1000px
- **Format**: PNG
- **Quality**: High resolution, clear text

#### step-1.png
- **Description**: Create or join a debate screen
- **Should show**: 
  - Debate creation form OR
  - Browse debates screen with "Apply" buttons

#### step-2.png
- **Description**: Presenting an argument
- **Should show**: 
  - Argument composition screen
  - Evidence addition interface
  - Rich text editor

#### step-3.png
- **Description**: Turn-based exchange in progress
- **Should show**: 
  - Debate view with multiple turns
  - Back-and-forth argument display
  - Voting interface

#### step-4.png
- **Description**: Concluded debate with insights
- **Should show**: 
  - Debate summary
  - AI-generated analysis
  - Vote results/statistics

---

### 6. Support Page Icons

#### icon-email.png
- **Size**: 60x60px
- **Description**: Email/envelope icon

#### icon-bug.png
- **Size**: 60x60px
- **Description**: Bug/insect icon for bug reports

#### icon-feedback.png
- **Size**: 60x60px
- **Description**: Feedback icon (megaphone, speech bubble, etc.)

---

### 7. Social Media Icons

#### icon-twitter.png
- **Size**: 24x24px
- **Format**: PNG with white/transparent background
- **Description**: Twitter/X logo
- **Download**: Official X brand resources

#### icon-facebook.png
- **Size**: 24x24px
- **Format**: PNG with white/transparent background
- **Description**: Facebook logo
- **Download**: Official Facebook brand resources

#### icon-linkedin.png
- **Size**: 24x24px
- **Format**: PNG with white/transparent background
- **Description**: LinkedIn logo
- **Download**: Official LinkedIn brand resources

---

## Quick Creation Guide

### Option 1: Using Figma (Recommended)
1. Create mockups in Figma
2. Export at 2x or 3x resolution for retina displays
3. Use Figma's export features for proper sizing

### Option 2: Using Screenshot Tools
1. Take screenshots of your actual app
2. Use tools like Mockuphone.com or Smartmockups.com to add device frames
3. Resize and optimize using tools like TinyPNG

### Option 3: Using Stock Resources
- Unsplash (https://unsplash.com/) - Free stock photos
- Pexels (https://pexels.com/) - Free stock photos
- Mockup World (https://www.mockupworld.co/) - Free mockup templates

### Option 4: Hire a Designer
- Fiverr - Budget-friendly designers
- Upwork - Professional designers
- 99designs - Design contests

---

## Image Optimization

Before adding images to the website:

1. **Compress images** using:
   - TinyPNG (https://tinypng.com/)
   - ImageOptim (Mac)
   - Squoosh (https://squoosh.app/)

2. **Use appropriate formats**:
   - PNG for logos, icons (with transparency)
   - JPG for photos, screenshots
   - SVG for simple icons (scalable)
   - WebP for modern browsers (optional)

3. **Naming convention**:
   - Use lowercase
   - Use hyphens for spaces
   - Be descriptive: `hero-mockup.jpg` not `image1.png`

4. **Target file sizes**:
   - Icons: < 50KB each
   - Screenshots: < 200KB each
   - Hero image: < 300KB
   - Badges: < 20KB each

---

## Temporary Placeholders

Until you have the final images, you can use:

1. **Placeholder services**:
   - https://via.placeholder.com/800x1000/667eea/ffffff?text=Hero+Mockup
   - https://dummyimage.com/800x1000/667eea/fff&text=Hero

2. **Icon placeholder**:
   - Use emoji temporarily (📱, 🤖, 📊, etc.)
   - Use Font Awesome icons via CDN

3. **App store badges**:
   - Download official badges from Apple and Google
   - Use black or white versions depending on background

---

## Installation Instructions

Once you have the images:

1. Save all images to the `images/` directory
2. Ensure filenames match exactly (case-sensitive):
   - `logo.jpg`
   - `app-store-badge.svg`
   - `google-play-badge.png`
   - etc.

3. Refresh the website to see the images load

4. Test on multiple devices to ensure images display correctly

---

## Priority Order

If you need to add images gradually, prioritize:

1. **High Priority** (website won't look right without these):
   - logo.jpg
   - app-store-badge.svg
   - google-play-badge.png
   - hero-mockup.jpg

2. **Medium Priority** (nice to have):
   - Feature icons (icon-*.png)
   - Step screenshots (step-*.png)

3. **Low Priority** (can be skipped initially):
   - Social media icons (can use text links temporarily)
   - Support page icons (can use emoji or text)

---

## Questions?

If you need help with image creation or have questions:
- Email: support@hashitout.net
- Refer to the main README.md for more information

---

## App Store Compliance

### Delete Account Page

The `delete-account.html` page is **required for Google Play and Apple App Store compliance**. Both app stores require apps to provide:

1. A clear way for users to request account deletion
2. Information about what data gets deleted
3. Timeline for deletion
4. Contact information for deletion requests

**URL for App Store Submission:**
```
https://hashitout.net/delete-account.html
```

This URL should be entered in:
- **Google Play Console:** App content > Privacy policy > Data safety > Account deletion
- **Apple App Store Connect:** App Privacy > Data deletion

---

**Last Updated**: October 23, 2025
