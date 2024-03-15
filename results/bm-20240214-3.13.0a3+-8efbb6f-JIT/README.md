# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [8efbb6f](https://github.com/brandtbucher/cpython/commit/8efbb6f)
- commit date: 2024-02-14T13:14:31-08:00
- commit merge base: [4297d7301b97aba2e0df9f9cc5fa4010e53a8950](https://github.com/brandtbucher/cpython/commit/4297d7301b97aba2e0df9f9cc5fa4010e53a8950)
- ref: justin_relax

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7908686753)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.12x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-3.10.4.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x faster (HPT: reliability of 99.41%, 1.00x faster at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-3.11.0.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.95%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-3.12.0.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 99.30%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-base-mem.png)
- [📄table](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-base.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-8efbb6f-vs-base.png)

