# Results

- fork: python
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [ffed8d9](https://github.com/python/cpython/commit/ffed8d9)
- commit date: 2024-03-04T10:16:56-08:00
- commit merge base: [981f27dcc4be8bc4824464c9d75f2ea6c868863f](https://github.com/python/cpython/commit/981f27dcc4be8bc4824464c9d75f2ea6c868863f)
- ref: ffed8d985b57a97def2e

## linux x86_64 (azure)

- [pystats raw](bm-20240304-azure-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-pystats.json)
- [pystats table](bm-20240304-azure-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-pystats.md)

### vs. base

- [pystats diff](bm-20240304-azure-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8145881148)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.14x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.10.4.md)
- [📈time plot](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.68%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.11.0.md)
- [📈time plot](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.12.0.md)
- [📈time plot](bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4%2B-ffed8d9-vs-3.12.0.png)

