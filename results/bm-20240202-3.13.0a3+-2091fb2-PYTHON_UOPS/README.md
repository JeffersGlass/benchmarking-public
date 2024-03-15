# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [2091fb2](https://github.com/python/cpython/commit/2091fb2)
- commit date: 2024-02-02T11:26:31+00:00
- commit merge base: [41fde89e471003b3e70fdd76d6726fba9982a1eb](https://github.com/python/cpython/commit/41fde89e471003b3e70fdd76d6726fba9982a1eb)
- ref: 2091fb2a85c1aa2d9b22

## linux x86_64 (azure)

- [pystats raw](bm-20240202-azure-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-pystats.json)
- [pystats table](bm-20240202-azure-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7817609354)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-vs-3.10.4.md)
- [📈time plot](bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 90.46%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-vs-3.11.0.md)
- [📈time plot](bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 99.92%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-vs-3.12.0.md)
- [📈time plot](bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3%2B-2091fb2-vs-3.12.0.png)

