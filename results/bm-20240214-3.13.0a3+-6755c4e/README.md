# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [6755c4e](https://github.com/python/cpython/commit/6755c4e)
- commit date: 2024-02-14T13:52:42+00:00
- commit merge base: [6d9141ed766f4003f39362937dc397e9f734c7e5](https://github.com/python/cpython/commit/6d9141ed766f4003f39362937dc397e9f734c7e5)
- ref: 6755c4e0c8803a246e63

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7902264284)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.10.4.md)
- [📈time plot](bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.11.0.md)
- [📈time plot](bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.12.0.md)
- [📈time plot](bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3%2B-6755c4e-vs-3.12.0.png)

