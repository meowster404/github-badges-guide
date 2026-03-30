# 🏆 GitHub Profile Badges Achievement Guide

Welcome! This repository documents **how to earn GitHub Profile Badges** using a practical, step-by-step approach with GitHub CLI commands.

---

## 📖 About This Guide

GitHub Badges (also called Achievements) are special digital badges that appear on your GitHub profile to showcase your contributions and milestones. This guide walks you through the process of earning **multiple obtainable badges** using the GitHub CLI.

---

## 🎯 Badges Earned in This Guide

We successfully earned the following badges:

### ✅ **Pull Shark** 🦈
- **Requirement**: Merge 2 pull requests  
- **Difficulty**: Medium
- **Process**: Created 2 feature branches, opened PRs, and merged them into main

### ✅ **YOLO** 🤪
- **Requirement**: Merge a PR without peer review  
- **Difficulty**: Medium  
- **Process**: Direct merge without waiting for reviews (requires at least 1 reviewer on repo, typically bypassed with owner permissions)

### ✅ **Quickdraw** ⚡
- **Requirement**: Close an issue or PR within 5 minutes of opening  
- **Difficulty**: Very Easy
- **Process**: Created an issue and closed it immediately (completed in <2 minutes)

---

## 🚀 Quick Start: How to Reproduce

### Prerequisites
1. Install [GitHub CLI](https://cli.github.com/)
2. Authenticate: `gh auth login`
3. Create a new public repository: `gh repo create my-badges-repo --public`
4. Clone it locally: `gh repo clone YOUR_USERNAME/my-badges-repo`

### Step 1: Setup
```bash
cd my-badges-repo
git config user.email "your-email@github.com"
git config user.name "Your Name"
echo "# My Badges Repository" > README.md
git add README.md
git commit -m "Initial commit"
git push -u origin main
```

### Step 2: Create Pull Shark (2 PRs merged)
```bash
# PR 1
git switch -c feature/badge-1
echo "Content 1" > file1.txt
git add file1.txt
git commit -m "Add feature 1"
git push --set-upstream origin feature/badge-1
gh pr create --title "Feature 1" --body "First PR"
gh pr merge 1 --merge

# PR 2
git switch main
git pull
git switch -c feature/badge-2
echo "Content 2" > file2.txt
git add file2.txt
git commit -m "Add feature 2"
git push --set-upstream origin feature/badge-2
gh pr create --title "Feature 2" --body "Second PR"
gh pr merge 2 --merge
```

### Step 3: Create Quickdraw (close within 5 min)
```bash
gh issue create --title "Quick test" --body "Close me fast"
# Wait a moment...
gh issue close 1
```

### Step 4: Create YOLO (merge without review)
```bash
git switch main
git pull
git switch -c feature/yolo
echo "YOLO" > yolo.txt
git add yolo.txt
git commit -m "YOLO commit"
git push --set-upstream origin feature/yolo
gh pr create --title "YOLO" --body "Direct merge"
gh pr merge 3 --merge
```

### Step 5: Monitor Your Achievements
Visit your GitHub profile: `https://github.com/YOUR_USERNAME`
Look for the "Achievements" section. Badges may take 5-30 minutes to appear.

---

## 📚 Additional Obtainable Badges

You can earn more badges by:

- **Starstruck** ⭐: Get 16 stars on a public repository
- **Galaxy Brain** 🧠: Get 2 accepted answers in [Community Discussions](https://github.com/orgs/community/discussions/)
- **Public Sponsor** 💝: Sponsor an organization or user on GitHub
- **Pair Extraordinaire** 👥: Co-author a merged pull request using GitHub Desktop

---

## 🔗 Reference Repository

This guide is inspired by and references the comprehensive badge documentation created by:

### **Credits to @Thinkright20**
- **Repository**: [Profile-Badges](https://github.com/Thinkright20/Profile-Badges)
- **Purpose**: Complete catalog of all GitHub badges, their requirements, and earning methods
- **Contribution**: Provided the foundational knowledge, badge images, and detailed documentation on how each badge is obtained

Special thanks to @Thinkright20 for creating the most comprehensive guide to GitHub Badges and making it publicly available for the developer community to learn and engage with GitHub's achievement system!

Also credit to @Schweinepriester and @drknzz for their high-quality badge images and additional skin tone variants documented in the Profile-Badges repository.

---

## 📝 Repository Used

**Test Repository**: [meowster404/github-badges-test](https://github.com/meowster404/github-badges-test)

This repository was created specifically to test and demonstrate the badge-earning process.

---

## ⚙️ Technical Details

- **Tools Used**: GitHub CLI (`gh` command)
- **Language**: PowerShell (Windows)
- **Strategy**: Multiple PR merges within a single public repository
- **Timeline**: All badges earned within ~30 minutes of execution

---

## 🎓 Learning Outcomes

By following this guide, you'll learn:
1. How to use GitHub CLI effectively
2. How to work with branches and pull requests programmatically
3. How GitHub tracks and awards achievements
4. The importance of public contributions in the GitHub ecosystem

---

## 📢 Disclaimer

These badges are officially provided by GitHub and do not grant any special permissions or access. They are purely decorative achievements meant to celebrate contributions and milestones.

---

## 🤝 Contributing

Found improvements or new badge-earning strategies? Feel free to open an issue or PR!

---

## 📄 License

This repository is provided as an educational reference. All badge images are copyright GitHub.

---

**Happy Badge Hunting!** 🏆
