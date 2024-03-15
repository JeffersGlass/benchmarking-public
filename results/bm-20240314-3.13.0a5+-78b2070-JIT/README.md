# Results

- fork: brandtbucher
- version: 3.13.0a5+
- tier 2: False
- jit: True
- commit hash: [78b2070](https://github.com/brandtbucher/cpython/commit/78b2070)
- commit date: 2024-03-14T17:22:32-07:00
- commit merge base: [8c094c3095feb4de2efebd00f67fb6cc3b2bc240](https://github.com/brandtbucher/cpython/commit/8c094c3095feb4de2efebd00f67fb6cc3b2bc240)
- ref: justin_relax_absolut

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8289604081)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.10.4.md)
- [📈time plot](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 55.11%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.11.0.md)
- [📈time plot](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 95.43%, 1.00x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.12.0.md)
- [📈time plot](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 95.20%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-base-mem.png)
- [📄table](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-base.md)
- [📈time plot](bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-base.png)

