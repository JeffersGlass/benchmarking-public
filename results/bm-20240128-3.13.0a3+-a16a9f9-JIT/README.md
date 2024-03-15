# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [a16a9f9](https://github.com/python/cpython/commit/a16a9f9)
- commit date: 2024-01-28T18:52:58-08:00
- commit merge base: [f6d9e5926b6138994eaa60d1c36462e36105733d](https://github.com/python/cpython/commit/f6d9e5926b6138994eaa60d1c36462e36105733d)
- ref: a16a9f978f42b8a09297

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7909040686)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3%2B-a16a9f9.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3%2B-a16a9f9-vs-3.10.4.md)
- [📈time plot](bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3%2B-a16a9f9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 62.55%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3%2B-a16a9f9-vs-3.11.0.md)
- [📈time plot](bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3%2B-a16a9f9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 62.40%, 1.00x slower at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3%2B-a16a9f9-vs-3.12.0.md)
- [📈time plot](bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3%2B-a16a9f9-vs-3.12.0.png)

