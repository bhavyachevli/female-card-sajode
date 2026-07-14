# Invitation site

This is a static invitation site. It uses `audio.mpeg` (already present) and expects a background video file named `video.mp4` in the same folder.

Local test

1. Place your video file next to `index.html` and name it `video.mp4` (or edit `index.html` to match your filename).
2. Run a simple static server (Python):

```powershell
python -m http.server 8000
```

Open http://localhost:8000 in your browser.

Deploy to Vercel

Option A — Quick deploy with Vercel CLI:

```powershell
npm i -g vercel
cd path\to\invitation_websites
vercel
```

Follow the prompts to deploy. When asked for the project root choose the current folder.

Option B — Git + Vercel dashboard:
1. Push this folder to a GitHub (or GitLab/Bitbucket) repository.
2. In Vercel dashboard, "New Project" → Import your repo → Deploy (static site, build step none).

Notes
- If you have multiple video files, name them in `index.html` or add multiple `<source>` elements.
- If you want me to perform the Vercel deploy, grant an access token or authorize the Vercel CLI on your machine and tell me to proceed.
