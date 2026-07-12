SIZIGIA LINEUP — PWA PACKAGE
============================

What's in here
--------------
index.html               the app itself
manifest.json            app name, colors, icons (makes it "installable")
sw.js                    service worker — caches everything for offline use
icon-192.png / icon-512.png / icon-512-maskable.png / icon-180.png   app icons


Fastest way to share this with other people (no account needed)
-----------------------------------------------------------------
1. Go to https://app.netlify.com/drop on a computer.
2. Drag this whole folder onto the page.
3. Netlify gives you a public URL in a few seconds, e.g.
   https://random-name-123.netlify.app
4. Send that link to anyone — WhatsApp, whatever. They open it in Safari,
   tap the Share icon, then "Add to Home Screen". Done: real app icon,
   opens full-screen, works offline.

That's it — no sign-up is required for a one-off drop. If you want the
link to stay stable so you can push updates later, make a free Netlify
account and "claim" the site after dropping it once.


Alternative: GitHub Pages (free, keeps a fixed URL, easy to update)
--------------------------------------------------------------------
1. Create a free GitHub account if you don't have one.
2. Create a new repository (e.g. "sizigia-lineup") and upload all the
   files in this folder to it.
3. In the repo: Settings → Pages → set "Deploy from branch" → main → save.
4. GitHub gives you a URL like https://yourname.github.io/sizigia-lineup/
5. Share that link. To push an update later, just re-upload the changed
   files to the same repo — everyone's app updates next time they open it.


If you make changes later
--------------------------
Open sw.js and bump the CACHE_NAME (e.g. 'sizigia-cache-v1' -> 'v2') so
returning visitors pick up the new version instead of an old cached copy.


Just want to keep sharing the single file instead?
----------------------------------------------------
sizigia-lineup.html (outside this folder) still works exactly as before —
send it directly, no hosting needed. The trade-off is that everyone has to
manually add it to their home screen from Files/Safari each time, and it
won't auto-update. The web link above is the easier option for a group.
