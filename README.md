## Dashing2 Binaries

To separate code from external data, we are providing statically-built binaries for Dashing2.
These are kept in `osx/` and `linux/` directories, within which they are grouped by release.

For each of these, there are versions for SSE2, AVX, AVX2, AVX512F, and AVX512BW.

For Intel CPUs, simply select the version compiled for your hardware.
This is likely AVX2 `_savx2`, and almost certainly SSE2 `_s128`.

## Status

v2.0.4 - First 2.0 version.
v2.1.0 - First 2.1 version. We recommend v2.1.1
v2.1.1 - OSX available, Linux in process

We will continue to update this with a list of statically-compiled binaries.
