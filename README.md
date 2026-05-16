# 🪵 Srinivas Wood And Interiors — Business Website

A modern, fully responsive one-page business website for **Srinivas Wood And Interiors**, a premium carpentry and interior design business based in Hyderabad, Telangana.

---

## 📁 Project Structure

```
srinivas-wood-interiors/
│
├── index.html        ← The entire website (single file)
└── README.md         ← This file
```

> The entire website lives in a **single `index.html` file** — no build tools, no npm, no installation needed.

---

## 🚀 Getting Started

### Option 1 — Open Directly
Just double-click `index.html` in your file explorer. It opens in any browser.

### Option 2 — Local Server (recommended for best performance)
If you have Python installed:
```bash
# Python 3
python -m http.server 8000

# Then open in browser:
# http://localhost:8000
```

Or with Node.js:
```bash
npx serve .
```

---

## 🛠️ Technologies Used

| Technology | Purpose | How it's loaded |
|---|---|---|
| **HTML5** | Page structure | Native |
| **Tailwind CSS v3** | Utility-first styling | CDN |
| **Three.js r128** | 3D animated hero scene | CDN |
| **Playfair Display** | Display / heading font | Google Fonts CDN |
| **Lato** | Body / UI font | Google Fonts CDN |
| **Unsplash** | Gallery stock images | URL (free) |

> ✅ No npm, no webpack, no build step — everything loads from CDN.

---

## 📄 Website Sections

### 1. 🔝 Navbar
- Fixed top navigation with glass-blur effect
- Logo with custom SVG wood icon
- Smooth scroll links to all sections
- Mobile hamburger menu with slide-down panel

### 2. 🏠 Hero (3D Animated)
A fully interactive Three.js 3D scene featuring:
- **3D wood-panelled room** with floor planks and back wall
- **Two 3D cupboards** with doors and brass handles
- **Centre wooden table** with turned legs
- **6 floating wood planks** gently bobbing in the air
- **220 rising dust particles** like sawdust in light
- **Dynamic pulsing lights** — warm amber and orange tones
- **Mouse / touch parallax** — camera follows cursor movement
- Responsive across all screen sizes (mobile, tablet, desktop)

### 3. 🔨 Our Services
8 service cards in a 3-column responsive grid:

| # | Service |
|---|---|
| 1 | Custom Wood Furniture |
| 2 | Windows |
| 3 | Doors |
| 4 | Interior Carpentry |
| 5 | Pooja Room Unit |
| 6 | Furniture Repairs |
| 7 | Cupboards |
| 8 | POP Ceiling |

Each card has a custom SVG icon, title, and description.

### 4. 🖼️ Gallery (Interactive Filterable)
- **Category filter tabs**: All Work, Kitchen, Bedroom, Wardrobe, Living Room, Window & Doors, Cupboards
- Click any tab to filter photos with smooth animation
- Click any photo to open a **lightbox** (full-screen viewer)
- Lightbox includes **Previous / Next navigation** and image counter
- Category badge and label on each photo tile
- Keyboard `Escape` closes the lightbox

### 5. ✅ Why Choose Us
Three trust pillars with animated icons:
- **15+ Years Experience**
- **Premium Materials**
- **On-Time Delivery**

Stats bar: 500+ Projects · 15+ Years · 100% Satisfaction · 5★ Rating

### 6. 📞 Contact & Footer
- 📍 Location — Serilingampally, Hyderabad
- 📞 Phone — `+91 93940 27583` (tap-to-call)
- 📧 Email — `melojubunny9288@gmail.com` (tap-to-mail)
- 💬 **WhatsApp button** with pulsing animation — opens pre-filled chat
- Quote request form (Name, Phone, Service dropdown, Message)
- Footer copyright bar

---

## 📱 Responsive Behaviour

| Breakpoint | Behaviour |
|---|---|
| **Mobile < 600px** | 70° FOV, camera pulls back, shadows off, 3 planks, 80 particles, cupboards hidden, text centred, touch parallax |
| **Tablet < 900px** | 58° FOV, lighter shadows (512px maps), fluid typography |
| **Desktop ≥ 900px** | Full scene — 6 planks, 220 particles, full cupboards, 1024px shadows, mouse parallax |

