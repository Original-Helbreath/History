# executables: Programs and libraries

Every `.exe` and `.dll`: game clients (`HelGame.exe`, `NewHelGame.exe`), launchers and updaters (`Helbreath.exe`), helper DLLs, and the installers (release assets). **Never run any of them outside a disposable virtual machine.**

The 2024 Korean client (`korea-2024/`) came from helbreath.com as `Helbreath_setup_win10_20240927.zip` (472,855,926 bytes, SHA-256 `cb4adad63317432b83b5d10252776907a093311b1c0bc36befc3af3b2dc2d42c`), holding the installer `Helbreath_setup_win10.exe` (NSIS-3 Unicode, 473,199,768 bytes, SHA-256 `ac3a3094993fb8f7b23f8e2f7f975e380db22826e5db6ed083688ea17c5a31f0`). Neither is held in History or as a release asset; their contents were unpacked with 7-Zip 26.00 into the type folders. The installer's PE header date (2021-09-25) is that of the NSIS stub, not of the package.

## Files

| File | Version | Region | Date | Size (bytes) | SHA-256 | Stored |
|---|---|---|---|---|---|---|
| `2.02/Helbreath.exe` | 2.02 | International (English) | 2001-08-21 (installer-entry) | 282,624 | `31356536fa16ee03960e3596ada0a7bfd8a3a8d91344d7aa65d849b4369b0049` | git |
| `2.02/HelGame.exe` | 2.02 | International (English) | 2001-08-21 (installer-entry) | 692,224 | `c9cdd7f76678ecfc489bbcd2c213770d730b3f46b7d6d77a9aeefb29329de2a1` | git |
| `2.02/search.dll` | 2.02 | International (English) | 2001-06-11 (installer-entry) | 143,360 | `af86c041e0d663bc455826e3e15d4377b52a1304348874ef354df9ed8ad8bc22` | git |
| `2.02/Uninstal.exe` | 2.02 | International (English) | unknown | 49,723 | `e2ec88816d8f80c7edc5ef105f9320ecd3022b89d3e5e665d916458a53c833f4` | git |
| `2.02/zlib.dll` | 2.02 | International (English) | 2000-07-03 (installer-entry) | 73,728 | `cf484e35a28e62e206767ef7371066166131abfde254305e7b3e7197ad1a08a3` | git |
| `2.23/HelGame.exe` | 2.23 | USA | 2003-04-15 (archive-entry) | 302,592 | `d98018f475c1093a965507b0c219d5aae08a9c2a4168639cc9a4545d6dc6f55f` | git |
| `2001-beta/Helbreath.exe` | pre-2.02 'Helbreath Beta' (built 2001-05-08) | USA | 2001-05-08 (installer-entry) | 282,624 | `1bc47731b160a4edbd3eaf3b97a8107f9915477f6390391d026eb7f1c9fe5b74` | git |
| `2001-beta/HelGame.exe` | pre-2.02 'Helbreath Beta' (built 2001-05-08) | USA | 2001-05-08 (installer-entry) | 638,976 | `d321e245b72536413d7fa40ef9ba35ab3d5771bf4e193ffa43959deba11df9d2` | git |
| `2001-beta/search.dll` | pre-2.02 'Helbreath Beta' (built 2001-05-08) | USA | 2001-04-10 (installer-entry) | 1,364,016 | `e19c2e7707ffb5691cb6eba73d935e0df5415ab97b23deab3ad17c67d67f50ea` | git |
| `2001-beta/Uninstal.exe` | pre-2.02 'Helbreath Beta' (built 2001-05-08) | USA | unknown | 49,681 | `2a3f140fe0aecbb46d6c5f82e35a6841ff4921cb436e20e1a74a4d194320fad6` | git |
| `3.0/cximage.dll` | 3.0 'The Apocalypse' | USA | 2003-06-12 (installer-entry) | 159,744 | `53aef3609bb800ff72ce5ae3cfcad2d1ee68e84f7b275926a0aacb87984c5b77` | git |
| `3.0/Helbreath.exe` | 3.0 'The Apocalypse' | USA | 2003-11-11 (installer-entry) | 495,704 | `13c6419ec195659321d3b9ed5a24a3d6657caf68c4e78ddd108c963792e516fc` | git |
| `3.0/NewHelGame.exe` | 3.0 'The Apocalypse' | USA | 2003-11-11 (installer-entry) | 320,000 | `4f2c91c2dd6715804250716e43a1c2b9dec69e7d56c1f1606dac2e85e881b58c` | git |
| `3.0/search.dll` | 3.0 'The Apocalypse' | USA | 2002-10-18 (installer-entry) | 135,168 | `42cae5fd3bdc359a3bb81316066100afe7d767d276472291c05614119f8c4d13` | git |
| `3.1/HelGame.exe` | 3.1 | USA | 2003-11-28 (archive-entry) | 318,976 | `642029013799f6a57dc776a9f1cd8a36c6faae95007fba91e22515f734b1613d` | git |
| `3.72/HelGame.exe` | 3.72 'Winter' | USA | 2004-12-17 (archive-entry) | 444,416 | `06fe71b7806c3a8cdf11a56b9a9bcff46d76fa7633755e36370b5f9bf3fbe9ed` | git |
| `3.80/HelGame.exe` | 3.80 'Wish Ball' | USA | 2005-02-23 (archive-entry) | 444,928 | `4db2a894b7422af42844f36bcd77eba27a94da2823f474f0d4e76e6dc5bbe783` | git |
| `3.81/HelGame.exe` | 3.81 | USA | 2005-07-22 (archive-entry) | 436,224 | `9b7fe97f7274f68839a362431c2d527d36f650cd5c1a2bd357fd092f230d695e` | git |
| `3.82-bundle/GateServer.exe` | 3.82 community bundle (helbreath-v3.82, GitHub zip of 2020-04-26) | community private server; its LOGIN.CFG points to 51.15.15.123:12981 | 2020-04-26 (archive-entry) | 86,016 | `6a4a540e5c798063e539e38a8a29b27420273478972dcb0e5dc5fef59621e471` | git |
| `3.82-bundle/Helbreath.exe` | 3.82 community bundle (helbreath-v3.82, GitHub zip of 2020-04-26) | community private server; its LOGIN.CFG points to 51.15.15.123:12981 | 2020-04-26 (archive-entry) | 321,536 | `51071bf5524720b33a835dc6424d718f60276c98a7b263f17bd2be05be45f065` | git |
| `3.82-bundle/MainServer.exe` | official Main Log / World Log server, 2.19/2.20 era | unknown | 2020-04-26 (archive-entry) | 393,216 | `9e79b5fdda12a0fe07d1e2a3d2fc4863ad2681feb50aaa55869e33ce70ee2a24` | git |
| `3.82-bundle/WorldServer.exe` | official Main Log / World Log server, 2.19/2.20 era | unknown | 2020-04-26 (archive-entry) | 106,496 | `1cf95991524081ece784ebb5d8ee6741ad60ca2bc9b9b1631d67c0fcb683082d` | git |
| `4.08/Helbreath.exe` | 4.08 | USA | 2007-06-16 (installer-entry) | 495,704 | `6b6f71c0ac0121e1582d9446eca32c2233904d77ca6367caf899928c62b2d027` | git |
| `4.08/Helgame.exe` | 4.08 | USA | 2008-12-14 (installer-entry) | 420,864 | `139f816eddd643345704bf5733c3a2d39c82b3608afe1fa7b1608bb099da0c30` | git |
| `4.12.01/Helgame.exe` | 4.12.01 | USA | 2010-04-23 (archive-entry) | 412,672 | `d5c0a6e5f9c45b6ddb2f9f1ca7038a98458ae9a6715cf275fb1e52119e59ac34` | git |
| `4.12.01/unins000.exe` | 4.12.01 | USA | 2008-12-31 (archive-entry) | 695,578 | `880c830bcd1e792c89bb5bf963cd42dd868b6d6031b86c613268e934931509fd` | git |
| `korea-2024/CryptoDLL.dll` | Korea 2024-09-27 client (no version number stated) | Korea | 2008-12-31 (installer-entry) | 282,624 | `42a40d3a650e156b39e266563dad9036514fb07e43d630e28709ef8cc4b2233a` | git |
| `korea-2024/Helbreath.exe` | Korea 2024-09-27 client (no version number stated) | Korea | 2024-09-27 (installer-entry) | 1,895,832 | `a7f6bb54c34855f206fd0e054ba5c6e57d921885c1c2819572d2797ae8d3969d` | git |
| `korea-2024/HelGame.exe` | Korea 2024-09-27 client (no version number stated) | Korea | 2024-09-27 (installer-entry) | 1,179,136 | `f0d85632a1ddb503d1abde50a2d4a5774d349d92b17570c8b29fad86c351a432` | git |
| `korea-2024/mfc90u.dll` | Korea 2024-09-27 client (no version number stated) | Korea | 2007-11-07 (installer-entry) | 1,162,744 | `e30aabb518361fbeaf8068ffc786845ee84abbf1f71ae7d2733a11286531595a` | git |
| `korea-2024/msvcp100.dll` | Korea 2024-09-27 client (no version number stated) | Korea | 2013-10-01 (installer-entry) | 431,936 | `972fd609d31aded22502a01c3ee1f3e23f5769392c7ca3c36a402dc7c44e0af8` | git |
| `korea-2024/msvcr100.dll` | Korea 2024-09-27 client (no version number stated) | Korea | 2013-10-01 (installer-entry) | 758,592 | `43af6d081b5ded0bd3b1b269719b3a63400da25a805d46d579c4dd2a77861ba1` | git |
| `korea-2024/msvcr90.dll` | Korea 2024-09-27 client (no version number stated) | Korea | 2007-11-07 (installer-entry) | 655,872 | `ed0170d3de86da33e02bfa1605eec8ff6010583481b1c530843867c1939d2185` | git |
| `korea-2024/uninstall.exe` | Korea 2024-09-27 client (no version number stated) | Korea | 2024-05-27 (installer-entry) | 41,004 | `bb5970a487ca5a38cb08bb2a8231868223f5b3d21e33b8e4b5c82297dbe05489` | git |
| `launcher-japan-2002/Helbreath.exe` | unknown | Japan | 2002-10-31 (wayback-capture) | 303,104 | `6e0121311ef9b6a53d14b78c39761dfa88c705095bac1a6c6418b43ad3a45f15` | git |
| `launcher-korea-2002/Helbreath.exe` | unknown | Korea | 2002-04-13 (wayback-capture) | 307,200 | `7f29e6afc37f9bd032187753c417e31d8ce3897553eda3f2df24f1e6148576f8` | git |
| `test-server-2007/HelGame.exe` | unknown | USA test server | 2007-05-30 (archive-entry) | 394,752 | `bd35ac76bb053cc31c0b7d2ddaecde6de7f1ad6c0a222736ec6403e739786c6b` | git |

