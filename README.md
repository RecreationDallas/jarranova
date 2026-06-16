# Jarranova — Marketing Site

A single-page marketing site for Jarranova, a strategic advisory firm. Static HTML/CSS with a small amount of vanilla JavaScript (scroll reveals + mobile menu). No build step, no dependencies.

## Live site

- Production: https://jarranova.netlify.app

## Structure

```
.
├── index.html        # the entire page (markup + CSS + JS inline)
├── netlify.toml       # hosting config: publish dir, security & cache headers
├── assets/            # logos, icons, and the headshot
│   ├── wordmark.svg          # JARRANOVA wordmark (hero)
│   ├── wordmark-footer.svg   # JARRANOVA wordmark (footer)
│   ├── logo-mark.svg         # "J" mark
│   ├── hero-divider.svg      # hero divider line
│   ├── hero-star.svg         # hero nova star
│   ├── cta-star.svg          # closing CTA star
│   ├── linkedin.svg          # LinkedIn icon
│   └── headshot.jpg          # Marissa Jarratt photo
└── README.md
```

## Editing & previewing

It's a plain HTML file — open `index.html` in any browser to preview locally. All styles and scripts are inline in that one file.

Fonts load from Google Fonts (Bricolage Grotesque, Poppins, Cormorant Garamond).

## Deploying

Hosted on Netlify. To publish changes:

```bash
netlify deploy --prod --dir .
```

### Notes
- **Replacing an image in place** (same filename): browsers cache assets for a day,
  so bump the version query on its `src` (e.g. `headshot.jpg?v=3`) to force an
  immediate refresh for everyone.
- Contact CTAs open `mailto:hello@jarranova.com`.
