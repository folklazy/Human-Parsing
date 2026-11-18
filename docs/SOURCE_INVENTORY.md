# Source inventory and evidence audit

**Status: CANDIDATE SOURCES ONLY.** No claim of file-level inspection or release selection is made by creating this document.

## Known related repositories

- [Human Parsing Study](https://github.com/folklazy/Human_Parsing_Study)
- [Human Parsing CCTV600 Benchmark](https://github.com/folklazy/Human_Parsing_CCTV600_Benchmark)

## Required inventory table

| Source repository / SSH path | Branch / commit SHA | Key file / directory | Type | Keep? | Why | Evidence / hash | Permission |
|---|---|---|---|---|---|---|---|
| TO_AUDIT | NOT_VERIFIED | NOT_VERIFIED | code / benchmark / weight / dataset / demo / obsolete | TBD | TBD | TBD | TBD |

Types: shipping source; canonical research evidence; derived report; debug/temporary; unused experiment; restricted data; secret.

## Review checklist

1. Inspect the **real** VS Code/SSH workspace as well as GitHub; a file may exist only locally.
2. Run `git status`, inspect branches/commits and repository AGENTS instructions before copying.
3. Identify which code/config the final working app uses; require a code path or execution log.
4. Record filenames and hashes for curated files and reference original proof.
5. Keep non-shipping evidence in original archives, and list it here rather than mirroring huge folders.
6. Run focused regression/smoke checks after any migration and report observed results.
7. Explicitly flag restricted or unlicensed material and request owner decision rather than guessing.
