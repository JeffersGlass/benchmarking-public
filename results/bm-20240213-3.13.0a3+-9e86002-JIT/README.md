# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [9e86002](https://github.com/brandtbucher/cpython/commit/9e86002)
- commit date: 2024-02-13T15:36:57-08:00
- commit merge base: [4297d7301b97aba2e0df9f9cc5fa4010e53a8950](https://github.com/brandtbucher/cpython/commit/4297d7301b97aba2e0df9f9cc5fa4010e53a8950)
- ref: justin_continue

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7894500164)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002.json)

### vs. 3.10.4

- Geometric mean: 1.33x faster (HPT: reliability of 100.00%, 1.25x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.md)
- [📈time plot](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x faster (HPT: reliability of 98.24%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.md)
- [📈time plot](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.84%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.md)
- [📈time plot](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base-mem.png)
- [📄table](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.md)
- [📈time plot](bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7894500164)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.md)
- [📈time plot](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 76.61%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.md)
- [📈time plot](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.md)
- [📈time plot](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 84.55%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base-mem.png)
- [📄table](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.md)
- [📈time plot](bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7894500164)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.md)
- [📈time plot](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.11x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.md)
- [📈time plot](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.md)
- [📈time plot](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.md)
- [📈time plot](bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7894500164)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.md)
- [📈time plot](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.18x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.md)
- [📈time plot](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 50.23%, 1.00x faster at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.md)
- [📈time plot](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base-mem.png)
- [📄table](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.md)
- [📈time plot](bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3%2B-9e86002-vs-base.png)

