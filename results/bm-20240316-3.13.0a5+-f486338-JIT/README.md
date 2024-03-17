# Results

- fork: jeffersglass
- version: 3.13.0a5+
- tier 2: False
- jit: True
- commit hash: [f486338](https://github.com/jeffersglass/cpython/commit/f486338)
- commit date: 2024-03-16T12:04:12-05:00
- commit merge base: [1904f0a2245f500aa85fba347b260620350efc78](https://github.com/jeffersglass/cpython/commit/1904f0a2245f500aa85fba347b260620350efc78)
- ref: justin_supernodes_on

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/JeffersGlass/benchmarking-public/actions/runs/8310940868)
- cpu model: AMD EPYC 7763 64-Core Processor
- platform: Linux-6.5.0-1016-azure-x86_64-with-glibc2.35
- [raw results](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338.json)

### vs. 3.10.4

- Geometric mean: 1.32x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.32x
- missing benchmarks: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.10.4.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 99.80%, 1.00x faster at 99th %ile)
- Memory usage: 1.23x
- missing benchmarks: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.11.0.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 98.51%, 1.00x faster at 99th %ile)
- Memory usage: 1.16x
- missing benchmarks: aiohttp, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.12.0.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 73.05%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- [🧠memory plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-base-mem.png)
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-base.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-base.png)

