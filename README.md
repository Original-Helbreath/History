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

| Folder | What | Versions |
|---|---|---|
| [`installers/`](installers/) | Official full installers and web launchers, by version and region. The large ones are release assets. | 2.02 (2001), Korea/Japan launchers (2002), USA 3.0 (2003), USA 4.08 (2009), USA full install (2011 capture) |
| [`patches/`](patches/) | Official patches in version order, as the official sites served them. | 2.23 (2003) to 3.81 (2005), test server (2007) |
| [`clients/`](clients/) | As-found client installs: what an installed game folder held, per version. The full trees are release archives; the folder keeps listings and the small config files. | 2.02, 3.0 |
| [`art/`](art/) | Preview PNGs of notable sprite sheets, by subject, with the version each first appears in. | 2.02, 2.23 |
| [`sources/`](sources/) | Historical source and server-file drops, as the original archives. | 2.03, 2.20, 3.51 |
| [`tools/`](tools/) | Period utilities the official sites offered (DirectX, unzip tools). Listed and linked, not copied. | 2001-2006 |
| [`documents/`](documents/) | Timeline, version history, official domains, and the game's own manuals. | 1999-2005 |

Each folder has a `README.md` (what it holds, which version, date, source URL, SHA-256) and a `MANIFEST.json`.

## Manifests

Every file in a folder, and every release asset belonging to it, has one record in that folder's `MANIFEST.json`.
`README.md` and `MANIFEST.json` themselves are this project's own writing and are not listed.

| Field | Meaning |
|---|---|
| `path` | Path relative to the folder, or the asset name for a release asset. |
| `stored` | `git` (in this repo), or `release <repo>/<tag>` (a GitHub release asset; see below). |
| `size`, `sha256` | Size in bytes and SHA-256 of the file exactly as stored. |
| `what` | What the file is. |
| `source` | Where it came from: official site, FilePlanet, forum, retail CD, and so on. |
| `url` | The exact download URL. Wayback captures are given as `https://web.archive.org/web/<timestamp>id_/<original URL>`. `unknown` when not recorded. |
| `documented` | The file's own date, and `documented_kind` says what that date is: `wayback-capture` (when the Wayback Machine saved it), `archive-entry` (newest entry date inside the archive), `installer-entry` (the date stored for the file in its installer), `document-property` (the date saved in the document), `host-listing` (the date the hosting site shows), or `unknown`. |
| `downloaded` | The day this project downloaded it, from file-system dates and our download records. |
| `extracted_from` | The extraction chain from the downloaded file down to this one, outermost first, or `null` when the file is the download itself. |
| `notes` | Anything else, including what is unverified. |

Anything that could not be established is written as `unknown`, never guessed.

## Release assets (files over 100 MB)

Files over 100 MB are not in git. The originals are already release assets of
[Downloads-Archive](https://github.com/Original-Helbreath/Downloads-Archive/releases/tag/originals) and are linked
rather than duplicated. Files that only this repo offers (the 2.02 installer and trailer taken off the retail CD,
and ready-made as-found client archives) are assets of this repo's own release `history-1`. Each is listed in the
README and manifest of the folder it belongs to.

## Where it came from

Nothing here was made by this project except the READMEs, the manifests, the documents in `documents/` and the
preview PNGs in `art/` (decoded from the original `.pak` files without changes). The downloads themselves are kept
untouched in [Downloads-Archive](https://github.com/Original-Helbreath/Downloads-Archive); the research behind every
date is in [2.20-Documentation](https://github.com/Original-Helbreath/2.20-Documentation) `research/`.

## Project

Part of [Original Helbreath](https://github.com/Original-Helbreath): keeping the original 1999-2005 Siementech Helbreath alive.
Issues are tracked on the [project board](https://github.com/orgs/Original-Helbreath/projects/1).
Helbreath is the property of its rights holders; this archive is kept for preservation.
