# PS99 Macro Hub

PS99 Macro Hub is a Windows desktop macro hub for Pet Simulator 99 (Roblox), **made by campa**.
It was originally built for the **V1LN** clan. Access is currently granted to the **LSQ** clan, and possibly the **INXY** clan.

> **BETA ΓÇô not yet fully tested.** Expect bugs; report them to campa.

This repository is the official distribution channel. **[Download the latest PS99MacroHub-Setup.exe](https://github.com/tamaspota/Clan_Macro_PS99_campa/releases/latest/download/PS99MacroHub-Setup.exe)** — this is the only installer you need. It contains the signed update package, and the Hub verifies it before installing.

GitHub automatically shows **Source code (zip)** and **Source code (tar.gz)** on its Releases page. These are repository snapshots, **not installers**; you do not need to download them.

## Current signed release: v1.0.54 (2026-11-05)

The signed **v1.0.54** update is now available: [release and Setup installer](https://github.com/tamaspota/Clan_Macro_PS99_campa/releases/tag/v1.0.54). Existing users can use the Hub update bell → **Check now** → **Install signed update**. The release keeps the existing member/ALT/task workflows and adds an **Owner-only Discord Publishing settings table** to configure clan names, Guild IDs, channels and approved Discord role IDs without editing code. The new **Navo Clan & Community** Discord target is distinct from the older NAVO Members guild.

**Important:** publishing v1.0.54 does not automatically install/restart the separate Owner-host AccessBot or enable a newly added clan's /access or Post switches. Owner-managed bot rollout and live access checks remain separate. Remote Staff publishing remains disabled until a trusted authorization relay is available. Halloween Games automatic candy-repeat/bonus task changes are not part of the signed live update.

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
