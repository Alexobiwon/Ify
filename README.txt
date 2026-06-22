BLOOM — How to put it on her iPhone
====================================

This is a "home-screen web app." There's no App Store, no review, no
developer account. You host these files once, send her the link, and she
adds it to her home screen. It then opens full-screen with its own icon,
just like a normal app, and works offline after the first open.

WHAT'S IN THIS FOLDER
- index.html            the app
- manifest.webmanifest  makes it install as a standalone app
- sw.js                 lets it work offline
- icon-180/192/512.png  the app icon
Keep all of these together in the same folder.


STEP 1 — PUT IT ONLINE (pick ONE; all are free)

Option A — Netlify Drop (easiest, ~1 minute, no coding)
  1. Go to  https://app.netlify.com/drop
  2. Drag this whole folder onto the page.
  3. It gives you a link like  https://something.netlify.app
  4. (Optional) make a free account so the link stays permanent.

Option B — GitHub Pages (good if you already use GitHub)
  1. Create a new repo and upload these files to it.
  2. Settings > Pages > deploy from the main branch (root).
  3. Your link will be  https://<you>.github.io/<repo>/

Option C — Cloudflare Pages or Vercel
  Upload the folder; both give you a free https link the same way.


STEP 2 — SEND HER THE LINK
Text or WhatsApp her the link from Step 1.


STEP 3 — SHE ADDS IT TO HER HOME SCREEN (on the iPhone)
  1. Open the link in **Safari** (this part must be Safari, not Chrome).
  2. Tap the Share button (the square with an arrow).
  3. Scroll down and tap **"Add to Home Screen."**
  4. Tap **Add.**
  The Bloom icon now sits on her home screen and opens full-screen.

That's it. The workout videos need internet, but the plan, meals and
checklist work offline once it's been opened once.


WANT TO PERSONALISE IT?
Open index.html in any text editor:
- The welcome line is near the top, inside the <section id="view-today"> block.
- Workout videos and meals are in the <script> section (the `workouts`
  and `meals` lists) if you ever want to swap something.

A note: this is general wellness guidance, not medical advice. With high
blood pressure, it's worth her running the plan past her doctor first.
