# Developing Locally (after creating the remote repository)

Follow these steps to get the code on your machine, make changes safely, and contribute via pull requests.

---

## 1) Prerequisites
- **Git** installed (and available on your PATH).
- **GitHub account** with access to the repository.
- **Authentication** set up (HTTPS with Personal Access Token, or SSH keys).
- **Language runtime/tools** for this project (e.g., Python/Node/Java) and any package manager (pip/npm/maven/etc.).

> [!IMPORTANT]
> Do **not** place your working copy inside OneDrive/Dropbox/iCloud sync folders. Keep repos in a local folder like `C:\GitRepos\` or `~/projects/` to avoid corruption and performance issues.

---

## 2) Clone the repository

**Option A — HTTPS (works anywhere)**
```bash
git clone https://github.com/<OWNER>/<REPO>.git
cd <REPO>
```

**Option B — SSH (requires SSH keys; may not work on some VPNs)**
```bash
git clone git@github.com:<OWNER>/<REPO>.git
cd <REPO>
```

> Verify the remote:
> ```bash
> git remote -v
> ```
> You should see `origin` pointing to your GitHub repo.

---

## 3) One-time Git configuration (recommended)
```bash
git config user.name "Your Name"
git config user.email "you@your.org"
git config pull.rebase false   # or true if your team prefers rebase
```

Optional quality-of-life:
```bash
git config core.autocrlf input      # macOS/Linux
# git config core.autocrlf true     # Windows (if needed)
git config init.defaultBranch main
```

---

## 4) Create a feature branch
Never commit directly to `main` unless your project explicitly allows it.

```bash
git checkout -b feature/short-description
```

---

## 5) Set up the project locally
Language/tooling will vary—adapt the steps below to your stack.

**Python (example)**
```bash
python -m venv .venv
# macOS/Linux
source .venv/bin/activate
# Windows
# .venv\Scripts\activate

pip install -U pip
pip install -r requirements.txt   # or 'pip install -e .'
```

**Node.js (example)**
```bash
npm ci           # or 'npm install'
npm run build    # or 'npm start' / 'npm test'
```

**Java/Maven (example)**
```bash
mvn -q -DskipTests package
```

---

## 6) Run tests and lints locally (if available)
```bash
# examples
pytest
npm test
mvn test
pre-commit run --all-files
```

---

## 7) Make changes and commit
```bash
git status
git add <files>
git commit -m "Short, imperative message: what changed and why"
```

> Keep commits focused. Include references to issues (e.g., `Fixes #123`) when appropriate.

---

## 8) Push your branch and open a Pull Request
```bash
git push -u origin feature/short-description
```

Then open GitHub → your repo → **Compare & pull request**.  
Fill in a clear title/description (screenshots, context, test notes).

**GitHub CLI alternative**
```bash
gh auth login
gh pr create --fill   # uses the commit messages for PR title/body
# or
gh pr create -t "Title" -b "What/Why/How"
```

---

## 9) Address review feedback
- Push more commits to the same branch; the PR updates automatically:
  ```bash
  git add <more files>
  git commit -m "Address review: ..."
  git push
  ```
- When approved and checks are green, **merge** via GitHub UI (or follow your project policy).

---

## 10) Update your local `main` and clean up
After your PR is merged:
```bash
git checkout main
git pull origin main
git branch -d feature/short-description     # delete local branch
git push origin --delete feature/short-description   # delete remote branch (optional)
```

---

## Common extras

**.gitignore**
- Ensure a proper `.gitignore` for your language/tooling to avoid committing build artifacts, secrets, or large files.

**Git LFS (large files)**
- If the project uses big binary files, configure **Git LFS**:
  ```bash
  git lfs install
  git lfs track "*.bin"
  ```

**Branch naming**
- Follow your team’s convention (e.g., `feature/...`, `fix/...`, `docs/...`, `chore/...`).

**Commit style**
- Prefer concise, imperative messages (e.g., `Add X`, `Fix Y`, `Refactor Z`).

---

## Troubleshooting

**Auth failures (HTTPS)**
- Regenerate a **Personal Access Token** (with `repo` scope) and use it as your password.

**SSH doesn’t connect**
- Check `ssh -T git@github.com` and your `~/.ssh/config`.
- Some corporate VPNs block SSH—use HTTPS instead.

**Line endings**
- If you see noisy diffs on Windows, set `core.autocrlf true` and re-checkout the repo.

**OneDrive conflicts**
- Move your repo outside any synced folder; restart your shell and retry.

---
