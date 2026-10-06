# Anywebapp

A one-page web app for GitHub Pages. You type a link, it opens that link. Next time you start it, it opens the same link by itself.

## Setup

1. Repo **Settings → Pages → Build and deployment**: Source "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
2. After a minute the site is live at `https://<your-username>.github.io/Anywebapp/`.
3. Open that address in Safari on the iPad → Share button → **Add to Home Screen**.
4. Start it from the home screen, type your link, tap **Open**.

The link is saved on the device. When you start the app it waits about a second before opening it, so you can tap "Stop, I want to change the link" if you want a different one.

You can also pass the link in the address: `.../Anywebapp/?url=https://example.com`

## Changing the home screen icon

Replace `icon.png` with your own image (square PNG, 512×512 works well, at least 180×180). Keep the file name.

To change the name under the icon, edit `apple-mobile-web-app-title` in `index.html` and `name`/`short_name` in `manifest.json`.

iOS copies the icon when you add the app to the home screen. After changing it, delete the home screen icon and add it again (sometimes clearing Safari's website data helps if the old icon sticks).
