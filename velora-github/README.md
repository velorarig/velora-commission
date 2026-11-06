# Velora | Live2D Artist & Rigger

Commission website for Velora (Live2D models, chibi VTubers and rigging).
It is a plain static site, so it works on GitHub Pages with no build step.

## How to publish on GitHub Pages

1. Create a new repository on GitHub (for example `velora`). Make it **Public**.
2. Click **Add file > Upload files** and drag in `index.html` and the `source` folder from this package.
   The file called `index.html` in the main folder is the one that is shown on the website.
3. Click **Commit changes**.
4. Go to **Settings > Pages**.
5. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, then press **Save**.
6. Wait about one minute. Your site will be at `https://YOUR-USERNAME.github.io/velora/`.

Tip: name the repository `YOUR-USERNAME.github.io` if you want the site at `https://YOUR-USERNAME.github.io/`.

## What is inside

| File | What it is |
|---|---|
| `index.html` | The website. All images are embedded, so it works on its own. |
| `source/` | An editable copy with separate image files in `source/assets/`. Not needed for the website to work. |

## Things to edit (open `index.html`, search for the words below)

- **Prices:** find `SERVICES`. Chibi prices and the Expression add-on price are placeholders.
- **Add-on prices:** find `ADDONS`.
- **Ko-fi payment link:** find `kofiPayUrl` and put your Ko-fi commission or shop page link there.
- **Email button (optional):** find `email:` in `CONFIG` and add your email.
- **FAQ answers:** search for `<summary>` to find each question.

## Adding new artwork or videos

The `source/` copy keeps images as normal files, which makes this easy:

1. Put the new image in `source/assets/`.
2. Add a line to `WORKS` in `source/index.html`. A YouTube video looks like
   `{ cats:["rigging"], tag:"Rigging · Demo", title:"Face tracking test", desc:"...", youtube:"VIDEO_ID" },`
3. To make it the live site, copy `source/index.html` and the `source/assets` folder to the main folder of the repository (so `index.html` and `assets/` sit side by side), replacing the old `index.html`.

Art and designs belong to Velora. Please do not use or repost without permission.
