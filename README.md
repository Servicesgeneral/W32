# VeloSave Landing Page

A responsive Arabic RTL landing page for VeloSave, with a direct APK download and Android installation instructions.


## Files
- `index.html` — landing page
- `privacy.html` — starter privacy policy (must be reviewed against the app's real behavior)
- `assets/style.css` — styles
- `assets/script.js` — tiny script for current year
- `downloads/VeloSave-debug.apk` — APK extracted from the ZIP supplied by the project owner

## APK details checked from the supplied archive
- Filename inside archive: `app-debug.apk`
- Size: 21,325,575 bytes (about 20.3 MiB)
- This is a debug APK; use a signed release build for public distribution when available.
- Version name/code were not verified from the binary in this environment.

## Change the download file
Replace `downloads/VeloSave-debug.apk` with your final release APK. If you rename it, update the download link in `index.html` (both links) to match.


## Deploy on GitHub Pages
1. Create a GitHub repository, e.g. `velosave-site`.
2. Upload the contents of this folder to the repository root (not the folder itself).
3. In the repository, open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish, then open the Pages URL shown in settings.


## Optional: GitHub Releases for APK hosting
For a larger release APK or cleaner update workflow:
1. Open the repository's **Releases** section and create a new release/tag.
2. Upload the final APK as a release asset.
3. Copy the asset's direct download URL.
4. Replace the APK href in `index.html` with the direct release asset URL. Keep the `download` attribute for same-origin files; it may be ignored on external URLs.

## Before public launch
- Replace the debug APK with a signed release APK.
- Confirm the app's actual features and adjust descriptions accordingly.
- Review privacy policy to reflect actual data collection, SDKs, analytics, ads, and permissions.
- Add real screenshots only when available.
- Test the download and installation on a physical Android phone.
