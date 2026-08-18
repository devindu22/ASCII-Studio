# 🎨 ASCII Studio

> Convert any image into detailed, high-resolution ASCII artwork directly in your browser. Built with zero dependencies and pure vanilla JavaScript.

![ASCII Studio Banner](https://img.shields.io/badge/ASCII-Studio-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow.svg?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange.svg?style=for-the-badge)

---

## 🌟 Features

- **⚡ Real-time Image Processing:** Instantaneous pixel-to-character conversion powered by the HTML5 Canvas API.
- **🎨 Color Palette Presets:**
  - **Full RGB Color:** Retains original image colors on each character.
  - **Cyberpunk / Neon:** Neon pinks, cyans, and purples for a retro-futuristic aesthetic.
  - **Matrix Green:** Classic terminal aesthetic.
  - **Monochrome & Sepia:** High-contrast retro look.
- **🔤 Customizable Density Ramps:** Choose from pre-built character sets (Standard, Detailed, Blocks, Binary, Retro) or type your own custom string.
- **🎛️ Fine-Tuned Controls:**
  - Adjustable scale/resolution (font size & grid density).
  - Brightness, contrast, and inversion settings.
  - Gamma correction for shadow and highlight detail.
- **💾 Multiple Export Options:**
  - Export rendered ASCII art as a high-resolution **PNG/JPEG** image.
  - Copy raw **plain text** to your clipboard.

---

## 🚀 Quick Start

No installation, Node.js environment, or build step required!

1. Clone or download this repository:
   ```bash
   git clone [https://github.com/your-username/ascii-studio.git](https://github.com/your-username/ascii-studio.git)

2. Navigate to the project folder:
```bash
cd ascii-studio

```


3. Open `index.html` in any modern web browser (Chrome, Firefox, Edge, Safari).

---

## 🛠️ How It Works

ASCII Studio operates by extracting raw pixel data from an uploaded image using an offscreen HTML5 `<canvas>` element:

1. **Pixel Sampling:** The input image is scaled down to match the selected resolution grid.
2. **Luminance Calculation:** Each pixel's RGB values are converted to perceived luminance ($L$) using the formula:

$$L = 0.2126 \times R + 0.7152 \times G + 0.0722 \times B$$


3. **Character Mapping:** The brightness score (0–255) maps linearly to a character in the selected character ramp (e.g., `@%#*+=-:. `).
4. **Rendering:** Characters are redrawn onto the visible canvas with custom colors, line spacing, and fonts.

---

## 💻 Tech Stack

* **HTML5:** Semantic layout and Canvas API rendering.
* **CSS3:** Responsive layout using CSS Grid/Flexbox and dynamic styling variables.
* **JavaScript (ES6+):** File API reading, canvas context manipulation, and asynchronous rendering loop.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.

---

