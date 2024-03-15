# Results

- fork: mdboom
- version: 3.13.0a5+
- tier 2: False
- jit: True
- commit hash: [c3a9b5a](https://github.com/mdboom/cpython/commit/c3a9b5a)
- commit date: 2024-03-14T10:18:03-04:00
- commit merge base: [2a54c4b25e05e30c50b915302fa846dd0d4e018b](https://github.com/mdboom/cpython/commit/2a54c4b25e05e30c50b915302fa846dd0d4e018b)
- ref: estimate_too_short

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8282284020)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.10.4.md)
- [📈time plot](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 89.92%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.11.0.md)
- [📈time plot](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 66.82%, 1.00x slower at 99th %ile)
- Memory usage: 1.16x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.12.0.md)
- [📈time plot](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 0.99x
- [🧠memory plot](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-base-mem.png)
- [📄table](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-base.md)
- [📈time plot](bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-base.png)

