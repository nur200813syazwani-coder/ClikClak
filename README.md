# ClikClak PWA package

This package wraps the supplied ClikClak HTML app as an installable Progressive Web App.

## Publish with GitHub Pages
1. Sign in to GitHub and create a repository named `clikclak`.
2. Upload **the contents of this folder** (not the ZIP itself) to the repository's root:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icons/` folder
3. Open repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main` and folder `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. Your link will look like:
   `https://YOUR-USERNAME.github.io/clikclak/`

## Install on iPad
1. Open the published link in **Safari**.
2. Tap Share (square with upward arrow).
3. Choose **Add to Home Screen**. If shown, enable **Open as Web App**.
4. Tap Add, then launch ClikClak from the Home Screen.

## Important data note
The supplied app stores its records in **IndexedDB** (browser-local storage), not a shared cloud database. Data saved on your computer, iPad and iPhone will be separate. Clearing Safari website data or deleting the web app may also affect locally stored records. Use the app's backup/export feature regularly and keep backup files somewhere safe.

The service worker caches the app shell for faster repeat loading and basic offline app-shell access. It does not synchronise inventory or orders between devices.
