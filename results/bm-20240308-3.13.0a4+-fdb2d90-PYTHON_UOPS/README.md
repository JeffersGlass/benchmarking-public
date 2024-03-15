# Results

- fork: python
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [fdb2d90](https://github.com/python/cpython/commit/fdb2d90)
- commit date: 2024-03-08T13:49:52+03:00
- commit merge base: [0003285c8d78f0b463f2acc164655456fcfc3206](https://github.com/python/cpython/commit/0003285c8d78f0b463f2acc164655456fcfc3206)
- ref: fdb2d90a274158aee23b

## linux x86_64 (azure)

- [pystats raw](bm-20240308-azure-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-pystats.json)
- [pystats table](bm-20240308-azure-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-pystats.md)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8206475018)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-97-generic-x86_64-with-glibc2.35
- [raw results](bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-vs-3.10.4.md)
- [📈time plot](bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x slower (HPT: reliability of 99.96%, 1.02x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-vs-3.11.0.md)
- [📈time plot](bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.14x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: 0.89x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-vs-3.12.0.md)
- [📈time plot](bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4%2B-fdb2d90-vs-3.12.0.png)

