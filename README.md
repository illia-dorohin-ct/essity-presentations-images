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

> Currently, files are named sequentially (`image001.png`, `image002.png`, etc.), but you can give any name to new files.

## How Image URLs Work

Every file in this repository is publicly accessible via a predictable URL:

```
https://raw.githubusercontent.com/illia-dorohin-ct/essity-presentations-images/main/{path-to-file}
```

For example, if you upload a file to `tena-media/slide05/photo.png`, its URL will be:

```
https://raw.githubusercontent.com/illia-dorohin-ct/essity-presentations-images/main/tena-media/slide05/photo.png
```

This URL is what you paste into the image field in the admin panel.

---

## How to Add a New Image

1. Open the target folder on GitHub (e.g. `tena-media/slide05/`)
2. Click **Add file** → **Upload files**
3. Drag and drop your image or click "choose your files"
4. Click **Commit changes**
5. Build the URL by combining the base URL with the file path:
   ```
   https://raw.githubusercontent.com/illia-dorohin-ct/essity-presentations-images/main/tena-media/slide05/your-file-name.png
   ```
6. Paste the URL into the image field in the admin panel

## How to Replace an Existing Image

1. Navigate to the folder containing the image
2. Click **Add file** → **Upload files**
3. Upload a file with the **same name** as the one you want to replace
4. Click **Commit changes** — GitHub will overwrite the old file
5. The URL stays the same, no changes needed in the admin panel

## How to Delete an Image

1. Navigate to the file on GitHub
2. Click the **...** menu (top-right of the file view) → **Delete this file**
3. Click **Commit changes**
4. Remove the URL from the admin panel (clear the image field)

## Important Notes

- This repository must remain **public** for images to be accessible on the website
- Do not rename the repository or change the branch name (`main`)
- After adding or replacing images, allow ~1 minute for GitHub CDN cache to update
- Maximum file size on GitHub: 100 MB per file
