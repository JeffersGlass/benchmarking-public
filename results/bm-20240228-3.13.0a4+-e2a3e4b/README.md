# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: False
- commit hash: [e2a3e4b](https://github.com/python/cpython/commit/e2a3e4b)
- commit date: 2024-02-28T17:55:56+00:00
- commit merge base: [f58f8cef7445ea04a69ba3e2848fffdb6b72df91](https://github.com/python/cpython/commit/f58f8cef7445ea04a69ba3e2848fffdb6b72df91)
- ref: e2a3e4b7488aff6fdc70

## linux x86_64 (azure)

- [pystats raw](bm-20240228-azure-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-pystats.json)
- [pystats table](bm-20240228-azure-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-pystats.md)

### vs. base

- [pystats diff](bm-20240228-azure-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8094586089)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-3.10.4.md)
- [📈time plot](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-3.11.0.md)
- [📈time plot](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-3.12.0.md)
- [📈time plot](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-base-mem.png)
- [📄table](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-base.md)
- [📈time plot](bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4%2B-e2a3e4b-vs-base.png)

