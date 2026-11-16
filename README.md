# A Pup's Guide to Taming Your Wolf

A responsive, pastel home for the original BL webcomic. The site is static HTML, CSS, and JavaScript with no build step.

## Preview

Open `index.html` in a browser, or serve this folder with a static server (for example, `python -m http.server 8000`) and visit `http://localhost:8000`.

To publish with GitHub Pages, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, then save. GitHub will show the site URL there when it is ready.

## Add chapters

Create an `art/` folder for page images. Add each chapter to the `chapters` array in `index.html`:

```js
{ number: "01", title: "Chapter title", summary: "Short summary.", pages: ["art/chapter-01/001.jpg", "art/chapter-01/002.jpg"] }
```

The image paths are relative to `index.html`; pages appear in the given order in the vertical reader.

## Add character art and details

The character cards identify only the dog beastman and wolf beastman from the existing premise. Replace the placeholder cards in the `characters` array and rendering section of `index.html` when you have names, descriptions, personality notes, and artwork to share.

## Site files

- `index.html` — all page sections, styles, and editable chapter/profile data.
