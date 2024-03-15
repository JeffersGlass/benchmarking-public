# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: False
- commit hash: [f58f8ce](https://github.com/python/cpython/commit/f58f8ce)
- commit date: 2024-02-29T02:51:59+09:00
- commit merge base: [0a61e237009bf6b833e13ac635299ee063377699](https://github.com/python/cpython/commit/0a61e237009bf6b833e13ac635299ee063377699)
- ref: main

## linux x86_64 (azure)

- [pystats raw](bm-20240229-azure-x86_64-python-main-3.13.0a4%2B-f58f8ce-pystats.json)
- [pystats table](bm-20240229-azure-x86_64-python-main-3.13.0a4%2B-f58f8ce-pystats.md)

### vs. base

- [pystats diff](bm-20240229-azure-x86_64-python-main-3.13.0a4%2B-f58f8ce-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8084880106)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-3.10.4.md)
- [📈time plot](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-3.11.0.md)
- [📈time plot](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-3.12.0.md)
- [📈time plot](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 73.34%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-base-mem.png)
- [📄table](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-base.md)
- [📈time plot](bm-20240229-linux-x86_64-python-main-3.13.0a4%2B-f58f8ce-vs-base.png)

