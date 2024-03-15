# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: False
- commit hash: [72dbea2](https://github.com/python/cpython/commit/72dbea2)
- commit date: 2024-03-07T12:24:38+01:00
- commit merge base: [72d3cc94cd8cae1925e7a14f297b06ac6184f916](https://github.com/python/cpython/commit/72d3cc94cd8cae1925e7a14f297b06ac6184f916)
- ref: main

## linux x86_64 (azure)

- [pystats raw](bm-20240307-azure-x86_64-python-main-3.13.0a4%2B-72dbea2-pystats.json)
- [pystats table](bm-20240307-azure-x86_64-python-main-3.13.0a4%2B-72dbea2-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8187451848)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240307-linux-x86_64-python-main-3.13.0a4%2B-72dbea2.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240307-linux-x86_64-python-main-3.13.0a4%2B-72dbea2-vs-3.10.4.md)
- [📈time plot](bm-20240307-linux-x86_64-python-main-3.13.0a4%2B-72dbea2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240307-linux-x86_64-python-main-3.13.0a4%2B-72dbea2-vs-3.11.0.md)
- [📈time plot](bm-20240307-linux-x86_64-python-main-3.13.0a4%2B-72dbea2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240307-linux-x86_64-python-main-3.13.0a4%2B-72dbea2-vs-3.12.0.md)
- [📈time plot](bm-20240307-linux-x86_64-python-main-3.13.0a4%2B-72dbea2-vs-3.12.0.png)

