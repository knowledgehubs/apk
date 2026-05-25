# HTML to Android APK

Automatically converts `index.html` into a downloadable Android APK using GitHub Actions. No Android Studio or local setup needed.

## How it works

1. Push any change to `index.html`
2. GitHub Actions builds the APK automatically
3. Download `app-debug.apk` from the **Actions** tab → run → **Artifacts**

## Setup (one-time)

1. Upload all files from this zip to a new GitHub repository
2. **Replace `index.html`** with your own HTML file
3. Make sure GitHub Actions is enabled on your repo (it is by default)
4. Push — the build starts automatically

## Files in this repo

```
.github/
  workflows/
    android_build.yml   ← the build pipeline (do not edit)
index.html              ← YOUR app goes here
.gitignore
README.md
```

## Downloading the APK

1. Go to your repo on GitHub
2. Click the **Actions** tab
3. Click the latest workflow run
4. Scroll to **Artifacts** at the bottom
5. Click **android-debug-apk** to download

The APK is a debug build — you can install it directly on any Android device with "Install from unknown sources" enabled.
