# Results

- fork: faster-cpython
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [5208402](https://github.com/faster%2dcpython/cpython/commit/5208402)
- commit date: 2024-03-12T09:18:04+00:00
- commit merge base: [ffd79bea0f032df5a2e7f75e8c823a09cdc7c7a2](https://github.com/faster%2dcpython/cpython/commit/ffd79bea0f032df5a2e7f75e8c823a09cdc7c7a2)
- ref: replicate_fast_local

## linux x86_64 (azure)

- [pystats raw](bm-20240312-azure-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-pystats.json)
- [pystats table](bm-20240312-azure-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8246559397)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240312-linux-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402.json)

### vs. 3.10.4

- Geometric mean: 1.22x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240312-linux-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-vs-3.10.4.md)
- [📈time plot](bm-20240312-linux-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240312-linux-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-vs-3.11.0.md)
- [📈time plot](bm-20240312-linux-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240312-linux-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-vs-3.12.0.md)
- [📈time plot](bm-20240312-linux-x86_64-faster%252dcpython-replicate_fast_local-3.13.0a4%2B-5208402-vs-3.12.0.png)

