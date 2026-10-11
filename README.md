# DojaVerse

Unofficial, interactive Doja Cat fan encyclopedia. One `index.html`, no build step.
Not affiliated with or endorsed by Doja Cat, her management, or her labels.

## Files
`index.html` (app), `data.json` (catalog), `.nojekyll`, `.gitignore`, `README.md`

## Publish on GitHub Pages (website only)
1. Create a free account at github.com.
2. Click **New repository**, name it `dojaverse`, choose **Public**, click **Create repository**.
3. Click **Add file > Upload files**, drag in every file from this folder (including `.nojekyll`), click **Commit changes**.
4. Open **Settings > Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select branch **main** and folder **/ (root)**, click **Save**.
5. Wait 1 to 2 minutes, then open `https://USERNAME.github.io/dojaverse/`.

## Publish with Git
```
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/USERNAME/dojaverse.git
git push -u origin main
```

## Editing data
Open `data.json` on GitHub, click the pencil icon, edit, and **Commit changes**. Or add songs in the app's **Add song** form, click **Export JSON**, and paste the result into `data.json`.
Hard refresh (Ctrl+Shift+R) if changes do not appear.

## Troubleshooting
| Problem | Fix |
|---|---|
| 404 page | Check Settings > Pages is on, and that `index.html` is in the repo root |
| Blank page | Open browser console; make sure `index.html` was uploaded unmodified |
| Changes not showing | Wait 2 minutes, then hard refresh |
| "data.json could not be loaded" | Confirm the file name is exactly `data.json` in the root |

GitHub Pages is public hosting: anyone can view the source. The app stores favorites, playlists and scores only in the visitor's own browser (localStorage).
