# Results

- fork: brandtbucher
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [594cca3](https://github.com/brandtbucher/cpython/commit/594cca3)
- commit date: 2024-02-29T11:14:23-08:00
- commit merge base: [f0df35eeca2ccdfd58cfb9801f06ffa23537270b](https://github.com/brandtbucher/cpython/commit/f0df35eeca2ccdfd58cfb9801f06ffa23537270b)
- ref: justin_jumps

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8101604797)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3.json)

### vs. 3.10.4

- Geometric mean: 1.32x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.34x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 99.40%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.82%, 1.00x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base-mem.png)
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8101604797)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.36x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 83.39%, 1.00x faster at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base-mem.png)
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8101604797)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 99.90%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8101604797)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3.json)

### vs. 3.10.4

- Geometric mean: 1.07x faster (HPT: reliability of 99.91%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.17x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8101604797)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 2.08x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.90x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 99.95%, 1.00x slower at 99th %ile)
- Memory usage: 1.83x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 86.73%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base-mem.png)
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4%2B-594cca3-vs-base.png)

