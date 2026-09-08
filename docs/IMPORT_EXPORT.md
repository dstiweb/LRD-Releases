# CSV import and export

CSV is LRD's general interchange format. It is intended for exchange with spreadsheets, other databases and migration tools.

A Discogs-specific adapter is planned for a later version and will be implemented separately from the generic CSV adapter.

## CSV import

The import assistant supports:

- automatic detection of common encodings and delimiters;
- source preview before import;
- automatic field recognition;
- manual source-to-target field assignment;
- creation of custom fields for unknown source columns;
- selectable custom-field types;
- reusable import profiles;
- duplicate detection using configurable comparison fields;
- duplicate strategies: add, skip or update;
- optional handling of empty values;
- a complete test run before records are written;
- progress bar, percentage and record count;
- optional full database backup before import;
- import log for problematic rows.

Multi-line memo/description fields are supported according to CSV quoting rules.

## CSV export

The export assistant supports:

- all records or only the current search/filter result;
- selectable normal and custom fields;
- configurable column order;
- UTF-8 BOM, UTF-8 and Windows-1252 where appropriate;
- semicolon, comma, tab or pipe delimiters;
- German, English or internal field names as headers;
- neutral exchange formatting or current display formatting;
- export preview;
- reusable export profiles.

## Recommended exchange format

For reliable round trips, use a Unicode encoding such as UTF-8, stable field names and neutral values where possible:

- dates: `YYYY-MM-DD`
- decimal values: decimal point in neutral format
- text values: quoted according to CSV rules when required

## Full backup vs CSV

CSV is intended for data interchange. For a complete LRD backup, use the SQLite backup function instead of CSV.
