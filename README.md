# CliCraft
Handy commands when working from command line.

# Git/GitHub
Create new repository and push it to GitHub.

1. Log into GitHub
2. Select "New Repository"
3. Give the repository a name

From a terminal execute the following:

```bash
mkdir <name-of-project>
cd <name-of-project>
echo "# A headline" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/<GitHub-user-name>/<name-of-repository>.git
git push -u origin master
```

