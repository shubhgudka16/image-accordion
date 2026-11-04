<div align="center">

# 🖼️ Image Accordion

### A smooth, interactive image accordion built with **pure HTML & CSS** — no JavaScript required.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![No JS](https://img.shields.io/badge/JavaScript-Not%20Needed-success?style=for-the-badge&logo=javascript&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

[🔴 Live Demo](https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/) · [🐛 Report Bug](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME/issues) · [✨ Request Feature](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME/issues)

<br>

<img src="assets/preview.gif" alt="Image Accordion Preview" width="800">

</div>

---

## 📖 About The Project

**Image Accordion** is a beginner-friendly front-end project that displays four beautiful landscape cards representing different times of the day. Click on any card and it smoothly expands to reveal its title and description, while the other cards shrink to make room.

The whole interaction is powered by the **CSS radio-button hack** (`input:checked + label`) — so the animation works without writing a single line of JavaScript.

## ✨ Features

- 🎨 **Pure CSS interaction** — expand/collapse using hidden radio inputs
- 🌅 **Four themed cards** — Morning, Midday, Evening, Night
- 🎞️ **Smooth animation** using `cubic-bezier` transitions
- 🌈 **Gradient background** with soft card shadows and rounded corners
- 🖱️ **Click-to-expand** with only one card open at a time
- 🪶 **Lightweight** — just one HTML file and one CSS file

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML5** | Page structure, radio inputs & labels |
| **CSS3** | Flexbox layout, transitions, gradients, sibling selectors |

## 📂 Project Structure

```
image-accordion/
│
├── 📄 index.html      # Markup for the accordion cards
├── 🎨 image.css       # All styling and animations
├── 📜 script.js       # (Optional / currently unused)
├── 📁 assets/
│   └── preview.gif    # Screenshot / demo GIF for the README
└── 📘 README.md
```

## 🚀 Getting Started

### Prerequisites

You only need a web browser (Chrome, Firefox, Edge, Safari). An internet connection is required to load the background images.

### Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   ```

2. **Go to the project folder**
   ```bash
   cd YOUR-REPO-NAME
   ```

3. **Open the project**
   - Double-click `index.html`, **or**
   - Right-click → *Open with* → your browser, **or**
   - Use the **Live Server** extension in VS Code

4. **Click any card** to expand it and see the animation in action! 🎉

## 🎯 How It Works

```html
<input type="radio" name="slide" id="c1" checked>
<label for="c1" class="card"> ... </label>
```

```css
input { display: none; }

input:checked + label {
  width: 600px;           /* the selected card grows */
}

input:checked + label .description {
  opacity: 1;             /* its text fades in */
}
```

1. Each card is a `<label>` linked to a hidden radio `<input>`.
2. Radio buttons in the same group allow **only one** selection at a time.
3. The `:checked` selector with the `+` sibling combinator widens the selected card.
4. The `transition` property makes the resize smooth.

## 🎨 Customization

- **Change images** — edit the `background-image` URLs for `#one`, `#two`, `#three`, `#four` in `image.css`.
- **Change text** — update the `<h4>` and `<p>` inside each card in `index.html`.
- **Change expanded width** — modify `input:checked + label { width: 600px; }`.
- **Change colors** — tweak the `body` gradient in `image.css`.
- **Add more cards** — copy one `input` + `label` block, give it a new `id`, and add a matching background image.

## 🗺️ Roadmap

- [x] Basic accordion with 4 cards
- [x] Smooth CSS transitions
- [ ] Make it fully responsive for mobile screens
- [ ] Add keyboard navigation
- [ ] Add hover effects on collapsed cards
- [ ] Store images locally for offline use

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m "Add some AmazingFeature"`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 License

Distributed under the **MIT License**. See `LICENSE` for more information.

## 🙏 Acknowledgements

- Wallpapers from [HDQWalls](https://hdqwalls.com), [HDWallpapers](https://www.hdwallpapers.in) and [Rare Gallery](https://rare-gallery.com)
- [Shields.io](https://shields.io) for the badges

## 👨‍💻 Author

**Shubh**
Diploma in Computer Engineering Student · Government Polytechnic, Jamnagar



---

<div align="center">

⭐ **If you liked this project, give it a star!** ⭐

*This was one of my first projects as a beginner — and I'm proud of how far I've come.* 🚀

</div>
