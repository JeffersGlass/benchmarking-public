# Results

- fork: brandtbucher
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [c49f898](https://github.com/brandtbucher/cpython/commit/c49f898)
- commit date: 2024-01-04T11:46:36-08:00
- commit merge base: [1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8](https://github.com/brandtbucher/cpython/commit/1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8)
- ref: counter_table

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7428345067)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898.json)

### vs. 3.10.4

- Geometric mean: 1.35x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-3.10.4.md)
- [📈time plot](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.99%, 1.01x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-3.11.0.md)
- [📈time plot](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-3.12.0.md)
- [📈time plot](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 99.96%, 1.00x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-base-mem.png)
- [📄table](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-base.md)
- [📈time plot](bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2%2B-c49f898-vs-base.png)

