# Movie Recap · Burmese Dub Frontend

GitHub Pages frontend for the Movie Recap n8n dubbing pipeline.

## Setup

1. Push this repo to GitHub
2. Settings → Pages → Source: `main` branch, `/ (root)`
3. Access at `https://<username>.github.io/<repo>/`

## Webhook

Calls: `https://n8n.srv1235044.hstgr.cloud/webhook/movie-recap`

Payload:
```json
{ "url": "https://www.xiaohongshu.com/explore/..." }
```

## CORS Note

If browser blocks the webhook call, add to n8n response headers:
`Access-Control-Allow-Origin: https://<username>.github.io`
