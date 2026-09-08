# Backup and restore

LRD stores the complete collection in an SQLite database. A complete database backup is therefore the preferred full backup format.

## Automatic backups

Automatic backups can be enabled in LRD. The retention time is configurable, for example 30 days.

Only automatic backups older than the configured retention period are removed automatically.

Typical filename:

```text
auto_2026-09-08_080000.sqlite
```

## Manual backups

Manual backups are never deleted automatically. They remain until the user explicitly deletes them.

Typical filename:

```text
manual_2026-09-08_153500.sqlite
```

## Default backup directory

LRD prefers a `Backups` folder next to the executable when that location is writable.

If the program directory is not writable, LRD can use:

```text
%LOCALAPPDATA%\LRD\Backups
```

The backup directory can be changed in the program settings.

## Backup integrity

LRD creates backups using SQLite's backup mechanism and checks the resulting database with SQLite integrity checking.

## Recommendation

A local backup protects against many accidental edits or database problems, but it does not protect against complete disk failure. Important collections should additionally be copied to another physical storage device or another backup location chosen by the user.
