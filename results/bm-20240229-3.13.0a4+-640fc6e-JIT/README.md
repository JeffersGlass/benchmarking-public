# Results

- fork: brandtbucher
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [640fc6e](https://github.com/brandtbucher/cpython/commit/640fc6e)
- commit date: 2024-02-29T16:03:55-08:00
- commit merge base: [e7ba6e9dbe5433b4a0bcb0658da6a68197c28630](https://github.com/brandtbucher/cpython/commit/e7ba6e9dbe5433b4a0bcb0658da6a68197c28630)
- ref: justin_nops

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 88.43%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 98.15%, 1.00x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 99.82%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- new benchmarks: aiohttp, django_template, djangocms, genshi_text, genshi_xml, gunicorn, html5lib, pylint, thrift
- [🧠memory plot](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base-mem.png)
- [📄table](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.md)
- [📈time plot](bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-97-generic-x86_64-with-glibc2.35
- [raw results](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.36x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 61.53%, 1.00x faster at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base-mem.png)
- [📄table](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.md)
- [📈time plot](bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.md)
- [📈time plot](bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e.json)

### vs. 3.10.4

- Geometric mean: 1.06x faster (HPT: reliability of 99.95%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.md)
- [📈time plot](bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: 2.07x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.90x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 99.30%, 1.00x slower at 99th %ile)
- Memory usage: 1.82x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 82.99%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- [🧠memory plot](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base-mem.png)
- [📄table](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.md)
- [📈time plot](bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4%2B-640fc6e-vs-base.png)

