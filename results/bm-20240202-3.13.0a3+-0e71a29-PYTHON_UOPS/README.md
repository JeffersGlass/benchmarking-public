# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [0e71a29](https://github.com/python/cpython/commit/0e71a29)
- commit date: 2024-02-02T12:14:34+00:00
- commit merge base: [2091fb2a85c1aa2d9b22c02736b07831bd875c2a](https://github.com/python/cpython/commit/2091fb2a85c1aa2d9b22c02736b07831bd875c2a)
- ref: 0e71a295e9530c939a5e

## linux x86_64 (azure)

- [pystats raw](bm-20240202-azure-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-pystats.json)
- [pystats table](bm-20240202-azure-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-pystats.md)

### vs. base

- [pystats diff](bm-20240202-azure-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7789330846)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-3.10.4.md)
- [📈time plot](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x slower (HPT: reliability of 95.13%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-3.11.0.md)
- [📈time plot](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-3.12.0.md)
- [📈time plot](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x slower (HPT: reliability of 99.98%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-base-mem.png)
- [📄table](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-base.md)
- [📈time plot](bm-20240202-linux-x86_64-python-0e71a295e9530c939a5e-3.13.0a3%2B-0e71a29-vs-base.png)

