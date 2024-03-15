# Results

- fork: python
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [ac10947](https://github.com/python/cpython/commit/ac10947)
- commit date: 2024-01-15T11:41:06+00:00
- commit merge base: [2010d45327128594aed332befa687c8aead010bc](https://github.com/python/cpython/commit/2010d45327128594aed332befa687c8aead010bc)
- ref: ac10947ba79a15bfdaa3

## linux x86_64 (azure)

- [pystats raw](bm-20240115-azure-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-pystats.json)
- [pystats table](bm-20240115-azure-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7544748039)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-vs-3.10.4.md)
- [📈time plot](bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 98.99%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-vs-3.11.0.md)
- [📈time plot](bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-vs-3.12.0.md)
- [📈time plot](bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2%2B-ac10947-vs-3.12.0.png)

