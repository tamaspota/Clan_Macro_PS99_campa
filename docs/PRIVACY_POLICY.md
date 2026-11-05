# PS99 Macro Hub — Privacy Policy

**Effective date:** 5 November 2026  
**Operator / privacy contact:** campa (Discord: `campa_ao`)  
**Scope:** the private PS99 Macro Hub Discord application/access bot and its linked Windows desktop application.

## 1. What information is processed

**Discord bot and access service:** To decide whether a request is permitted, the system may process a person's Discord user ID and username, server (guild) IDs, role IDs, access eligibility, requested access/command details and authorization results. The service uses these identifiers to grant, deny or revoke private access. A personal `/access` authorization code, where supported, is valid for **24 hours** and is tied to the intended account; code expiry does not necessarily mean all audit records are immediately erased.

**Windows Hub operational telemetry:** The [official distribution README](../README.md) documents the following transmitted information when a user runs the desktop software:
- a **hashed hardware identifier**, not the raw hardware ID;
- the user's Discord ID and name;
- app session start/end and duration, with approximately 60-second heartbeat events;
- which automation task ran and its duration;
- crash, abnormal stop, network interruption, install/startup and denied/expired-access diagnostics;
- the user's IP address and approximate country, region and city derived from it by Cloudflare.

The published desktop documentation states that **passwords, Roblox cookies, screenshots and local files are not transmitted** as part of this telemetry. Do not send secrets through Discord bot commands or support requests.

## 2. Purposes and necessity

Data is used to verify eligibility, issue and revoke time-limited permissions, secure the service against misuse, diagnose connectivity and application failures, and support authorized release notices. The desktop tool's documented startup telemetry/authorization check is mandatory for starting the Hub; the user is shown a notice and can decline to continue.

This private service is not intended for advertising or selling users' personal data.

## 3. Processing systems and access

The Discord platform processes interactions and identity information according to its own policies. The Windows tool's published telemetry design uses an **operator-controlled Cloudflare collector** for startup and operational events. Official Windows downloads are distributed through GitHub Releases. The public README states that collected telemetry is accessible to the operator.

Third-party providers may process technical information needed to deliver their respective services. Their independent privacy notices also apply.

## 4. Data retention

The current [official distribution documentation](../README.md) states a **90-day retention period for Windows usage telemetry**. Personal access codes have a 24-hour validity period, which is not the same as a verified deletion schedule. Other authorization/security records should be retained only for as long as needed to administer permitted access, investigate misuse and meet any applicable legal obligations.

Retention and deletion mechanisms are operational responsibilities of the operator; this policy does not claim that deletion has been independently audited.

## 5. Privacy requests and choices

Users may ask the operator what personal data is held, request correction or deletion, or object to processing where applicable law provides those rights. Contact **campa (`campa_ao`) through Discord DM** and identify the Discord account concerned without sending passwords, tokens or access codes. Requests are handled subject to identity verification and applicable legal requirements.

Removing the bot or ceasing to use the Hub stops future ordinary use, but does not itself prove that earlier audit records have been deleted.

## 6. Legal basis and safeguards

For users in jurisdictions where a legal basis is required, processing is intended to support the requested restricted service, authorization checks and the operator's legitimate interests in security and reliability, as applicable. Any processing requiring consent under local law must be handled accordingly. Access is role-based, authorization is revocable, and secret credentials must not be published in source repositories or support messages.

## 7. Updates

If the bot's commands, collected data, service providers or retention periods change, this policy must be updated to describe the actual operation. This policy covers only PS99 Macro Hub, not unrelated bots installed on the same Discord servers.

