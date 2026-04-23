# ◆ Story Bank

> Turn your resume into polished STAR interview stories. Built for senior data engineers targeting top companies.

## What it does

1. **Upload resume** → extracts all experiences automatically
2. **Gap detection** → identifies missing metrics, context, ownership, impact
3. **Guided questions** → fills the gaps before generating stories
4. **Story Bank** → polished STAR stories, tagged and organized
5. **JD Matcher** → paste any job description → get your top matching stories with exact framing

## Deploy in 5 minutes

### 1. Clone / download this project

### 2. Push to GitHub
```bash
git init
git add .
git commit -m "init"
git remote add origin https://github.com/YOUR_USERNAME/story-bank.git
git push -u origin main
```

### 3. Deploy on Vercel (free)
- Go to vercel.com → Sign up with GitHub
- Click "Add New Project" → import your repo
- Leave all settings as default → click Deploy
- You get a live URL like `story-bank.vercel.app`

### 4. Share the link
That's it. Users open the link, enter their free Anthropic API key, and they're good to go.

## How users get their API key

1. Go to console.anthropic.com
2. Sign up for a free account (free credits included)
3. Go to API Keys → Create Key
4. Paste it into the app — stored locally, never shared

## Local development

```bash
npm install
npm start
```

## Tech stack

- React (frontend)
- Vercel serverless function (proxy — keeps user's key secure, handles CORS)
- Anthropic Claude API (AI)
- localStorage (story persistence — no database needed)

## Project structure

```
story-bank/
├── api/
│   └── claude.js        # Vercel serverless proxy
├── public/
│   └── index.html
├── src/
│   ├── App.js           # Main app
│   └── index.js
├── package.json
└── vercel.json
```
