# zackvanallen.com

Personal portfolio site — Applied AI, health research, and strategy.

## Quick Deploy to GitHub Pages

### 1. Create the repo
- Go to [github.com/new](https://github.com/new)
- Name it exactly: `ZvanAllen.github.io` (must match your GitHub username)
- Set to **Public**
- Click **Create repository**

### 2. Push the files
```bash
cd zvanallen.github.io
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/ZvanAllen/ZvanAllen.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages
- Go to **Settings → Pages** in your repo
- Source: **Deploy from a branch**
- Branch: **main** / **/ (root)**
- Click **Save**

Your site will be live at: `https://zvanallen.github.io` within a few minutes.

## Later: Connect Your Custom Domain

1. In **Settings → Pages → Custom domain**, enter `zackvanallen.com`
2. Add these DNS records at your domain registrar:
   - `A` records pointing to:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - `CNAME` record: `www` → `zvanallen.github.io`
3. Check **Enforce HTTPS** once DNS propagates
4. Uncomment the CNAME file in the repo (or create one with `zackvanallen.com`)
