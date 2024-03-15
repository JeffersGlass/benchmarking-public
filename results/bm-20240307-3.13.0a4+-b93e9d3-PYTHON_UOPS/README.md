# Results

- fork: faster-cpython
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [b93e9d3](https://github.com/faster%2dcpython/cpython/commit/b93e9d3)
- commit date: 2024-03-07T14:45:26+00:00
- commit merge base: [72d3cc94cd8cae1925e7a14f297b06ac6184f916](https://github.com/faster%2dcpython/cpython/commit/72d3cc94cd8cae1925e7a14f297b06ac6184f916)
- ref: optimize_inline_valu

## linux x86_64 (azure)

- [pystats raw](bm-20240307-azure-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-pystats.json)
- [pystats table](bm-20240307-azure-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-pystats.md)

### vs. base

- [pystats diff](bm-20240307-azure-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8190029525)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-3.10.4.md)
- [📈time plot](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 97.35%, 1.00x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-3.11.0.md)
- [📈time plot](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-3.12.0.md)
- [📈time plot](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 68.17%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-base-mem.png)
- [📄table](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-base.md)
- [📈time plot](bm-20240307-linux-x86_64-faster%252dcpython-optimize_inline_valu-3.13.0a4%2B-b93e9d3-vs-base.png)

