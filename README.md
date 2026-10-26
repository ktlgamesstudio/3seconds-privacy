# 3 Seconds privacy policy website

Static, build-free GitHub Pages site for KTL Games. The landing page defaults to English and links to six approved localized policies. The files in this directory are the **only** files needed for publication; do not upload the Unity project or the audit worksheet.

## Local files

- `index.html` — English landing page and language selector.
- `privacy-policy.en.html`, `.tr.html`, `.de.html`, `.fr.html`, `.es.html`, `.pt-BR.html` — approved policy text preserved exactly inside each `<main>`; a navigation header and footer surround it.
- `assets/site.css` — shared responsive styling.
- `assets/3-seconds-icon.png` — approved 3 Seconds app icon.
- `.nojekyll` — tells GitHub Pages to serve the files directly without Jekyll processing.

All links are relative, so the site works at either a repository-root or project-subpath GitHub Pages address. No account, server application, analytics script, cookie banner, or build step is required by this website itself.

## Deploy on GitHub Pages — manual steps

1. Sign in to GitHub and create a **new public repository** dedicated to this policy website. A public repository is required for GitHub Pages on GitHub Free. Choose any available repository name; this packet does not assume or reserve one. Do not upload the Unity project.
2. Upload the **contents** of this `privacy-website` folder to the root of the repository, preserving `assets/`. The repository root must contain `index.html` and the six `privacy-policy.*.html` files. Include `.nojekyll`; it is an empty hidden file. Commit the upload to the repository's default branch.
3. In the repository, open **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, select the branch containing these files, choose **/(root)**, and click **Save**.
4. Wait for the Pages deployment to succeed. In **Settings → Pages**, select **Visit site** to obtain the actual public address. Do not guess the address from the repository name. Test `index.html`, all six language links, and the direct English policy page on the live site without signing in.
5. Enter the verified public privacy-policy address in Google Play Console. For a single default policy link, use the actual published English policy page; the page's header gives access to the other five languages. Add a privacy-policy entry point inside the Android app before release, then verify it opens the published page.
6. Before release, reconcile the published policy and Play Data Safety form with the final app binary, SDK configuration, and consent behavior. Keep the six translations synchronized when disclosures change.

GitHub's current instructions: [create a Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) and [configure a branch publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Local preview

Open `index.html` directly, or serve this directory with any static HTTP server. No package installation is needed.

## Publication status

Prepared locally only. No GitHub repository, remote, or public URL has been created.
