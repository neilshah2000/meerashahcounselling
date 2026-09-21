# Meera Shah Counselling — website

Single-page static site (plain HTML + CSS, one small inline script for the mobile menu). No build step.

```
index.html          the site — hero + sections: #home, #about-counselling-and-psychotherapy,
                    #about-me, #faq, #testimonials, #contact
css/style.css       all styles; tokens at the top of :root
images/             portrait, BACP/PSA badges, hero background
privacy/            privacy policy page  (DRAFT — see TODO inside)
cookies/            cookies page
_redirects          Netlify-style 301s from the old WebHealer URLs
<old-slug>/         redirect shims (meta refresh + canonical) for hosts without redirect support:
                    about-me/, faq/, testimonials/, about-counselling-and-psychotherapy/,
                    contact-form/, privacy_notice/, privacy-policy/, pagek/, website-cookies/
old/                everything pulled from the original site — source HTML, images, extracted
                    copy (content.md) and design tokens (design-tokens.css)
```

## Preview locally

    python3 -m http.server 8000
    open http://localhost:8000/

## Before launch

1. **Contact form backend** — `index.html` form `action` is a placeholder. Point it at Formspree / Netlify Forms / your own handler (fields: `name`, `email`, `phone`, `message`, `consent`).
2. **Privacy policy** — `privacy/index.html` is a draft skeleton; the old site had none. Meera to complete (retention period, date).
3. **Hi-res headshot** — `images/meera-portrait.jpg` is 300×451 from the old site; ask for a larger original.
4. **Credentials** — the copy says UKCP accredited (home/about) and BACP registered (FAQ/badge). Confirm both are current.
5. If hosting on Netlify/Cloudflare, **delete the shim folders** — static files are served before `_redirects` is consulted, so the 301s never fire while they exist. On plain hosting keep the shim folders and ignore `_redirects`.
