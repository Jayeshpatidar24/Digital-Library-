# Jayesh Library — Android project

This is the source project for Jayesh Library. It is not an APK until the cloud build finishes.

## Build an APK using only your Android phone (GitHub account required)

1. Download this ZIP and extract it using your phone's file manager or an archive app.
2. Open GitHub in Chrome and create a **new repository**. Name it `JayeshLibrary`; for the easiest setup, choose **Public** and do not add a README/license/gitignore.
3. In the new repository, use **Add file → Upload files** and upload the *contents* of the `JayeshLibrary` folder, not the outer folder itself. Make sure the `.github/workflows/android-apk.yml` file is included. On mobile, enabling “Desktop site” in Chrome may make these options easier to find.
4. Commit the uploaded files to the `main` branch.
5. Open the repository's **Actions** tab. If prompted, enable workflows. Select **Build Jayesh Library APK**, then tap **Run workflow → Run workflow** if it has not started automatically.
6. Open the completed workflow run. Under **Artifacts**, tap `Jayesh-Library-debug-APK` to download the APK artifact ZIP.
7. Extract that downloaded ZIP. Tap `app-debug.apk` to install it. If Android asks, allow your browser or file manager to install unknown apps.

The first build can take several minutes. GitHub's layout may differ slightly on mobile; use Chrome's **Desktop site** if you cannot see Actions or Run workflow.

## Included in this starter build
- Dark/light theme toggle
- Import local files using Android's file picker
- Persistent bookshelf, search, and format filters
- PDF page-by-page reader
- Basic EPUB chapter rendering
- CBZ/ZIP image-comic reader
- TXT/MD reader with font-size controls
- Books stay on the device; no upload/account backend

## Current limitations
- This starter project has not been compiled/tested in this environment; the GitHub build will reveal any build errors.
- EPUB rendering is basic and may not preserve all chapter order, images, CSS, or navigation.
- CBR/RAR and DRM-protected books are not supported.
- Cover tiles are format-based placeholders rather than extracted book covers.
- PDF has previous/next controls but no direct page-number jump or zoom slider yet.
- This is a foundation build, not a production-ready release.
