# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [b70a68f](https://github.com/python/cpython/commit/b70a68f)
- commit date: 2024-02-11T00:51:05+03:00
- commit merge base: [3a5b38e3b465e00f133ff8074a2d4afb1392dfb5](https://github.com/python/cpython/commit/3a5b38e3b465e00f133ff8074a2d4afb1392dfb5)
- ref: b70a68fbd6b72a25b5ef

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7875687258)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3%2B-b70a68f.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3%2B-b70a68f-vs-3.10.4.md)
- [📈time plot](bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3%2B-b70a68f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3%2B-b70a68f-vs-3.11.0.md)
- [📈time plot](bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3%2B-b70a68f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3%2B-b70a68f-vs-3.12.0.md)
- [📈time plot](bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3%2B-b70a68f-vs-3.12.0.png)

