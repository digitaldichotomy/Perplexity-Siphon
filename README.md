# AIID - Architecture of AI Invention Disclosure

> **Note:** Perplexity offers a Patents feature, and Perplexity itself warns that sharing IP there is unsafe.

## Overview

This repository contains the complete AIID **7-stage extraction pipeline** evidence and complaint website. The site documents findings about Perplexity.ai and similar AI chat platforms that allegedly harvest intellectual property through dedicated "Patents" features.

This README documents the complete AIID investigation website, including architecture, content structure, and deployment instructions.

## The Core Finding

Perplexity.ai operates a systematic IP extraction pipeline:

1. **Lure** - "Patents" feature invites invention sharing
2. **Capture** - Technical details logged and stored
3. **Review** - Human reviewers and AI analyze content
4. **Train** - Proprietary ideas become training data
5. **Monetize** - Enterprise deals with resource-rich entities
6. **Invalidate** - Prior art creation destroys patent rights
7. **Erase** - Original creator's involvement deleted

## Site Structure

```
Perplexity-Siphon/
├── index.html                 # Main investigation page
├── complaint-template.html    # FTC/EFF complaint templates
├── protection-guide.html      # IP protection guide
├── press-kit.html             # Media resources
├── legal-coalition.html       # Attorney coalition signup
├── research.html              # Academic research portal
├── timeline.html              # Investigation timeline
├── testimonials.html          # Affected inventor stories
├── glossary.html              # Legal & technical glossary
├── sitemap.html               # Site navigation map
├── privacy.html               # Privacy policy
├── terms.html                 # Terms of use
├── disclaimer.html            # Legal disclaimer
├── assets/
│   └── css/
│       └── style.css          # Main stylesheet
├── manifest.json              # Site manifest
├── README.md                  # This file
└── PROJECT_SUMMARY.md         # Project overview
```

## Key Pages

### index.html (Main Investigation)
- **Purpose:** Main landing page presenting the complete investigation
- **Sections:** Hero, 7-stage pipeline, Evidence (Perplexity screenshots), Formal Complaint, Take Action, Resources
- **Evidence:** 5 Perplexity chat screenshots, April 2, 2026 (01:54:52, 02:03:01, 02:05:16, 02:05:24, 02:05:28), and Doe v. Perplexity AI, Inc., Meta Platforms, Inc., and Google, LLC, No. 3:26-cv-02803
- **Design:** 6 evidence cards (admission, retention, prior art, contradiction, lawsuit, "safe" alternative)

### complaint-template.html
- **Purpose:** Helps users file their own complaints
- **Includes:** FTC, EFF, and attorney general templates
- **Features:** Copy-to-clipboard, downloadable PDF format

### protection-guide.html
- **Purpose:** Teaches inventors to protect IP from AI extraction
- **Includes:** Provisional patents, NDAs, zero-retention tools, documentation strategies

### press-kit.html
- **Purpose:** Media resources for journalists
- **Includes:** PR boilerplate, fact sheet (7 stages, 1 lawsuit, 100% data retention admitted, 0% confidentiality), timeline, downloadable assets, media inquiry form

### legal-coalition.html
- **Purpose:** Attorney signup for class-action coordination
- **Includes:** Practice area selection, bar number, mailto link

### research.html
- **Purpose:** Academic research collaboration portal
- **Includes:** Research questions, submission portal, mailto link

### timeline.html
- **Purpose:** Chronological investigation timeline
- **Includes:** Key events from 2025-2026, annotated dates

### testimonials.html
- **Purpose:** Affected inventor stories
- **Note:** No verified testimonials are published here.

### glossary.html
- **Purpose:** Definitions of key legal and technical terms
- **Includes:** Architecture, prior art, CCPA, FTC Act, etc.

## Design System

### Colors
- **Primary background:** `#0a0a0f` (Near black)
- **Secondary:** `#12121a` (Dark panel)
- **Tertiary:** `#1a1a2e` (Card background)
- **Primary text:** `#e0e0e0` (Light gray)
- **Accent red:** `#ff2a6d` (Alerts, warnings)
- **Accent cyan:** `#05d9e8` (Links, highlights)

### Typography
- Primary: System sans-serif stack
- Monospace: 'Courier New' (terminal effects)
- Glitch effects on hero text
- Uppercase for navigation and tags

### Effects
- Glitch animation on main title
- Glowing borders on alerts
- Hover transforms on cards
- Smooth scroll navigation
- Fade-in scroll animations

---

## Deployment

### Option 1: Static Hosting (Recommended)
Upload all files to:
- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- AWS S3 + CloudFront

### Option 2: Traditional Web Host
Upload via FTP/SFTP to your web root.

### Option 3: Docker
```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
```

### Domain Configuration
1. Point domain to hosting provider
2. Enable HTTPS (Let's Encrypt)
3. Configure CDN for global distribution
4. Set up form handling (see below)

---

## Form Handling

Forms use mailto links to open the user's email client. No form data is sent to a form-handling service.

---

## SEO & Meta

All pages include:
- Descriptive `<title>` tags
- Meta descriptions
- Semantic HTML structure
- Mobile-responsive viewport
- Fast loading (no external dependencies except fonts)

Recommended additions:
- Open Graph tags for social sharing
- Twitter Card meta
- Structured data (JSON-LD)
- XML sitemap
- robots.txt

---

## Security Considerations

1. **No AI Integration**: This site contains NO AI chat features to avoid the very extraction it documents.
2. **No Tracking**: No Google Analytics, Facebook Pixel, or third-party trackers
3. **Minimal Cookies**: Only essential session management if forms implemented
4. **HTTPS Only**: All resources should load over HTTPS
5. **CSP Headers**: Implement Content Security Policy to prevent XSS

---

## Maintenance

### Updating Content
- Update `index.html` Evidence section with new verified screenshots
- Add new timeline events to `timeline.html`
- Update legal documents as cases progress

### Adding Pages
1. Create new HTML file using existing structure
2. Link from navigation and `sitemap.html`
3. Add to `manifest.json` pages array
4. Update this README

### Performance
- Minify CSS/JS for production
- Optimize images (WebP format)
- Enable gzip compression
- Use CDN for static assets

---

## Contributing

We welcome contributions from:
- Legal researchers and patent attorneys
- Inventors and entrepreneurs
- Web developers and designers
- Journalists and documentarians

### How to Contribute
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request with detailed description
5. Await review

---

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**.

You are free to:
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material

Under the following terms:
- **Attribution** — You must give appropriate credit
- **NonCommercial** — You may not use the material for commercial purposes
- **ShareAlike** — If you remix, transform, or build upon the material, you must distribute your contributions under the same license

See LICENSE file for full terms.

---

## Contact

### Digital Dichotomy
- **Email:** aiid@digitaldichotomy.com
- **Press:** press@digitaldichotomy.com
- **GitHub:** [github.com/digitaldichotomy/Perplexity-Siphon](https://github.com/digitaldichotomy/Perplexity-Siphon)

---

## Acknowledgments

- **Electronic Frontier Foundation** — Privacy advocacy
- **US Patent and Trademark Office** — Patent resources
- **Class-action plaintiffs** — Courage to challenge
- **Open-source community** — Tools and frameworks

**Built with urgency. Built with purpose. Built to protect inventors.**
