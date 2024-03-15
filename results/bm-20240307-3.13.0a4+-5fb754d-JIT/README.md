# Results

- fork: brandtbucher
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [5fb754d](https://github.com/brandtbucher/cpython/commit/5fb754d)
- commit date: 2024-03-07T20:04:02-08:00
- commit merge base: [c62144a02cfae412a9deb4059fae141693a6edc9](https://github.com/brandtbucher/cpython/commit/c62144a02cfae412a9deb4059fae141693a6edc9)
- ref: defer_decref

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8206441528)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d.json)

### vs. 3.10.4

- Geometric mean: 1.22x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: 1.34x
- missing benchmarks: dask, flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative, unpack_sequence
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-3.10.4.md)
- [📈time plot](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: dask, flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative, unpack_sequence
- [📄table](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-3.11.0.md)
- [📈time plot](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: dask, sqlalchemy_declarative, sqlalchemy_imperative, unpack_sequence
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-3.12.0.md)
- [📈time plot](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: 🔴 unpack_sequence
- [🧠memory plot](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-base-mem.png)
- [📄table](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-base.md)
- [📈time plot](bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4%2B-5fb754d-vs-base.png)

