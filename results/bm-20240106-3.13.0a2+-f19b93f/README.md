# Results

- fork: python
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [f19b93f](https://github.com/python/cpython/commit/f19b93f)
- commit date: 2024-01-06T22:30:12-08:00
- commit merge base: [541c5dbb81c784afd587406be2cc82645979a107](https://github.com/python/cpython/commit/541c5dbb81c784afd587406be2cc82645979a107)
- ref: f19b93fce04fb0bc9b59

## linux x86_64 (azure)

- [pystats raw](bm-20240106-azure-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-pystats.json)
- [pystats table](bm-20240106-azure-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7440558039)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-vs-3.10.4.md)
- [📈time plot](bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-vs-3.11.0.md)
- [📈time plot](bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-vs-3.12.0.md)
- [📈time plot](bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2%2B-f19b93f-vs-3.12.0.png)

