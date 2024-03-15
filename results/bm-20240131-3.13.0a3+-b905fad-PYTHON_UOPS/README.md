# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [b905fad](https://github.com/python/cpython/commit/b905fad)
- commit date: 2024-01-31T17:33:46+02:00
- commit merge base: [765b9ce9fb357bdb79a50ce51207c827fbd13dd8](https://github.com/python/cpython/commit/765b9ce9fb357bdb79a50ce51207c827fbd13dd8)
- ref: b905fad83819ec9102ec

## linux x86_64 (azure)

- [pystats raw](bm-20240131-azure-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-pystats.json)
- [pystats table](bm-20240131-azure-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-pystats.md)

### vs. base

- [pystats diff](bm-20240131-azure-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7729402502)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.md)
- [📈time plot](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.68%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.md)
- [📈time plot](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.md)
- [📈time plot](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base-mem.png)
- [📄table](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.md)
- [📈time plot](bm-20240131-linux-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7729402502)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.md)
- [📈time plot](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 95.85%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.md)
- [📈time plot](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.md)
- [📈time plot](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base-mem.png)
- [📄table](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.md)
- [📈time plot](bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7729402502)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad.json)

### vs. 3.10.4

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.md)
- [📈time plot](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 99.42%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.md)
- [📈time plot](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 98.24%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.md)
- [📈time plot](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.md)
- [📈time plot](bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7729402502)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad.json)

### vs. 3.10.4

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.md)
- [📈time plot](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.md)
- [📈time plot](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.md)
- [📈time plot](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.md)
- [📈time plot](bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7729402502)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit-Mach-O
- [raw results](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.md)
- [📈time plot](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.md)
- [📈time plot](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.md)
- [📈time plot](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base-mem.png)
- [📄table](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.md)
- [📈time plot](bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3%2B-b905fad-vs-base.png)

