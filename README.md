# Joey M Photography website

This folder is the whole site: `index.html` plus a `photos/` folder.

## Put it online with GitHub Pages

1. On GitHub, click **New repository**. Name it something like `photography`, set it to **Public**, and create it.
2. On the new repo page, click **uploading an existing file**. Drag in `index.html`, `README.md` and the whole `photos` folder, then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, pick **main** and **/(root)**, then click **Save**.
4. After a minute or two the site will be live at **https://joeymcreatives.github.io/photography/** (or whatever name you gave the repo).

## Your contact details

Your email and Instagram are already filled in. To change them later, open `index.html` in any text editor (even Notepad works), find **EDIT YOUR SITE HERE** near the bottom, and edit the `SITE` section. Leave a link as `""` to hide it.

## Changing photos

- **Add a photo:** put the file in `photos/`, then add a line to the `PHOTOS` list, for example:
  `{ file: "events-08.jpg", group: "events", focus: "50% 50%", date: "2026-12-20", alt: "Couple's first dance" },`
  - `group` is one of `events`, `people` or `places`
  - `focus` picks which part of the photo stays in view when it's cropped to the grid. "50% 50%" is the center. A lower second number keeps more of the top.
  - The gallery shows 3 photos per row, so it looks neatest with 15, 18 or 21 photos.
- **Remove a photo:** delete its line from `PHOTOS`.
- **Top photo:** change `HERO`.
- **Row of three:** change `FEATURED`.
- **Category covers:** change `COVERS`.
- **Photo in the About section:** add a file named `me.jpg` to `photos/` and it shows up automatically.

Keep photos around 1800px on the long side so the site loads fast. The ones in here were already resized, and their hidden camera data (including any location info) was removed.
