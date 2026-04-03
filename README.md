# AI Sales Lead Evaluation Agent — Vercel Edition

## 📁 Project Structure
```
lead-eval-vercel/
├── api/
│   └── evaluate.js     ← Serverless function (proxies Claude API)
├── public/
│   └── index.html      ← Frontend UI
├── vercel.json         ← Routing config
├── package.json
└── README.md
```

---

## 🚀 Deploy to Vercel (Step-by-Step)

### Step 1 — Create a GitHub repo
1. Go to https://github.com and sign in
2. Click "New repository"
3. Name it: lead-eval-agent
4. Set it to Public or Private — both work
5. Click "Create repository"

### Step 2 — Upload the files
In your new GitHub repo:
1. Click "uploading an existing file"
2. Upload these files maintaining the folder structure:
   - api/evaluate.js
   - public/index.html
   - vercel.json
   - package.json
3. Click "Commit changes"

### Step 3 — Sign up on Vercel
1. Go to https://vercel.com
2. Click "Sign Up" → choose "Continue with GitHub"
3. Authorize Vercel to access your GitHub

### Step 4 — Import your project
1. On the Vercel dashboard click "Add New..." → "Project"
2. Find your "lead-eval-agent" repo and click "Import"
3. Leave all settings as default — Vercel auto-detects everything
4. DO NOT click Deploy yet

### Step 5 — Add your API key
1. On the same import screen, expand "Environment Variables"
2. Add:
   - Name:  ANTHROPIC_API_KEY
   - Value: your sk-ant-... key from https://console.anthropic.com
3. Click "Add"

### Step 6 — Deploy
1. Click "Deploy"
2. Wait ~30 seconds
3. You'll get a live URL like: https://lead-eval-agent.vercel.app

---

## ✅ Vercel Advantages over Render
- Never sleeps (no cold start delays)
- Faster global CDN
- Free tier is more generous
- Auto-deploys on every GitHub push

## 🔑 Updating your API key later
1. Go to your project on vercel.com
2. Settings → Environment Variables
3. Edit ANTHROPIC_API_KEY → Save
4. Redeploy (Deployments → Redeploy)
