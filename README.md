# Code Transfer Tool

A lightweight, **client-side web application** for transferring code snippets across devices via a shareable URL. Designed for developers who need a quick and secure way to move code between machines without creating GitHub commits or triggering notifications.

---

## Features

- **Dark mode UI** optimized for developer workflow  
- **Monospace code font** (`Fira Code` / `Courier New`) for readability  
- **Live line count** as you type or paste code  
- **Copy code** button for one-click copying  
- **Compressed URLs** using LZ-based compression for shorter links  
- **Fully offline & static** – deployable on GitHub Pages, no backend required  
- **Safe for ephemeral testing** (e.g., SMTP or config snippets)

---

## Demo

You can deploy the tool on **GitHub Pages** or open `index.html` directly in your browser.

---

## Usage

1. **Paste your code** into the textarea.  
2. Check the **line count** displayed below the textarea.  
3. Click **“Generate URL”** to create a compressed, shareable link.  
4. Click **“Copy Code”** to copy the text to your clipboard.  
5. Share the generated URL to retrieve the code on another device.

> **Note:** The tool stores the code **only in the URL hash**. Clearing the textarea and regenerating the URL will remove the text from the link.

---

## Installation / Deployment

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/code-transfer-tool.git
````

2. Deploy on GitHub Pages:

   * Go to repository **Settings → Pages**
   * Set the source to `main / root`
   * Access the tool via `https://<your-username>.github.io/code-transfer-tool/`

3. Open `index.html` in your browser (optional offline usage).

---

## Technical Details

* **Frontend**: HTML, CSS, JavaScript
* **Compression**: [LZString](https://pieroxy.net/blog/pages/lz-string/index.html) for compact URL storage
* **Browser support**: Modern browsers (Chrome, Edge, Firefox, Safari)
* **Storage**: URL hash only; no backend or database required
* **Font**: `Fira Code` / fallback to `Courier New` for code readability

---

## Security Considerations

* Avoid using **sensitive production credentials**.
* This tool is **ephemeral**: anyone with the link can view the code.
* Best practice: use placeholder credentials or temporary test accounts (e.g., SMTP sandbox users).

---

## Future Improvements

* Syntax highlighting with Prism.js or CodeMirror
* URL length warning for very large code snippets
* One-click URL copy/share feature
* Optional dark/light mode toggle

---

## License / Usage

This project is **completely free to use**.

* You can copy, modify, or deploy it however you want.
* No attribution required (but appreciated).
* No warranties — use at your own discretion.

---

## Author

**Mid-level Python Developer** – focus on DevOps automation, developer tools, and efficient workflow solutions.
GitHub: [iantolentino](https://github.com/iantolentino)
