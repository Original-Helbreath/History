# sprites: Sprite paks

Every `.pak` sprite file the clients shipped. A version folder holds only the paks that are new or changed in that version; an unchanged pak is stored once, in the version it first appeared in, and its manifest row lists every version it was found in (`also_in`). The format is documented in [PAKLib](https://github.com/shadowevil/PAKLib).

## By version

| Version folder | Files | Size (bytes) | Version | Region | File dates | Source |
|---|---|---|---|---|---|---|
| `2.02/` | 167 | 572,728,752 | 2.02 | International (English) | 1999-01-21 to 2001-08-21 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso |
| `2.23/` | 45 | 111,678,256 | 2.23 | USA | 2002-12-21 to 2003-03-21 | https://web.archive.org/web/20141104104043id_/http://www.helbreathusa.com/patch_v223.zip |
| `3.0/` | 255 | 468,561,812 | 3.0 'The Apocalypse' | USA | 2002-01-09 to 2003-11-11 | https://archivedle.download.it/ftp1/012003/hbusa_apocalypse.exe |
| `3.1/` | 1 | 4,023,442 | 3.1 | USA | 2003-10-25 to 2003-10-25 | https://web.archive.org/web/20130630001212id_/http://www.helbreathusa.com/Patch_3.0_to_3.1.zip |
| `3.82-bundle/` | 31 | 84,743,492 | 3.82 community bundle (helbreath-v3.82, GitHub zip of 2020-04-26) | community private server; its LOGIN.CFG points to 51.15.15.123:12981 | 2020-04-26 to 2020-04-26 | unknown |
| `4.08/` | 44 | 121,026,822 | 4.08 | USA | 2003-05-13 to 2008-12-07 | https://archivedle.download.it/ftp1/042009/56439557/helbreathusa_setup_408.exe |
| `4.12.01/` | 4 | 15,977,080 | 4.12.01 | USA | 2009-02-02 to 2009-11-26 | https://web.archive.org/web/20110711161458id_/http://www.helbreathusa.com/downloadHB/Helbreath%20USA%20Install.zip |

Per-file sizes, SHA-256, dates and extraction chains are in `MANIFEST.json`.

## Manifest

`MANIFEST.json` has one row per file: path, size, SHA-256, version, region and era (each with a confidence: verified, inferred or unknown, and its basis), and every origin: source, exact URL, the file's own date and what kind of date it is, the day it was downloaded, and the extraction chain. The format is described in the [top README](../README.md#manifests).
