# community: Community and private-server material (not official)

Material made or changed by the Helbreath private-server community, kept apart from the official files and labelled as such. `archives/`: four modern drops as downloaded (the 2022 HBX client source, a 2022 C++ client rewrite, a 2022 Vue web UI, and a 2015 web shop called helbreathusa). `3.82-bundle/`: everything from the community helbreath-v3.82 bundle (a 2020 GitHub zip) other than its client files and server binaries: game-server configs and maps, docs, tools and 3.82 sources, in their original tree. `models/`: fan-made 3D models of the Aresden and Elvine town crests (binary STL files dated 2021-10-05, as supplied), each also converted to GLB (glTF 2.0, metres, Y-up) and OBJ (mm, as in the STL) so common 3D tools can open them. The bundle's client files and its official `MainServer.exe` / `WorldServer.exe` are in the type folders under version `3.82-bundle`; a file identical to an official build is stored once, under the official version.

## By version

| Version folder | Files | Size (bytes) | Version | Region | File dates | Source |
|---|---|---|---|---|---|---|
| `3.82-bundle/` | 478 | 18,400,941 | 3.82 community bundle (helbreath-v3.82, GitHub zip of 2020-04-26) | community private server; its LOGIN.CFG points to 51.15.15.123:12981 | 2020-04-26 to 2020-04-26 | unknown |
| `archives/` | 4 | 26,087,502 | modern C++/vcpkg client rewrite (2022) | community | 2015-02-11 to 2022-12-21 | https://forum.helbreathx.net/files/file/11-clients-sources-helbreath/ (file page; the download link needs a forum login); https://forum.helbreathx.net/files/file/9-helbreathusazip-206-mb/ (file page; the download link needs a forum login) |

Per-file sizes, SHA-256, dates and extraction chains are in `MANIFEST.json`.

## Manifest

`MANIFEST.json` has one row per file: path, size, SHA-256, version, region and era (each with a confidence: verified, inferred or unknown, and its basis), and every origin: source, exact URL, the file's own date and what kind of date it is, the day it was downloaded, and the extraction chain. The format is described in the [top README](../README.md#manifests).
