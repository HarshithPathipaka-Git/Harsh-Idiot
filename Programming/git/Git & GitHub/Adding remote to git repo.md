# For remote adding
## use always ssh url to clone the repo
- For New git 
echo "# git-demo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:HarshithPathipaka-Git/git-demo.git
git push -u origin main


- for existing 
git remote add origin git@github.com:HarshithPathipaka-Git/git-demo.git
git branch -M main
git push -u origin main