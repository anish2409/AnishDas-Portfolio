# Anish Das — Portfolio Deployment Guide

## Folder Structure
```
anish-das-portfolio/
└── index.html          ← entire site (self-contained, no dependencies)
```

---

## Method 1: GitHub Pages (Recommended — Free, Custom Domain Support)

### Step 1 — Create the repository
1. Go to github.com → click **New repository**
2. Name it exactly: `anish2409.github.io`  ← (replace anish2409 with your GitHub username)
3. Set visibility to **Public**
4. Click **Create repository**

### Step 2 — Upload the file
```bash
# Option A: via Git CLI
git clone https://github.com/anish2409/anish2409.github.io
cp index.html anish2409.github.io/
cd anish2409.github.io
git add index.html
git commit -m "Launch portfolio"
git push origin main
```

```
# Option B: via GitHub web UI
1. Open your new repo on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop index.html
4. Click "Commit changes"
```

### Step 3 — Enable GitHub Pages
1. Go to repo **Settings** → **Pages** (left sidebar)
2. Under "Source" → select `main` branch → folder `/root`
3. Click **Save**

### Live URL (ready in ~60 seconds):
```
https://anish2409.github.io
```

---

## Method 2: Netlify (Drag & Drop — Fastest Method)

1. Go to **app.netlify.com** → sign up/log in
2. On the dashboard, find the drag-and-drop zone that says **"Drag and drop your site folder here"**
3. Drag your entire `anish-das-portfolio/` folder into it
4. Live in 10 seconds!

### Live URL format:
```
https://random-name-123.netlify.app
```

### Custom URL (optional):
- Go to **Site Settings** → **Domain Management** → **Add custom domain**
- Set: `anishpf.netlify.app` (free) or connect your own domain

---

## Method 3: Vercel (CLI — Best for Custom Domains)

### Step 1 — Install Vercel CLI
```bash
npm install -g vercel
```

### Step 2 — Deploy
```bash
cd anish-das-portfolio
vercel
```

Follow prompts:
- Set up project? → `Y`
- Which scope? → select your account
- Link to existing project? → `N`
- Project name? → `anish-das-portfolio`
- In which directory? → `.` (current)
- Override settings? → `N`

### Live URL:
```
https://anish-das-portfolio.vercel.app
```

### Redeploy after edits:
```bash
vercel --prod
```

---

## Customization Checklist

| Item | How to update |
|------|---------------|
| Profile photo | Find `photo-slot` div → replace with `<img src="your-photo.jpg"/>` |
| GitHub project links | Find `href="https://github.com/anish2409"` → replace with direct repo URLs |
| Live demo links | Find `href="#"` on `.plb.live` buttons → paste deployed URLs |
| Certificate images | Find `.cprev` divs → replace with `<img src="cert.jpg"/>` |
| Resume download | Add `<a href="resume.pdf" download>` button in hero |

---

## Top 3 Upgrades to Stand Out Among 10,000+ Candidates

### Upgrade 1 — Add a measurable GitHub Activity Heatmap
Embed your real GitHub contribution graph using:
```html
<img src="https://ghchart.rshah.org/6ee7b7/anish2409" alt="Anish's GitHub Activity"/>
```
**Recruiter psychology**: Activity graphs signal consistency and work ethic without self-reporting. A green heatmap is trusted data, not a claim.

### Upgrade 2 — Record a 90-second Loom walkthrough of your best project
Add a thumbnail video preview card under Project 01. Walk through the Power BI dashboard + model architecture.
**Recruiter psychology**: In a stack of 200 resumes, a face + voice + demo creates a memory anchor. 90% of candidates only submit text. You become "the BI chatbot person."

### Upgrade 3 — Add a "Research" section with your conference paper abstract + PDF link
Even one peer-reviewed citation places you in the top 1% of entry-level applicants. Most freshers have zero published work.
**Recruiter psychology**: The moment a hiring manager sees "International Conference + Microsoft CMT", the mental category shifts from "fresher" to "researcher who also writes code." That shift is worth 3 interview rounds.

---

## Recruiter Psychology: What Gets You Shortlisted in Under 10 Seconds

Recruiters spend an average of **6–8 seconds** on a first pass. Here's what makes this portfolio convert:

1. **₹50L+ in the first viewport** — Financial impact numbers stop the scroll. Recruiters are trained to find ROI signals, and ₹50L above the fold is one.

2. **"Oral Presentation · Microsoft CMT" badge** — Conference credentials on a fresh graduate profile are rare enough to be a pattern-break. It triggers "I need to read more."

3. **Three pillars with filled bars** — Visual skill representation is processed faster than text lists. The recruiter instantly maps your profile to a role before reading a word.

4. **No buzzword fluff** — Every sentence answers "so what?" — Federated Learning → privacy + enterprise scale. XGBoost + 7,000 records → production ML, not a tutorial. This signals maturity.

5. **Dark/light toggle** — Small UX detail, large signal. It shows frontend awareness, attention to detail, and that you built something, not downloaded it.
