# Life OS Prime

Personal dashboard for daily check-ins, routine, goals and the weekly review.
Works offline and installs like an app. Data stays on this one device.

## Files (all at the top level of the repo)

```
life-os/
├── index.html
├── manifest.json
├── sw.js
├── README.md
└── icons/
    ├── icon-192.png
    ├── icon-512.png
    ├── icon-maskable-512.png
    └── apple-touch-icon.png
```

## Step 1: Create the repo

1. On GitHub, click **New repository**.
2. Name: `life-os`. Visibility: **Public** (free GitHub Pages needs this).
3. Click **Create repository**.

## Step 2: Upload the files

1. Unzip `life-os-repo.zip`.
2. In the new repo, click **uploading an existing file** (or **Add file**, then **Upload files**).
3. Open the unzipped folder, select **everything inside it** (the 4 files and the `icons` folder), and drag them in.
   Don't drag the outer folder itself, or the app ends up one level too deep.
4. Click **Commit changes**.

## Step 3: Turn on GitHub Pages

1. In the repo: **Settings**, then **Pages**.
2. Source: **Deploy from a branch**. Branch: `main`, folder: `/ (root)`. Click **Save**.
3. Wait 1–2 minutes. Your app is at:
   https://imyashguptaa.github.io/life-os/

## Step 4: Install on your phone

- **Android (Chrome):** open the link, tap the ⋮ menu, then **Install app** or **Add to Home screen**.
- **iPhone (Safari):** open the link, tap **Share**, then **Add to Home Screen**.

Open it once while online. After that it works offline.

## Removing Daily Momentum (do this BEFORE your first check-in)

Daily Momentum and Life OS live on the same site (`imyashguptaa.github.io`),
so they share the same browser storage area.

- Remove the Daily Momentum icon from your home screen **before** you start logging in Life OS.
- If your phone asks "Also clear data for this site?" while removing it, that is safe only now,
  before your first Life OS check-in. After you start logging, never clear data for this site.
- Leave the `daily-momentum` repo as it is, or archive it. Don't delete Life OS data to clean it up.

## Updating later

1. Replace `index.html` with the new version.
2. In `sw.js`, change `VERSION = "life-os-v1"` to `"life-os-v2"` (then v3, and so on).
3. Commit. Open the app twice while online to get the new version.

## Your data

- Saved only in this browser on this phone.
- Every Sunday: **Review** tab, then **Export backup**. Keep the file in Google Drive.
- **Never upload a backup file to this repo.** It's public.
- Clearing Chrome's data, or clearing data for this site, deletes your check-ins. Export first.
- New phone: **Export backup** on the old one, **Import backup** on the new one.

## AI coach

The coach buttons copy a prompt with your data. Paste it into a Claude chat and send.
