# other: Other files

Files of no other type shipped with a client: uninstaller data, a brush file, the updater list, Thumbs.db, Visual SourceSafe `vssver.scc` files (kept under the client folder they were found in), and the NSIS uninstaller data block that 7-Zip exposes from the 2024 Korean installer as `uninstall.exe.nsis` (installer bytes, not an installed file and not a decompiled script).

## Files

| File | Version | Region | Date | Size (bytes) | SHA-256 | Stored |
|---|---|---|---|---|---|---|
| `4.12.01/Brush.brs` | 4.12.01 | USA | 2007-11-20 (archive-entry) | 331,000 | `0bce2aff9121de52a482cfffeb9266336769adc8f339e0b28b12452f921e9418` | git |
| `4.12.01/Thumbs.db` | 4.12.01 | USA | 2010-09-19 (archive-entry) | 13,312 | `6c35868615372fb6f041a32e3fbb939aa79e09d39f49553025bc5924b35e761a` | git |
| `4.12.01/unins000.dat` | 4.12.01 | USA | 2008-12-31 (archive-entry) | 50,885 | `f9bc958358d6cb7246861ced80604b0e9bcdc90a98eb6969c7570201af19d1e0` | git |
| `4.12.01/update.lst_` | 4.12.01 | USA | 2010-09-03 (archive-entry) | 1,305 | `e561eecedb4ec560031fb409d99039e9b9d47714e4a77419cf766038a95ddf65` | git |
| `korea-2024/music/vssver.scc` | Korea 2024-09-27 client (no version number stated) | Korea | 2008-10-31 (installer-entry) | 208 | `e37762f4baa4266068394e04f1a8fb461a2e6d633b4888f24c51e1da0354ce68` | git |
| `korea-2024/sounds/vssver.scc` | Korea 2024-09-27 client (no version number stated) | Korea | 2008-10-31 (installer-entry) | 3,744 | `68327f9a052fcbec15b41ca141070cd02f7ebb22ca5502890856929ae687d45d` | git |
| `korea-2024/uninstall.exe.nsis` | Korea 2024-09-27 client (no version number stated) | Korea | unknown | 1,068 | `7a61c4668968ab42174beaeaa2e130fd5e0c4b82a06788b957b18b052261809e` | git |

## Not in git

Over 100 MB, or kept elsewhere; download from the link given.

| File | Version | Region | Date | Size (bytes) | SHA-256 | Stored |
|---|---|---|---|---|---|---|
| `4.12.01-SPRITES.zip` | 4.12.01 | USA | 2009-07-17 (archive-entry) | 56,542,388 | `166831d4df3e0603f0b79414c7768ab07e505cad8dc034d8ea9cff7d39783782` | inside history-1 Helbreath.USA.Install.zip (Helbreath USA Install.exe -> SPRITES/SPRITES.zip) |

- `4.12.01-SPRITES.zip`: Kept out of git to stay near the size budget: every pak in it is stored loose under sprites/ (one copy per SHA-256). Not a separate release asset: 7-Zip extracts it from the zip and its RAR self-extractor byte-exact (SHA-256 checked 2026-10-27); every pak in it is stored loose under sprites/.

## Manifest

`MANIFEST.json` has one row per file: path, size, SHA-256, version, region and era (each with a confidence: verified, inferred or unknown, and its basis), and every origin: source, exact URL, the file's own date and what kind of date it is, the day it was downloaded, and the extraction chain. The format is described in the [top README](../README.md#manifests).
