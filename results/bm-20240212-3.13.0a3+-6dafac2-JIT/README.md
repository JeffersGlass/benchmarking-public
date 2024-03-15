# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [6dafac2](https://github.com/brandtbucher/cpython/commit/6dafac2)
- commit date: 2024-02-12T15:29:49-08:00
- commit merge base: [4297d7301b97aba2e0df9f9cc5fa4010e53a8950](https://github.com/brandtbucher/cpython/commit/4297d7301b97aba2e0df9f9cc5fa4010e53a8950)
- ref: justin_continue

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7879444178)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2.json)

### vs. 3.10.4

- Geometric mean: 1.33x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.md)
- [📈time plot](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x faster (HPT: reliability of 99.69%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.md)
- [📈time plot](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.69%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.md)
- [📈time plot](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base-mem.png)
- [📄table](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.md)
- [📈time plot](bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7879444178)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.md)
- [📈time plot](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 96.37%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.md)
- [📈time plot](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.md)
- [📈time plot](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 82.95%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base-mem.png)
- [📄table](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.md)
- [📈time plot](bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7879444178)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.md)
- [📈time plot](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.md)
- [📈time plot](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.md)
- [📈time plot](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.md)
- [📈time plot](bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7879444178)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2.json)

### vs. 3.10.4

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.md)
- [📈time plot](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.md)
- [📈time plot](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.md)
- [📈time plot](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 85.18%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.md)
- [📈time plot](bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7879444178)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.md)
- [📈time plot](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.99%, 1.01x slower at 99th %ile)
- Memory usage: 1.18x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.md)
- [📈time plot](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 61.38%, 1.00x faster at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.md)
- [📈time plot](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- [🧠memory plot](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base-mem.png)
- [📄table](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.md)
- [📈time plot](bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-6dafac2-vs-base.png)

