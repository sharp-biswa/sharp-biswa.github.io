# 🧠 Minsky.in — Design & Technical Analysis

> **Source:** [minsky.in](https://www.minsky.in/) | Analyzed: September 2026

---

## 🎬 Recording

![Browser recording of Minsky.in analysis](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_website_analysis_1790536311749.webp)

---

## 📸 Page Screenshots

````carousel
![Homepage — Hero Section](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_homepage_1790536339243.png)
<!-- slide -->
![Hero Section (Scrolled)](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_hero_section_1790536364391.png)
<!-- slide -->
![Services / Capabilities Section](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_services_section_1790536375452.png)
<!-- slide -->
![Capabilities Cards — More](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_capabilities_more_1790536382871.png)
<!-- slide -->
![Our Works Showcase](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_works_section_1790536395765.png)
<!-- slide -->
![Clients & Partners](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_clients_section_1790536407729.png)
<!-- slide -->
![Contact Form & Footer](C:/Users/Biswaranjan Sahoo/.gemini/antigravity-ide/brain/27023185-bf39-4724-93ae-77aa3795440e/minsky_footer_section_1790536417494.png)
````

---

## 🛠️ Technical Stack & Libraries

| Category | Technology | Evidence |
|---|---|---|
| **Framework** | **Next.js** (React SSR/SSG) | Bundle paths: `/_next/static/chunks/` |
| **CSS Framework** | **Tailwind CSS** | Arbitrary values like `px-[1vw]`, `py-[0.5vh]`, `3xl:text-m`, `bg-background`, `text-primary` |
| **Canvas Animation** | **HTML5 Canvas (custom)** | Interactive background grid rendering floating tech keywords |
| **Transitions** | **CSS3 Keyframes** | `transition duration-200`, `hover:scale-95` |
| **Animation** | **No external anim lib** | Pure CSS3 micro-interactions and custom JS canvas |

> [!NOTE]
> No third-party animation libraries (GSAP, Framer Motion, AOS, Lottie) were detected. All animations appear to be built with CSS3 and custom canvas JS logic.

---

## 🧩 UI Sections & Components

### 1. 🔝 Header / Navigation
- **Logo:** Top-left square-boxed with monospace `Minsky` text
- **Navbar:** Floating **center-top pill** with glassmorphism (semi-transparent dark backdrop blur)
- **Nav Links:** `Home | Works | Services | Products | Blog | Contact`

### 2. 🦸 Hero Section
- **Headline:** Bold minimal display text — *"We Design, Develop, & Deploy WebApps."*
- **Background:** Dynamic **HTML5 Canvas** matrix grid with floating tech stack labels: `React`, `TypeScript`, `GraphQL`, `Docker`, `AWS`, `Redux`, `Node`, `Jest`, `GCP`, etc.
- **Aesthetic:** Full-bleed dark background with animated keyword cloud

### 3. 💡 Development Philosophy Section
| Left Column | Right Column |
|---|---|
| **CLI Terminal Widget** — simulates Linux boot: `$ systemctl start minsky`, `[ OK ] Started webdev.service`, `WELCOME TO MINSKY`, `$ _` | **Philosophy Text** — Human-centric engineering, sustainable software ethos |

### 4. 🃏 Capabilities (Services) — 3-Column Card Grid
Each card has:
- Custom **outline vector icon**
- Short title + description
- **Arrow button (↗)** in top-right corner for navigation
- Cards: *AI-Native Apps*, *Web Design*, *Full-Stack Product Development*

### 5. 📁 Our Works Showcase
- Numerically indexed project list: `[01] COORD`, `[02] TNGSS`, `[03] TVK`, `[04] ICDIC`
- **Split layout:** Left = project title, category tags, description | Right = interactive preview mockup gallery
- Clean border-separated rows with expand/hover interactions

### 6. 🤝 Clients & Partners
- Horizontal monochrome **logo strip** (grayscale)
- Brands: *Be-Inspace, FaMe TN, Govt of Tamil Nadu, StartupTN Global Summit, COORD*

### 7. 📬 Contact Form & Footer
- Dark-mode **input form** — Full Name, Email, Phone, Message fields
- High-contrast CTA button: `CONTACT`
- **Quick Links & Socials:** LinkedIn, Instagram, X (Twitter), Email, Phone
- **System Status Bar (bottom):** Real-time status, geolocation `BLR 12.97°N 77.59°E`, night mode indicator `NIGHT SHIFT [SND ○]`

---

## 🎨 Color Palette

| Role | Color | Hex |
|---|---|---|
| Primary Background | Deep Black | `#000000` / `#050505` |
| Card Surfaces | Dark Charcoal | `#111111` / `#161616` |
| Card Borders | Subtle White | `rgba(255,255,255,0.1)` |
| Primary Text | Pure White | `#FFFFFF` |
| Secondary Text | Neutral Grey | `#A1A1AA` / `#71717A` |
| Accent / Terminal | Neon Green | `#2EE06E` |
| Night Mode Accent | Amber | `#F59E0B` |

**Design Style:** **Cyber-Minimalism / Developer Neo-Brutalism**
- Hacker terminal aesthetic with clean grid lines
- High contrast dark backgrounds
- Developer-oriented micro-copy and interactive console logging

---

## 🔤 Typography

| Use Case | Font Style |
|---|---|
| Headings & Body | Modern geometric sans-serif — *Inter / Geist / Space Grotesk* |
| Terminal / Code / System | Monospace — *Geist Mono / JetBrains Mono* |

---

## ✨ Animations & Interactions

| Animation | Technique |
|---|---|
| Floating tech-word background | Custom HTML5 Canvas animation loop |
| CLI terminal typing simulation | CSS + JS character-by-character rendering |
| Hover on nav/buttons | CSS `transition duration-200`, `hover:scale-95` |
| Glassmorphism navbar | CSS `backdrop-filter: blur()` |
| Scroll reveals | CSS transitions (likely with Intersection Observer) |
| Console Easter Eggs | Custom JS: ASCII branding, Konami Code `↑↑↓↓←→←→ba` |
| Time-aware UI | JS: `NIGHT SHIFT` alert changes color/mode based on time of day |

---

## 🏷️ Key Design Principles Observed

1. **Terminal/CLI Aesthetic** — Embraces developer culture with boot sequences, status bars, ASCII art
2. **Glassmorphism** — Pill navbar with backdrop blur
3. **Dark Mode First** — Pure black background as the foundation
4. **Content-Focused Minimalism** — No decorative clutter; every element serves a purpose
5. **Interactive Storytelling** — CLI widget, floating canvas, and console logs tell the brand story
6. **Responsive Grid** — 3-column card layouts collapse gracefully at breakpoints (via Tailwind)
7. **Monochrome Client Logos** — Keeps visual hierarchy clean and uncluttered
