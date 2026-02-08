# 🌿 Natours – Advanced CSS & Sass Homework-4

**A beautiful, fully responsive static landing page for a fictional outdoor tour company.**

Built as a personal homework project following Jonas Schmedtmann’s Advanced CSS & Sass course, with my own customizations, Sass architecture improvements, and GitHub Pages deployment.

Live Demo: https://sobhan-srza.github.io/homework-4 (or wherever you deployed it)

---

## ✨ Key Features

- ✅ **Mobile-first responsive design** (phone → tablet → desktop)
- ✅ **Pure CSS 3D flip cards** for tour packages
- ✅ **Hamburger menu** with animated background expansion (no JS!)
- ✅ **Floating label form** with validation styles
- ✅ **Video background** section (stories)
- ✅ **Skewed hero section** with clip-path
- ✅ **Smooth hover animations** & entrance animations
- ✅ **Sass 7-1 architecture** (clean, scalable, maintainable)
- ✅ **Custom media query mixin** with named breakpoints
- ✅ **GitHub Pages auto-deployment** via GitHub Actions
- ✅ **Zero JavaScript** – everything is pure HTML + CSS

---

## 📁 Project Structure

```
homework-4/
├── index.html                          # Main HTML file
├── style.css                           # Compiled CSS (auto-generated)
├── .gitignore
├── package.json
├── README.md
├── .github/
│   └── workflows/
│       └── static.yml                  # GitHub Pages deployment workflow
├── sass/
│   ├── main.scss                       # Entry point – imports everything
│   ├── _animations.scss
│   ├── _base.scss
│   ├── _buttons.scss
│   ├── _footer.scss
│   ├── _header.scss
│   ├── _icons.scss
│   ├── _mixins.scss                    # Media queries, clearfix, gradients, etc.
│   ├── _navigation.scss
│   ├── _section-about.scss
│   ├── _section-book.scss
│   ├── _section-features.scss
│   ├── _section-stories.scss
│   ├── _section-tours.scss
│   ├── _typography.scss
│   ├── _utilities.scss
│   └── _variables.scss                 # All colors, breakpoints, grid sizes
└── images/                             # (not committed – add your own)
    ├── persian-caesar-1.png
    ├── persian-caesar-2.png
    ├── nature-video.mp4
    └── ...
```

### Sass Architecture (7-1 Pattern)
- `main.scss` → imports all partials in logical order
- `_variables.scss` → colors, breakpoints, grid
- `_mixins.scss` → reusable code (respond, gradient-text, etc.)
- One partial per major section/component

---

## 🛠️ Available Commands (NPM Scripts)

```bash
npm install          # Install dev dependencies (Sass)
npm run watch        # Compile Sass → style.css and watch for changes (recommended)
```

That’s it! No build step needed – just open `index.html` in your browser.

---

## 🚀 Deployment (GitHub Pages)

The project uses GitHub Actions to automatically deploy on every push to `main`:

- File: `.github/workflows/static.yml`
- Deploys the entire repository root as static site
- No extra configuration needed

Just push → site updates instantly!

---

## 🎨 Color Palette & Variables (from `_variables.scss`)

```scss
$color-primary:        #55c57a;
$color-primary-light:  #a2ff91;
$color-primary-dark:   #1aae7d;
$color-title-light:    #63da8b;
$color-title-dark:     #197b55;
$color-secondary-light:#ffb900;
$color-secondary-dark: #ff7730;
$color-tertiary-light: #2998ff;
$color-tertiary-dark:  #5643fa;
$color-grey-dark:      #777;
$color-grey-light-1:   #f7f7f7;
$color-grey-dark-3:    #333;
```

Breakpoints:
- `phone`: 37.5em (600px)
- `tab-port`: 56.25em (900px)
- `tab-land`: 75em (1200px)
- `big-desktop`: 112.5em (1800px)

---

## 📌 Important Notes

- All images and the video are referenced locally (`./images/`). Replace them with your own assets.
- The project contains **no JavaScript** – everything is CSS-only.
- Floating labels work via `:focus` + `:not(:placeholder-shown)` trick.
- Tour cards use `perspective` + `rotateY` for 3D flip effect.
- Story section uses `shape-outside` + `clip-path` for circular text wrap.

---

## 🙏 Credits & Thanks

- Original design & course by **Jonas Schmedtmann** (@jonasschmedtmann)
- My custom Sass refactoring, Persian logo, and deployment setup by **Sobhan-SRZA**
- Special thanks to **DeepSeek** for helping with the final touches

---

## 📬 Contact & Socials

- Website: https://srza.ir
- Telegram: @d_opa_mine & @Sobhan_SRZA
- Instagram, Twitch, YouTube, GitHub: links in original README
- Discord communities linked in README

---

⭐ Feel free to star this repo if you found it useful!

Made with ❤️ and a lot of Sass

**Sobhan-SRZA** – February 2026

---

**This README is ready to copy-paste into your GitHub repository.**  
Just replace the live demo link and add your images when you push.  

Let me know if you want a **dark mode version**, **TypeScript/React rewrite**, or **Netlify/Vercel deployment** next! 🚀