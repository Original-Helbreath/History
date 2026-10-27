# configs: Configuration and game text

`CONTENTS/` text (item names, messages, magic and skill tables), `LOGIN.CFG` (the log server address each client connected to) and other text files. Files from a `MAPDATA/` folder are under `mapdata/`. `badword.txt` is XOR-obfuscated as shipped.

## By version

| Version folder | Files | Size (bytes) | Version | Region | File dates | Source |
|---|---|---|---|---|---|---|
| `2.02/` | 51 | 534,116 | 2.02 | International (English) | 2000-04-19 to 2001-08-21 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso |
| `2.23/` | 14 | 50,183 | 2.23 | USA | 2003-04-10 to 2003-04-12 | https://web.archive.org/web/20141104104043id_/http://www.helbreathusa.com/patch_v223.zip |
| `3.0/` | 30 | 94,237 | 3.0 'The Apocalypse' | USA | 2001-06-27 to 2003-10-23 | https://archivedle.download.it/ftp1/012003/hbusa_apocalypse.exe |
| `3.81/` | 1 | 10,259 | 3.81 | USA | 2005-02-15 to 2005-02-15 | https://web.archive.org/web/20060707141807id_/http://www.helbreathusa.com:80/hbusa_update_3.72_to_3.81.zip |
| `3.82-bundle/` | 19 | 83,717 | 3.82 community bundle (helbreath-v3.82, GitHub zip of 2020-04-26) | community private server; its LOGIN.CFG points to 51.15.15.123:12981 | 2020-04-26 to 2020-04-26 | unknown |
| `4.08/` | 8 | 74,971 | 4.08 | USA | 2004-04-12 to 2008-12-15 | https://archivedle.download.it/ftp1/042009/56439557/helbreathusa_setup_408.exe |
| `4.12.01/` | 8 | 67,672 | 4.12.01 | USA | 2009-03-16 to 2010-09-03 | https://web.archive.org/web/20110711161458id_/http://www.helbreathusa.com/downloadHB/Helbreath%20USA%20Install.zip |

Per-file sizes, SHA-256, dates and extraction chains are in `MANIFEST.json`.

## Manifest

`MANIFEST.json` has one row per file: path, size, SHA-256, version, region and era (each with a confidence: verified, inferred or unknown, and its basis), and every origin: source, exact URL, the file's own date and what kind of date it is, the day it was downloaded, and the extraction chain. The format is described in the [top README](../README.md#manifests).
