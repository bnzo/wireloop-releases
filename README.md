# Wireloop releases

Downloads of Wireloop, an indoor cycling game for macOS (Apple silicon). Each [release](https://github.com/bnzo/wireloop-releases/releases) has the app as a zip, its SHA-256, and `latest.json`, which the game reads to tell you when a new version is out (Wireloop > Check for Updates…).

## Install

1. Download `Wireloop-<version>-arm64.zip` from the [latest release](https://github.com/bnzo/wireloop-releases/releases/latest).
2. Unzip it and move **Wireloop** to your Applications folder.
3. Open it. The first time, macOS asks you to allow it (below).

## Allow Wireloop the first time

Wireloop is not notarized by Apple yet, so the first time you open it macOS blocks it and asks you to confirm that you trust it. You do this once; after that it opens like any other app.

**1. The first try is blocked.** Open Wireloop from Applications. macOS says "Wireloop.app" Not Opened. Click **Done**, not Move to Trash.

<p align="center">
  <img width="372" height="396" alt="Screenshot 2026-11-18 at 16 22 10" src="https://github.com/user-attachments/assets/98ded7a7-8f84-4ab9-a220-77e48130b48c" />
</p>

**2. Allow it in System Settings.** Open System Settings (Apple menu > System Settings…) and go to **Privacy & Security**. Scroll down to **Security**: it says "Wireloop.app" was blocked to protect your Mac. Click **Open Anyway**.

<p align="center">
  <img width="835" height="948" alt="Screenshot 2026-11-18 at 16 22 34" src="https://github.com/user-attachments/assets/611632af-29ee-42a1-a4e3-3bb002c12570" />
</p>

**3. Confirm.** macOS asks once more, Open "Wireloop.app"?. Click **Open Anyway**.

<p align="center">
  <img width="372" height="462" alt="Screenshot 2026-11-18 at 16 22 47" src="https://github.com/user-attachments/assets/f27faf21-2d91-488e-b044-a860842803c0" />
</p>

**4. Approve with Touch ID or your password.** Touch the Touch ID sensor, or click **Use Password…** and type your Mac's administrator password. Wireloop opens.

<p align="center">
  <img width="372" height="450" alt="Screenshot 2026-11-18 at 16 22 57" src="https://github.com/user-attachments/assets/16ae920e-8bec-4bf7-b5a0-cef12d5bb52e" />
</p>

If you prefer Terminal, this does the same in one go:

```sh
xattr -dr com.apple.quarantine "/Applications/Wireloop.app"
```

Wireloop then asks once for what it uses: Bluetooth (your trainer and controllers), the Music app (the music player), and the microphone and speech recognition (searching videos by voice). Allow what you want to use; you can change it later in Privacy & Security.

## Update

Wireloop checks for a new version when it starts and can install it itself (Wireloop > Check for Updates…). By hand: quit Wireloop and replace it with the new one. Your rides and settings are kept.
