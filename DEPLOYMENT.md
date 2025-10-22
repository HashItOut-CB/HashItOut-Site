# Quick Deployment Guide - Hash it Out Website

This guide will help you deploy the Hash it Out website to a live domain (hashitout.net).

## Pre-Deployment Checklist

Before deploying, ensure you have:

- [ ] Added all required images to the `images/` folder (or placeholders)
- [ ] Updated app store links when your app is published
- [ ] Verified all email addresses work (@hashitout.net)
- [ ] Tested the website locally in multiple browsers
- [ ] Checked mobile responsiveness
- [ ] Reviewed all content for accuracy

## Recommended: Deploy to Netlify (Easiest)

Netlify offers free hosting with HTTPS and custom domains.

### Step 1: Sign Up
1. Go to https://www.netlify.com/
2. Click "Sign up" and create a free account

### Step 2: Deploy Site
**Option A: Drag and Drop**
1. Log into Netlify
2. Go to "Sites"
3. Drag the entire `HashItOut-Site` folder onto the deploy area
4. Wait for deployment (usually 30 seconds)
5. Your site is live at a temporary URL (e.g., `random-name-12345.netlify.app`)

**Option B: Connect to Git (Recommended for updates)**
1. Push your code to GitHub, GitLab, or Bitbucket
2. In Netlify, click "Add new site" > "Import an existing project"
3. Connect your Git provider
4. Select the repository
5. Deploy settings:
   - Build command: (leave empty)
   - Publish directory: `/` or `.`
6. Click "Deploy site"

### Step 3: Custom Domain (hashitout.net)
1. In Netlify, go to your site's settings
2. Click "Domain management" > "Add custom domain"
3. Enter: `hashitout.net`
4. Netlify will provide DNS records

### Step 4: Configure DNS
In your domain registrar (where you bought hashitout.net):

1. Add these DNS records:
   ```
   Type: A
   Name: @
   Value: 75.2.60.5
   
   Type: CNAME
   Name: www
   Value: [your-site-name].netlify.app
   ```

2. Or use Netlify's nameservers (easier):
   - Go to Netlify DNS settings
   - Copy the 4 nameservers (e.g., dns1.p01.nsone.net)
   - In your domain registrar, change nameservers to Netlify's

3. Wait 24-48 hours for DNS propagation (usually faster)

