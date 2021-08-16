## Dashing2 Binaries

To separate code from external data, we are providing statically-built binaries for Dashing2.
These are kept in `osx/` and `linux/` directories, within which they are grouped by release.

For each of these, there are versions for SSE2, AVX, AVX2, AVX512F, and AVX512BW.

For Intel CPUs, simply select the version compiled for your hardware.
This is likely AVX2 `_savx2`, and almost certainly SSE2 `_s128`.

## Status

Binaries are only available for OSX currently; we hope to have this addressed in the next few days.
