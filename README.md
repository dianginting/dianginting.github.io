# Dian Andrian Ginting — Portfolio

Personal portfolio site built as a single-page application with no frameworks or build tools.

## Setup GitHub Pages

### Step 1: Create the Repository

1. Go to [github.com/new](https://github.com/new)
2. Name the repository `dianginting.github.io` (for a user site) or `portfolio` (for a project site)
3. Set visibility to **Public**
4. Do **not** initialize with a README (you already have one)

### Step 2: Push the Code

```bash
cd /Users/dianginting/IdeaProjects/portfolio
git init
git add index.html README.md CNAME
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/dianginting/dianginting.github.io.git
git push -u origin main
```

If using a project-level repo (`portfolio`) instead:

```bash
git remote add origin https://github.com/dianginting/portfolio.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Navigate to **Settings** > **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Select the **main** branch and **/ (root)** folder
5. Click **Save**

### Step 4: Access Your Site

- **User site**: `https://dianginting.github.io`
- **Project site**: `https://dianginting.github.io/portfolio`

The site typically deploys within 1-2 minutes.

### Step 5: Custom Domain (Optional)

1. Purchase a domain from any registrar
2. Add a CNAME DNS record pointing to `dianginting.github.io`
3. Edit the `CNAME` file in this repo with your domain (e.g., `dian.dev`)
4. In **Settings** > **Pages**, enter your custom domain and enable **Enforce HTTPS**

## Local Preview

Open `index.html` directly in a browser, or serve it locally:

```bash
# Python 3
python3 -m http.server 8000

# Then open http://localhost:8000
```

## Structure

```
portfolio/
  index.html   - Complete site (HTML + CSS + JS, no dependencies)
  CNAME         - Custom domain config (empty by default)
  README.md     - This file
```
