# 🚀 Portfolio Website — Vercel Deployment Guide

## What's Inside

```
portfolio/
├── index.html      ← Your entire portfolio (edit this)
├── resume.pdf      ← Add your resume here (rename to resume.pdf)
└── vercel.json     ← Vercel config (don't edit)
```

---

## ✅ Step 1 — Customize Your Portfolio

Open `index.html` and find & replace these placeholders:

| Placeholder | Replace With |
|---|---|
| `Your Name` | Your actual name |
| `YN` | Your initials |
| `[Your University]` | Your university name |
| `[Your Research Area]` | Your field e.g. "Machine Learning" |
| `your.email@university.edu` | Your email |
| `[Company Name]` | Real company/lab names |
| `resume.pdf` | Link to your actual resume |
| Social links `href="#"` | Your real profile URLs |

Also update the **stats** in the hero card (projects, papers, years).

---

## 🌐 Step 2 — Deploy to Vercel (3 Methods)

### Method A — Drag & Drop (Easiest, no terminal)

1. Go to [vercel.com](https://vercel.com) and sign up (free)
2. Click **"Add New Project"**
3. Drag your entire `portfolio/` folder onto the upload area
4. Click **Deploy**
5. ✅ Live in ~30 seconds!

---

### Method B — GitHub (Recommended for updates)

1. Create a free account at [github.com](https://github.com)
2. Create a **new repository** called `portfolio`
3. Upload all files from this folder to the repo
4. Go to [vercel.com](https://vercel.com) → **"Add New Project"**
5. Import your GitHub repo
6. Click **Deploy**
7. ✅ Live! Every future push to GitHub auto-deploys.

---

### Method C — Vercel CLI (Terminal)

```bash
# Install Vercel CLI
npm install -g vercel

# Go into your portfolio folder
cd portfolio

# Login and deploy
vercel login
vercel

# Follow the prompts — done!
```

---

## 🖼️ Step 3 — Add Your Resume PDF

1. Export your CV as a PDF
2. Name it exactly `resume.pdf`
3. Place it in the same folder as `index.html`
4. Re-deploy (or push to GitHub if using Method B)

---

## 🎨 Step 4 — Personalize Further

### Change colors
Find `:root` in `index.html` and edit:
```css
--accent: #c8f557;   /* lime green → change to any color */
--accent2: #7efff5;  /* cyan accent */
--bg: #0a0a0f;       /* dark background */
```

### Add real project links
Find each `href="#"` inside project cards and replace with:
- GitHub repo URL
- Live demo URL
- Research paper URL

### Update blog posts
Replace the placeholder blog titles/excerpts with your real writing, and update `href="#"` to your actual blog post URLs (Medium, Dev.to, Hashnode, etc.)

### Add a profile photo
Replace the `YN` initials avatar with:
```html
<img src="photo.jpg" style="width:90px;height:90px;border-radius:50%;object-fit:cover;border:2px solid var(--accent)" alt="Your Name" />
```
Then upload `photo.jpg` to the folder.

---

## 🔗 Custom Domain (Optional)

1. Buy a domain (e.g. yourname.dev) from Namecheap or GoDaddy
2. In Vercel dashboard → your project → **Settings → Domains**
3. Add your domain and follow DNS instructions
4. ✅ yourname.dev is live!

---

## 🔄 Making Updates Later

- **With GitHub**: Edit files → commit → push → auto-deploys in ~20 seconds
- **Without GitHub**: Re-drag the folder to Vercel dashboard

---

## 💡 Tips

- Keep `vercel.json` as-is — don't delete it
- Images go in the same folder, reference as `src="filename.jpg"`
- Test locally by opening `index.html` in your browser first
- Vercel free plan is more than enough for a portfolio

---

*Your portfolio is now live and professional. Good luck! 🎉*
