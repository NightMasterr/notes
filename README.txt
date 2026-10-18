NOTES APP -> ANDROID APK  (free, no coding, nothing to install on your PC)
=========================================================================

1. Make a free account at https://github.com (skip if you have one).
2. Click "+" (top right) -> "New repository". Name it "notes", choose Private, click "Create repository".
3. On the new page click "uploading an existing file".
4. Open this folder on your PC, select EVERYTHING inside it
   (www, assets, .github, package.json, capacitor.config.json, .gitignore)
   and drag it all into the browser page. Wait until the upload finishes.
   Then click "Commit changes".
5. Click the "Actions" tab. A run called "Build APK" starts by itself
   (if not: Actions -> Build APK -> Run workflow).
6. Wait about 5-10 minutes until it shows a green check mark.
7. Click the finished run, scroll down to "Artifacts", click "Notes-APK". A zip downloads.
8. Unzip it: inside is Notes.apk  <- this is your Android app.
9. Send Notes.apk to your phone (Telegram "Saved Messages", Google Drive, or a USB cable).
10. On the phone tap the file -> allow installing from that app -> Install.
    If Play Protect warns: "More details" -> "Install anyway".

If step 5 shows nothing: check that ".github/workflows/build-apk.yml" exists in your repository.
If it is missing: Add file -> Create new file, type that exact path as the name,
paste the contents of build-apk.yml from this folder, and commit.

If the run turns red: open it, copy the last red error lines and send them to Claude.
