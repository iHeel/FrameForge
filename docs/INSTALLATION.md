# Installing FrameForge Free

Download the Windows x64 EXE from this repository's Releases. Do not use the green Code → Download ZIP button to install the application. Run the installer, review the terms and choose model downloads on first launch. Prefer the default install path.

The Free edition requires Windows 10/11 x64 and a Vulkan-capable GPU with a compatible vendor driver. It does not include CPU-only AI processing. Python is bundled; models are downloaded after separate confirmation and license acceptance.

Use SHA256SUMS.txt from the same release to compare your files:

```powershell
Get-FileHash -LiteralPath '.\FrameForge-Free-1.2.1-Setup.exe' -Algorithm SHA256
```

Compare the full hash; it is not enough to see that the command ran. The build is unsigned and may trigger SmartScreen. Do not disable antivirus or system-wide security features.

Free and full editions use separate default folders and settings. Do not nest one edition inside the other's install directory. Use the uninstaller for the edition you want to remove; videos are preserved.

For offline use, install the required models while connected, then process locally. First-time model downloads require internet access.


## Moving from an older build

This download is a full installer, not an automatic in-app updater. Close FrameForge before installing. If setup requires removing the previous edition, note that the current uninstaller removes downloaded models and settings. Keep original and exported videos outside the installation folder, and plan to download models again after a clean reinstall.
