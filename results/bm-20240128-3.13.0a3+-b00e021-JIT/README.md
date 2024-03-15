# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [b00e021](https://github.com/brandtbucher/cpython/commit/b00e021)
- commit date: 2024-01-28T23:08:20-08:00
- commit merge base: [a16a9f978f42b8a09297c1efbf33877f6388c403](https://github.com/brandtbucher/cpython/commit/a16a9f978f42b8a09297c1efbf33877f6388c403)
- ref: justin

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7909040686)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-3.10.4.md)
- [📈time plot](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 71.53%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-3.11.0.md)
- [📈time plot](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 50.99%, 1.00x slower at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-3.12.0.md)
- [📈time plot](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-base-mem.png)
- [📄table](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-base.md)
- [📈time plot](bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3%2B-b00e021-vs-base.png)

