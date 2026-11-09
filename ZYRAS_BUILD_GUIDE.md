# Zyras World Viewer — personal customization

This is modified source code for Aurora Viewer, not a precompiled Windows application.

## Changes
- Embedded purple fantasy wallpaper on Aurora's live login screen.
- Zyras World Viewer title and logo.
- Purple/lavender palette in default theme and `skins/zyras-world/theme.json`.
- Removed the first-login news sidebar; existing login, credentials and Preferences controls remain.
- Windows executable icon and product metadata customized.
- Manual GitHub Actions workflow at `.github/workflows/zyras-windows.yml`.

## Build locally on Windows
Follow Aurora's Windows toolchain setup in its README and run:

```powershell
cargo build --release --locked -p aurora-viewer --features xr-static-loader
```

The executable is initially `target/release/aurora-viewer.exe`; the workflow copies it to `Zyras-World-Viewer.exe` in a download ZIP.

## GitHub Actions
1. Create a repository under your GitHub account and upload this source (or push it with Git).
2. Open **Actions** > **Build Zyras World Viewer (Windows)** > **Run workflow**.
3. Once the build succeeds, download the `Zyras-World-Viewer-Windows` artifact.

A successful build does not guarantee runtime compatibility; launch and test the program on Windows before relying on it. Aurora is an actively evolving project.

## Attribution
The original Aurora Viewer project and its license remain in the repository. Third-party character and weapon imagery is for personal use only; it is not licensed for redistribution.
