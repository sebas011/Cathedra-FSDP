# Cathedra FSDP — Office updates

Download the ready-to-run Windows application from **[the latest release](https://github.com/sebas011/Cathedra-FSDP/releases/latest)**.

## Download and update

1. Sign in to GitHub with an account that has access to this private repository.
2. Open Releases, then the latest Cathedra FSDP Office update.
3. Under Assets, download **Cathedra-FSDP-0.5.19-Update.zip** and extract the ZIP completely.
4. Open **UPDATE-INSTRUCTIONS.txt** in the extracted folder. Make and download a backup in your usual Office app, save your edits and use Exit Cathedra.
5. Follow the two-folder prompts: the NEW folder is the extracted download; the EXISTING folder is your original app containing Cathedra FSDP.exe and data/cathedra.db.
6. Successful output includes `status: verified`, `version: 0.5.19` and `database_replaced: false`. Reopen the **original Office app** through your usual shortcut and check its version, scholar total and newest records.

For the supplied ASUS Office folder, the ZIP also contains **docs/OFFICE_RETRY_0.5.19.txt**, with the original installation path and a concise retry command. Choose the actual extracted folder containing **tools** if Windows adds a second nested folder.

GitHub's Code > Download ZIP and automatic Source code links contain delivery documentation. Download the named application ZIP under Release Assets to obtain the app.

The existing Office database stays authoritative. This download contains application files and an intentional empty installation seed, with no working scholar database, account records or backups. Do not copy a development data folder or replace the Office data/cathedra.db. Python and Node are not required.

The updater verifies the package, takes a protected snapshot, rehearses any required migration on a private copy, retains the old runtime and preserves the working database during replacement. Read [the full update walkthrough](UPDATE-INSTRUCTIONS.txt).

## Version 0.5.19

Windows runtime inventory verification now handles case-insensitive tool enumeration and separates the required direct tool files from extra nested tool documents or copies, with clearer package/path diagnostics. The required runtime files remain the same. A preflight failure can occur before an update-state journal is created. Keep the full traceback and recovery files; never delete/reset journals or blindly restore an older database.

When all required old runtime files pass their hash checks, the updater archives unlisted application leftovers separately under data/updates and retains a strictly verified old runtime before replacement. Its receipt identifies the residue archive and any repaired files. It does not assume filenames or ignore missing/corrupted required files, links or unreadable files.

Schema 13 and the one-grant-per-row CSV layout remain unchanged. Local verification passed **420 backend and 185 frontend tests**, production packaging, the 147-file runtime manifest and a synthetic data-preserving version18-to-version19 upgrade. Complete actual Office-PC acceptance after updating.

SHA256SUMS.txt records the release ZIP checksum. This repository contains only delivery instructions and checksums; working records and the development checkout are not uploaded. Older Releases and their assets are retained.
