# Results

- fork: python
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [471aa75](https://github.com/python/cpython/commit/471aa75)
- commit date: 2023-12-30T16:18:06-07:00
- commit merge base: [f48a1bcb2914addee971814fd014e4d8075ea6a9](https://github.com/python/cpython/commit/f48a1bcb2914addee971814fd014e4d8075ea6a9)
- ref: 471aa752415029c50869

## linux x86_64 (azure)

- [pystats raw](bm-20231230-azure-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-pystats.json)
- [pystats table](bm-20231230-azure-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7367240496)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231230-linux-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231230-linux-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.10.4.md)
- [📈time plot](bm-20231230-linux-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231230-linux-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.11.0.md)
- [📈time plot](bm-20231230-linux-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231230-linux-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.12.0.md)
- [📈time plot](bm-20231230-linux-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7367240496)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20231230-pythonperf2-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231230-pythonperf2-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.10.4.md)
- [📈time plot](bm-20231230-pythonperf2-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.96%, 1.01x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231230-pythonperf2-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.11.0.md)
- [📈time plot](bm-20231230-pythonperf2-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 91.28%, 1.00x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231230-pythonperf2-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.12.0.md)
- [📈time plot](bm-20231230-pythonperf2-x86_64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7367240496)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20231230-darwin-arm64-python-471aa752415029c50869-3.13.0a2%2B-471aa75.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231230-darwin-arm64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.10.4.md)
- [📈time plot](bm-20231230-darwin-arm64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231230-darwin-arm64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.11.0.md)
- [📈time plot](bm-20231230-darwin-arm64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 98.86%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231230-darwin-arm64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.12.0.md)
- [📈time plot](bm-20231230-darwin-arm64-python-471aa752415029c50869-3.13.0a2%2B-471aa75-vs-3.12.0.png)

