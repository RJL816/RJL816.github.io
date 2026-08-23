# Jialun Ren - Academic Personal Homepage

A bilingual (Chinese / English) static academic personal homepage for graduate school applications (保研/夏令营), designed for GitHub Pages deployment.

## Design Concept — "Traces & Anchors" (学习痕迹)

The visual identity grows out of the owner's own research (TAPC): every gradient update leaves a "learning trace", and EMA consolidates traces into an **anchor**. The page turns that metaphor into a design language:

- **Engineering-drawing (blueprint) aesthetic** — drafting grid, Prussian-blue ink lines, corner ticks, dimension annotations (R 120 / φ 250), plate numbers and a drawing title block in the footer
- **Red-pencil annotations** — handwritten notes, a name seal, stamps, and `+` bullets, creating tension between machine drawing and human hand
- **Trace animations** — the hero name has converging echo layers; dotted trace lines flow into an anchor in the hero and TAPC section; a fixed left rail lights up anchors as you scroll

## Features

- **Bilingual** — One-click toggle between Chinese and English, language preference saved automatically
- **Single-page design** — 9 sections: Hero, About, Research, Project, Publications, Awards, Skills, Contact, Footer
- **Responsive** — Desktop, tablet, and mobile layouts
- **Zero dependencies** — Pure HTML + CSS + vanilla JavaScript, no build tools required
- **Fonts** — Google Fonts: Fraunces + Noto Serif SC (display), Inter (body), JetBrains Mono (technical annotations), Long Cang (handwritten notes)

## Project Structure

```
.
├── index.html    # Main page with i18n logic
├── style.css     # Stylesheet
├── assets/       # Static assets (create this folder)
│   ├── cv.pdf    # Your CV / Resume
│   └── avatar.jpg # Your profile photo (optional)
└── README.md
```

## Quick Start

1. Create a new GitHub repository named **`RJL816.github.io`**
2. Clone the repository to your local machine
3. Copy all files from this project into the repository
4. Replace placeholder information (search for `TODO`)
5. Commit and push to GitHub
6. Your site will be live at `https://RJL816.github.io` within a few minutes

## Customization

### Replace Placeholder Information

Search the codebase for `TODO` and replace all occurrences with your actual information.

### Language Switching

The page defaults to Chinese. Click the **中 / EN** toggle in the top navigation bar to switch to English. Your language preference is saved in the browser's `localStorage` and persists across visits.

To modify or add translations, edit the `i18n` object in the `<script>` section at the bottom of `index.html`. Each language (`zh` / `en`) contains key-value pairs mapping `data-i18n` attribute values to display text.

### Add Your Profile Photo

1. Place a square photo named `avatar.jpg` in the `assets/` folder
2. In `index.html`, find the `.hero-avatar-placeholder` div and replace it with the commented-out `<img>` tag above it

### Add Your CV

Place your CV/Resume PDF at `assets/cv.pdf`.

### Add Publications

In `index.html`, find the `<!-- TODO: 添加更多论文 -->` comment and add additional publication entries. Remember to add corresponding i18n keys in both `zh` and `en` dictionaries.

## Tech Stack

- HTML5 (semantic elements)
- CSS3 (custom properties, flexbox, grid, responsive)
- Vanilla JavaScript (i18n, smooth scroll, mobile menu)
- No frameworks, no build tools, no npm

## License

Feel free to use and modify for your personal academic homepage.

---

© 2026 Jialun Ren. Powered by GitHub Pages.
