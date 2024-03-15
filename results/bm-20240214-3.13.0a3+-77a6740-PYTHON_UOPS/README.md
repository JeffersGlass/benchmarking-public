# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [77a6740](https://github.com/faster%2dcpython/cpython/commit/77a6740)
- commit date: 2024-02-14T15:57:04+00:00
- commit merge base: [6755c4e0c8803a246e632835030c0b8837b3b676](https://github.com/faster%2dcpython/cpython/commit/6755c4e0c8803a246e632835030c0b8837b3b676)
- ref: cold_exits

## linux x86_64 (azure)

- [pystats raw](bm-20240214-azure-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-pystats.json)
- [pystats table](bm-20240214-azure-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-pystats.md)

### vs. base

- [pystats diff](bm-20240214-azure-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-pystats-vs-base.md)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7905574975)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740.json)

### vs. 3.10.4

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-3.10.4.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x slower (HPT: reliability of 99.76%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-3.11.0.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.13x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 0.89x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-3.12.0.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-base-mem.png)
- [📄table](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-base.md)
- [📈time plot](bm-20240214-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a3%2B-77a6740-vs-base.png)

