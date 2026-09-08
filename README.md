# TikTok OAuth Callback Relay

A tiny GitHub Pages site that acts as the HTTPS bridge between TikTok's OAuth redirect and the Post Automator desktop app.

## How it works
1. TikTok redirects to `https://YOUR-USERNAME.github.io/tiktok-callback/?code=xxx&state=yyy`
2. This page immediately redirects to `postautomator://callback?code=xxx&state=yyy`
3. macOS opens Post Automator and completes the login

## Deploy to GitHub Pages (one-time setup)

1. Go to [github.com/new](https://github.com/new)
2. Create a repo named **`tiktok-callback`** (public)
3. Upload the `index.html` from this folder
4. Go to repo **Settings → Pages → Source → Deploy from branch → main → / (root)**
5. Your URL will be: `https://YOUR-USERNAME.github.io/tiktok-callback/`

## TikTok Developer Portal

Enter this as your Redirect URI:
```
https://YOUR-USERNAME.github.io/tiktok-callback/
```
