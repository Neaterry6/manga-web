# Manga Reader

A feature-rich manga reading web app built with HTML, CSS, and JavaScript, using the MangaDex API. Features include offline support, user accounts, recommendations, downloads, and push notifications.

## Setup

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd manga-readerInstall dependencies:npm installRun locally:npm startOpen http://localhost:3000 in your browser.DeploymentDeploy to Vercel:Push the repository to GitHub.Connect the repository to Vercel via the dashboard.Deploy with default settings (Vercel auto-detects the static site).FeaturesSocial login (simulated)Manga bookmarks and favoritesChapter downloads as ZIPPush notificationsOffline reading via service workerAdvanced recommendationsResponsive design---

### Deployment Instructions
1. **Create Repository**:
   - Create the directory structure and save the files.
   - Initialize Git:
     ```bash
     mkdir manga-reader
     cd manga-reader
     git init
     git add .
     git commit -m "Initial commit: Manga reader app"
     ```
   - Push to GitHub:
     ```bash
     git remote add origin <your-repo-url>
     git push -u origin main
     ```

2. **Vercel Setup**:
   - Sign up/log in at [vercel.com](https://vercel.com).
   - Click **New Project**, import your `manga-reader` repository.
   - Set **Root Directory** to `public`.
   - Leave other settings default and click **Deploy**.

3. **Test**:
   - Access the deployed URL (e.g., `https://manga-reader.vercel.app`).
   - Verify features: manga loading, offline mode, notifications, downloads.
   - Check service worker in DevTools > Application > Service Workers.

4. **Updates**:
   - Commit and push changes:
     ```bash
     git add .
     git commit -m "Update feature"
     git push
     ```
   - Vercel auto-deploys.

---

### Notes
- **Vercel Fix**: The `vercel.json` now uses `rewrites` instead of `routes`, ensuring compatibility with `headers`.
- **Loading Image**: Ensure `public/assets/loading.png` is included. If unavailable, use a placeholder and update paths.
- **MangaDex API**: May have rate limits or CORS issues. For production, proxy requests via a Vercel Function.
- **Local Testing**: Run `npm install && npm start` to test at `http://localhost:3000`.
- **Troubleshooting**:
  - Service worker issues: Verify `sw.js` at `/sw.js`.
  - CORS: Set up a proxy if MangaDex API fails.
  - Notifications: Test in Chrome/Firefox; iOS support is limited.