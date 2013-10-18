KeePassX with password database sharing
=======================================

These changes allow multiple KeePassX instances to open same file (e.g. on a
network share) for reading.

All the changes are done against stock keepassx 0.4.3.

## What is done

 * Don't keep database file open, close it just after loading.
 * Option to open database file in read-only mode.
 * Disabled "Save" button in read-only mode.

## TODO

 * Disable all database changing actions in the GUI in read-only mode.
