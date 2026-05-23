RewardX → Netlify deployment
=============================

This folder contains the public-facing site for vertexapp0.netlify.app.
It serves two purposes:
  1. Hosts ads.txt for GameMonetize verification (already done).
  2. Hosts play.html — a wrapper that loads GameMonetize games so the
     referrer domain is vertexapp0.netlify.app (approved publisher).

How to deploy
-------------
Option A — Netlify Drop (fastest):
  1. Visit https://app.netlify.com/drop
  2. Drag this entire `netlify/` folder onto the page
  3. Your site updates immediately

Option B — Git-connected (if site is linked to a repo):
  1. Commit play.html (and your existing index.html + ads.txt)
  2. git push → Netlify auto-deploys

After deploy, verify the wrapper works:
  https://vertexapp0.netlify.app/play.html?id=aos9uibpduazpzx0d4vuodsxolxrb9w4
The Mini Shape Shifting game should load full-screen.
