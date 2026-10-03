# 🌲 Camp Prepper — Interactive Outdoor Gear Checklist

[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Responsive](https://img.shields.io/badge/Design-Responsive%20Grid-success)](#responsive-web-design)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

An interactive, retro-themed web application designed to help campers prepare essential gear before their trip. Built with vanilla JavaScript, dynamic DOM manipulation, real-time status tracking, and a responsive 8-bit aesthetic.

---

## 📸 Preview & User Experience

- **Interactive Item Selection**: Click on any camping item to toggle its readiness state (visual checkmark overlay and border status change).
- **Live Readiness Counter**: Automatically updates the count of packed items (e.g., *"3 of 8 items ready!"*).
- **Dynamic CTA Transition**: The action button intelligently transitions from `Reset` to `Go Camping!` once all 8 items are packed, unlocking the celebration view.
- **State Reset & Multi-Page Flow**: Single-click full reset capability and seamless multi-page progression to the success destination.

---

## ✨ Key Features & JavaScript Concepts Demonstrated

| Feature | Technical Implementation |
| :--- | :--- |
| **DOM Event Handling** | `addEventListener` on `DOMContentLoaded` and item selection |
| **Dynamic Asset Swapping** | Dynamic string replacement for `src` attributes (`.png` $\leftrightarrow$ `_checked.png`) |
| **State Tracking** | Centralized item counter and status evaluator (`updatePreparationStatus`) |
| **Class State Management** | `classList.add`, `classList.remove`, and `classList.contains` |
| **Conditional Flow** | Dynamic UI state transitions based on checklist completion |
| **Multi-page Routing** | Programmatic navigation via `document.location.assign()` |

---

## 📱 Responsive Web Design

The user interface adapts across all viewport sizes using modern CSS techniques:
- **Fluid Layout**: Built with CSS Grid and dynamic column wrapping:
  - **Desktop ($\ge 900\text{px}$)**: 4-column item grid.
  - **Tablet ($540\text{px} - 900\text{px}$)**: 2-column item grid.
  - **Mobile ($< 540\text{px}$)**: Single-column stacked card layout.
- **Fluid Typography**: Uses CSS `clamp()` for crisp readability across mobile and desktop displays without overflow.
- **Touch-Optimized**: High contrast tap targets and hover/active animations for mobile and desktop input.

---

## 📂 Project Structure

```text
camp-prepper/
├── assets/
│   └── images/          # Gear item thumbnails, checkmarks, and banners
├── css/
│   └── app.css          # Responsive styling, CSS Grid, and retro typography
├── js/
│   ├── app.js           # Core checklist logic, state manager, and DOM manipulation
│   └── jquery.js        # Supporting utility library
├── camping.html         # Celebration & completion landing view
├── index.html           # Main interactive checklist entry point
├── LICENSE              # MIT License
├── .gitignore           # Git ignore configuration
└── README.md            # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
No build tools, bundlers, or package installations are required. Just a modern web browser.

### Local Installation & Launch
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/camp-prepper.git
   cd camp-prepper
   ```
2. Open `index.html` in your favorite browser:
   ```bash
   # On macOS:
   open index.html

   # On Linux:
   xdg-open index.html

   # On Windows:
   start index.html
   ```

---

## 🛠️ Built With

- **HTML5**: Semantic document structure
- **CSS3**: CSS Grid, Flexbox, Transitions, `clamp()` fluid typography
- **JavaScript (ES6+)**: Event listeners, dynamic DOM manipulation, state logic
- **Google Fonts**: [Press Start 2P](https://fonts.google.com/specimen/Press+Start+2P)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
