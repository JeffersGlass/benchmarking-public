# Results

- fork: brandtbucher
- version: 3.13.0a2+
- tier 2: False
- jit: True
- commit hash: [172d924](https://github.com/brandtbucher/cpython/commit/172d924)
- commit date: 2024-01-03T17:39:48-08:00
- commit merge base: [1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8](https://github.com/brandtbucher/cpython/commit/1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8)
- ref: justin_jump_removal

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7416387415)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-3.10.4.md)
- [📈time plot](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 90.72%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-3.11.0.md)
- [📈time plot](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 86.88%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-3.12.0.md)
- [📈time plot](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.04x
- [🧠memory plot](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-base-mem.png)
- [📄table](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-base.md)
- [📈time plot](bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2%2B-172d924-vs-base.png)

