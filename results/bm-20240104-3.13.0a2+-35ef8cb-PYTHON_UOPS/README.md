# Results

- fork: python
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [35ef8cb](https://github.com/python/cpython/commit/35ef8cb)
- commit date: 2024-01-04T11:14:15+00:00
- commit merge base: [4c4b08dd2bd5f2cad4e41bf29119a3daa2956f6e](https://github.com/python/cpython/commit/4c4b08dd2bd5f2cad4e41bf29119a3daa2956f6e)
- ref: 35ef8cb25917bfd6cbbd

## linux x86_64 (azure)

- [pystats raw](bm-20240104-azure-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-pystats.json)
- [pystats table](bm-20240104-azure-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7855691461)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.10.4.md)
- [📈time plot](bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 99.00%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.11.0.md)
- [📈time plot](bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.12.0.md)
- [📈time plot](bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7409552531)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.10.4.md)
- [📈time plot](bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 93.56%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.11.0.md)
- [📈time plot](bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.12.0.md)
- [📈time plot](bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2%2B-35ef8cb-vs-3.12.0.png)