### Step 5: Enable HTTPS
1. In Netlify, go to "Domain management" > "HTTPS"
2. Click "Verify DNS configuration"
3. Click "Provision certificate" (free Let's Encrypt SSL)
4. Enable "Force HTTPS"

Your site is now live at https://hashitout.net! 🎉

---

## Alternative: Deploy to Vercel

Vercel is another excellent free hosting option.

### Steps:
1. Sign up at https://vercel.com/
2. Click "Add New Project"
3. Import your Git repository (or drag and drop folder)
4. Deploy settings:
   - Framework Preset: Other
   - Build Command: (leave empty)
   - Output Directory: `.`
5. Click "Deploy"
6. Add custom domain in settings (similar to Netlify)

---

## Alternative: GitHub Pages (Free)

Good for static sites, but requires a GitHub account.

### Steps:
1. Create a GitHub repository named `hashitout-website`
2. Push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/hashitout-website.git
   git push -u origin main
   ```
3. Go to repository Settings > Pages
4. Source: Deploy from branch
5. Branch: main, folder: / (root)
6. Save
7. Site will be live at: `yourusername.github.io/hashitout-website`

### Custom Domain:
1. Add a file named `CNAME` to the root with content: `hashitout.net`
2. Configure DNS at your registrar:
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   Value: 185.199.109.153
   Value: 185.199.110.153
   Value: 185.199.111.153
   
   Type: CNAME
   Name: www
   Value: yourusername.github.io
   ```

---

## Alternative: Traditional Web Hosting

If you have traditional web hosting (cPanel, Plesk, etc.):

### Via FTP:
1. Use an FTP client (FileZilla, Cyberduck)
2. Connect to your hosting account
3. Navigate to `public_html` or `www` directory
4. Upload all files from `HashItOut-Site` folder
5. Ensure `index.html` is in the root
6. Site should be live immediately

### Via cPanel:
1. Log into cPanel
2. Go to File Manager
3. Navigate to `public_html`
4. Upload files or use the Upload button
5. Extract if you uploaded a .zip file

---

## Post-Deployment Tasks

After your site is live:

### 1. Test Everything
- [ ] Visit https://hashitout.net
- [ ] Test all pages (home, support, privacy)
- [ ] Click all links
- [ ] Test mobile menu
- [ ] Test FAQ accordions
- [ ] Verify email links work
- [ ] Check on mobile devices

### 2. Set Up Email Forwarding
Configure email forwarding for @hashitout.net addresses:
- support@hashitout.net
- bugs@hashitout.net
- feedback@hashitout.net
- privacy@hashitout.net

This can usually be done in your domain registrar's control panel or through Google Workspace, Zoho Mail, or similar.

### 3. Add Analytics (Optional)
To track visitors:

**Google Analytics:**
```html
<!-- Add before </head> in all HTML files -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

**Or use privacy-friendly alternatives:**
- Plausible Analytics
- Fathom Analytics
- Simple Analytics

### 4. Submit to Search Engines
Help search engines find your site:
- Google Search Console: https://search.google.com/search-console
- Bing Webmaster Tools: https://www.bing.com/webmasters

### 5. Create Sitemap (Optional)
Create a `sitemap.xml` file:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://hashitout.net/</loc>
    <lastmod>2025-10-22</lastmod>
    <priority>1.0</priority>
  </url>
  <url>
    <loc>https://hashitout.net/support.html</loc>
    <lastmod>2025-10-22</lastmod>
    <priority>0.8</priority>
  </url>
  <url>
    <loc>https://hashitout.net/privacy.html</loc>
    <lastmod>2025-10-22</lastmod>
    <priority>0.5</priority>
  </url>
</urlset>
```

---

## Updating the Website

### If deployed via Netlify/Vercel with Git:
1. Make changes to your local files
2. Commit changes: `git commit -am "Update content"`
3. Push to GitHub: `git push`
4. Site auto-deploys in 30-60 seconds

### If deployed via drag-and-drop or FTP:
1. Make changes to local files
2. Re-upload changed files via Netlify drag-and-drop or FTP
3. Clear browser cache to see changes

---

## Troubleshooting

### Site Not Loading
- Check DNS settings (use https://dnschecker.org/)
- Verify nameservers are pointing to correct host
- Wait for DNS propagation (up to 48 hours)
- Clear browser cache and try incognito mode

### Images Not Showing
- Verify image filenames match exactly (case-sensitive)
- Check images are in the `images/` folder
- Verify image paths in HTML files
- Check browser console for 404 errors

### Mobile Menu Not Working
- Verify `script.js` is loading (check browser console)
- Ensure JavaScript is enabled
- Test in different browsers

### Email Links Not Working
- Verify email addresses are correct
- Check if email client is set up
- Test with different email clients

---

## Need Help?

If you encounter issues during deployment:

1. Check the hosting provider's documentation
2. Search for specific error messages
3. Contact your hosting provider's support
4. Email: support@hashitout.net

---

## Security Best Practices

Once live:
- [ ] Enable HTTPS (SSL certificate)
- [ ] Force HTTPS redirect
- [ ] Set up security headers (can be done in Netlify/Vercel)
- [ ] Keep backups of your website files
- [ ] Monitor for uptime (use UptimeRobot or similar)

---

## Cost Summary

**Free Options:**
- Netlify: Free (includes HTTPS, CDN, custom domain)
- Vercel: Free (includes HTTPS, CDN, custom domain)
- GitHub Pages: Free (requires GitHub account)

**Domain Name:**
- hashitout.net: ~£10-15/year (already owned)

**Optional Costs:**
- Email forwarding: Free to £5/month
- Analytics: Free to £10/month
- Premium hosting: £5-20/month (not needed for static site)

---

**Estimated Total Deployment Time:** 30-60 minutes  
**Technical Difficulty:** Beginner-friendly

Good luck with your deployment! 🚀
