# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [ffed8d9](https://github.com/python/cpython/commit/ffed8d9)
- commit date: 2024-03-04T10:16:56-08:00
- commit merge base: [981f27dcc4be8bc4824464c9d75f2ea6c868863f](https://github.com/python/cpython/commit/981f27dcc4be8bc4824464c9d75f2ea6c868863f)
- ref: ffed8d985b57a97def2e

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8145868526)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.10.4.md)
- [📈time plot](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 96.37%, 1.00x faster at 99th %ile)
- Memory usage: 1.23x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.11.0.md)
- [📈time plot](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.43%, 1.00x faster at 99th %ile)
- Memory usage: 1.16x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.12.0.md)
- [📈time plot](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.12.0.png)

