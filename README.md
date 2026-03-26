# Be The Answer — Landing Page

The marketing website for Be The Answer (betheanswer.cloud).

## Deploy to Vercel (recommended)

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import this repo
3. Click Deploy (no settings to change — it auto-detects static HTML)
4. Add your custom domain in Vercel dashboard → Settings → Domains → `betheanswer.cloud`
5. Update your domain's DNS to point to Vercel (they'll show you exactly what to set)

## After deploying the Score API

Once your score API is live on Railway, update this line in `index.html`:

```javascript
const SCORE_API_URL = 'https://YOUR-API-DOMAIN.com/api/score';
```

Replace with your Railway URL:

```javascript
const SCORE_API_URL = 'https://betheanswer-api-production.up.railway.app/api/score';
```

Commit and push — Vercel auto-redeploys on every push.

## Local preview

Just open `index.html` in your browser. The score widget runs in demo mode until the API is connected.
