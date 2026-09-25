# Oracle Perps — preprod preview

Static preview of `feat/ten-changes` from
[organizdgeneral/perps-oracle](https://github.com/organizdgeneral/perps-oracle)
(PR #5), served for review only.

**Built from `c436f4d`, merged up to main @ `ecda1f9`, 26 Sep 2026.**

Frontend only, pointed at the live production API at `https://oracleperps.com/api`.
The backend changes in the same branch are not running here: judge those from
the PR diff.

Because production does not yet serve `/api/stream`, the change-signal
subscription 404s and the tape falls back to its timer. That is the intended
degradation path, not a bug.

Not affiliated with, or a replacement for, oracleperps.com.
