# Interactive Virtual Birthday Celebration App

A responsive, interactive web application designed to send personalized birthday wishes featuring a 3D WebGL background, custom glassmorphism card styling, interactive confetti effects, and smooth step-by-step navigation.

---

## 🌟 Key Features

* **3D Animated Background:** Interactive 3D floating hearts powered by **Three.js** and WebGL, rendered with lighting, extrusion, and natural floating animations.
* **Glassmorphism UI:** Translucent frosted glass card layouts styled using custom CSS and **Tailwind CSS**.
* **Fully Responsive:** Custom media queries ensuring compact, border-padded layouts optimized for mobile displays (iOS and Android) as well as desktop viewports.
* **Interactive Confetti Effects:** Custom celebratory particle animations powered by `canvas-confetti`.
* **Multi-Step Navigation:** Smooth transition between custom message slides, prompt screens, and gallery slides using **GSAP** and CSS transitions.

---

## 🛠️ Built With

* **HTML5** & **CSS3**
* **JavaScript (ES6+)**
* **[Three.js](https://threejs.org/)** – 3D Graphics & WebGL animations
* **[Tailwind CSS](https://tailwindcss.com/)** – Utility-first CSS framework
* **[GSAP (GreenSock)](https://greensock.com/gsap/)** – High-performance animations
* **[Canvas Confetti](https://www.npmjs.com/package/canvas-confetti)** – Browser particle celebrations

---

## 📁 Project Structure

```text
.
├── index.html          # Initial entry slide
├── ready.html          # Readiness prompt slide
├── bday1.html          # Main birthday greeting slide
├── gallery.html        # Image gallery and photo carousel
├── messages.html       # Intermediate message cards
├── finalmessages.html  # Final scrollable birthday letter
├── stylegallery.css    # Gallery and responsive carousel stylesheet
└── README.md           # Project documentation

```

---

## 🚀 Getting Started

### Prerequisites

To view or modify this project locally, all you need is a modern web browser (Google Chrome, Mozilla Firefox, Safari, or Microsoft Edge). No server installation or node environment is strictly required, as dependencies are loaded via CDN.

### Local Setup

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/your-repo-name.git

```


2. **Navigate to the project directory:**
```bash
cd your-repo-name

```


3. **Open in browser:**
Open `ready.html` or `index.html` directly in your browser, or use a local server like VS Code's **Live Server** extension for real-time reloading.

---

## ⚙️ Customization Guide

### 1. Changing Text & Recipient Name

Search for `Y/N` or existing placeholder text within `bday1.html` and `finalmessages.html` to update names and custom letters:

```html
<h1 class="text-4xl md:text-4xl font-bold mb-10 text-gradient leading-[1.3]">
    Hi [Name]!
</h1>

```

### 2. Updating Color Schemes

* **Background Gradient:** Modify the CSS `background` property in the `body` tag:
```css
body {
    background: linear-gradient(5deg, #b026ff, #7A00C6);
}

```


* **3D Hearts Color Array:** Edit the hex colors in the JavaScript array block inside `ready.html` or `bday1.html`:
```javascript
const colors = [
    0x8A2BE2, 0x9370DB, 0xBA55D3, 0x9932CC
];

```



---

## ☁️ Deployment

This project is optimized for static hosting on **Vercel**, **GitHub Pages**, or **Netlify**.

### Deploying to Vercel

1. Push your repository to GitHub.
2. Log into [Vercel](https://vercel.com/) and click **Add New Project**.
3. Import your GitHub repository.
4. Keep the default build settings (Framework Preset: *Other*) and click **Deploy**.
