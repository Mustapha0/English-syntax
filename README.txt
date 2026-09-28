ENGLISH SYNTAX
==============

An offline Android app for learning English syntax by building sentence
trees yourself.

ABOUT THE APP
-------------
English Syntax teaches how English sentences are put together, from the
basics (what is a phrase?) to the ideas used in modern linguistics. It has
29 short lessons. Each lesson gives you:

  - A brief explanation of the concept
  - A worked example with a tree diagram
  - A hands-on exercise: tap words to select a span, choose a label
    (NP, VP, PP, S, CP, AdjP, AdvP), and build the tree yourself
  - Instant feedback: the app marks each part correct, missing, or
    mislabeled, and explains why, so you learn from every mistake

Topics covered include constituents, noun/verb/prepositional phrases,
clauses and complementizers, PP attachment and ambiguity, complements vs.
adjuncts, constituency tests, context-free grammars, phrase structure
rules, X-bar theory, argument structure and theta roles, Case, binding,
head movement, wh-movement, passives, control and raising, island
constraints, principles and parameters, the Minimalist Program, and the
syntax-semantics and syntax-phonology interfaces.

Lessons you complete with a perfect tree get a checkmark, and your
progress is saved on your device. Everything works fully offline: no
account, no internet connection needed to learn.

The app also has a "Buy me a coffee" button (paypal.me/afkharm) and a
small banner ad (Google AdMob). Ads need internet to load; the lessons
do not.


BUILD THE APK IN THE CLOUD (no local installs needed)
=====================================================
This folder has everything GitHub needs to build a real, installable APK
for you automatically. You only need a free GitHub account.

1. Create a repository at https://github.com (leave it empty).
2. Upload everything from this folder, including the hidden ".github"
   folder and the ".gitignore" file. (If your file browser hides dot
   files, turn on "show hidden files", or use GitHub Desktop.)
3. Open the repo's "Actions" tab. The build starts automatically
   (or click "Run workflow"). It takes about 3-6 minutes.
4. When it shows a green check, open the run, scroll to "Artifacts", and
   download "english-syntax-debug-apk". Unzip it to get app-debug.apk.
5. Send app-debug.apk to your phone and tap it to install (allow
   "unknown sources" when Android asks - normal for a personal build).

If installing over an older version fails, uninstall the old one first
(each cloud build is signed with a fresh debug key).


ADS SETTINGS
============
- Banner ad unit ID and test-mode switch: www/index.html
  (ADMOB_BANNER_ID and ADMOB_TESTING). Set ADMOB_TESTING to true to see
  safe Google test ads while trying things out.
- AdMob App ID: .github/workflows/build-apk.yml (ADMOB_APP_ID).
- Never tap your own live ads; Google can ban the AdMob account for it.
- New ad units can take up to an hour before ads start showing.


CHANGING THINGS LATER
=====================
- App icon: replace the images in the assets/ folder (icon-only.png,
  icon-foreground.png, icon-background.png; 1024x1024). The build
  generates all Android icon sizes from them.
- App name: "appName" in capacitor.config.json (and the title in
  www/index.html).
- Donation link: search for paypal.me in www/index.html.
- After any change, commit to GitHub and the Actions tab rebuilds the APK.
