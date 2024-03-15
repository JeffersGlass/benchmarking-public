# Results

- fork: python
- version: 3.13.0a2+
- tier 2: False
- jit: True
- commit hash: [1ae7ceb](https://github.com/python/cpython/commit/1ae7ceb)
- commit date: 2024-01-04T15:05:31+01:00
- commit merge base: [35ef8cb25917bfd6cbbd7c2bb55dd4f82131c9cf](https://github.com/python/cpython/commit/35ef8cb25917bfd6cbbd7c2bb55dd4f82131c9cf)
- ref: 1ae7ceba29771baf8f2e

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7415170316)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 74.20%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base-mem.png)
- [📄table](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.md)
- [📈time plot](bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2%2B-1ae7ceb-vs-base.png)

