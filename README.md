# Faithful Gameday

A 49ers gameday soundboard — five sound buttons, a selfie/camera button, a live
crowd-noise meter (uses your mic), and confetti on the foghorn.

This is a **static site** — no build step, no framework, no server. Just HTML, CSS,
and vanilla JavaScript. To run it, you only need to serve the folder.

## Files

```
index.html            The whole app
assets/
  background.png      Stadium background
  button.png          Red gameday button
  camera.png          Selfie camera icon
  Gameday_Song.mp3    GAMEDAY SONG
  Hypesong.mp3        HYPESONG
  foghorn.mp3         FOGHORN
  Defense.mp3         DEFENSE
  Fox.mp3             FOX
  confetti.min.js     canvas-confetti (vendored locally)
```

## Run it locally

Open a terminal in this folder and run any static server, e.g.:

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000

> The microphone noise meter and the selfie camera require **HTTPS** (or
> localhost). GitHub Pages serves over HTTPS, so both work once published.

## Publish on GitHub Pages

1. Create a new repository on github.com and upload **all** of these files
   (the `index.html` and the whole `assets/` folder), keeping the structure.
2. In the repo: **Settings → Pages → Build and deployment → Source = Deploy from a branch.**
3. Set the branch to **main** and the folder to **/ (root)**, then **Save**.
4. Wait ~1 minute. Your site goes live at
   `https://<your-username>.github.io/<your-repo-name>/`

All asset paths are relative, so it works no matter what you name the repo —
no configuration needed.
