# Joey M Photography website

This folder is the whole site: `index.html` plus a `photos/` folder.

## Put it online with GitHub Pages

1. On GitHub, click **New repository**. Name it something like `photography`, set it to **Public**, and create it.
2. On the new repo page, click **uploading an existing file**. Drag in `index.html`, `README.md` and the whole `photos` folder, then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, pick **main** and **/(root)**, then click **Save**.
4. After a minute or two the site will be live at **https://joeymcreatives.github.io/photography/** (or whatever name you gave the repo).

## Before you share it

Open `index.html` in any text editor (even Notepad works) and look for **EDIT YOUR SITE HERE** near the bottom:

- `email`: put in the email address where booking requests should go. The booking form opens the visitor's email app addressed to this.
- `instagram` and `facebook`: paste the full links, for example `https://instagram.com/yourhandle`. Leave them as `""` to hide them.

## Changing photos

- **Add a photo:** put the file in `photos/`, then add a line to the `PHOTOS` list, for example:
  `{ file: "events-09.jpg", group: "events", shape: "tall", date: "2026-12-20", alt: "Couple's first dance" },`
  - `group` is one of `events`, `people`, `places` or `cats`
  - `shape` is `tall` for portrait photos, `wide` for 16:9, or `3:2` / `4:3`
- **Remove a photo:** delete its line from `PHOTOS`.
- **Top photo:** change `HERO`. The `focus` value moves the crop up or down: lower numbers show more of the top.
- **Row of three:** change `FEATURED`.
- **Category covers:** change `COVERS`.
- **Photo in the About section:** add a file named `me.jpg` to `photos/` and it shows up automatically.

Keep photos around 1800px on the long side so the site loads fast. The ones in here were already resized, and their hidden camera data (including any location info) was removed.
