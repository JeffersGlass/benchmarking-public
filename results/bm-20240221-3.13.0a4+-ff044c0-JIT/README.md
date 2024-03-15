# Results

- fork: brandtbucher
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [ff044c0](https://github.com/brandtbucher/cpython/commit/ff044c0)
- commit date: 2024-02-21T18:39:34-08:00
- commit merge base: [7f5e3f04f838686d65f1053a5e47f5d3faf0b228](https://github.com/brandtbucher/cpython/commit/7f5e3f04f838686d65f1053a5e47f5d3faf0b228)
- ref: justin_relax

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.md)
- [📈time plot](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 50.62%, 1.00x faster at 99th %ile)
- Memory usage: 1.23x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.md)
- [📈time plot](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 74.35%, 1.00x slower at 99th %ile)
- Memory usage: 1.16x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.md)
- [📈time plot](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.09x
- [🧠memory plot](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base-mem.png)
- [📄table](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.md)
- [📈time plot](bm-20240221-linux-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.36x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.md)
- [📈time plot](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 69.91%, 1.00x slower at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.md)
- [📈time plot](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.md)
- [📈time plot](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 93.99%, 1.00x slower at 99th %ile)
- Memory usage: 1.09x
- [🧠memory plot](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base-mem.png)
- [📄table](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.md)
- [📈time plot](bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.md)
- [📈time plot](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.md)
- [📈time plot](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.98%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.md)
- [📈time plot](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.md)
- [📈time plot](bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0.json)

### vs. 3.10.4

- Geometric mean: 1.07x faster (HPT: reliability of 99.97%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.md)
- [📈time plot](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.17x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.md)
- [📈time plot](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.md)
- [📈time plot](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.md)
- [📈time plot](bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 2.08x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.md)
- [📈time plot](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.90x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.md)
- [📈time plot](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.37%, 1.00x slower at 99th %ile)
- Memory usage: 1.83x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.md)
- [📈time plot](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 95.14%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base-mem.png)
- [📄table](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.md)
- [📈time plot](bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4%2B-ff044c0-vs-base.png)

