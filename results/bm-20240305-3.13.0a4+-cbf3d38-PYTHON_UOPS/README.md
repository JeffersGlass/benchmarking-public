# Results

- fork: python
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [cbf3d38](https://github.com/python/cpython/commit/cbf3d38)
- commit date: 2024-03-05T11:23:46+00:00
- commit merge base: [a29998a06bf75264c3faaeeec4584a5f75b45a1f](https://github.com/python/cpython/commit/a29998a06bf75264c3faaeeec4584a5f75b45a1f)
- ref: cbf3d38cbeb6e640d595

## linux x86_64 (azure)

- [pystats raw](bm-20240305-azure-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-pystats.json)
- [pystats table](bm-20240305-azure-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8157194403)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-vs-3.10.4.md)
- [📈time plot](bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.60%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-vs-3.11.0.md)
- [📈time plot](bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-vs-3.12.0.md)
- [📈time plot](bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4%2B-cbf3d38-vs-3.12.0.png)

