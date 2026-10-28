# moreads 🍒
a dark cherry site for book lovers (static site + firebase for accounts and shared data).

## 1. put the site on github
1. create a new repository on github (for example `moreads`), public.
2. upload all files from this folder: `index.html`, `firebase-config.js`, `firestore.rules`, `README.md`.
3. repository → settings → pages → source: "deploy from a branch" → branch `main`, folder `/ (root)` → save.
4. in a minute the site opens at `https://YOUR-NAME.github.io/moreads/`.

## 2. connect firebase (free) – needed for registration, discussions, friends, chat
1. go to https://console.firebase.google.com → add project.
2. build → authentication → get started → sign-in method → enable **google**.
   authentication → settings → authorized domains → add `YOUR-NAME.github.io`.
3. build → firestore database → create database (production mode).
4. firestore → rules → paste the contents of `firestore.rules` → publish.
5. project settings (gear) → your apps → web `</>` → register app → copy the `firebaseConfig` values into `firebase-config.js` and commit.

done: people sign in with google, everything saves automatically.
without firebase the site still works locally (personal lists and assistant are saved in the browser only).
