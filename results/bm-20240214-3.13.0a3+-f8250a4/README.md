# Results

- fork: mdboom
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [f8250a4](https://github.com/mdboom/cpython/commit/f8250a4)
- commit date: 2024-02-14T11:42:28-05:00
- commit merge base: [6755c4e0c8803a246e632835030c0b8837b3b676](https://github.com/mdboom/cpython/commit/6755c4e0c8803a246e632835030c0b8837b3b676)
- ref: force_mimalloc

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7904507906)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-3.10.4.md)
- [📈time plot](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-3.11.0.md)
- [📈time plot](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-3.12.0.md)
- [📈time plot](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 59.02%, 1.00x faster at 99th %ile)
- Memory usage: 1.08x
- [🧠memory plot](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-base-mem.png)
- [📄table](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-base.md)
- [📈time plot](bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3%2B-f8250a4-vs-base.png)

