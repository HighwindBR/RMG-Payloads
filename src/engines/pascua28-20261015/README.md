# TraceFS engine snapshot for S926BXXUHEZIF

This directory contains the native engine sources imported without edits from
[`pascua28/Root-My-Galaxy-Payloads`](https://github.com/pascua28/Root-My-Galaxy-Payloads),
at commit [`1ef1ed475dd7b9822a00b0cfbd07baa4b04b12b0`](https://github.com/pascua28/Root-My-Galaxy-Payloads/commit/1ef1ed475dd7b9822a00b0cfbd07baa4b04b12b0)
(October 15, 2026). The original repository is Apache-2.0 licensed.

The root `Makefile` selects these files only for
`TARGET=e2s-S926BXXUHEZIF`, including the TraceFS KASLR discovery
implementation in `slide_app.c` and its accompanying native dependencies.
Other targets continue to compile from the original `src/` files.

This source snapshot **does not change** the existing DZDR/DZG1 artifacts,
and does not itself establish that the distributed UHEZIF binary can be
reproduced byte-for-byte. Device testing and a reproducible Android NDK build
remain separate validation steps.

Do not modify the legacy engine as part of UHEZIF-only work without
revalidating the existing firmware profiles.
