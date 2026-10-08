# Simple personal GitHub Pages website

This site uses only HTML + CSS. No Jekyll, JavaScript, package manager, or build step is required.

## Pages included

- `index.html` - bio and contact information
- `research.html` - research interests and projects
- `publications.html` - publications
- `teaching.html` - teaching
- `cv.html` - web CV + link to a CV PDF
- `presentations.html` - posters and talks, with PDF links

## First edits to make

Search the HTML files for these placeholders and replace them:

- `Your Name`
- `YOUR-USERNAME`
- `you@example.com`
- `[your role / field]`
- `[institution / city]`

Replace `assets/headshot-placeholder.svg` with your own JPG/PNG, then update the image path in all six HTML pages.

## Add a poster PDF

1. Upload your PDF into `assets/posters/`, for example:
   `assets/posters/my-poster-2026.pdf`
2. Open `presentations.html`.
3. Copy an existing block that starts with:
   `<div class="presentation">`
4. Change the title, conference, authors, and year.
5. Change the link to:
   `href="assets/posters/my-poster-2026.pdf"`

The `target="_blank"` attribute makes the PDF open in a new browser tab.

Example:

```html
<div class="presentation">
  <div>
    <h3>My poster title</h3>
    <p class="meta">Conference Name · Zurich · 2026</p>
    <p>Your Name, Coauthor Name</p>
  </div>
  <a class="button-link"
     href="assets/posters/my-poster-2026.pdf"
     target="_blank" rel="noopener">View poster (PDF)</a>
</div>
```

## Replace the CV PDF

Replace `assets/cv.pdf` with your real CV, keeping the filename `cv.pdf`.

## Publish with GitHub Pages

1. Create a public repository named `YOUR-USERNAME.github.io`.
2. Upload the contents of this folder to the repository root.
3. Go to **Settings -> Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose `main` and `/ (root)`, then save.

Your site will be at `https://YOUR-USERNAME.github.io/`.

## Change colours

Edit the variables at the top of `style.css`.
