# Results

- fork: mdboom
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [39bbca4](https://github.com/mdboom/cpython/commit/39bbca4)
- commit date: 2023-12-21T11:30:06-05:00
- commit merge base: [05a370abd6cdfe4b54be60b3b911f3a441026bb2](https://github.com/mdboom/cpython/commit/05a370abd6cdfe4b54be60b3b911f3a441026bb2)
- ref: compact_long

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7290755702)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4.json)

### vs. 3.10.4

- Geometric mean: 1.34x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.10.4.md)
- [📈time plot](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.98%, 1.01x faster at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.11.0.md)
- [📈time plot](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.12.0.md)
- [📈time plot](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 99.81%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: 🔴 dask
- [🧠memory plot](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base-mem.png)
- [📄table](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base.md)
- [📈time plot](bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7290755702)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.10.4.md)
- [📈time plot](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.97%, 1.00x faster at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.11.0.md)
- [📈time plot](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 93.85%, 1.00x slower at 99th %ile)
- Memory usage: 0.86x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.12.0.md)
- [📈time plot](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 78.65%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: 🔴 dask
- [🧠memory plot](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base-mem.png)
- [📄table](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base.md)
- [📈time plot](bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7290755702)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4.json)

### vs. 3.10.4

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.10.4.md)
- [📈time plot](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.11.0.md)
- [📈time plot](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.12.0.md)
- [📈time plot](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: 🔴 dask
- [🧠memory plot](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base-mem.png)
- [📄table](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base.md)
- [📈time plot](bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2%2B-39bbca4-vs-base.png)

