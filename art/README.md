# art: Sprite previews

PNG previews of notable sprite sheets, grouped by subject, decoded from the original paks without any change (no colour-key edits). Paks with many sheets (a monster has 40: 5 actions by 8 directions) are sampled: every 8th sheet, so one direction per action. Each row says which version the pak comes from. Crusade-era art is under `crusade/`. No Heldenian-era art is held: no client after 3.0 has been unpacked.

## By version

| Version folder | Files | Size (bytes) | Version | Region | File dates | Source |
|---|---|---|---|---|---|---|
| `characters/` | 112 | 4,302,062 | 2.02 | International (English) | 1999-05-14 to 2003-03-06 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso; https://web.archive.org/web/20141104104043id_/http://www.helbreathusa.com/patch_v223.zip |
| `crusade/` | 41 | 2,203,859 | 2.02 | International (English) | 2001-05-23 to 2001-07-16 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso |
| `interface/` | 20 | 3,674,322 | 2.23 | USA | 2001-07-22 to 2003-03-12 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso; https://web.archive.org/web/20141104104043id_/http://www.helbreathusa.com/patch_v223.zip |
| `items/` | 13 | 870,162 | 2.02 | International (English) | 2001-04-02 to 2001-05-08 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso |
| `monsters/` | 70 | 2,690,924 | 2.02 | International (English) | 1999-03-06 to 2001-07-14 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso |
| `npcs/` | 58 | 930,213 | 2.02 | International (English) | 1999-06-28 to 2001-07-21 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso |
| `world/` | 31 | 6,483,282 | 2.02 | International (English) | 1999-07-09 to 2003-03-06 | https://archive.org/download/helbreath-the_crusade-2001/HelbreatH.iso; https://web.archive.org/web/20141104104043id_/http://www.helbreathusa.com/patch_v223.zip |

Per-file sizes, SHA-256, dates and extraction chains are in `MANIFEST.json`.

## Manifest

`MANIFEST.json` has one row per file: path, size, SHA-256, version, region and era (each with a confidence: verified, inferred or unknown, and its basis), and every origin: source, exact URL, the file's own date and what kind of date it is, the day it was downloaded, and the extraction chain. The format is described in the [top README](../README.md#manifests).
