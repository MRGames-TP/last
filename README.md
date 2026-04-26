# Taitrts — HTML5 Tetris clone

Small frontend Tetris prototype. This folder includes a GitHub Actions workflow that can build an unsigned Android APK.

Local preview
-------------

Open `index.html` in a browser or serve the folder:

Windows (PowerShell):
```powershell
# from the taitrts folder
Start-Process .\index.html
# or serve over HTTP
python -m http.server 8000
```

Build an unsigned APK via GitHub Actions
--------------------------------------

1. Push this project to a GitHub repository under your account (root contains `taitrts/` and `.github/workflows`).
2. On GitHub, go to Actions → Build APK → Run workflow.
3. When the run finishes, download the `taitrts-apk` artifact (contains the unsigned APK).

Notes
-----
- The APK produced by CI is unsigned. Sign it with `apksigner` before distribution.
- Building locally requires Node.js and Android Studio / SDK. I can help with local instructions if needed.