# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [6755c4e](https://github.com/python/cpython/commit/6755c4e)
- commit date: 2024-02-14T13:52:42+00:00
- commit merge base: [6d9141ed766f4003f39362937dc397e9f734c7e5](https://github.com/python/cpython/commit/6d9141ed766f4003f39362937dc397e9f734c7e5)
- ref: 6755c4e0c8803a246e63

## linux x86_64 (azure)

- [pystats raw](bm-20240214-azure-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-pystats.json)
- [pystats table](bm-20240214-azure-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-pystats.md)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7905574975)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.14x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.10.4.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 77.54%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.11.0.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.12.0.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.12.0.png)

