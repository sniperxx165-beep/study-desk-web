# Study Desk — web app (PWA)

This is the same Study Desk app (with sync + auto-sync built in), set up to be
hosted as a website so it can be installed on iPhone, Android, Windows, Mac,
and Linux alike — no App Store, no installer files needed.

## Deploy it with GitHub Pages (free)

1. Create a new GitHub repo (can use GitHub Desktop like before) called
   something like `study-desk-web`.
2. Put all the files from this folder directly at the repo's root:
   `index.html`, `manifest.json`, `service-worker.js`, and the four
   `icon-*.png` files.
3. Commit and push.
4. On the repo's GitHub page, go to **Settings → Pages**. Under "Build and
   deployment," set Source to "Deploy from a branch," branch `main`, folder
   `/ (root)`. Save.
5. GitHub gives you a URL like `https://yourname.github.io/study-desk-web/`.
   It can take a minute or two to go live the first time.

## Installing it

- **iPhone (Safari):** open the URL → tap the Share icon → "Add to Home
  Screen." It now opens full-screen like a normal app.
- **Android (Chrome):** open the URL → menu (⋮) → "Install app" (or "Add to
  Home screen").
- **Windows/Mac/Linux (Chrome/Edge):** open the URL → there's usually an
  install icon in the address bar → click it to install as a desktop app.
- Anyone can also just open the URL in any browser without installing
  anything at all — it works either way.

## Syncing

Nothing changes here — open "Sync across devices" the same way as on
desktop, enter your existing Render server URL and code (or a new one), and
it'll sync exactly the same way, since it's the identical code talking to
the identical server.

## Note on hosting publicly
Anyone with the URL can open the app itself, but they can't see YOUR data
unless they also know your specific sync code — the app itself has no
data in it until sync is configured. Treat it the same as sharing the
`.exe` with friends: fine for casual use, just don't publish your sync code
publicly anywhere.
