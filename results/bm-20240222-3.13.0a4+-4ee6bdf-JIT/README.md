# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [4ee6bdf](https://github.com/python/cpython/commit/4ee6bdf)
- commit date: 2024-02-22T12:23:48-08:00
- commit merge base: [1002fbe12e0bd8c9a54bc5addbf5d94a5b35f91f](https://github.com/python/cpython/commit/1002fbe12e0bd8c9a54bc5addbf5d94a5b35f91f)
- ref: 4ee6bdfbaa792a3aa93c

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8024976735)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4%2B-4ee6bdf.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.22x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4%2B-4ee6bdf-vs-3.10.4.md)
- [📈time plot](bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4%2B-4ee6bdf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 93.16%, 1.00x slower at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4%2B-4ee6bdf-vs-3.11.0.md)
- [📈time plot](bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4%2B-4ee6bdf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.23%, 1.00x slower at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4%2B-4ee6bdf-vs-3.12.0.md)
- [📈time plot](bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4%2B-4ee6bdf-vs-3.12.0.png)

