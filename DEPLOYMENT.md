# 🚀 Deployment Guide for 3Brothers Bikeshop Website

## Pre-Deployment Checklist

### ✅ Files Created
- [x] `robots.txt` - Search engine crawler instructions
- [x] `sitemap.xml` - Site structure for search engines
- [x] `404.html` - Custom error page
- [x] `.htaccess` - Apache server configuration
- [x] SEO meta tags added to all pages

### 📝 Before Going Live

1. **Update Domain URLs**
   - Replace `https://yourdomain.com` in:
     - `robots.txt` (line 10)
     - `sitemap.xml` (all `<loc>` tags)
     - All HTML files (Open Graph meta tags)

2. **Add Favicon Files**
   - Create/add `favicon.ico` to root directory
   - Optional: Add `apple-touch-icon.png` (180x180px)
   - Use a tool like [favicon.io](https://favicon.io) to generate from logo

3. **Configure .htaccess**
   - Uncomment HTTPS redirect lines (lines 7-8) once SSL is active
   - Test rewrite rules work on your server

4. **Verify Contact Information**
   - Phone: (213) 275-1830
   - Address: 3008 S Vermont Ave, Los Angeles, CA 90007
   - Update if needed

5. **Test All Links**
   - Navigation links
   - Footer links
   - External links (maps, social media)
   - Phone number click-to-call

## Deployment Methods

### Option 1: Traditional Hosting (Hostinger, Bluehost, etc.)
```bash
# Via FTP/SFTP:
1. Upload all files to public_html or www directory
2. Ensure .htaccess is uploaded (may be hidden)
3. Set file permissions: 644 for files, 755 for directories
```

### Option 2: GitHub Pages
```bash
# Push to GitHub and enable Pages
git add .
git commit -m "Ready for deployment"
git push origin main

# Then: Settings → Pages → Select branch: main → Save
```

### Option 3: Netlify (Recommended for beginners)
```bash
# Option A: Drag & Drop
1. Go to app.netlify.com
2. Drag your project folder
3. Done!

# Option B: Git Integration
1. Push to GitHub
2. Connect Netlify to your repo
3. Deploy settings: Build command: (none), Publish directory: /
```

### Option 4: Vercel
```bash
vercel --prod
```

## Post-Deployment Tasks

### SEO Setup
1. **Google Search Console**
   - Add and verify your site
   - Submit sitemap: `https://yourdomain.com/sitemap.xml`

2. **Google My Business**
   - Claim/update your business listing
   - Add photos, hours, location

3. **Analytics**
   - Add Google Analytics 4 tracking code
   - Add to `<head>` section of all pages:
   ```html
   <!-- Google Analytics -->
   <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
   <script>
     window.dataLayer = window.dataLayer || [];
     function gtag(){dataLayer.push(arguments);}
     gtag('js', new Date());
     gtag('config', 'G-XXXXXXXXXX');
   </script>
   ```

### SSL Certificate
- Most hosts provide free SSL (Let's Encrypt)
- After SSL is active, uncomment HTTPS redirect in `.htaccess`

### Performance Testing
- [Google PageSpeed Insights](https://pagespeed.web.dev/)
- [GTmetrix](https://gtmetrix.com/)
- [Lighthouse](https://developers.google.com/web/tools/lighthouse) (in Chrome DevTools)

### Browser Testing
- Chrome, Firefox, Safari, Edge
- Mobile devices (iOS & Android)
- Check responsive design at different screen sizes

## Maintenance

### Regular Updates
- Update hours/prices as needed
- Check broken links monthly
- Update sitemap lastmod dates when content changes
- Monitor Google Search Console for issues

### Backup
- Keep local backup of all files
- Use Git for version control
- Consider automated backups from hosting provider

## Troubleshooting

### .htaccess not working?
- Server might not support mod_rewrite
- Contact hosting support or remove .htaccess temporarily

### 404 page not showing?
- Check server configuration
- Ensure 404.html is in root directory

### SEO not working?
- Wait 2-4 weeks for Google to index
- Submit sitemap in Google Search Console
- Check robots.txt isn't blocking pages

## Support

For website issues, contact the developer.
For business updates, edit HTML files directly or contact your developer.

---

**Live Date**: _[Add date when live]_  
**Last Updated**: January 2, 2026
