# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [ad30059](https://github.com/brandtbucher/cpython/commit/ad30059)
- commit date: 2024-02-02T13:23:10-08:00
- commit merge base: [1aec0644447e69e981d582449849761b23702ec8](https://github.com/brandtbucher/cpython/commit/1aec0644447e69e981d582449849761b23702ec8)
- ref: justin_cold

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.12x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.md)
- [📈time plot](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 69.95%, 1.00x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.md)
- [📈time plot](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 89.73%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.md)
- [📈time plot](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 1.02x
- [🧠memory plot](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base-mem.png)
- [📄table](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.md)
- [📈time plot](bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.13x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.md)
- [📈time plot](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 51.60%, 1.00x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.md)
- [📈time plot](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.md)
- [📈time plot](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: 1.02x
- [🧠memory plot](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base-mem.png)
- [📄table](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.md)
- [📈time plot](bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.md)
- [📈time plot](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 99.99%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.md)
- [📈time plot](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 82.40%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.md)
- [📈time plot](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 96.95%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.md)
- [📈time plot](bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059.json)

### vs. 3.10.4

- Geometric mean: 1.10x faster (HPT: reliability of 99.96%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.md)
- [📈time plot](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.md)
- [📈time plot](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.11x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.md)
- [📈time plot](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 99.86%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.md)
- [📈time plot](bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.35x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.md)
- [📈time plot](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.md)
- [📈time plot](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 90.91%, 1.00x slower at 99th %ile)
- Memory usage: 1.22x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.md)
- [📈time plot](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 96.66%, 1.00x slower at 99th %ile)
- Memory usage: 1.06x
- [🧠memory plot](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base-mem.png)
- [📄table](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.md)
- [📈time plot](bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3%2B-ad30059-vs-base.png)

