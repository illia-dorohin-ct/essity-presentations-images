# Essity Presentations — Images

This repository stores images used in Essity presentation slides. Images are served directly from GitHub via public URLs.

## Repository Structure

```
tena-media/
  presentation/   — brand-level images (logo, background)
  slide01/         — images for slide 1
  slide02/         — images for slide 2
  ...

lotus-media/
  presentation/   — brand-level images (logo)
  slide01/         — images for slide 1
  slide03/         — images for slide 3
  ...
```

Each slide folder contains sequentially numbered images: `image001.png`, `image002.jpg`, etc.
Screenshots are marked with a `_screenshot` suffix: `image003_screenshot.png`.

## How Image URLs Work

Every file in this repository is publicly accessible via:

```
https://raw.githubusercontent.com/illia-dorohin-ct/essity-presentations-images/main/{path}
```

For example:

```
https://raw.githubusercontent.com/illia-dorohin-ct/essity-presentations-images/main/tena-media/presentation/image001.png
```

This URL is used in the admin panel as the image source.

---

## How to Add a New Image

1. Open the target folder on GitHub (e.g. `tena-media/slide05/`)
2. Click **Add file** → **Upload files**
3. Drag and drop your image or click "choose your files"
4. Name the file following the convention: `image007.png` (next sequential number)
5. Click **Commit changes**
6. Copy the raw URL: click on the file → click **Raw** button → copy the URL from the browser
7. Paste the URL in the admin panel (image field)

## How to Replace an Existing Image

1. Navigate to the file on GitHub (e.g. `tena-media/slide05/image003.png`)
2. Click the **pencil icon** (Edit) or the **...** menu → **Delete this file** → commit
3. Upload the new image with the **same filename** (see "How to Add" above)
4. The URL stays the same — no changes needed in the admin panel

**Alternative (faster):**
1. Navigate to the folder
2. Click **Add file** → **Upload files**
3. Upload a file with the **same name** as the one you want to replace
4. GitHub will overwrite it automatically
5. Commit changes — the URL stays the same

## How to Delete an Image

1. Navigate to the file on GitHub
2. Click the **...** menu (top-right of the file view) → **Delete this file**
3. Click **Commit changes**
4. Remove the URL from the admin panel (clear the image field)

## Naming Convention

| Type | Format | Example |
|------|--------|---------|
| Regular image | `image{NNN}.{ext}` | `image001.png`, `image012.jpeg` |
| Screenshot | `image{NNN}_screenshot.{ext}` | `image005_screenshot.png` |

- Numbers are zero-padded to 3 digits (001, 002, ...)
- Each slide folder has its own numbering starting from 001
- Supported formats: `.png`, `.jpg`, `.jpeg`

## Important Notes

- This repository must remain **public** for images to be accessible on the website
- Do not rename the repository or change the branch name (`main`)
- After adding or replacing images, allow ~1 minute for GitHub CDN cache to update
- Maximum file size on GitHub: 100 MB per file
