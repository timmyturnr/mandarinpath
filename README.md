# MandarinPath iPhone app package

This package turns the existing MandarinPath HTML app into an installable Progressive Web App (PWA).

## Important iPhone-only limitation
An actual signed native `.ipa` cannot be built or installed directly from an iPhone alone using Apple's standard tools. This package is the practical free route: host it over HTTPS, then add it to the iPhone Home Screen. It opens in an app-like full-screen window and has offline caching.

## Free installation using GitHub Pages
1. In Safari on your iPhone, sign in or create a free account at https://github.com.
2. Create a new repository named `mandarinpath`. For the simplest setup, make it public.
3. Upload the files and folders in this package to the repository root. Upload `index.html`, `manifest.webmanifest`, `sw.js`, and the `icons` folder with its four PNG files. Do not upload the ZIP itself as the only file.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
6. Wait for GitHub Pages to publish. The site URL will look like `https://YOUR-USERNAME.github.io/mandarinpath/`.
7. Open that URL in Safari on your iPhone. Tap **Share** (square with arrow) → **Add to Home Screen**. If offered, enable **Open as Web App**, then tap **Add**.
8. Launch MandarinPath from the new Home Screen icon. Open it once while online so the offline cache can install.

## Notes
- Hosting is free on GitHub Pages for a public repository.
- The app contains no ads, trackers, or paid features.
- Browser speech synthesis depends on the Mandarin voice available on iOS.
- Learning progress uses local browser storage. Avoid clearing Safari website data for this site.
- If you update files later, refresh the site while online. Service-worker updates may take a moment to apply.
