# Deploy to GitHub Pages

## Folder contents

- index.html, research.html, newsroom.html, ieva-flpp.html: the four pages (self-contained)
- images/: add your graphics here (see images/README.md for filenames and sizes)
- .nojekyll: tells GitHub to publish the files as they are

## First deployment (no software needed)

1. Create a free account at github.com and sign in.
2. Click **+** (top right) > **New repository**. Name it `oralhealthresearch`, choose **Public**, click **Create repository**.
3. On the empty repository page click **uploading an existing file**.
4. Unzip this folder on your computer. Select everything inside it (all four .html files, the `images` folder and `.nojekyll`) and drag it into the browser window. Hidden files such as `.nojekyll` may not show in Finder or Explorer; if so, skip it, the site works without it.
5. Click **Commit changes**.
6. Go to **Settings > Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and folder **/ (root)**, then **Save**.
7. After 1 to 2 minutes the site is live at `https://YOUR-USERNAME.github.io/oralhealthresearch/`.

## Adding the graphics

1. Prepare the files as described in `images/README.md` (exact filenames).
2. Open the repository, go to the `images` folder, click **Add file > Upload files**, drop the images, **Commit changes**.
3. Wait about a minute and refresh the site (Ctrl/Cmd + Shift + R). Missing images keep their gray placeholder.

## Updating a page

Replace the .html file: open the repository, **Add file > Upload files**, drop the new file with the same name, commit.

## Custom domain (later)

1. Settings > Pages > **Custom domain**: enter your domain (for example `www.oralhealthresearch.lv`) and save.
2. At your domain registrar add a **CNAME** record: name `www`, value `YOUR-USERNAME.github.io`. For a bare domain add four **A** records pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153 and 185.199.111.153.
3. When the DNS check passes, tick **Enforce HTTPS**.

## Notes

- Page links are relative, so keep all four .html files in the same folder.
- File names are case sensitive on GitHub: keep them lowercase.
- Free GitHub Pages sites have a 1 GB size limit; keep images compressed.
