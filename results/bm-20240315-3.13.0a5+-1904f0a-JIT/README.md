# Results

- fork: python
- version: 3.13.0a5+
- tier 2: False
- jit: True
- commit hash: [1904f0a](https://github.com/python/cpython/commit/1904f0a)
- commit date: 2024-03-15T00:11:49+00:00
- commit merge base: [be1c808fcad201adc4d5d6cca52ddb24aeb5e367](https://github.com/python/cpython/commit/be1c808fcad201adc4d5d6cca52ddb24aeb5e367)
- ref: 1904f0a2245f500aa85f

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/JeffersGlass/benchmarking-public/actions/runs/8310940868)
- cpu model: AMD EPYC 7763 64-Core Processor
- platform: Linux-6.5.0-1016-azure-x86_64-with-glibc2.35
- [raw results](bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.30x
- missing benchmarks: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.10.4.md)
- [📈time plot](bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 97.53%, 1.00x faster at 99th %ile)
- Memory usage: 1.21x
- missing benchmarks: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.11.0.md)
- [📈time plot](bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 98.74%, 1.00x faster at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.12.0.md)
- [📈time plot](bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.12.0.png)

