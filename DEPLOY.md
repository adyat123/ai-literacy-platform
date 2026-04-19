# Deployment Guide — AI Literacy Platform

## What you have
- `public/index.html` — the full frontend app
- `api/chat.js` — the secure backend (hides your API key)
- `vercel.json` — Vercel configuration
- `package.json` — project metadata

---

## Step 1 — Push to GitHub

1. Go to github.com and click **"New repository"**
2. Name it `ai-literacy-platform`
3. Keep it **Public**, click **Create repository**
4. On the next page, click **"uploading an existing file"**
5. Upload ALL files keeping the folder structure:
   - `public/index.html`
   - `api/chat.js`
   - `vercel.json`
   - `package.json`
6. Click **Commit changes**

---

## Step 2 — Deploy on Vercel

1. Go to vercel.com and click **"Add New Project"**
2. Click **"Import"** next to your `ai-literacy-platform` repo
3. Leave all settings as default
4. Click **Deploy**

Your site will be live at: `https://ai-literacy-platform.vercel.app`

---

## Step 3 — Add your API key (keeps it secret)

1. In Vercel, go to your project → **Settings** → **Environment Variables**
2. Click **Add New**
3. Name: `ANTHROPIC_API_KEY`
4. Value: paste your `sk-ant-...` key
5. Click **Save**
6. Go to **Deployments** → click the three dots on your latest deployment → **Redeploy**

The AI tutor is now live and your key is completely hidden from users.

---

## Step 4 — Share it!

Your live URL looks like: `https://ai-literacy-platform.vercel.app`

Put this on your:
- Resume (under Projects)
- Common App activities section
- GitHub profile README
- LinkedIn

---

## Resume description

**AI Literacy Platform** | React, JavaScript, Claude API (Anthropic), Vercel
- Built and deployed a full-stack interactive AI education web app serving two distinct audiences (children and senior citizens)
- Engineered a secure Node.js serverless backend on Vercel to proxy Anthropic API calls, protecting credentials from client exposure
- Implemented custom prompt engineering to create audience-adaptive AI tutors with age-appropriate language and tone
- Features 8 structured lesson modules, quiz logic with instant feedback, and conversation state management
- Actively used in live workshops reaching 1,000+ learners across in-person and virtual sessions

---

## Estimated monthly cost

| Usage | Estimated cost |
|-------|---------------|
| 1 workshop (30 students, 10 messages each) | ~$0.02 |
| 100 visitors/month, 10 messages each | ~$0.15 |
| 1,000 visitors/month, 10 messages each | ~$1.50 |

Uses Claude Haiku (cheapest model) to keep costs minimal.
