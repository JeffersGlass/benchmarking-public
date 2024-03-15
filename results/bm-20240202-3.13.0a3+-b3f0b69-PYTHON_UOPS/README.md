# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [b3f0b69](https://github.com/python/cpython/commit/b3f0b69)
- commit date: 2024-02-02T13:50:51+00:00
- commit merge base: [d29f57f6036353b4e705a42637177442bf7e07e5](https://github.com/python/cpython/commit/d29f57f6036353b4e705a42637177442bf7e07e5)
- ref: b3f0b698daf2438a6e59

## linux x86_64 (azure)

- [pystats raw](bm-20240202-azure-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-pystats.json)
- [pystats table](bm-20240202-azure-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7782279360)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-vs-3.10.4.md)
- [📈time plot](bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 83.53%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-vs-3.11.0.md)
- [📈time plot](bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 99.82%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-vs-3.12.0.md)
- [📈time plot](bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3%2B-b3f0b69-vs-3.12.0.png)

