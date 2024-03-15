# Results

- fork: Fidget-Spinner
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [cf59bba](https://github.com/Fidget%2dSpinner/cpython/commit/cf59bba)
- commit date: 2024-01-27T00:43:24+08:00
- commit merge base: [384429d1c0cf011dcf88d4043e0328de8b063c24](https://github.com/Fidget%2dSpinner/cpython/commit/384429d1c0cf011dcf88d4043e0328de8b063c24)
- ref: tier2_abstract_inter

## linux x86_64 (azure)

- [pystats raw](bm-20240127-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-pystats.json)

### vs. base

- [pystats diff](bm-20240127-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7675023928)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.md)
- [📈time plot](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 92.49%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.md)
- [📈time plot](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 99.41%, 1.00x slower at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.md)
- [📈time plot](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- [🧠memory plot](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base-mem.png)
- [📄table](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.md)
- [📈time plot](bm-20240127-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7673268297)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 84.91%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 0.90x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- [🧠memory plot](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base-mem.png)
- [📄table](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.md)
- [📈time plot](bm-20240127-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7673268297)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x faster (HPT: reliability of 99.57%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 94.90%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 87.39%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.md)
- [📈time plot](bm-20240127-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7673268297)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 82.21%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.md)
- [📈time plot](bm-20240127-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7675018377)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit
- [raw results](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.13x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.md)
- [📈time plot](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.md)
- [📈time plot](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.md)
- [📈time plot](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- [🧠memory plot](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base-mem.png)
- [📄table](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.md)
- [📈time plot](bm-20240127-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-cf59bba-vs-base.png)

