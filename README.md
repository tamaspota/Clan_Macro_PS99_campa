# PS99 Macro Hub

PS99 Macro Hub is a Windows desktop macro hub for Pet Simulator 99 (Roblox), **made by campa**.
It was originally built for the **V1LN** clan. Access is currently granted to the **LSQ** clan, and possibly the **INXY** clan.

> **BETA – not yet fully tested.** Expect bugs; report them to campa.

This repository is the official distribution channel. **The only file you need is `PS99MacroHub-Setup.exe`** from the latest release. The other assets (`PS99MacroHub-<version>.zip`, `release-manifest.json`, `.sig`) are the **internal update package** used automatically by the installer and the in-app updater — do not download them.

## Install

1. Install the **.NET 8 Desktop Runtime (x64)** from Microsoft (dotnet.microsoft.com → .NET 8.0 → Desktop Runtime), if you don't have it yet.
2. Open **Releases** (right side of this page), pick the latest version and download **`PS99MacroHub-Setup.exe`**.
3. Right-click `PS99MacroHub-Setup.exe` → **Run as administrator** and follow the installer.
4. Start **PS99 Macro Hub** and **sign in with Discord**. You must be a member of an authorised clan server.
5. Ask **campa** for your personal **access code**, paste it in the Hub and press **Activate**. Each code works only for your Discord account and is valid for **24 hours**; ask for a new one when it expires.

Updates are delivered through this repository's Releases. The Hub verifies every update's signature before installing it.

## Usage data (please read)

The Hub sends usage data to the Owner (campa) so the clan can see who uses it and spot problems:

- a **hashed hardware ID** (HWID hash — the raw ID never leaves your PC)
- your **Discord user ID and name**
- when the Hub was open and online (session start/end, minutes; a heartbeat about every 60 s)
- which task/macro ran and for how many minutes
- abnormal ends (network drop, PC shutdown/crash, Hub crash)

No passwords, Roblox cookies, screenshots or files are sent. While offline the data is queued on your PC and sent later. You are shown this notice on first start; if you do not accept, the Hub closes.

## Notes

- Windows 10/11 x64 only.
- Never share your access code or your Discord login with anyone.
- Use at your own risk. Macros are automation aids and can misbehave if the game UI changes; re-calibrate image slots after game updates.
