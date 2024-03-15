# Results

- fork: faster-cpython
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [a1a724c](https://github.com/faster%2dcpython/cpython/commit/a1a724c)
- commit date: 2024-03-11T12:14:19+00:00
- commit merge base: [ffd79bea0f032df5a2e7f75e8c823a09cdc7c7a2](https://github.com/faster%2dcpython/cpython/commit/ffd79bea0f032df5a2e7f75e8c823a09cdc7c7a2)
- ref: replicate_more_load_

## linux x86_64 (azure)

- [pystats raw](bm-20240311-azure-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-pystats.json)
- [pystats table](bm-20240311-azure-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8237132733)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240311-linux-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c.json)

### vs. 3.10.4

- Geometric mean: 1.17x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240311-linux-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-vs-3.10.4.md)
- [📈time plot](bm-20240311-linux-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240311-linux-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-vs-3.11.0.md)
- [📈time plot](bm-20240311-linux-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.11x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240311-linux-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-vs-3.12.0.md)
- [📈time plot](bm-20240311-linux-x86_64-faster%252dcpython-replicate_more_load_-3.13.0a4%2B-a1a724c-vs-3.12.0.png)

