# Cathedra FSDP — Office updates

Current download: **0.5.23**. Download **Cathedra-FSDP-0.5.23-Update.zip** under Assets on the [latest release](https://github.com/sebas011/Cathedra-FSDP/releases/latest). GitHub's Source code ZIP is for development.

## Update your existing Office installation

1. Download the application ZIP and compare its checksum with SHA256SUMS.txt before extraction.
2. Extract All into a new update folder. Close the installed Cathedra app normally.
3. Follow [UPDATE-INSTRUCTIONS.txt](UPDATE-INSTRUCTIONS.txt), selecting the existing installation containing Cathedra FSDP.exe and data as the target.
4. Preserve the Office **data/cathedra.db**. Never replace it with a development database or the empty installation seed.
5. Open the original Office installation, confirm version 0.5.23 and check the newest scholar records.

## Google Sheets reporting

Use the [detailed Google Sheets setup guide](docs/GOOGLE_SHEETS_SETUP.md). It covers creating the Cloud project, enabling the Sheets API, Desktop credentials, approved test users, spreadsheet sharing, the app connection and troubleshooting.

The reporting tab contains only No., Name, Age, Tenure, Department, Rank/position, Previous degree, Program, Delivering HEI, Grant type, Date started, Date ended, Extension, Status and Remarks. It keeps one grant per row and profile details on the scholar's first row. Other tabs and the local database remain unchanged. Configure and sign in separately on the Office PC: local Google credentials and connections are excluded from downloads.

This release also includes the 0.5.22 improvements since the previous GitHub download: single-year periods, Incomplete grant status, repayment progress, optional completion deadlines and allowed duration, the three-year grace calculation, and the multiline typing fix. CSV exports retain their full-detail layout.

The ZIP contains the Windows application and an intentionally empty schema 16 seed. It contains no working scholar records, accounts, backups, OAuth credentials, tokens or private installation receipts. The Office PC needs no separate Python/Node installation. This is an unsigned internal build; checksums verify integrity, not publisher identity.

Validation: 586 backend cases and 245 frontend tests, plus the packaged release gates recorded with the release. Intended Office-PC acceptance remains a separate check. Previous releases are preserved for reviewed recovery; do not run an older application against a newly migrated database.

[Release notes and downloads](https://github.com/sebas011/Cathedra-FSDP/releases/tag/v0.5.23) · [Source code](https://github.com/sebas011/Cathedra-FSDP-source-code)
