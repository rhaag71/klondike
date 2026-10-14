# Plain Klondike

Klondike solitaire. No ads, no accounts, no scores sent anywhere, no network calls.

## Put it on your iPhone
iOS only installs offline web apps from an HTTPS address, so host this folder once:

1. Push this folder to a GitHub repo and turn on GitHub Pages (Settings > Pages > deploy from branch).
   Any static HTTPS host works.
2. Open the Pages URL in **Safari** on the iPhone.
3. Share > **Add to Home Screen**.
4. Launch it from the home screen once while online. After that it runs fully offline.

## Test locally
    python3 -m http.server 8000
then open http://localhost:8000 (service workers are allowed on localhost).

## Updating
Change files, bump `CACHE` in `sw.js`, push. The phone picks it up next time it launches online.
