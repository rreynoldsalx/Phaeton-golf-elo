# Publish Package (GitHub Pages)

This folder is ready to be uploaded to a GitHub repository and served as a website.

## Files
- `index.html`: main dashboard page (this is the page visitors open)
- `assets/playerCatalog.js`: player lookup data used by the dashboard
- `assets/playerSeries.js`: historical player Elo series data
- `assets/tournamentStrengthData.js`: tournament strength timeline data
- `.nojekyll`: keeps GitHub Pages from applying Jekyll processing

## Quick local test
From this `publish/` folder:

```powershell
c:/Users/RyanReynolds/Desktop/Phaeton3/.venv/Scripts/python.exe -m http.server 8080
```

Then open: `http://localhost:8080`

## Deploy to GitHub Pages
1. Create a GitHub repository (or use an existing one).
2. Upload all files and subfolders in this folder to the repository root (or commit/push via git).
3. In GitHub: `Settings` -> `Pages`.
4. Under `Build and deployment`:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main` (or `master`), folder `/ (root)`
5. Save and wait 1-2 minutes.
6. GitHub will show your public site URL.

## URL format
- User/org site repo name: `<username>.github.io`
  - URL: `https://<username>.github.io/`
- Project repo (any other name):
  - URL: `https://<username>.github.io/<repo-name>/`

If this is a project repo, `index.html` in this folder will be the landing page at that URL.