## Not in git

Over 100 MB, or kept elsewhere; download from the link given.

| File | Version | Region | Date | Size (bytes) | SHA-256 | Stored |
|---|---|---|---|---|---|---|
| `Hb202full_ENG.exe` | 2.02 | International (English) | 2001-08-21 (installer-entry) | 211,830,945 | `6f5c3ecda251e85c84ad89b9c06bef24b32f01f060c53ea483762c6aaa52d9a2` | inside history-1 HelbreatH.iso (Hb202full_ENG.exe at the disc root) |
| `hbusa_apocalypse.exe` | 3.0 'The Apocalypse' | USA | 2003-11-14 (host-listing) | 241,288,011 | `46530f11079f28234da1b64bbbcea17370542986778da809c1b55f8bdf62be15` | release: Original-Helbreath/History/history-1 |
| `helbreathusa_setup_408.exe` | 4.08 | USA | 2009-04-30 (host-listing) | 214,673,897 | `923991c374ac25f2fac7f9e482cc61aa188421d8ebc6447e9664efa8f0ca3093` | release: Original-Helbreath/History/history-1 |
| `usa-2001-setup.exe` | pre-2.02 'Helbreath Beta' (built 2001-05-08) | USA | 2001-05-08 (iso-entry) | 157,269,112 | `2915984ce2a7bc7b9b49e73dc12e5c06daa3ba38df73f617fe87120913545a0f` | release: Original-Helbreath/History/history-1 |

- `Hb202full_ENG.exe`: The installer format is Siementech's own; 7-Zip cannot open it. Not a separate release asset: 7-Zip extracts it from HelbreatH.iso byte-exact (SHA-256 checked 2026-10-27).
- `hbusa_apocalypse.exe`: MD5 81431f5c33f98b153ad6fc43b89292b5 matched FilePlanet.
- `helbreathusa_setup_408.exe`: Inno Setup 5.2.3; unpacked into the type folders as version 4.08 with inno5.py (all 728 files matched the installer MD5s). MD5 8839990c498bcd9944ce486d3036eec3 matched FilePlanet.

## Manifest

`MANIFEST.json` has one row per file: path, size, SHA-256, version, region and era (each with a confidence: verified, inferred or unknown, and its basis), and every origin: source, exact URL, the file's own date and what kind of date it is, the day it was downloaded, and the extraction chain. The format is described in the [top README](../README.md#manifests).
