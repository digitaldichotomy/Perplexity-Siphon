# AIID - Architecture of AI Invention Disclosure
## Digital Dichotomy Investigation

**⚠️ WARNING: This site documents systematic intellectual property extraction by AI chat platforms. The evidence presented includes institutional self-incrimination by Perplexity.ai.**

---

## Overview

This multi-page website exposes the "7-Stage Extraction Pipeline" through which AI platforms like Perplexity.ai lure, capture, and monetize unprotected inventions—destroying patent rights and commodifying human genius.

### The Core Finding

Perplexity.ai maintains a dedicated "Patents" feature inviting inventors to share innovations, while **simultaneously admitting** in user interactions that:
- All chats are retained indefinitely and reviewed by humans
- Content is used to train AI models benefiting the platform's creators
- Sharing invention details creates prior art that destroys patent rights
- Data is shared with third parties (Meta, Google) without informed consent
- No attorney-client privilege or confidentiality protections exist

This is not a bug. This is the architecture of extraction.

---

## Site Structure

```
digitaldichotomy_aiid/
├── index.html                 # Main site - Hero, Pipeline, Evidence, Complaint
├── complaint-template.html    # Templates for FTC, AG, USPTO complaints
├── protection-guide.html      # Comprehensive IP protection strategies
├── press-kit.html            # Media resources and expert contacts
├── legal-coalition.html      # Attorney coalition signup
├── research.html             # Academic collaboration portal
├── privacy.html              # Privacy policy (minimal data collection)
├── terms.html                # Terms of use
├── disclaimer.html           # Legal disclaimer
└── assets/
    ├── css/
    │   └── style.css         # Dark cyberpunk theme, responsive
    ├── js/                   # (Future enhancements)
    └── images/               # (Add screenshots/evidence)
```

---

## Key Pages

### 1. Main Site (`index.html`)
- **Hero Section**: Glitch effects, key statistics, call-to-action
- **The Pipeline**: 7-stage extraction visualization
- **Evidence**: 6 smoking-gun cards with Perplexity admissions
- **Formal Complaint**: Full complaint to EFF/FTC
- **Action Cards**: 6 pathways for engagement
- **Resources**: Essential links for inventors

### 2. Complaint Template (`complaint-template.html`)
Ready-to-use templates for:
- Federal Trade Commission (FTC)
- State Attorney General
- USPTO Ombudsman

Includes filing instructions and customization guidance.

### 3. Protection Guide (`protection-guide.html`)
Comprehensive defensive strategies:
- Immediate actions if you've disclosed to AI
- Provisional patent filing (step-by-step)
- Documentation best practices
- NDA templates and usage
- AI safety rules (what NEVER to share)
- Monitoring for extraction

### 4. Press Kit (`press-kit.html`)
Resources for journalists:
- Story angles and quotes
- Downloadable assets (evidence archive, diagrams)
- Expert contacts
- Timeline and key documents
- Media inquiry contact

### 5. Legal Coalition (`legal-coalition.html`)
For attorneys interested in coordinated action:
- Target legal areas (FTC, privacy, patent interference)
- Relevant precedents (Cambridge Analytica, Andersen v. Stability AI)
- Coalition signup form
- Confidentiality protections

### 6. Research (`research.html`)
Academic collaboration portal:
- 6 research areas (platform analysis, legal framework, impact assessment)
- Publications and working papers
- Data repository access
- Researcher signup form

---

## Design System

### Color Palette
- **Background**: `#0a0a0f` (deep black)
- **Secondary**: `#12121a` (elevated surfaces)
- **Accent Red**: `#ff2a6d` (danger, alerts, extraction)
- **Accent Cyan**: `#05d9e8` (info, links, protection)
- **Accent Purple**: `#9d4edd` (legal, formal)
- **Text Primary**: `#e0e0e0` (headings)
- **Text Secondary**: `#a0a0b0` (body)

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

Current forms use `alert()` placeholders. For production:

### Option A: Formspree (Easiest)
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option B: Netlify Forms
Add `netlify` attribute to forms:
```html
<form name="coalition" netlify>
```

### Option C: Custom Backend
Deploy serverless functions (AWS Lambda, Vercel Functions) to handle submissions securely.

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

1. **No AI Integration**: This site contains NO AI chat features to avoid the very extraction it documents
2. **No Tracking**: No Google Analytics, Facebook Pixel, or third-party trackers
3. **Minimal Cookies**: Only essential session management if forms implemented
4. **HTTPS Only**: All resources should load over HTTPS
5. **CSP Headers**: Implement Content Security Policy to prevent XSS

---

## Maintenance

### Content Updates
- Update "Evidence" section as new admissions surface
- Add new lawsuit filings to timeline
- Expand "Resources" as tools emerge
- Publish research papers when available

### Technical Maintenance
- Monitor for broken links
- Update copyright year annually
- Review and update legal precedents
- Test forms quarterly

---

## Contributing

This is an open investigation. Contributions welcome:

1. **Evidence**: Additional platform admissions, screenshots
2. **Legal**: Case law, regulatory developments
3. **Technical**: Platform analysis, countermeasure development
4. **Research**: Academic papers, impact studies
5. **Translation**: Multi-language versions for global reach

Contact: aiid@digitaldichotomy.com

---

## License

Content: CC BY-NC-SA 4.0 (Attribution-NonCommercial-ShareAlike)
Code: MIT License

Exceptions: 
- Perplexity screenshots and quotes used under fair use for criticism/commentary
- Government documents in public domain

---

## Contact

**Investigation Lead**: MT Tech Industries / Digital Dichotomy  
**Email**: aiid@digitaldichotomy.com  
**Secure**: PGP key available upon request  
**Press**: press@digitaldichotomy.com  
**Legal**: legal@digitaldichotomy.com  
**Research**: research@digitaldichotomy.com

---

## Acknowledgments

This investigation builds on work by:
- Electronic Frontier Foundation (digital rights)
- Stanford HAI (AI ethics research)
- Inventors Digest (inventor advocacy)
- All affected inventors who shared their stories

---

**Preserve and Distribute. This is evidence.**

*Last Updated: April 2, 2026*
