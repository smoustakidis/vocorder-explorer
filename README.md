# VOCORDER breath-data explorer

Password-protected, browser-only explorer for the VOCORDER breath study.

This repository contains **only** the published build (`index.html`, `support.js`, `Plot.dc.html`).
`index.html` is the whole app encrypted with AES-256-GCM (key derived with PBKDF2-SHA256, 600,000 iterations);
no unencrypted study data are stored here. The password is shared separately with authorised team members.

Source and build script: private repository `smoustakidis/VOCORDER`, branch `explorer-app`, folder `LT_VOCORDER/app/`
(`python3 app/build_explorer.py --encrypt` → copy `vocorder_explorer/publish/*` here).

Do not upload the unlocked build (`vocorder_explorer/local/`) or any raw data to this repository.
