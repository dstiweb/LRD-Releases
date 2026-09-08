# LRD – Local Record Desk

**LRD – Local Record Desk** is a Windows desktop application for managing a private music and record collection.

LRD is deliberately designed as a **local desktop application**:

- your collection is stored locally in an SQLite database;
- no cloud account is required;
- no cloud synchronization is required;
- no telemetry or usage tracking is built into normal collection management;
- Internet access is not required for normal database maintenance.

The program is distributed as **Freeware** by Dietmar Steffen.

> Current development status: **Beta**

## Main features

- record and music collection management in a classic desktop form;
- direct editing with automatic save when moving to another record;
- combined search across multiple fields;
- configurable table view with selectable columns, order, sorting and filters;
- user-defined custom fields;
- CSV import with preview, field mapping, profiles, duplicate handling and test run;
- CSV export with configurable fields and formats;
- automatic and manual SQLite backups;
- German and English user interface;
- portable Windows x64 edition planned/provided through GitHub Releases.

## Download

Program binaries are **not stored in the repository history**. Download published versions from the repository's **Releases** section.

A typical release asset is named similar to:

```text
LRD-v0.7.13-Beta-x64-Portable.zip
```

## First start

LRD can create a new empty database itself. Optionally, five sample records can be inserted so the interface, search and table functions can be tested immediately.

Alternatively, an existing LRD SQLite database can be opened or data can be imported from CSV.

See [Installation](docs/INSTALLATION.md) for details.

## Windows SmartScreen

The current Beta builds are not digitally code-signed. Windows Defender SmartScreen may therefore warn when starting a downloaded LRD executable for the first time.

See [Windows SmartScreen](docs/SMARTSCREEN.md) before running a downloaded build.

## Backups

LRD supports complete SQLite database backups. Automatic backups can be retained for a configurable number of days. Manual backups are never deleted automatically.

See [Backup and restore](docs/BACKUP.md).

## Import and export

CSV import and export are designed as the general exchange mechanism. Import supports field mapping, custom fields, profiles, duplicate handling and a test run before data is written.

See [Import and export](docs/IMPORT_EXPORT.md).

A Discogs-specific import/export adapter is planned for a later version.

## Privacy and local data storage

The collection database remains under the user's control on the local computer. LRD does not require a user account or a cloud service for normal operation.

If optional online integrations are added later, they will be separate, explicitly initiated functions; the local collection database remains the primary data store.

## License

LRD is **Freeware**. See [LICENSE.txt](LICENSE.txt) for the exact terms.

Third-party notices are listed in [THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt).

Copyright © 2026 Dietmar Steffen.
