# 🖥️ AI ASCII Art Styler

> **Transform any image into stunning ASCII art — powered by AI luminance analysis and pixel mapping.**

A sleek, terminal-aesthetic web app that converts photos into ASCII art in real-time. No backend required, runs entirely in your browser using a built-in AI image processing engine.

![Preview](https://img.shields.io/badge/status-stable-brightgreen?style=flat-square&logo=github)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![HTML](https://img.shields.io/badge/built%20with-HTML%20%2B%20JS-orange?style=flat-square&logo=javascript)
![AI](https://img.shields.io/badge/AI-pixel%20luminance%20mapping-00ff40?style=flat-square)

---

## ✨ Features

| Feature | Description |
|---|---|
| 🤖 **AI Image Analysis** | Uses ITU-R BT.709 perceptual luminance mapping to intelligently select the best ASCII characters per pixel |
| 🎨 **4 Art Styles** | Classic · Dotted · Blocky · Gradient — each with unique character sets |
| 🎛️ **Density Control** | Adjustable output width (10–120 chars) for more or less detail |
| 🌈 **Color Presets** | White · Green · Retro Amber · Cyan · Custom color picker |
| 📋 **Copy to Clipboard** | One-click copy of the full ASCII text output |
| 🖼️ **Download as PNG** | Export your ASCII art as a stylized terminal-themed image |
| 📁 **Drag & Drop Upload** | Drag photos directly onto the app — PNG, JPG, WEBP supported |
| 💻 **CRT Terminal UI** | Dark mode, scanline effects, and flicker animations for the full retro feel |

---

## 🧠 How the AI Works

The app uses a **client-side AI pipeline** to process images:

1. **Pixel Sampling** — The uploaded image is drawn onto an HTML Canvas and downsampled to match the target character width
2. **Luminance Extraction** — Each pixel's brightness is calculated using the ITU-R BT.709 formula:
   ```
   L = 0.2126R + 0.7152G + 0.0722B
   ```
3. **Character Mapping** — The luminance value (0–255) is mapped to a character from the selected style's charset:
   - **Classic:** ` .'"\`^",:;Il!i><~+_-?][}{1)(|\/*#MW&8%B@$`
   - **Dotted:** ` ·.,:;•°·∘○◌◦●`
   - **Blocky:** ` ░▒▓█`
   - **Gradient:** ` ─╌┄╍═━`
4. **Real-time Render** — Output is rendered instantly in the browser with adjustable color and density

> No data is sent to any server. Everything runs locally in your browser. 🔒

---

## 🚀 Getting Started

### Option 1 — Open Directly in Browser
```bash
# Just double-click index.html, or open it in Chrome:
Ctrl + O → select index.html
```

### Option 2 — Serve Locally
```bash
# Python (no install required)
python -m http.server 8080

# Then open: http://localhost:8080
```

### Option 3 — Deploy to GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your app will be live at `https://yourusername.github.io/repo-name`

---

## 📸 Usage

1. **Upload** a photo via drag & drop or the upload button
2. **Select** an art style (Classic, Dotted, Blocky, or Gradient)
3. **Adjust** the density slider to control output detail
4. **Pick** a color (Green, White, Amber, Cyan, or Custom)
5. Click **[ G E N E R A T E ]**
6. **Copy** the text or **download** as a PNG image

---

## 🛠️ Tech Stack

- **Frontend:** Vanilla HTML5 + JavaScript (no frameworks)
- **Styling:** Tailwind CSS (CDN) + Custom CSS
- **Image Processing:** HTML Canvas API
- **AI Logic:** Client-side luminance mapping (ITU-R BT.709)
- **Fonts:** JetBrains Mono + Space Grotesk (Google Fonts)
- **Icons:** Material Symbols (Google)

---

## 💡 Use Cases

- **GitHub READMEs** — Add your ASCII portrait to your profile README
- **Content Creation** — Unique retro-aesthetic for social media posts
- **Developer Branding** — Stand out with ASCII art in your terminal/blog
- **Print Media** — Export high-contrast blocky art for posters or merch

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

<p align="center">
  Made with ⚡
</p>
