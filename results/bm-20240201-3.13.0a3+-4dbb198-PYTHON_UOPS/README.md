# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [4dbb198](https://github.com/python/cpython/commit/4dbb198)
- commit date: 2024-02-01T11:52:54+00:00
- commit merge base: [0bf42dae7e73febc76ea96fd58af6b765a12b8a7](https://github.com/python/cpython/commit/0bf42dae7e73febc76ea96fd58af6b765a12b8a7)
- ref: 4dbb198d279a06fed74e

## linux x86_64 (azure)

- [pystats raw](bm-20240201-azure-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-pystats.json)
- [pystats table](bm-20240201-azure-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7745893450)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-vs-3.10.4.md)
- [📈time plot](bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 98.52%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-vs-3.11.0.md)
- [📈time plot](bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-vs-3.12.0.md)
- [📈time plot](bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3%2B-4dbb198-vs-3.12.0.png)

