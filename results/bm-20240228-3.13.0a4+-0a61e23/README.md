# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: False
- commit hash: [0a61e23](https://github.com/python/cpython/commit/0a61e23)
- commit date: 2024-02-28T15:21:42+00:00
- commit merge base: [9578288a3e5a7f42d1f3bec139c0c85b87775c90](https://github.com/python/cpython/commit/9578288a3e5a7f42d1f3bec139c0c85b87775c90)
- ref: 0a61e237009bf6b833e1

## linux x86_64 (azure)

- [pystats raw](bm-20240228-azure-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-pystats.json)
- [pystats table](bm-20240228-azure-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8084880106)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-vs-3.10.4.md)
- [📈time plot](bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-vs-3.11.0.md)
- [📈time plot](bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-vs-3.12.0.md)
- [📈time plot](bm-20240228-linux-x86_64-python-0a61e237009bf6b833e1-3.13.0a4%2B-0a61e23-vs-3.12.0.png)

