# 🚀 Git Version-Controlled DevOps Project – Task 4

This project demonstrates the use of **Git best practices** to manage a DevOps workflow, including branching, pull requests, tagging, and documentation.

---

## 🎯 Objective
Set up a Git-based workflow that follows industry standards for:
- Repository initialization
- Branching strategy
- Pull request (PR) workflow
- Version tagging
- Proper documentation

---

## 🛠️ Tools & Technologies
- **Git** – Version control
- **GitHub** – Remote repository hosting and collaboration
- **Markdown** – Documentation format

---

## ✅ What Was Done
- Initialized a new Git repository locally
- Created and pushed to GitHub
- Established branching strategy (`main`, `dev`, `feature`)
- Added `.gitignore` file
- Implemented a sample build script (`build.sh`)
- Merged feature branch to dev via Pull Request
- Merged dev branch to main via Pull Request
- Tagged first stable release (`v1.0`)
- Documented all steps in Markdown (`README.md` and `docs.md`)

---

## 📂 Branching Strategy
- **main** → Production-ready code
- **dev** → Integration/testing branch
- **feature/*** → Isolated feature development

---

## 🔀 Pull Request Workflow
1. **feature → dev**
   - Feature branch changes are reviewed and merged into `dev`
2. **dev → main**
   - Tested and stable changes are merged into `main`
3. **Tag Release**
   - Tag created after merge to main for version tracking

---

## 📌 Commands Used
```bash
# Initialize repository
git init

# Add remote and push to GitHub
git remote add origin <repo-URL>
git branch -M main
git push -u origin main

# Create branches
git checkout -b dev
git push -u origin dev
git checkout -b feature/add-ci-cd
git push -u origin feature/add-ci-cd

# Add build script
echo "echo 'Running build...'" > build.sh
chmod +x build.sh
git add build.sh
git commit -m "Added basic build script"
git push

# Create and push tag
git tag -a v1.0 -m "First stable release"
git push origin v1.0


