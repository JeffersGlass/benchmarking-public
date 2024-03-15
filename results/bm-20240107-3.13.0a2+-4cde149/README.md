# Results

- fork: faster-cpython
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [4cde149](https://github.com/faster%2dcpython/cpython/commit/4cde149)
- commit date: 2024-01-07T07:04:13+00:00
- commit merge base: [f19b93fce04fb0bc9b59071915a6aa6b01860d8a](https://github.com/faster%2dcpython/cpython/commit/f19b93fce04fb0bc9b59071915a6aa6b01860d8a)
- ref: incremental_gc

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7440558039)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149.json)

### vs. 3.10.4

- Geometric mean: 1.35x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-3.10.4.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 99.84%, 1.01x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-3.11.0.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-3.12.0.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 94.08%, 1.00x slower at 99th %ile)
- Memory usage: 1.04x
- [🧠memory plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-base-mem.png)
- [📄table](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-base.md)
- [📈time plot](bm-20240107-linux-x86_64-faster%252dcpython-incremental_gc-3.13.0a2%2B-4cde149-vs-base.png)

