# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [d1b031c](https://github.com/python/cpython/commit/d1b031c)
- commit date: 2024-01-22T10:19:25+01:00
- commit merge base: [650f9e4c94711ff49ea4e13bf800945a6147b7e0](https://github.com/python/cpython/commit/650f9e4c94711ff49ea4e13bf800945a6147b7e0)
- ref: d1b031cc58516e1aba82

## linux x86_64 (azure)

- [pystats raw](bm-20240122-azure-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-pystats.json)
- [pystats table](bm-20240122-azure-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7610631691)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-vs-3.10.4.md)
- [📈time plot](bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 96.88%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-vs-3.11.0.md)
- [📈time plot](bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.97%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-vs-3.12.0.md)
- [📈time plot](bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3%2B-d1b031c-vs-3.12.0.png)

