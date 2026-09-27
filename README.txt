BRACKET & BRANCH — BUILD THE APK IN THE CLOUD (no local installs needed)
=========================================================================

This folder has everything needed for GitHub to build a real, installable,
fully offline APK for you automatically. You just need a free GitHub
account — no Android Studio, no Node.js, nothing installed on your own
computer.

STEPS

1. Go to https://github.com and create a free account if you don't have one.

2. Create a new repository:
   - Click the "+" in the top right -> "New repository"
   - Name it anything, e.g. "bracket-and-branch"
   - Keep it Public or Private, either works
   - Do NOT initialize with a README (leave it empty)
   - Click "Create repository"

3. Upload this folder's contents to that repository:
   - On the new repo's page, click "uploading an existing file"
   - Drag in every file and folder from this zip (unzip it first) —
     including the hidden ".github" folder and the ".gitignore" file.
     If your file browser hides files starting with a dot, use your
     computer's "show hidden files" setting, or use GitHub Desktop
     instead of the web uploader (it shows everything).
   - Commit the files (the green "Commit changes" button)

4. GitHub builds it automatically:
   - Click the "Actions" tab at the top of your repo
   - You'll see a workflow run start within a few seconds (or click
     "Run workflow" if it doesn't start automatically)
   - Wait for it to finish — usually 3 to 6 minutes. A green checkmark
     means success; red X means something failed (click into it, the
     logs will show what).

5. Download your APK:
   - Click into the finished workflow run
   - Scroll to "Artifacts" at the bottom
   - Download "bracket-and-branch-debug-apk" — it's a zip containing
     app-debug.apk
   - Unzip it, and that .apk is what you install on your phone.

INSTALLING ON YOUR PHONE

- Transfer app-debug.apk to your phone (email, cloud drive, USB, etc.)
- Tap the file to install
- Android will warn about "unknown sources" for a debug build not from
  the Play Store — allow it in the prompt, that's expected and normal
  for a personal build like this.

This APK bundles index.html directly inside itself as a local asset —
no Netlify, no live URL, no internet connection needed to run it.
