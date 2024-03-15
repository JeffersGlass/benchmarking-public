# Results

- fork: python
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [b6ae6da](https://github.com/python/cpython/commit/b6ae6da)
- commit date: 2024-03-11T13:37:48+00:00
- commit merge base: [6c4fc209e1941958164509204cdc3505130c1820](https://github.com/python/cpython/commit/6c4fc209e1941958164509204cdc3505130c1820)
- ref: main

## linux x86_64 (azure)

- [pystats raw](bm-20240311-azure-x86_64-python-main-3.13.0a4%2B-b6ae6da-pystats.json)
- [pystats table](bm-20240311-azure-x86_64-python-main-3.13.0a4%2B-b6ae6da-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8233787335)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240311-linux-x86_64-python-main-3.13.0a4%2B-b6ae6da.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240311-linux-x86_64-python-main-3.13.0a4%2B-b6ae6da-vs-3.10.4.md)
- [📈time plot](bm-20240311-linux-x86_64-python-main-3.13.0a4%2B-b6ae6da-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.99%, 1.02x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240311-linux-x86_64-python-main-3.13.0a4%2B-b6ae6da-vs-3.11.0.md)
- [📈time plot](bm-20240311-linux-x86_64-python-main-3.13.0a4%2B-b6ae6da-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240311-linux-x86_64-python-main-3.13.0a4%2B-b6ae6da-vs-3.12.0.md)
- [📈time plot](bm-20240311-linux-x86_64-python-main-3.13.0a4%2B-b6ae6da-vs-3.12.0.png)

