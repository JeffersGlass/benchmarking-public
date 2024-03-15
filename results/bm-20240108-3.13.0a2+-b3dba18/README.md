# Results

- fork: python
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [b3dba18](https://github.com/python/cpython/commit/b3dba18)
- commit date: 2024-01-08T19:31:52+00:00
- commit merge base: [bc71ae2b97bb59b1796be056fb821d9abdee840b](https://github.com/python/cpython/commit/bc71ae2b97bb59b1796be056fb821d9abdee840b)
- ref: b3dba18eab96dc956530

## linux x86_64 (azure)

- [pystats raw](bm-20240108-azure-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-pystats.json)
- [pystats table](bm-20240108-azure-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7452918643)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-vs-3.10.4.md)
- [📈time plot](bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-vs-3.11.0.md)
- [📈time plot](bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-vs-3.12.0.md)
- [📈time plot](bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2%2B-b3dba18-vs-3.12.0.png)

