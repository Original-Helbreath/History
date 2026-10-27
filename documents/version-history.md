# Versions held in this archive

One row per version, oldest first. Dates are the files' own (see `timeline.md` for what each kind of date means).
"Folder" is the version subfolder used inside every type folder (`sprites/3.0/`, `executables/3.81/`, ...).

| Version | Region / edition | Date | What survives | Folder | Source |
|---|---|---|---|---|---|
| 2.02 "Crusade" | International (English); inferred from the installer name `_ENG` and the 2001 date | 2001-08-21 | Full retail install (439 files) and trailer | `2.02` | 2001 retail CD, archive.org |
| 2.03 | not stated | 2001-08-31 | Game server source and build | `archives/sources/server-2.03` | SourceForge hb-online |
| launcher, 2002 | Korea | captured 2002-04-13 | `Helbreath.exe` from helbreath.com | `launcher-korea-2002` | Wayback |
| launcher, 2002 | Japan | captured 2002-10-31 | `Helbreath.exe` from helbreath.com/japan | `launcher-japan-2002` | Wayback |
| 2.19 / 2.20 | all regions, chosen at build time | about Feb-Mar 2003 (inferred) | Client, game server and gate server source | `archives/sources/` | forum and librehelbreath imports |
| 2.23 | USA | 2002-12-21 to 2003-04-16 | Incremental patch: 60 files, mostly sprites | `2.23` | Wayback, helbreathusa.com |
| 3.0 "The Apocalypse" | USA | 2003-11-14 | Full install (694 files as extracted) | `3.0` | FilePlanet |
| 3.1 | USA | 2003-12-01 | Patch: `GameDialog.pak` and `HelGame.exe` | `3.1` | Wayback |
| 3.51 | China, inferred from the forum post | 2005-01-07 | Server binary, map data, configuration, SQL; client source | `archives/server-files/3.51`, `archives/sources/client-3.51` | Outpost forum |
| 3.72 "Winter" | USA | 2004-12-17 | Update from 3.7 | `3.72` | Wayback |
| 3.80 "Wish Ball" | USA | 2005-02-23 | Update: `HelGame.exe` | `3.80` | Wayback |
| 3.81 | USA | 2005-07-22 | Update from 3.72 | `3.81` | Wayback |
| test server | USA | 2007-05-30 | `HelGame.exe` | `test-server-2007` | Wayback |
| 4.08 | USA | 2009-04-30 (FilePlanet); file times to 2009 | Full install (728 files; Inno Setup 5.2.3, unpacked with a stdlib extractor, every file MD5-checked) and release notes back to earlier 4.0x | `4.08` | FilePlanet |
| 4.12.01 | USA | zip entry 2010-09-19, captured 2011-07-11 | Full install (734 files; WinRAR self-extractor) with release notes, plus the shipped `SPRITES.zip` | `4.12.01` | Wayback |
| 3.82 community bundle | community private server (`LOGIN.CFG` 51.15.15.123) | zip entries 2020-04-26 | Client data, official Main/World Log binaries (2002), community server files and sources | `3.82-bundle`, `community/3.82-bundle` | community forum |

Missing: every patch between 2.02 and 2.23 (2.03 to 2.22) and between 3.1 and 3.7, and any Korean, Japanese or
Taiwanese full client. The 2.20 client source loads 48 sprite paks that neither 2.02 nor 2.23 provides; most of
them appear in 3.0 (`sprites/3.0/`): 47 of the 48, every one except `feedback.pak`. That suggests they were added
by the missing 2.x patches (inferred).
