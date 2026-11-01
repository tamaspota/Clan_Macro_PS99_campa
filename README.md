# PS99 Macro Hub

PS99 Macro Hub is a Windows desktop macro hub for Pet Simulator 99 (Roblox), **made by campa**.
It was originally built for the **V1LN** clan. Access is currently granted to the **LSQ** clan, and possibly the **INXY** clan.

> **BETA ΓÇô not yet fully tested.** Expect bugs; report them to campa.

This repository is the official distribution channel. **The only file you need is `PS99MacroHub-Setup.exe`** from the latest release. The other assets (`PS99MacroHub-<version>.zip`, `release-manifest.json`, `.sig`) are the **internal update package** used automatically by the installer and the in-app updater ΓÇö do not download them.

## Install

1. Install the **.NET 8 Desktop Runtime (x64)** from Microsoft (dotnet.microsoft.com ΓåÆ .NET 8.0 ΓåÆ Desktop Runtime), if you don't have it yet.
2. Open **Releases** (right side of this page), pick the latest version and download **`PS99MacroHub-Setup.exe`**.
3. Right-click `PS99MacroHub-Setup.exe` ΓåÆ **Run as administrator** and follow the installer.
4. Start **PS99 Macro Hub** and **sign in with Discord**. You must be a member of an authorised clan server.
5. Ask **campa** for your personal **access code**, paste it in the Hub and press **Activate**. Each code works only for your Discord account and is valid for **24 hours**; ask for a new one when it expires.

Updates are delivered through this repository's Releases. The Hub verifies every update's signature before installing it.

## Usage data (please read)

The Hub sends usage data to the Owner (campa) so the clan can see who uses it and spot problems:

- a **hashed hardware ID** (HWID hash ΓÇö the raw ID never leaves your PC)
- your **Discord user ID and name**
- when the Hub was open and online (session start/end, minutes; a heartbeat about every 60 s)
- which task/macro ran and for how many minutes
- abnormal ends (network drop, PC shutdown/crash, Hub crash)
- your **IP address** and the **coarse location** (country, region, city) Cloudflare derives from it, stored with each event
- a **startup log** each time the Hub starts, plus installs and denied/expired access attempts

No passwords, Roblox cookies, screenshots or files are sent. Since v1.0.25 the Hub **needs internet to start**: it logs the start to the clan collector (Cloudflare, ps99-telemetry.ps99hub-tamas.workers.dev) and unlocks only after a signed reply. Other data is queued while offline and sent later. Data is kept for 90 days and only the Owner can read it. You are shown this notice on first start; if you do not accept, the Hub closes.

## Notes

- Windows 10/11 x64 only.
- Never share your access code or your Discord login with anyone.
- Use at your own risk. Macros are automation aids and can misbehave if the game UI changes; re-calibrate image slots after game updates.

## v1.0.24 (BETA)
Updates come only from this public release channel (same for everyone) and Install/Update now closes and restarts the Hub automatically. If you started the Hub from an old Drive launcher, download `PS99MacroHub-Setup.exe` from the latest release once and use its desktop shortcut.

## v1.0.25 (BETA)
The Hub needs an internet connection to start (startup log incl. IP and coarse location, see Usage data). Discord outages get a short Owner-set grace period. Download PS99MacroHub-Setup.exe from the latest release.
