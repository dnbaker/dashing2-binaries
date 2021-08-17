## Dashing2 Binaries

To separate code from external data, we are providing statically-built binaries for Dashing2.
These are kept in `osx/` and `linux/` directories, within which they are grouped by release.

For each of these, there are versions for SSE2, AVX, AVX2, AVX512F, and AVX512BW.

For Intel CPUs, simply select the version compiled for your hardware.
This is likely AVX2 `_savx2`, and almost certainly SSE2 `_s128`.

## Status

v2.0.4 - present for both linux and osx. See `linux/` and `/osx` folders for specific versions.

We will update this with a list of statically-compiled binaries as development continues.
