# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [a768e12](https://github.com/python/cpython/commit/a768e12)
- commit date: 2024-01-27T23:47:55+02:00
- commit merge base: [823a38a960c245cbf309ef29120d3690ba1bcd2c](https://github.com/python/cpython/commit/823a38a960c245cbf309ef29120d3690ba1bcd2c)
- ref: a768e12f094a9b14a9a1

## linux x86_64 (azure)

- [pystats raw](bm-20240127-azure-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-pystats.json)
- [pystats table](bm-20240127-azure-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-pystats.md)

### vs. base

- [pystats diff](bm-20240127-azure-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7682132687)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.md)
- [📈time plot](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 97.86%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.md)
- [📈time plot](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.97%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.md)
- [📈time plot](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base-mem.png)
- [📄table](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.md)
- [📈time plot](bm-20240127-linux-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7682132687)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 96.96%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base-mem.png)
- [📄table](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7682132687)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x faster (HPT: reliability of 99.46%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 69.36%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7682132687)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7682132687)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit-Mach-O
- [raw results](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.md)
- [📈time plot](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.04x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.md)
- [📈time plot](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.md)
- [📈time plot](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base-mem.png)
- [📄table](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.md)
- [📈time plot](bm-20240127-darwin-arm64-python-a768e12f094a9b14a9a1-3.13.0a3%2B-a768e12-vs-base.png)

