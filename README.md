echo "node_modules/
.DS_Store
frontend/.next/" > .gitignore

git rm -r --cached node_modules frontend/node_modules frontend/.next .DS_Store 2>/dev/null
git add .gitignore
git commit -m "Add gitignore, remove node_modules"
git push
