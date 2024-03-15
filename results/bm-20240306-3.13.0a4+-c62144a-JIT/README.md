# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [c62144a](https://github.com/python/cpython/commit/c62144a)
- commit date: 2024-03-06T15:46:36-05:00
- commit merge base: [ce0ae1d784871085059a415aa589d9bd16ea8301](https://github.com/python/cpython/commit/ce0ae1d784871085059a415aa589d9bd16ea8301)
- ref: c62144a02cfae412a9de

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8206441528)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4%2B-c62144a.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: dask, flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4%2B-c62144a-vs-3.10.4.md)
- [📈time plot](bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4%2B-c62144a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 70.20%, 1.00x faster at 99th %ile)
- Memory usage: 1.23x
- missing benchmarks: dask, flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4%2B-c62144a-vs-3.11.0.md)
- [📈time plot](bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4%2B-c62144a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 82.52%, 1.00x slower at 99th %ile)
- Memory usage: 1.15x
- missing benchmarks: dask, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4%2B-c62144a-vs-3.12.0.md)
- [📈time plot](bm-20240306-linux-x86_64-python-c62144a02cfae412a9de-3.13.0a4%2B-c62144a-vs-3.12.0.png)

