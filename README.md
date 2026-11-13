# PS99 Macro Hub

PS99 Macro Hub is a Windows desktop macro hub for Pet Simulator 99 (Roblox), **made by campa**.
Access is currently granted to members of the **AO** and **NAVO** clan Discord servers.

> **BETA – not yet fully tested.** Expect bugs; report them to campa.

This repository is the official distribution channel. **[Download the latest PS99MacroHub-Setup.exe](https://github.com/tamaspota/Clan_Macro_PS99_campa/releases/latest/download/PS99MacroHub-Setup.exe)** — this is the only installer you need. It contains the signed update package, and the Hub verifies it before installing.

GitHub automatically shows **Source code (zip)** and **Source code (tar.gz)** on its Releases page. These are repository snapshots, **not installers**; you do not need to download them.

## Current signed release: v1.0.58 (2026-11-13)

The **signed v1.0.58** package is available: [GitHub release and Setup installer](https://github.com/tamaspota/Clan_Macro_PS99_campa/releases/tag/v1.0.58). Existing users can open the Hub update bell → **Check now** → **Install signed update**.

What's new in v1.0.58:

- **U101 (Masquerade Games): return to #8 Thorn Spire.** The guided Ultimate return goal now offers **#8 Thorn Spire (reset via #1)**. The route uses current images only (Event proof → Teleport → #1 → #1 arrival → Teleport → #8 → #8 arrival). It uses no fixed coordinates or movement and never presses Revive.
- **F6 / reconnect.** With the #8 goal saved and automatic recovery enabled for the task, F6 and a Roblox disconnect re-enter the current Event, go back to #8, check the arrival and resume the task once.
- **Lobby landing.** If an armed U101 task finds itself in the main-world lobby, the Hub runs the same bounded recovery (at most 2 per 30 minutes). If the evidence is unclear, it stops safely.
- Includes v1.0.57: ALT Event startup no longer waits up to 2 minutes on an unrecognised Teleport menu.

Calibrate the current U101 images and activate Event startup before use. Automatic recovery is opt-in per task. These features are not yet confirmed in live gameplay; please report problems.

## Install

1. Install the **.NET 8 Desktop Runtime (x64)** from Microsoft (dotnet.microsoft.com → .NET 8.0 → Desktop Runtime), if you don't have it yet.
2. Download **[PS99MacroHub-Setup.exe](https://github.com/tamaspota/Clan_Macro_PS99_campa/releases/latest/download/PS99MacroHub-Setup.exe)** (direct installer link; the release page is not required).
3. Right-click `PS99MacroHub-Setup.exe` → **Run as administrator** and follow the installer.
4. Start **PS99 Macro Hub** and **sign in with Discord**. You must be a member of an authorised clan server.
5. Ask **campa** for your personal **access code**, paste it in the Hub and press **Activate**. Each code works only for your Discord account and is valid for **24 hours**; ask for a new one when it expires.

Updates are delivered through this repository's Releases. The Hub verifies every update's signature before installing it.

## Usage data (please read)

The Hub sends usage data to the Owner (campa) so the clan can see who uses it and spot problems:

- a **hashed hardware ID** (HWID hash – the raw ID never leaves your PC)
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
## v1.0.26 (BETA)
The main task list shows only HG Fast hatch (zone 5) and HG Match games; both are added automatically. Only PS99MacroHub-Setup.exe needs to be downloaded.

## History
The project started about a year ago in the V1LN clan with an AHK script, after my internet kept dropping and I needed reliable recovery. I then built the V1LN version so the whole clan could use it. After a merge I joined the Lynx clan, and on 2026-10-25 I was put on LOA there. The Hub is currently available only to members of the authorised AO and NAVO Discord servers.

## Support
If you have a problem, DM campa on Discord. If you can't DM me, you wouldn't get access anyway.
