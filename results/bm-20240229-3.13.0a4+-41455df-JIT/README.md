# Results

- fork: brandtbucher
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [41455df](https://github.com/brandtbucher/cpython/commit/41455df)
- commit date: 2024-02-29T22:40:10-08:00
- commit merge base: [e7ba6e9dbe5433b4a0bcb0658da6a68197c28630](https://github.com/brandtbucher/cpython/commit/e7ba6e9dbe5433b4a0bcb0658da6a68197c28630)
- ref: justin_mprotect

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8160546330)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.21x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-3.10.4.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 98.25%, 1.00x faster at 99th %ile)
- Memory usage: 1.13x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-3.11.0.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.54%, 1.00x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-3.12.0.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 80.83%, 1.00x faster at 99th %ile)
- Memory usage: 0.92x
- [🧠memory plot](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-base-mem.png)
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-base.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-41455df-vs-base.png)

