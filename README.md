cd <your-visual-studio-project-folder>
git init
git add . # Add everything in the current directory (".")
git commit

git remote add origin <url-for-your-remote>
git fetch origin

# Rebase your local root commit onto the remote root commit
git rebase --onto origin/master --root

# Now you can push to your remote
git push origin master
