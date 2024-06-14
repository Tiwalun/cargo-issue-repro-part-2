# Reproduction for cargo issue

This is a reproduction for a cargo issue, where compilation fails with a confusing error message.
Running `cargo c` (with cargo 1.79) in this repository fails with the following error message:

```bash
$ cargo c
    Updating git repository `https://github.com/Tiwalun/cargo-issue-repro-part-1`
error: no matching package found
searched package name: `test_a`
perhaps you meant:      test_c
location searched: https://github.com/Tiwalun/cargo-issue-repro-part-1
required by package `test_b v0.1.0 (/home/dobo/work/tmp/cargo-repro/ws-2/test_b)
```
