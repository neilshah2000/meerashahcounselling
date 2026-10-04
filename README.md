# Meera Shah Counselling — website

Single-page static site (plain HTML + CSS, one small inline script for the mobile menu and contact form). No build step.

```
index.html          the site — hero + sections: #home, #about-counselling-and-psychotherapy,
                    #about-me, #faq, #testimonials, #contact
css/style.css       all styles; tokens at the top of :root
images/             portrait, BACP/PSA badges, hero background
privacy/            privacy policy page  (DRAFT — see TODO inside)
old/                everything pulled from the original site — source HTML, images, extracted
                    copy (content.md) and design tokens (design-tokens.css)
```

## Preview locally

    python3 -m http.server 8000
    open http://localhost:8000/

## Before launch

Search `index.html` for `TODO` — each item is marked in place.

1. **Contact form backend** — wired to Web3Forms with a *test* access key. Before launch, create the live key against info@meerashahcounselling.com and swap the `access_key` value in `index.html`.
2. **Email address** — none existed on the old site. A commented-out `<li>` in the contact section is ready to fill in.
3. **Credentials** — the site now says "Accredited Clinical Member (UKCP)" and "Registered Member (BACP)" consistently. Meera to confirm both are accurate and current.
4. **Reply time** — contact section promises a reply within two working days; Meera to confirm or change.
5. **Testimonials** — the two quotes from one client have been merged; add initials/context if clients consent.
6. **Inclusion paragraph** — the sentence about working with Black and minority ethnic clients was garbled on the old site and has been rewritten; Meera to check it says what she means.
7. **ADHD coaching** — the old headline mentioned it but nothing else on the site did. It's still in the `<title>`; add a sentence in the Welcome section if she offers it, or remove it from the title.
8. **Privacy policy** — `privacy/index.html` is a draft skeleton; the old site had none.
9. **Hi-res headshot** — `images/meera-portrait.jpg` is 300×451 from the old site.
