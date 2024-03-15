# Results

- fork: mdboom
- version: 3.13.0a5+
- tier 2: False
- jit: True
- commit hash: [cb999fb](https://github.com/mdboom/cpython/commit/cb999fb)
- commit date: 2024-03-13T16:36:53-04:00
- commit merge base: [61733a2fb9dc36d2246d922146a3462a2248832d](https://github.com/mdboom/cpython/commit/61733a2fb9dc36d2246d922146a3462a2248832d)
- ref: dont_getenv

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8271245860)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.10.4.md)
- [📈time plot](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 66.60%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.11.0.md)
- [📈time plot](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 81.76%, 1.00x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.12.0.md)
- [📈time plot](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 89.19%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-base-mem.png)
- [📄table](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-base.md)
- [📈time plot](bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-base.png)

