# AIID Website Deployment Checklist

## Pre-Deployment

### Content Review
- [ ] All evidence citations accurate and sourced
- [ ] Complaint templates reviewed by legal counsel
- [ ] Contact information current
- [ ] Copyright dates correct
- [ ] No placeholder text remaining

### Technical Setup
- [ ] Domain configured (digitaldichotomy.com/aiid)
- [ ] SSL certificate installed (Let's Encrypt)
- [ ] HTTPS enforced (redirect HTTP to HTTPS)
- [ ] Form handling configured (Formspree/Netlify)
- [ ] 404 page created

### SEO & Meta
- [ ] Open Graph tags added to all pages
- [ ] Twitter Card meta added
- [ ] XML sitemap generated
- [ ] robots.txt created
- [ ] Favicon created and linked

### Security
- [ ] CSP headers configured
- [ ] X-Frame-Options: DENY
- [ ] X-Content-Type-Options: nosniff
- [ ] Referrer-Policy: strict-origin
- [ ] Security.txt created

## Deployment Steps

### 1. Upload Files
```bash
# Option A: GitHub Pages
git init
git add .
git commit -m "Initial AIID deployment"
git push origin main

# Option B: Netlify CLI
netlify deploy --prod --dir=.

# Option C: Manual FTP
# Upload all files to web root via FTP/SFTP
```

### 2. Configure Forms
- Sign up for Formspree or enable Netlify Forms
- Update form action URLs in HTML files
- Test all forms submit correctly
- Set up email notifications

### 3. Domain & DNS
- Configure DNS A/AAAA records
- Set up www redirect
- Enable CDN (Cloudflare recommended)
- Configure caching rules

### 4. Testing
- [ ] All pages load correctly
- [ ] Navigation works on all pages
- [ ] Mobile responsive test
- [ ] Form submissions received
- [ ] SSL certificate valid
- [ ] No mixed content warnings
- [ ] 404 page functional

## Post-Deployment

### Monitoring
- [ ] Uptime monitoring (UptimeRobot)
- [ ] Error logging (Sentry optional)
- [ ] Analytics (Plausible or none - avoid Google)

### Launch
- [ ] Announce on social media
- [ ] Email press list
- [ ] Submit to Hacker News, Reddit r/privacy, r/inventors
- [ ] Notify EFF, EPIC, other advocacy orgs
- [ ] Update legal coalition contacts

### Maintenance Schedule
- **Weekly**: Check for broken links, form functionality
- **Monthly**: Review and update evidence
- **Quarterly**: Security review, dependency updates
- **Annually**: Full content audit

## Emergency Contacts

- **Technical Issues**: [Your contact]
- **Legal Questions**: [Attorney contact]
- **Press Inquiries**: press@digitaldichotomy.com
- **Security Reports**: security@digitaldichotomy.com

---

**Launch Date Target**: April 2026  
**Primary Domain**: digitaldichotomy.com/aiid  
**Backup Domain**: [TBD]
