# art: Sprite sheets in their original format

Every sheet of every sprite pak held, by version then pak (`<version>/<pak>/<sheet>`). Each sheet's bitmap is kept exactly as it is stored inside the pak (a Windows BMP, byte for byte, not converted). Beside it in git is `<sheet>.frames.json`: the sheet's frame rectangles and pivots read from the pak's frame table (extracted metadata, not an original file). The bitmaps are byte-for-byte slices of the paks under `sprites/`, so to stay within the git size budget they are published as one release archive per version (`History-art-<version>.7z`). Each manifest row gives the bitmap's offset and length inside its pak and its SHA-256, so any bitmap can be cut from the pak and checked. Format reference: [PAKLib](https://github.com/shadowevil/PAKLib). Crusade war art (`Cru*`, `Catapult`, `ManaCollector`, `ManaStone`, `Detector`, `GT-*`) is tagged era Crusade (inferred from the names); no source held dates Heldenian.

## By version

| Version folder | Files | Size (bytes) | Version | Region | File dates | Source |
|---|---|---|---|---|---|---|
| `3.82-bundle/` | 460 | 2,472,544 | 3.82 community bundle (helbreath-v3.82, GitHub zip of 2020-04-26) | community private server; its LOGIN.CFG points to 51.15.15.123:12981 | 2020-04-26 to 2020-04-26 | unknown |
| `3.0/` | 9583 | 26,142,256 | 3.0 'The Apocalypse' | USA | 2002-01-09 to 2003-11-11 | https://archivedle.download.it/ftp1/012003/hbusa_apocalypse.exe |
| `2.02/` | 6132 | 19,335,604 | 2.02 | International (English) | 1999-01-21 to 2001-08-21 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso |
| `4.08/` | 1047 | 4,122,183 | 4.08 | USA | 2003-05-13 to 2008-12-07 | https://archivedle.download.it/ftp1/042009/56439557/helbreathusa_setup_408.exe |
| `3.1/` | 11 | 18,342 | 3.1 | USA | 2003-10-25 to 2003-10-25 | https://web.archive.org/web/20130630001212id_/http://www.helbreathusa.com/Patch_3.0_to_3.1.zip |
| `2.23/` | 576 | 4,387,634 | 2.23 | USA | 2002-12-21 to 2003-03-21 | https://web.archive.org/web/20141104104043id_/http://www.helbreathusa.com/patch_v223.zip |
| `4.12.01/` | 53 | 1,475,160 | 4.12.01 | USA | 2009-02-02 to 2009-11-26 | https://web.archive.org/web/20110711161458id_/http://www.helbreathusa.com/downloadHB/Helbreath%20USA%20Install.zip |

Per-file sizes, SHA-256, dates and extraction chains are in `MANIFEST.json`.

## Manifest

`MANIFEST.json` has one row per file: path, size, SHA-256, version, region and era (each with a confidence: verified, inferred or unknown, and its basis), and every origin: source, exact URL, the file's own date and what kind of date it is, the day it was downloaded, and the extraction chain. The format is described in the [top README](../README.md#manifests).
