# Results

- fork: mdboom
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [522c622](https://github.com/mdboom/cpython/commit/522c622)
- commit date: 2023-12-20T10:52:46-05:00
- commit merge base: [05a370abd6cdfe4b54be60b3b911f3a441026bb2](https://github.com/mdboom/cpython/commit/05a370abd6cdfe4b54be60b3b911f3a441026bb2)
- ref: mdboom_compact_int_s

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7277743215)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622.json)

### vs. 3.10.4

- Geometric mean: 1.34x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.04x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-3.10.4.md)
- [📈time plot](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.98%, 1.00x faster at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-3.11.0.md)
- [📈time plot](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-3.12.0.md)
- [📈time plot](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 76.32%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: 🔴 dask
- [🧠memory plot](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-base-mem.png)
- [📄table](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-base.md)
- [📈time plot](bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2%2B-522c622-vs-base.png)

