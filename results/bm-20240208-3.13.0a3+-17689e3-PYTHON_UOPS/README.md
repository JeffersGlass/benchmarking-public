# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [17689e3](https://github.com/python/cpython/commit/17689e3)
- commit date: 2024-02-08T01:04:41-08:00
- commit merge base: [9e90313320a2af2d9ff7049ed3842344ed236630](https://github.com/python/cpython/commit/9e90313320a2af2d9ff7049ed3842344ed236630)
- ref: 17689e3c41d9f61bcd19

## linux x86_64 (azure)

- [pystats raw](bm-20240208-azure-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-pystats.json)
- [pystats table](bm-20240208-azure-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7833146692)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-vs-3.10.4.md)
- [📈time plot](bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 85.35%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-vs-3.11.0.md)
- [📈time plot](bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 99.03%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-vs-3.12.0.md)
- [📈time plot](bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3%2B-17689e3-vs-3.12.0.png)

