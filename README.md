# 🍽️ Comfort Bites — Restaurant Website

A full business-style restaurant website built with pure **HTML** and **Tailwind CSS**. No JavaScript. No build tools. Just open and go.

---

## 📁 Project Structure

```
/
├── index.html        # Home page
├── menu.html         # Menu page (food cards by category)
├── about.html        # About page (story, team, values)
├── contact.html      # Contact page (form, map, hours)
├── style.css         # Color variables and custom styles
└── README.md         # You are here
```

> All pages live in the root folder — no subdirectories, no config files.

---

## 🌟 Features

### Core Pages
| Page | Description |
|------|-------------|
| `index.html` | Hero section, featured food cards, opening hours, testimonials, CTA banner |
| `menu.html` | Full menu organised by category (Starters, Mains, Pizza, Desserts, Drinks) |
| `about.html` | Restaurant story, chef profile, core values |
| `contact.html` | Contact form, address & phone, Google Maps embed, full opening hours |

### Minimum Required Features ✅
- **Food Cards** — Image, name, price, description, and dietary tags
- **Opening Hours** — Displayed on both Home and Contact pages
- **Google Maps Embed** — Embedded iframe on the Contact page

### Bonus Features
- Sticky responsive navigation bar
- Mobile-friendly layout (Tailwind responsive prefixes)
- Category sections on menu page
- Testimonials / reviews section
- Chef's Pick / New / Popular badges on food cards
- Footer with links, socials, and contact info

---

## 🚀 Getting Started

No installation needed for the HTML. Just make sure Tailwind CLI is set up to compile `style.css`.

### Tailwind CLI Setup
```bash
# Install node_modules
npm install 

# Watch for changes during development
npx @tailwindcss/cli -i ./src/style.css -o ./src/output.css --watch

```

> Make sure each HTML file links to the compiled `output.css`, not `style.css` directly.

### Running the site

```bash
# Option 1 — Double-click index.html directly

# Option 2 — Node.js
npx serve .

# Option 3 — VS Code
# Install "Live Server" extension → click "Go Live"
```

---

## 🎨 Design

- **Fonts:** Cormorant Garamond (headings) + DM Sans (body) via Google Fonts
- **Theme:** Warm, comforting, and welcoming
- **Images:** Sourced from [Unsplash](https://unsplash.com) (free to use)

### Color Palette

| Role | Name | Value |
|------|------|-------|
| Primary | Deep Orange / Terracotta | `#c2531a` |
| Secondary | Cream / Soft Beige | `#f5ede0` |
| Accent | Warm Brown | `#7a4928` |

Colors are defined in `style.css` using Tailwind v4's `@theme` block:

```css
@import "tailwindcss";

@theme {
  --color-primary: #c2531a;
  --color-secondary: #f5ede0;
  --color-accent: #7a4928;
}
```

Use them in HTML as Tailwind utilities: `bg-primary`, `text-secondary`, `border-accent`, etc.

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| HTML5 | Page structure and content |
| Tailwind CSS (CLI) | Utility-first styling and layout |
| `style.css` | Color variables and custom overrides |
| Google Fonts | Typography |
| Google Maps iframe | Embedded map on Contact page |

> ⚠️ **No JavaScript** is used anywhere in this project.

---

## 🗺️ Google Maps

The map on `contact.html` uses a standard `<iframe>` embed. To use your real address:

1. Go to [maps.google.com](https://maps.google.com)
2. Search for your restaurant address
3. Click **Share → Embed a map**
4. Copy the `<iframe>` snippet
5. Replace the existing `<iframe>` inside `contact.html`

---

## ✏️ Customisation

| What to change | Where |
|----------------|-------|
| Restaurant name | `<title>` and nav logo in all HTML files |
| Address & phone | Footer in all pages + `contact.html` |
| Food items & prices | Food cards in `menu.html` and `index.html` |
| Opening hours | `index.html` hours section + `contact.html` |
| Colors | `style.css` |
| Hero image | `.hero-bg` background-image style in `index.html` |

---

## 📱 Browser Support

Works in all modern browsers: Chrome, Firefox, Safari, Edge.
Responsive from 320px mobile up to wide desktop.

---

## 📄 License

Free to use for personal and commercial projects.
Image credits go to [Unsplash](https://unsplash.com) contributors.