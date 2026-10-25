# Cathedra FSDP - Office updates

Current download: **0.5.26**. Download **Cathedra-FSDP-0.5.26-Update.zip** under Assets on the [latest release](https://github.com/sebas011/Cathedra-FSDP/releases/latest). GitHub's Source code ZIP is for development.

## Update your existing Office installation

1. Create a backup in the existing app, keep a copy outside its folder, and note your newest scholars for checking afterward.
2. Download the application ZIP and compare its checksum with SHA256SUMS.txt before extraction.
3. Use Extract All into a new update folder. Save edits and close the installed Cathedra app normally.
4. Follow [UPDATE-INSTRUCTIONS.txt](UPDATE-INSTRUCTIONS.txt). Select the NEW extracted folder first and your EXISTING installation containing Cathedra FSDP.exe and **data/cathedra.db** second.
5. Keep the existing Office database. Never replace it with a development database or the empty installation seed. The supported updater protects and rehearses it before replacing application files.
6. Reopen the original installation, confirm version 0.5.26, and check your newest scholar records. The retained database receives its protected additive upgrade at normal startup when needed.

## What changed in 0.5.26

- Administrators can open a scholar's Overview, expand Change history, then View previous and new values. New changes compare an explicit set of business fields. Long previews are marked when truncated; old events retain their existing metadata without invented values. Passwords, sessions and Google credentials are excluded.
- Assessment details in an annual grant and the dashboard contract follow-up show the factual reason, deadline basis where available, and assessed-on date. Recorded outcomes, separate cases, payment progress, application grouping and the three-year grace rules remain in force.
- Business dates use Asia/Manila consistently, including contract assessments and the default Office Log date. Security and recovery timestamp handling remains as previously implemented.

Schema 17 adds only nullable **activity_events.change_details**. Existing scholar records, grant history, accounts and Google connections stay in the original installation. Optional dates, Summer, literal calendar years, certification/enhancement programs, education records and existing data-entry requirements are retained.

## Google Sheets reporting

Use the [detailed Google Sheets setup guide](docs/GOOGLE_SHEETS_SETUP.md). It covers creating the Cloud project, enabling the Sheets API, Desktop credentials, approved test users, spreadsheet sharing, the app connection and troubleshooting. Set up and sign in separately on each PC/Windows account; local credentials and connections are excluded from downloads.

The reporting tab retains exactly No., Name, Age, Tenure, Department, Rank/position, Previous degree, Program, Delivering HEI, Grant type, Date started, Date ended, Extension, Status and Remarks. Each grant has its own row, with profile and education details on the scholar's first row. CSV exports retain their separate full-detail layout.

## Verification and recovery

All 628 backend tests and 270 frontend tests passed locally. The [exact-source Windows workflow](https://github.com/sebas011/Cathedra-FSDP-source-code/actions/runs/40190887672) also passed those regression counts, dependency checks and packaged Windows checks. Local verification includes an empty schema17 seed, 151 runtime files, both inventory verifiers, PowerShell 5.1/7 workflows, a packaged schema16-to17 upgrade with retained fictional records/history, and guarded installation preserving existing database and encrypted-Google bytes. Actual Office-PC acceptance remains separate.

The ZIP contains the Windows application and an intentionally empty seed for new installations. It contains no working scholar records, accounts, backups, OAuth credentials, tokens or private installation receipts. No separate Python/Node installation is required. This is an unsigned internal build; checksums verify integrity, not publisher identity. Previous releases remain available for reviewed recovery; do not run an older app against a newly migrated database.

[Release notes and downloads](https://github.com/sebas011/Cathedra-FSDP/releases/tag/v0.5.26) | [Source code](https://github.com/sebas011/Cathedra-FSDP-source-code)
