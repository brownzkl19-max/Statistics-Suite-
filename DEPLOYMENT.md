# Publish Statistics Suite

## 1. Enable GitHub Pages
1. Open the repository: https://github.com/brownzkl19-max/Statistics-Suite-
2. Select **Settings** → **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**, then save.
5. Wait for the Pages deployment to finish. The expected project URL is:
   https://brownzkl19-max.github.io/Statistics-Suite-/

The app is not publicly live until GitHub Pages is enabled and its deployment succeeds.

## 2. Embed it in Google Sites
1. Open the Google Site in edit mode.
2. Select **Insert** → **Embed** → **By URL**.
3. Paste the published GitHub Pages URL.
4. Insert the embed, resize the frame, and publish the Google Site.

GitHub Pages hosts the interactive application. Google Sites displays it inside an embed; it does not host the app's source files.

## 3. Submit the site to Google Search
1. Open Google Search Console: https://search.google.com/search-console/
2. Add a URL-prefix property for the GitHub Pages URL above.
3. Complete the ownership verification steps shown by Search Console.
4. Open **Sitemaps** and submit `sitemap.xml`.
5. Use **URL Inspection** to request indexing for the home page.

Search indexing and ranking are controlled by Google and are not guaranteed. A sitemap helps discovery but does not guarantee that a page will be indexed.

## 4. Install and test the app
- Open the published URL in a supported browser. Use the browser's install option when it is offered.
- On mobile, use the browser menu's **Add to Home Screen** or **Install app** option when available.
- Load the app once while online before testing offline mode.
- The service worker caches the app shell and falls back to the cached home page for navigation when offline.

## 5. Notes
- The service worker and install features require HTTPS; GitHub Pages provides HTTPS.
- After changing the cached app shell, update the cache version in `service-worker.js` so browsers refresh old cached files.
- CSV data is processed locally in the browser. Avoid loading confidential data on shared devices.
- The sitemap and canonical URL use the expected GitHub Pages address above. Confirm that Pages is enabled at that address before submitting it to Search Console.