# MHOBG Studio — Website Deployment Guide

## Overview
Single-page HTML/CSS/JS website. Zero build step. Drop the files on any static host.

## Files
- `index.html` — complete site (embedded CSS + JS)

## Deployment Options

### Option 1: GitHub Pages
```bash
# Create a new repo or use existing mhobgstudio/mhobgstudio.github.io
git init
git add index.html
git commit -m "Initial site"
git remote add origin https://github.com/mhobgstudio/mhobgstudio.github.io.git
git push -u origin main
# Enable GitHub Pages in repo Settings > Pages > source: main
```

### Option 2: Netlify (drag & drop)
1. Go to https://app.netlify.com
2. Drag the project folder onto the deploy area
3. Site is live immediately with a `*.netlify.app` URL
4. Custom domain: Settings > Domain Management

### Option 3: Vercel
```bash
npx vercel --prod
```

### Option 4: Firebase Hosting
```bash
npm install -g firebase-tools
firebase init hosting
firebase deploy
```

## Custom Domain
Point an A record or CNAME to your host. Add the domain in your hosting provider's settings.

## Updating
Simply edit `index.html` and re-deploy. All content (styles, scripts) is in one file for easy maintenance.

## Contact
For questions: mhobgstudio@gmail.com
