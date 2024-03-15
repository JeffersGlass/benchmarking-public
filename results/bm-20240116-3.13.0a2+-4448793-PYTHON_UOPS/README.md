# Results

- fork: faster-cpython
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [4448793](https://github.com/faster%2dcpython/cpython/commit/4448793)
- commit date: 2024-01-16T21:49:38+00:00
- commit merge base: [ac10947ba79a15bfdaa3ca92c6864214648ab364](https://github.com/faster%2dcpython/cpython/commit/ac10947ba79a15bfdaa3ca92c6864214648ab364)
- ref: cold_exits

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7555574423)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240116-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-4448793.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240116-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-4448793-vs-3.10.4.md)
- [📈time plot](bm-20240116-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-4448793-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x slower (HPT: reliability of 99.82%, 1.01x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240116-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-4448793-vs-3.11.0.md)
- [📈time plot](bm-20240116-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-4448793-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.14x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240116-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-4448793-vs-3.12.0.md)
- [📈time plot](bm-20240116-pythonperf2-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-4448793-vs-3.12.0.png)

