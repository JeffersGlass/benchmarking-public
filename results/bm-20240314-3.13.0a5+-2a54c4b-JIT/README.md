# Results

- fork: python
- version: 3.13.0a5+
- tier 2: False
- jit: True
- commit hash: [2a54c4b](https://github.com/python/cpython/commit/2a54c4b)
- commit date: 2024-03-14T13:57:02+01:00
- commit merge base: [97b80af897cd3376a5be66c8d5d63310723a1590](https://github.com/python/cpython/commit/97b80af897cd3376a5be66c8d5d63310723a1590)
- ref: 2a54c4b25e05e30c50b9

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8282284020)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.10.4.md)
- [📈time plot](bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 66.48%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.11.0.md)
- [📈time plot](bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 85.79%, 1.00x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.12.0.md)
- [📈time plot](bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.12.0.png)

