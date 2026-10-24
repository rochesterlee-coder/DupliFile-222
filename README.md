# DupliFile

A Windows file duplicator with three appearance choices: Light, Dark, and Colourful (rainbow-inspired accents/background). Includes multilingual UI and local settings/history.

## Run the app
1. Install Python 3.11+ on Windows.
2. Double-click `Run_DupliFile.bat`.

## Build a standalone EXE
1. Double-click `Build_DupliFile_EXE.bat`.
2. The first build needs internet to install PyInstaller.
3. Find `DupliFile.exe` inside the `dist` folder. The built app is designed to work offline.

Features: select multiple files, choose a destination, create 1–30 copies per file, change language, switch Light/Dark/Colourful themes, and save settings/history locally in `%APPDATA%\DupliFile\data.json`.

Existing files are never overwritten; copies get unique names. Source files are copied, not moved or deleted.


## Build the standalone EXE using GitHub (no Python installation on your PC needed)
1. Upload `.github/workflows/build-windows.yml` to your repository, keeping the folder structure exactly as shown.
2. Open the repository on GitHub and click **Actions**.
3. Select **Build DupliFile for Windows**, then click **Run workflow** (or wait for the workflow to run after a push).
4. When it finishes successfully, open that workflow run and download the **DupliFile-Windows** artifact.
5. Extract the artifact ZIP to get `DupliFile.exe`.

The build needs internet on GitHub's runner. Once downloaded, the standalone EXE is designed to run offline.
