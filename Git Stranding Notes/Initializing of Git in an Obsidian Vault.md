---
favicon: https://github.com
---
---
# Guide
```bash
# 1. Create a repository in GitHub

# 2 Open CLI and navigate it through the obsidian vault that contains  .obsidian folder
cd ..
cd <folder directory>
or in Windows 11, right-click in an open space inside the vault and click 'Open in Terminal'
or if git bash is installed → right-click in an open space inside the vault and click 'Open with Git Bash here'

# 3. Initialize the repository
git init

# 4. Connect repository to the created remote repo in GitHub 
git remote add origin <GitHub repository URL>

# 5. Fetch commits if behind
# e.g. Remote repository has Readme.md file, but local does not
git fetch 

# 6. Pull them from GitHub to local repository
git pull origin main
```