All font sizes use `clamp()` for fluid scaling between breakpoints.

---

## 🎨 Design System

### Color Palette
| Name | Hex | Usage |
|---|---|---|
| Wood Dark | `#3E1F0A` | Hero background, dark accents |
| Wood | `#6B3F1F` | Primary brand colour |
| Wood Light | `#A0622A` | Buttons, highlights, accents |
| Wood Pale | `#F5EDE3` | Light backgrounds, card borders |
| Charcoal | `#2C2C2C` | Body text |
| Charcoal Light | `#4A4A4A` | Secondary text |
| Cream | `#FAF7F2` | Page background |

### Typography
| Font | Weight | Usage |
|---|---|---|
| Playfair Display | 400, 700, 900 | Headings, section titles, card titles |
| Lato | 300, 400, 700 | Body text, labels, buttons, nav |

---

## 📞 Business Contact Details

| Field | Value |
|---|---|
| Business Name | Srinivas Wood And Interiors |
| Phone | +91 93940 27583 |
| Email | melojubunny9288@gmail.com |
| Location | Serilingampally, Hyderabad, Telangana |
| WhatsApp | wa.me/919394027583 |

---

## ✏️ How to Customise

### Change Phone Number
Search for `9394027583` in `index.html` and replace all 3 occurrences (tel link, display text, WhatsApp URL).

### Change Email
Search for `melojubunny9288@gmail.com` and replace both occurrences (href and display text).

### Add Your Own Gallery Photos
In the `#gallery` section, replace the `src` attribute of any `<img>` tag:
```html
<!-- Replace this Unsplash URL -->
<img src="https://images.unsplash.com/photo-xxxx..." .../>

<!-- With your own photo path -->
<img src="images/my-kitchen-photo.jpg" .../>
```
Also update the `onclick="openLightbox('URL', 'Title', 'Category')"` attribute to match.

### Add a New Gallery Category
1. Add a filter button in the `#filter-tabs` div:
```html
<button data-filter="bathroom" class="filter-btn ...">Bathroom</button>
```
2. Add photo cards with `data-category="bathroom"` in `#gallery-grid`.

### Add a New Service Card
Copy any existing service card block and update the icon, title, and description. The grid auto-adjusts.

### Change Business Name / Logo
Search for `Srinivas Wood And Interiors` in `index.html` and replace all occurrences.

---

## 🌐 Deploying Online (Free Options)

### GitHub Pages
1. Create a new GitHub repository
2. Upload `index.html`
3. Go to **Settings → Pages → Source → main branch**
4. Your site will be live at `https://yourusername.github.io/repo-name`

### Netlify (Drag & Drop)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop your `index.html` file
3. Live instantly — free custom subdomain

### Vercel
```bash
npx vercel --prod
```

---

## ⚡ Performance Notes

- All CDN resources load from fast global networks
- Images use `loading="lazy"` for deferred loading
- Three.js auto-reduces quality on mobile (no shadows, fewer objects)
- Resize handler is debounced (120ms) to avoid jank
- Pixel ratio capped at 2× to avoid GPU overload on high-DPI screens

---

## 📋 Browser Support

| Browser | Support |
|---|---|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Mobile Chrome | ✅ Full |
| Mobile Safari | ✅ Full |
| IE 11 | ❌ Not supported |

> Requires WebGL support for the 3D hero. All modern browsers support this by default.

---

## 📝 License

This website was built for **Srinivas Wood And Interiors**.  
Stock photos sourced from [Unsplash](https://unsplash.com) — free for commercial use.  
Three.js — [MIT License](https://github.com/mrdoob/three.js/blob/dev/LICENSE).  
Tailwind CSS — [MIT License](https://github.com/tailwindlabs/tailwindcss/blob/master/LICENSE).

---

*Built with ❤️ for Srinivas Wood And Interiors · Hyderabad, 2025*
