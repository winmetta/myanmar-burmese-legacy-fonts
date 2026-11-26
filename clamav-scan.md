# ClamAV scan result

One-time malware scan of this repository after the cleanup (executables,
installers, profiles and archives removed, see [README.md](README.md)).

| Item       | Value                                                           |
| ---------- | --------------------------------------------------------------- |
| Result     | **0 infected files**                                            |
| Scanned    | 926 files in 21 directories (390 MiB after unpacking)           |
| Date       | 2026-11-26 22:35 UTC                                            |
| Tool       | ClamAV 1.5.5 (`brew install clamav`)                            |
| Signatures | main 63, daily 28194, bytecode 339 (3,628,228 known signatures) |
| Excluded   | `.git/` only                                                    |

Command, run from the repository root:

```bash
clamscan -r --exclude-dir='\.git' --max-filesize=200M --max-scansize=1G .
```

The full per-file output, as printed by `clamscan`, is in
[`clamav-scan-output.txt`](clamav-scan-output.txt).

ClamAV only detects known threats. A clean result means no known malware
signature matched, not that the files are guaranteed safe. Repeat the scan
after adding new sources, because signatures change daily.
