## Dashing2 Binaries

To separate code from external data, we are providing statically-built binaries for Dashing2.
These are kept in `osx/` and `linux/` directories, within which they are grouped by release.

For each of these, there are versions for SSE2, AVX, AVX2, AVX512F, and AVX512BW.

For Intel CPUs, simply select the version compiled for your hardware.
This is commonly AVX2 `_savx2`, and almost certainly SSE2 `_s128`.
Recent hardware with AVX512F and AVX512, such as Knight's Landing, Sky Lake, or Coffee Lake, use newer vectorized operations where available.
To fully benefit from these, you would use `dashing2_s512` (for KNL) or `dashing2_s512bw` (for Skylake/CoffeeLake).

We will continue to update this with a list of statically-compiled binaries.

## Status

v2.0.4 - First 2.0 version. OSX + Linux.
v2.1.0 - First 2.1 version. OSX + Linux
v2.1.1 - OSX + Linux
v2.1.2 - Bug fix release, skipped in favor of 2.1.3
v2.1.3 - OSX + Linux, improved memory management
v2.1.5 - OSX + Linux. Faster formatting, better hashing, and differently-parallelized linear-time clustering.
v2.1.6 - OSX + Linux. Corrections/speedups to KNN/similarity-thresholded graph generation.
v2.1.7 - OSX + Linux. Add fasta-output for --parse-by-seq deduplication (--greedy).
v2.1.8 - OSX + Linux. Add support for direct sketching in SetSketch with pre-selected parameters. (via --setsketch-ab \<a,b\> --fastcmp \<nb\>, or --fastcmp-{bytes,shorts,words,nibbles})
v2.1.13 - OSX + Linux. Bug fixes and update hash map.
v2.1.14 - OSX + Linux. Bug fixes!
v2.1.15 - OSX + Linux. Bug fixes!
v2.1.16 - OSX + Linux. Bug fixes, small clean ups. Bump to c++20.
v2.1.17 - OSX + Linux. Bug fix: --parse-by-seq with packed truncated registers.


### Notes

Warning: v2.1.14 has a known performance regression with erroneous logging. We highly recommend avoiding it. v2.1.15 and later do not have this issue.
