# 🍰 CSS Fundamentals — The Magical Dessert Kitchen

A whimsical, dessert-themed guide to learning **CSS fundamentals**. Each chapter pairs a core CSS concept with a delicious pastry metaphor — from "CSS Fundamentals Sundae" to "Soufflé Surprise" — making the journey through styling both memorable and sweet.

> "Styled, structured, and rights reserved." — Reyrove

---

## 📖 What's Inside

Twelve chapters, each covering a foundational CSS topic with a sweet twist:

| # | Chapter | Dessert Metaphor | Concept |
|---|---------|------------------|---------|
| 1 | The Basics of Styling | 🍨 CSS Fundamentals Sundae | Syntax, selectors, properties |
| 2 | The Art of Colors and Backgrounds | 🎂 CSS Rainbow Cake | Colors, gradients, background images |
| 3 | Font Magic | 🍬 CSS Typography Macarons | Typography, fonts, text styling |
| 4 | Box of Secrets | 🍰 CSS Layer Cake | The box model (content, padding, border, margin) |
| 5 | Flexbox Feast | 🥐 CSS Éclair Delight | Flexbox layout |
| 6 | Grid Garden | 🍮 CSS Tiramisu Layers | CSS Grid layout |
| 7 | Advanced Styling | 🥟 CSS Choux Pastry Puffs | Pseudo-classes & pseudo-elements |
| 8 | Responsive Alchemy | 🥮 CSS Choux Pastry | Media queries & breakpoints |
| 9 | Animations and Transitions | 🍮 CSS Soufflé Surprise | CSS animations & transitions |
| 10 | The Power of Preprocessing | 🍮 CSS Crème Brûlée | Sass & Less |
| 11 | CSS Tricks and Hacks | 🍫 CSS Chocolate Fondant | Advanced techniques & CSS variables |
| 12 | The Future of CSS | 🍓 CSS Pavlova Perfection | New features (Subgrid, Houdini, Container Queries) |

---

## 🚀 Getting Started

### 1. Clone or download

```bash
git clone https://github.com/reyrove/HTML-Basics.git
cd HTML-Basics
```

Or simply download the ZIP and extract it.

### 2. Project structure

```
HTML-Basics/
├── index.html          # Main page — all 12 CSS chapters
├── desserts.css        # All styling (blue neon dark theme, responsive)
├── desserts.js         # Back-to-top button behavior
├── README.md
└── images/
    ├── fav.svg         # Favicon
    ├── dessert1.png    # Chapter 1 illustration
    ├── dessert2.png    # Chapter 2 illustration
    ├── ...
    └── dessert12.png   # Chapter 12 illustration
```

> ⚠️ **Important:** All chapter images **must** be placed inside the `images/` folder with the exact filenames shown above (`dessert1.png` … `dessert12.png`, lowercase). Filenames are case-sensitive on Linux and GitHub Pages.

### 3. Open it

Just double-click `index.html`, or serve it locally:

```bash
# Python 3
python -m http.server 8000

# or Node.js (npx)
npx serve .
```

Then visit `http://localhost:8000`.

---

## ✨ Features

- 🌌 **Dark theme** with a cool blue neon accent — easy on the eyes for long reading sessions
- 📱 **Fully responsive** — layouts adapt gracefully from desktop to small phones
- 🔝 **Smooth "Top" button** — appears after scrolling 100px with a soft glow, gently glides back to the top
- 📖 **Semantic HTML** — the site practices what it teaches (`<header>`, `<section>`, `<footer>`, etc.)
- 🖨️ **Code samples** — every chapter includes copy-friendly `<pre><code>` snippets
- 🍰 **Dessert metaphors** — complex CSS concepts explained through relatable pastry analogies
- ♿ **Accessible** — back-to-top button has `aria-label`, images have `alt` text

---

## 🛠️ Tech Stack

- **HTML5** — semantic markup
- **CSS3** — Flexbox, Grid, custom properties, media queries, animations
- **Vanilla JavaScript** — no frameworks, just a small enhancement for the back-to-top button
- **Google Fonts** — Playfair Display & Raleway
- **Font Awesome** & **Material Design Icons** — loaded for icon use

No build step. No dependencies to install. It just works.

---

## 🎨 Customization

### Change the accent color

In `desserts.css`, find the blue shades and replace them:

```css
/* Current accent */
color: #42a5f5;          /* headings, links, code */
background: #42a5f5;     /* back-to-top button */

/* Hover / darker shade */
color: #1e88e5;
background: #1e88e5;
```

### Change the background

```css
body {
    background-color: #121212;   /* page background */
}

.chapter {
    background-color: #1a1a1a;   /* chapter card */
    border: 1px solid #444444;   /* chapter border */
}
```

### Adjust the back-to-top trigger distance

In `desserts.js`:

```js
backToTopButton.classList.toggle('visible', scrollTop > 100);
//                                               ^^^ change this
```

### Change the button text

In `index.html`, find:

```html
<button id="backToTop" aria-label="Back to Top">Top</button>
```

Replace `Top` with any label you prefer.

---

## 📝 Adding a New Chapter

1. Copy an existing `<section class="chapter">` block in `index.html`.
2. Update the `<h1>`, `<p>` subtitle, and `<img src="images/dessertN.png">`.
3. Add your content inside `<div class="content">`.
4. Drop the new image into `images/` (e.g., `dessert13.png`).
5. Done — CSS and JS handle the rest automatically.

---

## ♿ Accessibility Notes

The site follows good semantic HTML practice:

- `<header>`, `<section>`, `<footer>` for landmark regions
- `<img>` tags include descriptive `alt` attributes
- The back-to-top button has an `aria-label`
- Color contrast (blue `#42a5f5` on dark `#121212`) meets WCAG AA for large text
- Button is keyboard-focusable and works with Enter/Space

If you extend the site, keep labels on form inputs, use real `<button>` elements, and preserve heading hierarchy (`h1` → `h2` → `h3`).

---

## 🧠 Learning Goals

This project is a **teaching aid**, not a production app. By reading through it (and its source), you'll encounter:

- Real-world use of CSS selectors and the cascade
- Colors, gradients, and background images
- Typography and text styling
- The CSS box model
- Flexbox and Grid layout systems
- Pseudo-classes and pseudo-elements
- Responsive design with media queries
- CSS animations and transitions
- Preprocessor concepts (Sass/Less)
- Modern CSS features (custom properties, Subgrid, Houdini, Container Queries)

---

## 📄 License

© 2025–2026 **Reyrove**. Styled, structured, and rights reserved.

This project is shared for learning purposes. Please credit the author if you fork or adapt it.

---

## 🙏 Credits

- Recipes, metaphors, and code — **Reyrove**
- Fonts — [Google Fonts](https://fonts.google.com/)
- Icons — [Font Awesome](https://fontawesome.com/) & [Material Design Icons](https://materialdesignicons.com/)
- Inspiration — every developer who ever compared CSS to baking 🧁

---

## 💬 Feedback

Found a bug? Have a better dessert metaphor? Open an issue or reach out:

- 🌐 Website: [reyrove.github.io](https://reyrove.github.io/)
- 💼 LinkedIn: [Reyrove](https://www.linkedin.com/feed/update/urn:li:ugcPost:7357186806821326848/)

Happy baking — I mean, styling! 🧑‍🍳💻