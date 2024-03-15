# Results

- fork: brandtbucher
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [84bbac4](https://github.com/brandtbucher/cpython/commit/84bbac4)
- commit date: 2024-02-29T15:31:42-08:00
- commit merge base: [e7ba6e9dbe5433b4a0bcb0658da6a68197c28630](https://github.com/brandtbucher/cpython/commit/e7ba6e9dbe5433b4a0bcb0658da6a68197c28630)
- ref: justin_mprotect

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8160546330)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-97-generic-x86_64-with-glibc2.35
- [raw results](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.35x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 85.79%, 1.00x faster at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 75.06%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: 🔴 aiohttp, django_template, genshi_text, genshi_xml, gunicorn, html5lib, pylint, thrift
- [🧠memory plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base-mem.png)
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8160546330)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 62.97%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: 🔴 aiohttp, django_template, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8160546330)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4.json)

### vs. 3.10.4

- Geometric mean: 1.09x faster (HPT: reliability of 99.97%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.14x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: 🔴 django_template, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8160546330)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 2.06x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.89x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 99.80%, 1.00x slower at 99th %ile)
- Memory usage: 1.82x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 94.81%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: 🔴 aiohttp, django_template, genshi_text, genshi_xml, gunicorn, html5lib, pylint, thrift
- [🧠memory plot](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base-mem.png)
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4%2B-84bbac4-vs-base.png)

