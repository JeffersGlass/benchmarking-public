# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [05e4720](https://github.com/python/cpython/commit/05e4720)
- commit date: 2024-01-19T10:25:05+00:00
- commit merge base: [a34e4db28a98904f6c9976675ed7121ed61edabe](https://github.com/python/cpython/commit/a34e4db28a98904f6c9976675ed7121ed61edabe)
- ref: 05e47202a34e6ae05e69

## linux x86_64 (azure)

- [pystats raw](bm-20240119-azure-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-pystats.json)
- [pystats table](bm-20240119-azure-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7612824167)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720.json)

### vs. 3.10.4

- Geometric mean: 1.35x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-vs-3.10.4.md)
- [📈time plot](bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 99.99%, 1.01x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-vs-3.11.0.md)
- [📈time plot](bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-vs-3.12.0.md)
- [📈time plot](bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3%2B-05e4720-vs-3.12.0.png)

