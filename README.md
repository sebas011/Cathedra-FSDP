# Cathedra FSDP — Office updates

Download the ready-to-run Windows application from **[the latest release](https://github.com/sebas011/Cathedra-FSDP/releases/latest)**.

## Download the Office update

1. Sign in to GitHub with an account that has access to this private repository.
2. Open **Releases**, then the latest Cathedra FSDP Office update.
3. Under **Assets**, download **Cathedra-FSDP-0.5.18-Update.zip**. Extract the ZIP completely.
4. Open **UPDATE-INSTRUCTIONS.txt** inside the extracted **Cathedra-FSDP-0.5.18-Update** folder.

GitHub's **Code > Download ZIP** and the automatically generated **Source code** links contain this repository's delivery documentation. Download the named application ZIP under **Release Assets** to obtain the app.

## Update your existing Office app

The Office database already on your Office PC stays authoritative. This download contains application files and an intentional empty installation seed; it contains no working scholar database, account records or backups. Do not replace the Office app's `data/cathedra.db` with files from your development PC.

1. Open your usual Office app and make a backup through **Backup & Export**. Download the backup and keep it outside the app folder.
2. Save your edits and use **Exit Cathedra**. Wait for the app to stop.
3. Follow the included updater instructions. The **NEW update folder** is the extracted download. The **EXISTING Office app folder** is the folder you already use, containing **Cathedra FSDP.exe** and **data/cathedra.db**. These are two different folders.
4. Successful updater output includes `status: verified`, `version: 0.5.18` and `database_replaced: false`.
5. Reopen the **original Office app** through your usual shortcut. Confirm version 0.5.18, your scholar total and the newest records.

The updater takes a protected snapshot, rehearses any required migration on a private copy, preserves the current database during application replacement and retains the previous application for recovery. Python and Node are not required on the Office PC.

See [the full update walkthrough](UPDATE-INSTRUCTIONS.txt). Download the complete release asset rather than individual executable files. Future prepared updates will be listed on the same Releases page.

## Version 0.5.18

CSV exports group each scholar's grants on consecutive rows: profile information appears on the first row, with one grant per row afterward. Each grant retains its dates, status, case and remarks. Source/import/legacy export columns are removed. Schema 13 remains unchanged.

Local verification passed **390 backend and 185 frontend tests**, production packaging, the 147-file runtime manifest and a synthetic 0.5.17-to-0.5.18 data-preserving upgrade. Actual Office-PC acceptance should be checked after updating.

**SHA256SUMS.txt** records the SHA-256 checksum of the release ZIP. Only delivery instructions and checksums are stored in this repository; working records and the development checkout are not uploaded.
