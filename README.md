## Dashing2 Binaries

To separate code from external data, we are providing statically-built binaries for Dashing2.
These are kept in `osx/` and `linux/` directories, within which they are grouped by release.

For each of these, there are versions for SSE2, AVX, AVX2, AVX512F, and AVX512BW.

For Intel CPUs, simply select the version compiled for your hardware.
This is commonly AVX2 `_savx2`, and almost certainly SSE2 `_s128`.
Recent hardware with AVX512F and AVX512, such as Knight's Landing, Sky Lake, or Coffee Lake, use newer vectorized operations where available.
To fully benefit from these, you would use `dashing2_s512` or `dashing2_s512bw`.

## Status

v2.0.4 - First 2.0 version. OSX + Linux.
v2.1.0 - First 2.1 version. OSX + Linux
v2.1.1 - OSX + Linux
v2.1.2 - Bug fix release, skipped in favor of 2.1.3
v2.1.3 - OSX + Linux, improved memory management
v2.1.5 - Linux + Linux; OSX in process. Faster formatting, better hashing, and differently-parallelized linear-time clustering.


We will continue to update this with a list of statically-compiled binaries.
