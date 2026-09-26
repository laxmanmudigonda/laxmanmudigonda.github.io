# Laxman Mudigonda — Portfolio

Complete editable source for the portfolio. Plain HTML, CSS, and JavaScript; no npm installation, build step, API keys, or backend required.

## Publish using GitHub's website

1. Extract this ZIP on your computer.
2. Create a public GitHub repository named `portfolio`.
3. Upload the extracted files into the repository root and commit to `main`. Upload the files themselves, not the ZIP or an enclosing folder. `index.html` must be at the repository root.
4. Open repository Settings → Pages.
5. Under Build and deployment, choose Deploy from a branch.
6. Select branch `main` and folder `/(root)`, then Save.
7. Wait for the Pages deployment to finish. Settings → Pages will show your published URL, normally `https://YOUR-USERNAME.github.io/portfolio/`.

For a shorter address, name the repository `YOUR-USERNAME.github.io`; the address will then be `https://YOUR-USERNAME.github.io/`.

The included `.nojekyll` file disables Jekyll processing. If your file picker hides it, you can create an empty file with this name using GitHub's Add file menu. The site uses relative asset URLs so project repositories work too.

## Optional: upload using Git

Create an empty GitHub repository first. From the extracted folder, replace YOUR-USERNAME below and run:

```sh
git init
git add .
git commit -m "Add personal portfolio"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
git push -u origin main
```

Then enable Pages using steps 4–7 above. Authenticate with your own GitHub account when prompted.

## Files and editing

- `index.html`: biography, experience, education, certifications, contact details, and page structure.
- `style.css`: colors, fonts, spacing, responsive layout, and interaction styling.
- `app.js`: project content, project filters and dialogs, skills explorer, and copy-email action.
- `favicon.svg`: browser tab icon.
- `.nojekyll`: static hosting configuration.

Edit the `projects` array in `app.js` to add or change projects. Edit `skillData` to update skills. Update the All work count in `index.html` when changing the number of projects. Contact email appears in both `index.html` and `app.js`.

## Preview locally

Open `index.html` directly for a quick look, or run this command from the folder if Python is installed:

```sh
python -m http.server 8000
```

Visit `http://localhost:8000`. Clipboard copying works on supported secure browser contexts; the email link is also available.

## Hosting notes

Google Fonts are loaded from an external stylesheet, with local sans-serif fallbacks. Email links open the visitor's mail application; there is no contact-form server. The portfolio has no analytics or tracking code.

This export is independent of the existing ChatGPT-hosted site. Updating GitHub does not update that site, and vice versa. Changes committed to the selected GitHub Pages publishing branch will trigger publication there.

Review project descriptions and personal contact details before making your repository public. Project source repositories and demos are not bundled here; this archive contains the portfolio website itself.

## Official instructions

https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
