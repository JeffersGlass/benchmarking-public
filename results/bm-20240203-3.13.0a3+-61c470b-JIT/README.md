# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [61c470b](https://github.com/brandtbucher/cpython/commit/61c470b)
- commit date: 2024-02-03T00:05:24-08:00
- commit merge base: [0990d55725cb649e74739c983b67cf08c58e8439](https://github.com/brandtbucher/cpython/commit/0990d55725cb649e74739c983b67cf08c58e8439)
- ref: justin_ghccc

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7766068737)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b.json)

### vs. 3.10.4

- Geometric mean: 1.32x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.md)
- [📈time plot](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 94.03%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.md)
- [📈time plot](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 89.80%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.md)
- [📈time plot](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 99.99%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base-mem.png)
- [📄table](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.md)
- [📈time plot](bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7766068737)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.md)
- [📈time plot](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 89.45%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.md)
- [📈time plot](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.md)
- [📈time plot](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 97.67%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base-mem.png)
- [📄table](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.md)
- [📈time plot](bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7766068737)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.md)
- [📈time plot](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.md)
- [📈time plot](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.24%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.md)
- [📈time plot](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 76.55%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.md)
- [📈time plot](bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7766068737)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b.json)

### vs. 3.10.4

- Geometric mean: 1.17x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.md)
- [📈time plot](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.md)
- [📈time plot](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.17x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.md)
- [📈time plot](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.md)
- [📈time plot](bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3%2B-61c470b-vs-base.png)

