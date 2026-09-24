# Shishir Madhav — Portfolio

A static portfolio website. It includes the portrait, project links, contact details, and a downloadable PDF resume. No package manager or build step is needed.

## Files

- `index.html` — complete website (HTML, CSS, and JavaScript)
- `assets/shishir-headshot.png` — portfolio portrait
- `assets/Shishir_Madhav_Resume.pdf` — downloadable resume

Keep `index.html` and the `assets` folder at the top level of your GitHub repository. Do not upload only the ZIP file to GitHub; extract it first.

## Push to GitHub

### In the browser

1. Create a new GitHub repository, for example `shishir-portfolio`.
2. Extract the ZIP and open the extracted folder.
3. In the repository, choose **Add file → Upload files** and upload `index.html`, `README.md`, and the entire `assets` folder. Make sure the uploaded file paths retain `assets/shishir-headshot.png` and `assets/Shishir_Madhav_Resume.pdf`.
4. Commit the files.

### With Git (alternative)

Open a terminal in the extracted folder and run:

```bash
git init
git add index.html README.md assets
git commit -m "Add portfolio website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/shishir-portfolio.git
git push -u origin main
```

Replace `YOUR-USERNAME` and the repository name with yours. Create the empty GitHub repository first. If Git asks for your identity, set your Git username and email on your computer.

## Deploy on Vercel

1. Open [Vercel New Project](https://vercel.com/new) and import your GitHub repository.
2. Select **Other** as the Framework Preset.
3. Keep the Root Directory as the repository root (`.`). Leave the Build Command empty, and serve the root directory as the Output Directory. If Vercel shows an Override toggle for Build Command, enable it and leave the command empty.
4. Click **Deploy**. Future pushes to the connected GitHub repository deploy automatically.

If `index.html` is at the repository root and there is no `public` folder, Vercel's Other preset serves the root files directly.

## Edit your portfolio

Open `index.html` in an editor. The page content, styling, and interactions are all in that file. After making changes, commit and push to GitHub. For a new resume, replace `assets/Shishir_Madhav_Resume.pdf` with the same filename, then push the change.

## Preview locally

From the extracted folder, run `python -m http.server 8000` and open `http://localhost:8000` in a browser.
