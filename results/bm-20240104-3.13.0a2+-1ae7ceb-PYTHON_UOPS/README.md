# Results

- fork: python
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [1ae7ceb](https://github.com/python/cpython/commit/1ae7ceb)
- commit date: 2024-01-04T15:05:31+01:00
- commit merge base: [35ef8cb25917bfd6cbbd7c2bb55dd4f82131c9cf](https://github.com/python/cpython/commit/35ef8cb25917bfd6cbbd7c2bb55dd4f82131c9cf)
- ref: 1ae7ceba29771baf8f2e

## linux x86_64 (azure)

- [pystats raw](bm-20240104-azure-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-pystats.json)
- [pystats table](bm-20240104-azure-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-pystats.md)

### vs. base

- [pystats diff](bm-20240104-azure-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7410542473)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.91%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 99.91%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base-mem.png)
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7410542473)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.md)
- [📈time plot](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 95.39%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.md)
- [📈time plot](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.md)
- [📈time plot](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 54.96%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base-mem.png)
- [📄table](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.md)
- [📈time plot](bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7410542473)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb.json)

### vs. 3.10.4

- Geometric mean: 1.11x faster (HPT: reliability of 99.98%, 1.03x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.md)
- [📈time plot](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.md)
- [📈time plot](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.md)
- [📈time plot](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base-mem.png)
- [📄table](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.md)
- [📈time plot](bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.png)

