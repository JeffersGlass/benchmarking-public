# Results

- fork: mdboom
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [34fc24a](https://github.com/mdboom/cpython/commit/34fc24a)
- commit date: 2024-01-04T12:15:41-05:00
- commit merge base: [1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8](https://github.com/mdboom/cpython/commit/1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8)
- ref: faster_negate

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7412668537)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a.json)

### vs. 3.10.4

- Geometric mean: 1.35x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-3.10.4.md)
- [📈time plot](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-3.11.0.md)
- [📈time plot](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-3.12.0.md)
- [📈time plot](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 96.40%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-base-mem.png)
- [📄table](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-base.md)
- [📈time plot](bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2%2B-34fc24a-vs-base.png)

