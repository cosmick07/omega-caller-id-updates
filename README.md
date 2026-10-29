# omega-caller-id-updates

Encrypted update files for the Omega Caller ID app on the Omega Dental reception PCs.

- `latest.json` — the current version for each channel (`pilot` = the pilot PC, `stable` = everyone).
- `releases/<version>.bin` — the app's code, encrypted (AES-256-GCM). It can't be read or used without the installed app.

The PCs check this repository every 30 minutes, download a newer version, check it, and install it at a quiet moment (no calls for 5 minutes).
