# Image Optimizer

ImageOptimizer is a single-page web application that lets you compress and resize images (PNG, JPEG, WebP, and more) entirely in the browser—no server, no uploads. View original and compressed dimensions & file sizes side-by-side, adjust output format, quality, and maximum width, then download optimized files with a single click. Built with pure HTML5, CSS3, and JavaScript, it works offline, supports drag-and-drop or file picker, and includes light/dark themes.

---

## Features

- **Client-Side Compression**  
  Compress images entirely in the browser without sending data to any server.

- **Multiple Formats**  
  Output as JPEG, PNG or WebP.

- **Quality Control**  
  Adjustable compression quality from 0.1 to 1.0.

- **Resize by Width**  
  Specify a maximum width (px) to downscale large images proportionally.

- **Batch Processing**  
  Drag & drop—or select—multiple image files at once.

- **Before & After Details**  
  Displays original filename, dimensions (px) and file size (KB), alongside compressed dimensions and size.

- **Download Optimized Files**  
  One-click download for each optimized image, with proper file extension.

- **Clear All**  
  Reset the workspace to start fresh.

- **Light & Dark Themes**  
  Toggle between light and dark modes for comfortable use any time of day.

- **100% Front-End**  
  No dependencies beyond a single HTML file; works on GitHub Pages, Netlify, or any static host.

---

## Live Demo

Check out the live demo on GitHub Pages:  
https://bocaletto-luca.github.io/ImageOptimizer/index.html

---

## Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/bocaletto-luca/ImageOptimizer.git
   cd ImageOptimizer
   ```

2. **Serve with a static HTTP server**  
   - **Python 3**  
     ```bash
     python3 -m http.server 8000
     ```
   - **Node.js (http-server)**  
     ```bash
     npx http-server . -p 8000
     ```

3. **Open in your browser**  
   Navigate to `http://localhost:8000/index.html`.

---

## Usage

1. **Add Images**  
   - Click the “Click or Drag & Drop Images Here” area, or drag image files (PNG, JPEG, WebP, etc.) onto it.

2. **Review Originals**  
   - Each image card shows the filename, original dimensions (px), and original file size (KB).

3. **Configure Output**  
   - Select your desired **Output Format** (JPEG, PNG, WebP).
   - Adjust **Quality** using the slider (0.1 = high compression, lower quality; 1.0 = low compression, high quality).
   - Optionally enter a **Max Width** (px) to resize images wider than that value.

4. **Compress All**  
   - Click **Compress All** to process every loaded image.  
   - After compression, each card updates to show new dimensions and compressed file size, and displays a **Download** link.

5. **Clear Workspace**  
   - Click **Clear All** to remove all images and start over.

6. **Toggle Theme**  
   - Click the 🌙/☀️ button to switch between dark mode and light mode.

---

## Customization

- **Colors & Styles**  
  Edit the CSS variables at the top of the `<style>` block in `index.html` to change background, text, primary, accent, and border colors.

- **Default Quality & Formats**  
  Modify the `<select>` options and default values for `#qualityRange` in the HTML.

- **Resize Logic**  
  Adjust the JavaScript block around the Canvas resizing code if you want different scaling behaviors (e.g., max height).

---

## File Structure

```
ImageOptimizer/
├── index.html    # Single-page application (HTML, CSS, JS)
├── LICENSE       # GNU General Public License v3.0
└── README.md     # This documentation
```

---

## Contributing

Contributions, bug reports, and feature requests are welcome!

1. Fork the repository  
2. Create a feature branch  
   ```bash
   git checkout -b feature/my-feature
   ```
3. Commit your changes  
   ```bash
   git commit -m "Add my awesome feature"
   ```
4. Push to your branch  
   ```bash
   git push origin feature/my-feature
   ```
5. Open a Pull Request on GitHub

Please test across major browsers and maintain code readability.

---

## License

This project is licensed under the **GNU General Public License v3.0** (GPL-3.0). See [LICENSE](LICENSE) for details.

---

## Author

**Bocaletto Luca**  
- GitHub: [@bocaletto-luca](https://github.com/bocaletto-luca)  
- Repository: [ImageOptimizer](https://github.com/bocaletto-luca/ImageOptimizer)
