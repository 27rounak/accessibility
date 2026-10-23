# Experiment 4: SEO and Accessibility Optimization

Compare `before.html` with `after.html`.

| Problem in before.html | Fix in after.html | Benefit |
|---|---|---|
| No `<!DOCTYPE>`, no `lang` | `<!DOCTYPE html>` and `<html lang="en">` | Valid HTML, screen readers pick correct language |
| Title is just "Page" | Descriptive `<title>` with keywords | Shown in search results and browser tabs |
| No meta description | `<meta name="description">` | Snippet shown in search results |
| No viewport meta | `<meta name="viewport">` | Mobile-friendly rendering |
| All `<div>`s | `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>` | Semantic structure helps crawlers and assistive tech |
| Headings are styled divs | One `<h1>`, then `<h2>` sections in order | Proper heading hierarchy |
| Image has no alt | Descriptive `alt`, width, height | Accessibility, image SEO, no layout shift |
| Links say "click here" | Meaningful link text (Home, Menu, Contact) | Better for SEO and screen readers |
| No Open Graph tags | `og:title`, `og:description`, `og:image` | Rich previews when shared |
| No canonical link | `<link rel="canonical">` | Avoids duplicate-content issues |
| No keyboard help | "Skip to main content" link, `aria-label` on nav, label tied to input | Keyboard and screen reader accessibility |

## How to verify
1. Open `after.html` in Chrome, press F12, open **Lighthouse**, run audit for SEO and Accessibility.
2. Run the same audit on `before.html` and compare scores (note both in your record).
3. Validate the markup at https://validator.w3.org/
