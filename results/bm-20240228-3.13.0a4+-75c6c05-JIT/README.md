# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [75c6c05](https://github.com/python/cpython/commit/75c6c05)
- commit date: 2024-02-28T12:50:09-08:00
- commit merge base: [df5212df6c6f08308c68de4b3ed8a1b51ac6334b](https://github.com/python/cpython/commit/df5212df6c6f08308c68de4b3ed8a1b51ac6334b)
- ref: 75c6c05fea212330f4b0

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8104150029)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4%2B-75c6c05.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.34x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4%2B-75c6c05-vs-3.10.4.md)
- [📈time plot](bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4%2B-75c6c05-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 76.07%, 1.00x slower at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4%2B-75c6c05-vs-3.11.0.md)
- [📈time plot](bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4%2B-75c6c05-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.08%, 1.00x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4%2B-75c6c05-vs-3.12.0.md)
- [📈time plot](bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4%2B-75c6c05-vs-3.12.0.png)

