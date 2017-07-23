# CliCraft
Handy commands when working from command line.

# Git/GitHub
Create new repository and push it to GitHub.

1. Log into GitHub using \<user-name\>
2. Select "New Repository" 
3. Give the repository a name \<repository-name\>

From a terminal execute:

```bash
mkdir <name-of-project>
cd <name-of-project>
echo "# A headline" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/<user-name>/<repository-name>.git
git push -u origin master
```

# find/grep
Combining find and grep to locate text in files.

Traverse current directory looking in all txt-files for a string "needle".

```bash
find . -type f -name '*.txt' -exec grep -Hine "needle" {} \;
```

Traverse current directory looking in multiple file types for a string "needle".

```bash
find . -type f \( -name '*.js' -o -name '*.htm' -o -name '*.html' -o -name '*.ejs' -o -name '*.json' \) -exec grep -Hine "needle" {} \;
```
