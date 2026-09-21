# Oracle Perps — preprod preview

Static preview build of the `feat/ten-changes` branch of
[organizdgeneral/perps-oracle](https://github.com/organizdgeneral/perps-oracle),
served for review only.

It runs the **frontend changes only**, pointed at the live production API at
`https://oracleperps.com/api`. The backend changes in the same branch are not
running here: judge those from the PR diff and the benchmark in it.

Because production does not yet serve `/api/stream`, the change-signal
subscription 404s and the tape falls back to its timer. That is the intended
degradation path, not a bug.

Not affiliated with, or a replacement for, oracleperps.com.
