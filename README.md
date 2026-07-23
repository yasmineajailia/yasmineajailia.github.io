# Portfolio — Yasmine Laajailia

An interactive desktop-style portfolio: draggable windows, a dock, and a
soft animated wallpaper. Data science and NLP work, presented as a small
operating system.

**Live:** https://yasmineajailia.github.io/portfolio/


## Built with

Plain HTML, CSS and JavaScript in a single file — no framework, no build
step, no dependencies. Canvas for the sparkle layer, CSS custom properties
for theming, and `IntersectionObserver`-free window management.

Supports light and dark themes (follows the system setting, with a toggle
in the menu bar) and respects `prefers-reduced-motion`.

## Running locally

Open `index.html` in a browser. That's it.

## Deploying

The site is one static file, so any static host works. For GitHub Pages:

1. **Settings → Pages**
2. **Source:** Deploy from a branch
3. **Branch:** `main`, folder `/ (root)`

## Contact form

The form opens the visitor's own mail client with the message pre-composed —
this needs no server, so it works on GitHub Pages as-is.

To deliver messages straight to an inbox instead, sign up for a free form
service such as [Formspree](https://formspree.io), then in `index.html`:

```html
<!-- replace this -->
<form id="contact-form">
<!-- with this -->
<form id="contact-form" action="https://formspree.io/f/YOUR_ID" method="POST">
```

The script skips its `mailto:` handling whenever the form has an `action`,
so no other changes are needed.
