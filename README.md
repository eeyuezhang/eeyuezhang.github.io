# Yue Zhang — research homepage

A lightweight, responsive English academic homepage for GitHub Pages. No framework, package installation, analytics, tracking, or external font service is required.

## Publish on GitHub Pages

Use a repository named `eeyuezhang.github.io`. Place this directory's contents at its root. In **Settings → Pages**, select **Deploy from a branch**, then **main** and **/(root)**. The expected URL is `https://eeyuezhang.github.io/`; only print it on business cards after the deployment is live and verified.

## Update the page

- **Biography, research, projects, patents, teaching, service:** edit `index.html`.
- **Publications:** edit `publications.json`. Keep the existing fields (`year`, `type`, `title`, `authors`, `venue`, `note`). Publication types are `journal` and `conference`.
- **Portrait:** replace `assets/portrait.png` with a new image using the same name, or change the image path in `index.html`.
- **Photo wall:** replace each `figure.photo-slot` placeholder with an image and caption. Upload images to `assets/`, add useful alt text, and use photos you have permission to publish. Example:

```html
<figure class="photo-slot has-photo">
  <img src="assets/conference-2026.jpg" alt="Yue Zhang at a research conference" loading="lazy">
  <figcaption>Conference name · City · Year</figcaption>
</figure>
```

- **Colors:** adjust the variables at the beginning of `style.css`.
- **Contact:** the page uses the public university email `yuezhang@stu.edu.cn`.

## Local preview

Run `python3 -m http.server 8000` in this directory and open `http://localhost:8000`. Use HTTP rather than opening `index.html` directly, because the publication list is loaded from JSON.

## Scope

This is a selected publication list rather than an exhaustive CV. It deliberately omits unpublished research, the original promotion presentation, personal information, private repository links, internal evaluation screenshots, and future career targets. No source PDF is included.
