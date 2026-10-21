# Publish Instructions — ECS Penetration Testing Repository

[← Back to main page](README.md)

**Repository:** https://github.com/elite-cybersecurity-specialist/penetration-testing  
**Repository owner:** ELITE CYBERSECURITY SPECIALIST  
**Default branch:** `main`

This package is prepared for the public GitHub repository that promotes **ECS Penetration Testing & Security Assessments**.

---

## 1) Recommended package verification

If you downloaded the ZIP and checksum files, verify them before extracting:

```bash
cd ~/Downloads
sha256sum -c ECS_Penetration_Testing_Repository_20261022_FINAL.zip.sha256
sha256sum -c ECS_Penetration_Testing_README_20261022.md.sha256
```

After extraction, you can also verify the repository content manifest:

```bash
cd ~/Downloads/GitHub/penetration-testing
sha256sum -c SHA256SUMS.txt
```

---

## 2) Configure Git identity

Use the required Git identity before committing:

```bash
git config user.name "Yuhisern Navaratnam"
git config user.email "Yuhisern@protonmail.com"
```

To make it global for future repositories:

```bash
git config --global user.name "Yuhisern Navaratnam"
git config --global user.email "Yuhisern@protonmail.com"
```

---

## 3) Option A — Clone the empty GitHub repository first (recommended)

This is the safest option because it avoids overwriting unrelated local files.

```bash
mkdir -p ~/Downloads/GitHub
cd ~/Downloads/GitHub
git clone https://github.com/elite-cybersecurity-specialist/penetration-testing.git
cd penetration-testing
```

Extract the package **into the repository root**:

```bash
unzip -o ~/Downloads/ECS_Penetration_Testing_Repository_20261022_FINAL.zip -d .
```

Review what will be committed:

```bash
git status
find . -maxdepth 2 -type f | sort
```

Then commit and publish:

```bash
git add .
git commit -m "Publish ECS penetration testing services portfolio"
git push -u origin main
```

---

## 4) Option B — Use an existing local repository directory

Use this only if you already created the local directory and you are sure it is meant for this repository.

```bash
cd ~/Downloads/GitHub/penetration-testing
pwd
ls -la
git status || true
git remote -v || true
```

If the directory is **not** a Git repository yet:

```bash
git init
git branch -M main
git remote add origin https://github.com/elite-cybersecurity-specialist/penetration-testing.git
```

If `origin` already exists, confirm that it points to the correct repository:

```bash
git remote set-url origin https://github.com/elite-cybersecurity-specialist/penetration-testing.git
git remote -v
```

Extract the package into the current repository root:

```bash
unzip -o ~/Downloads/ECS_Penetration_Testing_Repository_20261022_FINAL.zip -d .
```

Then publish:

```bash
git add .
git commit -m "Publish ECS penetration testing services portfolio"
git push -u origin main
```

---

## 5) Expected repository structure

```text
README.md
SECURITY.md
NOTICE.md
PROJECT_PLAN.md
PUBLISH_INSTRUCTIONS.md
SHA256SUMS.txt
.gitignore
.gitattributes
assets/
docs/
templates/
```

---

## 6) What to verify after the push

Visit the repository page and confirm the following:

1. The main penetration-testing banner appears at the top of the README.
2. The official ECS digital name card appears prominently near the top.
3. The supplementary graphics render correctly.
4. All internal Markdown links work.
5. The company profile PDF link opens correctly.
6. Contact details, registration number and company branding are accurate.
7. No confidential content or client-specific material was pushed.

---

## 7) If Git reports a conflict or problem

Check the local repository state:

```bash
git status
git branch
git remote -v
git log --oneline -5
```

If the remote already contains commits you do not have locally:

```bash
git pull --rebase origin main
```

Then resolve any conflicts carefully and retry the push.

**Do not force-push** unless you intentionally want to rewrite the repository and have confirmed that doing so is safe.

---

## 8) Important publishing note

Do not claim that the repository has been published until `git push -u origin main` completes successfully and the repository page displays the new files.
