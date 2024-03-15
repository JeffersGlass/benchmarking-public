# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [23db9c6](https://github.com/python/cpython/commit/23db9c6)
- commit date: 2024-03-05T15:23:08+00:00
- commit merge base: [0c81ce13602b88fd59f23f701ed8dc377d74e76e](https://github.com/python/cpython/commit/0c81ce13602b88fd59f23f701ed8dc377d74e76e)
- ref: 23db9c62272f7470aadf

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8175263769)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4%2B-23db9c6.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4%2B-23db9c6-vs-3.10.4.md)
- [📈time plot](bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4%2B-23db9c6-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 94.56%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4%2B-23db9c6-vs-3.11.0.md)
- [📈time plot](bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4%2B-23db9c6-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.60%, 1.00x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4%2B-23db9c6-vs-3.12.0.md)
- [📈time plot](bm-20240305-linux-x86_64-python-23db9c62272f7470aadf-3.13.0a4%2B-23db9c6-vs-3.12.0.png)

