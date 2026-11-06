# PS99 Macro Hub

PS99 Macro Hub is a Windows desktop macro hub for Pet Simulator 99 (Roblox), **made by campa**.
It was originally built for the **V1LN** clan. Access is currently granted to the **LSQ** clan, and possibly the **INXY** clan.

> **BETA ΓÇô not yet fully tested.** Expect bugs; report them to campa.

This repository is the official distribution channel. **[Download the latest PS99MacroHub-Setup.exe](https://github.com/tamaspota/Clan_Macro_PS99_campa/releases/latest/download/PS99MacroHub-Setup.exe)** — this is the only installer you need. It contains the signed update package, and the Hub verifies it before installing.

GitHub automatically shows **Source code (zip)** and **Source code (tar.gz)** on its Releases page. These are repository snapshots, **not installers**; you do not need to download them.

## Current signed release: v1.0.55 (2026-11-06)

The **signed v1.0.55** package is available: [GitHub release and Setup installer](https://github.com/tamaspota/Clan_Macro_PS99_campa/releases/tag/v1.0.55). Existing users can open the Hub update bell → **Check now** → **Install signed update**. Published source: `f6806e42b4fa34a02fd61c890da06a5c0d7e92d0`; validated Windows Release tests: **2680/2680 PASS**. The trusted Owner publisher downloaded and SHA-256 checked the public Setup after signing.

Changes include safer Owner-only Discord Publishing table editing (exact-row delete confirmation, undo and manual ordering), Usage Log endpoint/tab fixes, and guarded Halloween Games Zone 1 teleport handling when the menu is already open. These do **not** automatically change saved custom tasks or guarantee all Halloween queue/egg routes are calibrated.

**Separate Owner validation is still required:** the AccessBot binary is built but **not deployed** by the public installer; new guild `/access` authorization and no-ping Discord announcements must be tested by the Owner. The Staff remote relay remains disabled. The Halloween Fast Hatch egg interaction still requires a valid calibrated `hg_egg_e_prompt` target and live-gameplay verification. No unattended rewards/bonus task is promoted by this release.

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
The project started about a year ago in the V1LN clan with an AHK script, after my internet kept dropping and I needed reliable recovery. I then built the V1LN version so the whole clan could use it. After a merge I joined the Lynx clan, and on 2026-10-25 I was put on LOA there. On 2026-11-01 I joined LSQ, so the Hub is available for V1LN, LSQ and INXY, and only for members of those three Discord servers.

## Support
If you have a problem, DM campa on Discord. If you can't DM me, you wouldn't get access anyway.
