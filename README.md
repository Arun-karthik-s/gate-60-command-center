# GATE CS 2027 · 60+ Study Command Center

A focused, offline-first study app for GATE CSE 2027. It combines the 60+ roadmap, one-hour daily plan, syllabus tracking, PYQs, mock analysis, notes/formulae and progress analytics in one place.

## Design

The UI intentionally avoids the usual glossy/gradient “AI dashboard” look. It uses a restrained study-workspace layout built from the supplied palette:

- `#FFFFFF` — canvas / surfaces
- `#1B1B1B` — navigation / primary text
- `#FF4FA3` — primary action / active state
- `#00C2CB` — progress / secondary action
- `#FDB9C9`, `#FFDCBE`, `#F6F3B5`, `#BBF6F3`, `#A7E0F4` — soft status and section accents

## Run locally

Open `index.html` in a browser. The app stores study data in `localStorage` on that device.

For the PWA/offline install experience, serve the folder over HTTP (for example with VS Code Live Server or `python -m http.server`).

## Publish for anyone to view

### Recommended: GitHub Pages

1. Create a **public** GitHub repository, for example `gate-cs-2027-60-plus`.
2. Upload every file/folder from this directory, including `.github/workflows/deploy-pages.yml`.
3. Commit to the `main` branch.
4. Open **Settings → Pages**. Under the build/deployment section, select **GitHub Actions** if GitHub has not already selected it.
5. The included workflow publishes the site automatically. GitHub will show the public URL in the workflow run and Pages settings.

After that, every push to `main` updates the public site.

### Fast alternative: Netlify Drop

Use Netlify's drag-and-drop deploy page and drop this entire folder. Netlify gives you a public `*.netlify.app` URL immediately. A custom domain can be connected later.

## Important privacy note

The app is intentionally offline-first. Each visitor gets their **own local progress**. Hosting the app publicly does not combine everyone's study data into one database.

## Updating the app

Replace `index.html` and any supporting assets in the repository, commit, and push. The GitHub Pages workflow redeploys automatically.
