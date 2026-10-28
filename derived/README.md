# derived: Made by this project

**Nothing in this folder is an original file.** It holds files this project derived from originals held elsewhere in History, kept so they can be used without redoing the work. Each row in `MANIFEST.json` names the original it was made from (`derived_from`: its path and SHA-256), and the original stays in its type folder untouched.

## By version

| Folder | Rows | Stored here | Size stored (bytes) | Made from | Made |
|---|---|---|---|---|---|
| `sprites/korea-2024/` | 405 | 225 | 608,508,322 | the 405 encrypted paks in `sprites/korea-2024/` | 2026-10-28 |

## sprites/korea-2024: decrypted Korean sprite paks

The Korea 2024-09-27 client ships its sprite paks encrypted. These are the same paks decrypted into the plain 1999 PAK format that [PAKLib](https://github.com/shadowevil/PAKLib) reads, one per encrypted pak and under the same name.

- Decryption: XOR with the repeating key `4c b2 3e 1a` from offset 20, the key restarting at each sprite; within a sprite, the 100-byte header, the frame table and the bitmap are each running-XORed (`byte[i] ^= byte[i-4]`, restarting per region), except the frame count and the colour-key field.
- Restored bytes: BMP header bytes 12-17, a lost `BM` signature in some paks, and the last 2 bytes of 4-aligned bitmaps set to `00 00`. The last is inferred: every 1999 4-aligned bitmap (9,675 of them) has `00 00` there.
- 180 of the 405 decrypted paks are byte-identical (SHA-256) to paks already held as found: 162 from 3.0, 13 from 4.08 and 5 from 2.23. They are not stored a second time: their rows say `stored: git Original-Helbreath/History <path>` and `identical_to`. The other 225 are stored here.
- Checks reported by the decrypting agent (not repeated in this commit): all 405 parse, every bitmap's `bfSize` equals its length, and the 250 paks shared with 1999 have identical frame tables for 9,165 of 9,168 sprites. The 180 identical SHA-256 matches were checked in this commit.
- No file is over 100 MB (the largest is 43,141,384 bytes), so nothing here is a release asset.

## Manifest

`MANIFEST.json` has one row per derived file, in the format described in the [top README](../README.md#manifests), plus `derived_from` (the original's path and SHA-256) and, where the result matches a file already held, `identical_to`. Version, region and era are those of the original. The origin is this project (`documented_kind`: `written`).
