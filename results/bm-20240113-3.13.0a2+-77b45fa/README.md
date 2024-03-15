# Results

- fork: python
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [77b45fa](https://github.com/python/cpython/commit/77b45fa)
- commit date: 2024-01-13T15:26:55+02:00
- commit merge base: [dd56b5748317c3d504d6a9660d9207620c547f5c](https://github.com/python/cpython/commit/dd56b5748317c3d504d6a9660d9207620c547f5c)
- ref: 77b45fa6d0b8c0c14657

## linux x86_64 (azure)

- [pystats raw](bm-20240113-azure-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-pystats.json)
- [pystats table](bm-20240113-azure-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7515786611)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240113-linux-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240113-linux-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.10.4.md)
- [📈time plot](bm-20240113-linux-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240113-linux-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.11.0.md)
- [📈time plot](bm-20240113-linux-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240113-linux-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.12.0.md)
- [📈time plot](bm-20240113-linux-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7515786611)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240113-pythonperf2-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240113-pythonperf2-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.10.4.md)
- [📈time plot](bm-20240113-pythonperf2-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.95%, 1.01x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240113-pythonperf2-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.11.0.md)
- [📈time plot](bm-20240113-pythonperf2-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 87.12%, 1.00x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240113-pythonperf2-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.12.0.md)
- [📈time plot](bm-20240113-pythonperf2-x86_64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7515786611)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit
- [raw results](bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.10.4.md)
- [📈time plot](bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.99%, 1.01x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.11.0.md)
- [📈time plot](bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 60.65%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.12.0.md)
- [📈time plot](bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2%2B-77b45fa-vs-3.12.0.png)

