# Sujjal Chapagain — personal website

Plain HTML and CSS: no build step and nothing to install. GitHub Pages hosts it for free.

```
index.html               home page: About me + News (fits one screen)
research.html            research
projects.html            projects + machine learning practice
honors.html              honors & leadership
cv.html                  education, CV and documents
assets/css/style.css     colors, fonts, layout
assets/img/              put profile.jpg here
files/cv/                your CV (the "Download CV" button points here)
files/certificates/      certificates, posters, slides
.nojekyll                tells GitHub Pages to serve files as they are
```

## Put it online (one time)

1. On GitHub, create a **public** repository named exactly **`Sujjal1.github.io`**. Don't add a README.
2. In a terminal, from this folder:
   ```bash
   git init
   git add .
   git commit -m "Personal website"
   git branch -M main
   git remote add origin git@github.com:Sujjal1/Sujjal1.github.io.git
   git push -u origin main
   ```
3. On GitHub, open the repo's **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, then select branch **main** and folder **/ (root)**, and click Save.
4. After a minute or two the site is live at **https://Sujjal1.github.io**.

## Update it later

Edit the files, then run:
```bash
git add . && git commit -m "Update site" && git push
```
The site updates within a minute or two.

- **Sidebar:** it is repeated at the top of all five .html files. If you change it (e.g. add LinkedIn), change it in each file.
- **New project:** in `projects.html`, copy an `<article class="card">…</article>` block and edit it.
- **News item:** in `index.html`, add a `<li>` at the top of the News list. Keep about 3–4 items so the home page still fits one screen.
- **New CV:** replace `files/cv/Sujjal_Chapagain_CV.pdf`, keeping the same file name.
- **Photo:** add `assets/img/profile.jpg`, then follow the PHOTO comment in the sidebar (in each .html file).
- **LinkedIn:** remove the comment marks around the LinkedIn line in the sidebar and paste your URL.

To preview locally, open `index.html` in a browser.
