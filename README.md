# Helbreath History

A curated archive of the original **Helbreath** (Siementech, Seoul, 1999-2005) for players and preservationists:
the installers, patches, clients, art, historical source drops and documents that survive, sorted by version and
region, with where every file came from.

Helbreath was a 2D isometric online RPG of two warring nations, Aresden and Elvine. It ran in Korea (Siementech, later
Soft Family), as Helbreath International, in the USA (iEntertainment Network, from early 2003), in Japan, and in Taiwan
as 戰場 (Gamania, 2002). This repo is not a code project: nothing here is built, and nothing has been run.

> **Safety.** Every executable here is a 20-year-old binary kept as found. None of them has been run or scanned by
> this project. Treat them as untrusted: open them only in a disposable virtual machine.

## Layout

Files are grouped **by type**, then by **version** (`sprites/2.02/`, `sprites/3.0/`, `executables/3.81/`, ...). The original
install paths are kept in each file's manifest record (its extraction chain). A file is stored **once** per SHA-256, in the
version where it first appears; the record lists every other version it was found in (`also_in`). A version folder therefore
shows what that version added or changed. To get a playable folder tree instead, use the as-found client archives in the release.

| Folder | What |
|---|---|
| [`documents/`](documents/) | Start here: `timeline.md`, `version-history.md` (every version held, and what is missing), `domains.md`, and `shipped/` (manuals, release notes, rules shipped with the game). |
| [`executables/`](executables/) | Game clients, launchers, updaters, server binaries and DLLs; the installers as release assets. |
| [`sprites/`](sprites/) | `.pak` sprite files. |
| [`art/`](art/) | Every sheet of every pak, by version then pak: the bitmap as stored in the pak (byte for byte, as release archives) and its frame table as JSON (in git). |
| [`maps/`](maps/), [`sounds/`](sounds/), [`music/`](music/), [`fonts/`](fonts/) | Client game data. |
| [`configs/`](configs/) | `CONTENTS/` game text and tables, `LOGIN.CFG` server addresses, other text. |
| [`images/`](images/) | Installer artwork and palettes. |
| [`video/`](video/) | The 2001 Crusade trailer (release asset). |
| [`other/`](other/) | Anything else a client shipped (uninstaller data, updater list, SourceSafe files). |
| [`archives/`](archives/) | Original archives kept whole: official patches, historical source drops (2.03, 2.20, 3.51), 3.51 server files; disc image, as-found client trees and art archives (release assets). |
| [`community/`](community/) | **Not official.** Private-server community material: modern drops (2022 HBX client, rewrites, a web shop) and the community 3.82 bundle's server files and sources. |
| [`tools/`](tools/) | Third-party utilities the official sites offered. Listed and linked, not copied. |
| [`derived/`](derived/) | **Made by this project, not original.** Files derived from originals held here: the decrypted 2024 Korean sprite paks. |

Versions held: 2.02 "Crusade" (2001), 2.23 (2003), 3.0 "The Apocalypse" (2003), 3.1, 3.72, 3.80, 3.81 (2003-2005), a 2007
test-server client, USA 4.08 (2009) and 4.12.01 (2010), the 2002 Korean and Japanese launchers, sources 2.03, 2.19/2.20 and
3.51, the community 3.82 bundle (version folder `3.82-bundle`), and the 2024 Korean client from helbreath.com (version folder
`korea-2024`; its sprite paks and sounds are encrypted as shipped). See `documents/version-history.md`.

Each folder has a `README.md` (what it holds, which version, date, source URL, SHA-256) and a `MANIFEST.json`.

## Manifests

Every file in a folder, and every release asset belonging to it, has one record in that folder's `MANIFEST.json`
(`documents/shipped/` and each `art/<version>/` have their own). An `art` row also has `frames` (frame count) and
`bitmap` (the sheet's bitmap: file name, release archive, size, SHA-256, and `pak_offset` / `pak_length` inside its pak). A `derived` row also has `derived_from` (the original's path and SHA-256) and, when its bytes match a file already held, `identical_to`. `README.md` and `MANIFEST.json` themselves are not listed.

