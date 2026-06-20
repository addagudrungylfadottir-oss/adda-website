# How to publish your website

## Step 1 — Add your photo and CV
- Add your photo as `photo.jpg` in this folder
- Add your CV as `cv.pdf` in this folder

## Step 2 — Create a GitHub repository
1. Go to github.com and click **New repository**
2. Name it exactly: `addagylfa.com` (or your GitHub username, e.g. `yourusername.github.io`)
3. Set it to **Public**
4. Do NOT add a README

## Step 3 — Push this folder to GitHub
Open Terminal and run:
```
cd /Users/addagudrungylfadottir/Desktop/addagylfa-website
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

## Step 4 — Enable GitHub Pages
1. Go to your repo on GitHub → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)**
4. Click **Save**

## Step 5 — Point your domain to GitHub
In your domain registrar (wherever you bought addagylfa.com), add these DNS records:

**A records** (point to GitHub's IPs):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME record**:
```
www → YOUR_USERNAME.github.io
```

DNS can take up to 24 hours to propagate. Once done, your site will be live at addagylfa.com.
