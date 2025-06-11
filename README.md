# Manga Reader

A feature-rich manga reading web app built with HTML, CSS, and JavaScript, using the MangaDex API. Features include offline support, user accounts, recommendations, downloads, and push notifications.

## Setup

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd manga-readerInstall dependencies:npm installRun locally:npm startOpen http://localhost:3000 in your browser.DeploymentDeploy to Vercel:Push the repository to GitHub.Connect the repository to Vercel via the dashboard.Deploy with default settings (Vercel auto-detects the static site).FeaturesSocial login (simulated)Manga bookmarks and favoritesChapter downloads as ZIPPush notificationsOffline reading via service workerAdvanced recommendationsResponsive designDeployment Instructions for VercelCreate the Repository:Create the directory structure and save the files as shown above.Initialize a Git repository:mkdir manga-reader
cd manga-reader
git initAdd all files:git add .
git commit -m "Initial commit: Manga reader app"Create a GitHub repository (e.g., manga-reader) and push:git remote add origin <your-repo-url>
git push -u origin mainSign Up/Login to Vercel:Visit vercel.com and sign up or log in (GitHub login is recommended).Import the Repository:In the Vercel dashboard, click New Project.Select Import Git Repository and choose your manga-reader repository.Authorize Vercel to access GitHub if prompted.Configure the Project:Framework Preset: Vercel detects it as a static site.Root Directory: Set to public.Build Command: Leave blank.Output Directory: Leave as default (public).Environment Variables: None needed.Click Deploy.Test the Deployment:After deployment (~1-2 minutes), Vercel provides a URL (e.g., https://manga-reader.vercel.app).Test features: manga loading, offline mode, notifications, downloads, etc.Verify the service worker in DevTools > Application > Service Workers.Update the Site:Make changes, commit, and push:git add .
git commit -m "Update feature"
git pushVercel auto-deploys updates.
