# Move Well Austin Website

A responsive static website designed for GitHub Pages.

## Files

- `index.html` — page content and structure
- `styles.css` — responsive layout and branding
- `script.js` — mobile navigation and automatic footer year
- `.nojekyll` — tells GitHub Pages to publish the files directly

## Deploy with GitHub Pages

1. Create a public GitHub repository named `move-well-austin`.
2. Upload all files from this folder to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**
5. Save.

The site should publish at:

`https://YOUR-USERNAME.github.io/move-well-austin/`

## Replace the biography placeholder with a photograph

In `index.html`, find:

```html
<div class="portrait-placeholder">
```

Replace the full `portrait-placeholder` block with:

```html
<div class="portrait-photo">
  <img src="images/rebecca.jpg"
       alt="Rebecca Grigg, personal trainer and active aging specialist">
</div>
```

Then create an `images` directory and place the photograph at:

`images/rebecca.jpg`

Add this CSS to `styles.css`:

```css
.portrait-photo {
  overflow: hidden;
  min-height: 580px;
  border-radius: 190px 190px 28px 28px;
}

.portrait-photo img {
  width: 100%;
  height: 100%;
  min-height: 580px;
  object-fit: cover;
}
```

## Current contact information

- Rebecca Grigg
- Personal Trainer — Active Aging Specialist
- 210-630-9926
- Austin, Texas
- $125 per one-hour session
