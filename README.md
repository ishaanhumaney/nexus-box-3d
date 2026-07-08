# Nexus Box 3D

A lightweight, high-performance 3D product mockup container built natively with vanilla HTML and raw CSS 3D transforms. No heavy 3D canvas libraries, no external frameworks—just optimized layout math running straight on the GPU.



## Overview

This project is a pragmatic blueprint for bringing hardware assets to life on the web without sacrificing performance. By using native browser capabilities like `perspective`, `transform-style: preserve-3d`, and hardware-accelerated CSS variables, it renders a fully responsive, double-sided 3D retail box that users can interact with. It comes out of the box with an asymmetric theme toggle that updates UI states fluidly.

## Key Features

* **Native 3D Math:** Pure CSS implementation using `rotateX`, `rotateY`, and `translateZ` spatial offsets.
* **Zero Dependencies:** Zero frameworks, zero compilation steps, zero bloated bundle sizes.
* **Hardware Accelerated:** Fluid 60fps animations that hand rendering tasks off directly to the GPU.
* **Unified State Management:** Reactive dark and light theme states handled cleanly through raw CSS custom properties.
* **Semantic Accessibility:** Screen-reader-friendly DOM layouts with explicit `aria-label` declarations on interactive pieces.

## Tech Stack Breakdown

* **HTML5:** Structured semantic markup using flat components to optimize layout calculation times.
* **CSS3:** Advanced usage of 3D perspective depth tracking, cubic-bezier transition curves, and CSS variables.
* **JavaScript:** Extremely minimal, ultra-fast script block isolated solely for handling class mutations on state changes.

## Prerequisites & Web-Based Quick Start

Because this project is completely vanilla, there are no dependencies to install or build tools to compile. You can spin this up instantly right from your browser.

### Option A: GitHub Codespaces (100% In-Browser)
1. Click the **Code** button at the top right of this repository.
2. Select the **Codespaces** tab and click **Create codespace on main**.
3. Once the environment loads, install the simple live preview extension or run any simple HTTP static server to view your changes.

### Option B: Local Micro-Setup
If you want to view this on your machine locally, just download the code files and run a quick server snippet:

```bash
# Python 3
python -m http.server 8000

# Node.js (Static Server)
npx serve .
Open http://localhost:8000 or http://localhost:3000 in your web browser.
```

## Project Structure
```bash
nexus-box-3d/
├── .gitignore          # Ignores system junk and IDE setups
├── index.html          # Main layout markup and theme toggle handler
├── style.css           # 3D transforms, custom variables, and theme styling
└── README.md           # Documentation
```

## Roadmap
[ ] Add dynamic mouse-tracking to skew the box based on exact cursor coordinates.

[ ] Implement an explicit touch-drag gesture handler for mobile screens.

[ ] Create reusable CSS modifiers for alternative package shapes (e.g., slender tubes, wide horizontal cases).
