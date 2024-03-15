# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [1e610fb](https://github.com/python/cpython/commit/1e610fb)
- commit date: 2024-01-20T03:06:00+00:00
- commit merge base: [6313cdde58f34648a430d2830357c9d2a5b67b87](https://github.com/python/cpython/commit/6313cdde58f34648a430d2830357c9d2a5b67b87)
- ref: 1e610fb05fa4ba61a759

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8009520827)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240120-linux-x86_64-python-1e610fb05fa4ba61a759-3.13.0a3%2B-1e610fb.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240120-linux-x86_64-python-1e610fb05fa4ba61a759-3.13.0a3%2B-1e610fb-vs-3.10.4.md)
- [📈time plot](bm-20240120-linux-x86_64-python-1e610fb05fa4ba61a759-3.13.0a3%2B-1e610fb-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240120-linux-x86_64-python-1e610fb05fa4ba61a759-3.13.0a3%2B-1e610fb-vs-3.11.0.md)
- [📈time plot](bm-20240120-linux-x86_64-python-1e610fb05fa4ba61a759-3.13.0a3%2B-1e610fb-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240120-linux-x86_64-python-1e610fb05fa4ba61a759-3.13.0a3%2B-1e610fb-vs-3.12.0.md)
- [📈time plot](bm-20240120-linux-x86_64-python-1e610fb05fa4ba61a759-3.13.0a3%2B-1e610fb-vs-3.12.0.png)

