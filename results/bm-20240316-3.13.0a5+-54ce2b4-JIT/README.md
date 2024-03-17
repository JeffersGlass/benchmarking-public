# Results

- fork: jeffersglass
- version: 3.13.0a5+
- tier 2: False
- jit: True
- commit hash: [54ce2b4](https://github.com/jeffersglass/cpython/commit/54ce2b4)
- commit date: 2024-03-16T17:40:11-05:00
- commit merge base: [1904f0a2245f500aa85fba347b260620350efc78](https://github.com/jeffersglass/cpython/commit/1904f0a2245f500aa85fba347b260620350efc78)
- ref: justin_supernodes_on

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/JeffersGlass/benchmarking-public/actions/runs/8310952500)
- cpu model: AMD EPYC 7763 64-Core Processor
- platform: Linux-6.5.0-1016-azure-x86_64-with-glibc2.35
- [raw results](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4.json)

### vs. 3.10.4

- Geometric mean: 1.42x faster (HPT: reliability of 100.00%, 1.35x faster at 99th %ile)
- Memory usage: 1.31x
- missing benchmarks: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-3.10.4.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: 1.22x
- missing benchmarks: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-3.11.0.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.09x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 1.15x
- missing benchmarks: aiohttp, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-3.12.0.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-base-mem.png)
- [📄table](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-base.md)
- [📈time plot](bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-54ce2b4-vs-base.png)

