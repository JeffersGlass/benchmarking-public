# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [32f8ab1](https://github.com/python/cpython/commit/32f8ab1)
- commit date: 2024-02-15T09:45:21+01:00
- commit merge base: [dc978f6ab62b68c66d3b354638c310ee1cc844a6](https://github.com/python/cpython/commit/dc978f6ab62b68c66d3b354638c310ee1cc844a6)
- ref: 32f8ab1ab65c13ed70f0

## linux x86_64 (azure)

- [pystats raw](bm-20240215-azure-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1-pystats.json)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7921753721)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1-vs-3.10.4.md)
- [📈time plot](bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1-vs-3.11.0.md)
- [📈time plot](bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1-vs-3.12.0.md)
- [📈time plot](bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3%2B-32f8ab1-vs-3.12.0.png)