| Field | Meaning |
|---|---|
| `path` | Path relative to the folder, or the asset name for a release asset. |
| `stored` | `git` (in this repo), `release <repo>/<tag>` (a GitHub release asset; see below), or `git <repo> <path>` (kept in another repo). |
| `size`, `sha256` | Size in bytes and SHA-256 of the file exactly as stored. |
| `what` | What the file is. |
| `version`, `region`, `era` | The game version, the region or edition (Korea, International, USA, Japan, ...), and the era (Crusade, Apocalypse, ...) where known. Each is `{value, confidence, basis}`: `verified` (stated by the source, the file's name, a version string or the hosting page), `inferred` (worked out; `basis` says from what), or `unknown`. Taken from the first origin; each origin carries its own. |
| `also_in` | Other versions in which the same bytes were found. |
| `origins` | One entry per place the file was found, with the fields below. |
| `source` | Where it came from: official site, FilePlanet, forum, retail CD, and so on. |
| `url` | The exact download URL. Wayback captures are given as `https://web.archive.org/web/<timestamp>id_/<original URL>`. `unknown` when not recorded. |
| `documented` | The file's own date, and `documented_kind` says what that date is: `wayback-capture` (when the Wayback Machine saved it), `archive-entry` (newest entry date inside the archive), `installer-entry` (the date stored for the file in its installer), `host-listing` (the date the hosting site shows), `written` (this project's own documents), or `unknown`. 3.0 installer dates are decoded from an undocumented InstallShield field and say so in `notes`. |
| `downloaded` | The day this project downloaded it, from file-system dates and our download records. |
| `extracted_from` | The extraction chain from the downloaded file down to this one, outermost first, or `null` when the file is the download itself. |
| `notes` | Anything else, including what is unverified. |

Anything that could not be established is written as `unknown`, never guessed.

## Release assets (files over 100 MB)

Files over 100 MB are not in git; they are assets of this repo's own release `history-1`. History keeps its own copy
of every original download (except the 2024 Korean zip and installer; see `executables/README.md`): the disc images, installers and zips, the videos, and the per-version art archives. Each is
listed in the README and manifest of the folder it belongs to. Every original container is kept exactly once, and every
distinct file has one browsable copy. A container nested inside another kept container (the 2.02 installer inside the
retail ISO, `SPRITES.zip` inside the 4.12.01 install) is not stored a second time; its manifest row says `inside ...`
and how 7-Zip extracts it byte-exact.

To rebuild an installed game folder, use `documents/install-layouts/<version>.json` (2.02, 3.0, 4.08, 4.12.01, korea-2024). It
lists every path the installer wrote, with size, SHA-256, and where its bytes are kept in this repo. Each origin in the
manifests also carries `install_path`.

## Where it came from

Nothing here was made by this project except the READMEs, the manifests, the three documents in `documents/`, the
frame-table JSON files in `art/` (extracted metadata), the release archives it repacked (as-found client trees and art), and everything under `derived/` (the decrypted 2024 Korean sprite paks).
The 4.08 install was unpacked with a standard-library Inno Setup reader written for this archive; every file matched the MD5
the installer stores. The 2024 Korean NSIS installer was unpacked with 7-Zip 26.00; its zip and installer are not held.
`.gitattributes` turns off line-ending conversion, so every file checks out byte-for-byte as found. The downloads themselves are kept
untouched in [Downloads-Archive](https://github.com/Original-Helbreath/Downloads-Archive); the research behind every
date is in [2.20-Documentation](https://github.com/Original-Helbreath/2.20-Documentation) `research/`.

## Project

Part of [Original Helbreath](https://github.com/Original-Helbreath): keeping the original 1999-2005 Siementech Helbreath alive.
Issues are tracked on the [project board](https://github.com/orgs/Original-Helbreath/projects/1).
Helbreath is the property of its rights holders; this archive is kept for preservation.
