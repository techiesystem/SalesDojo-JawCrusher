# Propel Jaw Crusher Sales Dojo

A build-free, responsive HTML presentation preserving all 20 original slide graphics. Includes previous/next controls, searchable thumbnails, station filtering, direct screen selection, keyboard navigation, swipe and fullscreen.

## Deploy using GitHub Actions
1. Create a GitHub repository with `main` as the default branch.
2. Extract this ZIP and add its contents to the repository root. Include `.github/workflows/pages.yml`; some file explorers hide this folder.
3. Commit and push the files to `main`.
4. Open **Settings → Pages → Build and deployment → Source**, and choose **GitHub Actions**.
5. Open **Actions → Deploy Sales Dojo to GitHub Pages → Run workflow**, then select `main`.
6. Wait for the workflow to succeed. Open the published URL shown under Settings → Pages or the workflow deployment.

Typical project URL: `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`.

## Simpler alternative: deploy from a branch
Choose **Settings → Pages → Source → Deploy from a branch**, select **main** and **/docs**, then Save. Use one publishing method. When choosing branch publishing, remove `.github/workflows/pages.yml` to avoid a second deployment workflow.

## Files
- `docs/index.html`: viewer, styling, slide list and navigation.
- `docs/assets/slide-01.png` through `slide-20.png`: original slide graphics.
- `docs/.nojekyll`: static-file publishing marker.
- `.github/workflows/pages.yml`: automatic deployment on changes to main.

## Local use and edits
Open `docs/index.html` in a browser. No installation, API key, server, build step or third-party runtime dependency is required. Asset paths are relative, so the viewer also works beneath a repository path. Edit the slide titles/group labels in the `slides` array inside index.html. Replace image files while retaining names to update graphics. Deep links use `#screen-1` through `#screen-20`.

GitHub Pages access and availability follow your repository plan and organization settings. Publishing may expose the content publicly; check Settings → Pages access before sharing.

## Verification
All 20 assets are present; JavaScript syntax and navigation/filter logic passed checks. Visual browser QA and deployment to your GitHub account were not performed.

References:
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages
