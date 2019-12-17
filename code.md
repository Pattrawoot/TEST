chmod 600 ~/.ssh/id_rsa
git clone 

git checkout -b issue-4
git add code.md
git commit -m "    - close #4"
git remote update
git rebase origin/master
git checkout master
git merge issue-4 --no-ff
git push origin master