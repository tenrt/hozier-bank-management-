# Hozier Bank Management — Landing Page

A single marketing landing page for a fictional bank concept ("Hozier Bank Management"). Plain HTML/CSS/JS — no build step, no dependencies, no backend. Open `index.html` in any browser and it works.

**This is a design concept only.** It's a fictional institution — no real accounts, logins, or transactions are involved.

## Folder contents

```
hozier-bank-site/
├── index.html        ← the page itself
├── css/
│   └── styles.css     ← all styling (navy/charcoal + gold palette)
├── js/
│   └── script.js       ← small scroll-reveal animation
└── README.md          ← this file
```

## Preview it locally

Just double-click `index.html`, or from a terminal in this folder:

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

No installs needed — it's static HTML.

---

## Putting this on GitHub (step by step)

If you've never used GitHub before, here's the full path from "folder on my computer" to "live link I can share."

### 1. Create a free GitHub account
Go to [github.com](https://github.com) and sign up if you haven't already.

### 2. Install Git on your computer
- **Windows/Mac:** download from [git-scm.com](https://git-scm.com/downloads)
- **Mac (alternative):** `brew install git` if you use Homebrew
- **Linux:** `sudo apt install git` (Debian/Ubuntu) or your distro's equivalent

Check it worked:
```bash
git --version
```

### 3. Create a new repository on GitHub
1. Click the **+** icon (top right of github.com) → **New repository**
2. Name it something like `hozier-bank-site`
3. Leave it **Public** (required for free GitHub Pages hosting)
4. **Don't** check "Add a README" — you already have one
5. Click **Create repository**

GitHub will show you a page with setup commands — keep that tab open, you'll need the repository URL from it (looks like `https://github.com/YOUR-USERNAME/hozier-bank-site.git`).

### 4. Push this folder to GitHub

Open a terminal, navigate into this folder, then run:

```bash
cd path/to/hozier-bank-site

git init
git add .
git commit -m "Initial commit: Hozier Bank landing page"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/hozier-bank-site.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your actual GitHub username, and the repo name if you called it something else. Git may prompt you to log in — for the password, GitHub now requires a **Personal Access Token** instead of your account password:
- Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic) → Generate new token
- Give it `repo` scope, generate it, and paste it in when Git asks for a password

### 5. Turn on GitHub Pages (free hosting)
1. In your repository on GitHub, click **Settings**
2. In the left sidebar, click **Pages**
3. Under "Build and deployment" → **Source**, choose **Deploy from a branch**
4. Branch: `main`, folder: `/ (root)` → **Save**
5. Wait about a minute, then refresh — GitHub will show a link like:
   `https://YOUR-USERNAME.github.io/hozier-bank-site/`

That link is now live and shareable.

### 6. Making changes later
Whenever you edit the files:
```bash
git add .
git commit -m "Describe what you changed"
git push
```
GitHub Pages automatically redeploys within a minute or two.

---

## Customizing

- **Colors:** all in `css/styles.css` under the `:root { ... }` block at the top — change the hex values there and everything updates.
- **Text/copy:** edit directly in `index.html`.
- **Fonts:** loaded from Google Fonts via the `<link>` tags in `index.html`'s `<head>`.
