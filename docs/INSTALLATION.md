# Installation and portable use

## Portable edition

The recommended Beta distribution is a portable x64 ZIP archive.

1. Download the current `LRD-...-x64-Portable.zip` from GitHub Releases.
2. Extract the complete ZIP to a writable folder, for example:

   ```text
   C:\Users\<name>\Programs\LRD\
   ```

3. Start `LRD.exe`.
4. On first start, create a new LRD database or select an existing one.

Do not run LRD directly from inside the ZIP archive.

## Database location

LRD uses an SQLite database. A new database is named `LRD.sqlite` by default, but the user may choose another location and filename.

The database is not stored in a cloud service by LRD.

## Portable mode

The portable release contains `portable.flag`. In portable mode, LRD prefers writable locations relative to the program directory where appropriate. If a location is not writable, LRD can fall back to a user-writable Windows application-data directory.

## Windows versions

Current public builds target **64-bit Windows**.

## SmartScreen

The current Beta executable is not digitally signed. Read [SMARTSCREEN.md](SMARTSCREEN.md) before first start.
