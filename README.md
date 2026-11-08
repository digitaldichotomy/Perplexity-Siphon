# AIID - Architecture of AI Invention Disclosure
## Digital Dichotomy Investigation

> **Note:** Perplexity offers a Patents feature, and Perplexity itself warns that sharing IP there is unsafe.

---

## Overview

This multi-page website exposes the "7-Stage Extraction Pipeline" through which AI platforms like Perplexity.ai lure, capture, and monetize unprotected inventions—destroying patent rights and commodifying human genius.

### The Core Finding

Perplexity.ai maintains a dedicated "Patents" feature inviting inventors to share innovations, while **simultaneously admitting** in user interactions that:

- All chats are retained indefinitely and reviewed by humans
- Content is used to train AI models
- Sharing creates prior art that destroys patent rights
- Data is shared with third parties (Meta, Google)
- No attorney-client privilege or confidentiality protections exist

This is not a bug. This is the architecture of extraction.

## Site Structure

```
Perplexity-Siphon/
├── index.html                 # Main investigation
├── complaint-template.html    # FTC/EFF complaint
├── protection-guide.html      # IP protection strategies
├── terms.html                 # Terms of use
├── disclaimer.html            # Legal disclaimer
├── press-kit.html             # Media resources
├── legal-coalition.html       # Attorney coalition
├── research.html              # Research collaboration
├── sitemap.html               # Site map
├── timeline.html              # Investigation timeline
├── glossary.html              # Glossary of terms
├── testimonials.html          # Affected inventor stories
├── assets/css/style.css       # Main stylesheet
├── js/                        # JavaScript (Planned - not present in this repo)
└── images/                    # Screenshots (Planned - not present in this repo)
```

## Design System

### Color Palette

- **Background:** `#0a0a0f` (deep black)
- **Secondary:** `#12121a` (elevated surfaces)
- **Accent Red:** `#ff2a6d` (danger, alerts, extraction)
- **Accent Cyan:** `#05d9e8` (info, links, protection)
- **Accent Purple:** `#9d4edd` (legal, formal)
- **Text Primary:** `#e0e0e0` (headings)
- **Text Secondary:** `#a0a0b0` (body)

## Key Pages

### 1. Main Site
- **Hero:** Dramatic glitch title, "7 stages of extraction" stats
- **Pipeline:** 7-stage interactive flow diagram
- **Evidence:** 6 evidence cards with Perplexity admissions
- **Formal Complaint:** Full legal complaint text
- **Action Cards:** Share, File Complaint, Protect IP, Media, Legal, Research
- **Resources:** Links to USPTO, EFF, FTC, legal aid

### 2. Complaint Template
- Form templates for FTC, Attorney General, and USPTO
- Sections for personal info, incident details, evidence list
- Submission guidance and tracking

### 3. Protection Guide
- Steps to protect inventions before AI disclosure
- Provisional patent guidance
- NDA templates and strategies
- Zero-retention AI tools

### 4. Press Kit
- Boilerplate text for media use
- Fact sheet and statistics
- Key documents and evidence archive
- Downloadable assets (PDF, images)

### 5. Legal Coalition
- Attorney coalition signup
- Practice area selection
- Bar admission details
- Secure contact protocols

### 6. Research
- Academic research questions
- Case study methodology
- Submission portal for researchers
- Peer review coordination

## Typography
- **Primary:** System sans-serif stack
- **Code:** Monospace ('Courier New')
- **Headings:** Uppercase, letter-spaced

## Effects
- Glitch animation on hero title
- Glow effects on buttons and cards
- Hover transforms on interactive elements
- Smooth scroll navigation
- Fade-in on scroll

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

1. **Evidence**: New screenshots, admissions, case law
2. **Legal**: Complaint templates, legal analysis
3. **Technical**: Design improvements, accessibility
4. **Research**: Academic papers, data analysis
5. **Translation**: Multi-language versions

Contact: aiid@digitaldichotomy.com

---

## License

**Content**: CC BY-NC-SA 4.0 (Attribution-NonCommercial-ShareAlike)
**Code**: MIT License

**Exceptions**:
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

- **Electronic Frontier Foundation** (digital rights)
- **Stanford HAI** (AI ethics research)
- **Inventors Digest** (inventor advocacy)
- All affected inventors who shared their stories

---

**Preserve and Distribute. This is evidence.**

*Last Updated: April 2, 2026*
