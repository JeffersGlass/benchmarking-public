# Results

- fork: faster-cpython
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [14e3135](https://github.com/faster%2dcpython/cpython/commit/14e3135)
- commit date: 2024-01-07T13:17:57+00:00
- commit merge base: [f19b93fce04fb0bc9b59071915a6aa6b01860d8a](https://github.com/faster%2dcpython/cpython/commit/f19b93fce04fb0bc9b59071915a6aa6b01860d8a)
- ref: incremental_gc

## linux x86_64 (azure)

- [pystats raw](bm-20240107-azure-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-pystats.json)
- [pystats table](bm-20240107-azure-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-pystats.md)

### vs. base

- [pystats diff](bm-20240107-azure-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7445963407)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-3.10.4.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 99.97%, 1.01x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-3.11.0.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-3.12.0.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 98.41%, 1.00x slower at 99th %ile)
- Memory usage: 1.05x
- [🧠memory plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-base-mem.png)
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-base.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-14e3135-vs-base.png)

