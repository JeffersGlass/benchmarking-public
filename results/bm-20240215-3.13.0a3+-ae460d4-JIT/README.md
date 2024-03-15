# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [ae460d4](https://github.com/python/cpython/commit/ae460d4)
- commit date: 2024-02-15T10:54:57-08:00
- commit merge base: [e74fa294c9b0c67bfcbefdda5a069f0a7648f524](https://github.com/python/cpython/commit/e74fa294c9b0c67bfcbefdda5a069f0a7648f524)
- ref: ae460d450ab854ca66d5

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7923037887)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.md)
- [📈time plot](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 90.91%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.md)
- [📈time plot](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 74.32%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.md)
- [📈time plot](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.04x
- [🧠memory plot](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-base-mem.png)
- [📄table](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-base.md)
- [📈time plot](bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7923037887)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.md)
- [📈time plot](bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 84.09%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.md)
- [📈time plot](bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.md)
- [📈time plot](bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7923037887)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.md)
- [📈time plot](bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.md)
- [📈time plot](bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.md)
- [📈time plot](bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7923037887)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4.json)

### vs. 3.10.4

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.md)
- [📈time plot](bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.md)
- [📈time plot](bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.11x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.md)
- [📈time plot](bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7923037887)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.md)
- [📈time plot](bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.99%, 1.01x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.md)
- [📈time plot](bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 75.06%, 1.00x slower at 99th %ile)
- Memory usage: 1.13x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.md)
- [📈time plot](bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3%2B-ae460d4-vs-3.12.0.png)

