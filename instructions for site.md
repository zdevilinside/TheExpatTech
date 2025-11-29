

# 🚀 Hugo → GitHub Pages Deployment Checklist

## 1. Make changes locally
- Edit or add content in your Hugo site’s `content/` folder.
## 2 run the following command and verify the localsite:1313 shows the content properly.
  *hugo server -D*

## 3 Build the site
*hugo*
## 4 Commit changes
*git add .*
*git commit -m "Update Hugo site content"*
## 5 Push to Github
*git push origin main*

copy/paste of the instructions together
Hugo
git add .
git commit -m "reason for update"
git push origin main

## 6 Option B - Deploy from gh-pages branch
hugo
cd public
git init
git remote add origin https://github.com/USERNAME/REPO.git
git checkout -b gh-pages
git add .
git commit -m "Deploy site"
git push -f origin gh-pages

