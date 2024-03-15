# Results

- fork: Fidget-Spinner
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [fcdc84c](https://github.com/Fidget%2dSpinner/cpython/commit/fcdc84c)
- commit date: 2024-01-29T23:39:37+08:00
- commit merge base: [384429d1c0cf011dcf88d4043e0328de8b063c24](https://github.com/Fidget%2dSpinner/cpython/commit/384429d1c0cf011dcf88d4043e0328de8b063c24)
- ref: tier2_abstract_inter

## linux x86_64 (azure)

- [pystats raw](bm-20240129-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-pystats.json)
- [pystats table](bm-20240129-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-pystats.md)

### vs. base

- [pystats diff](bm-20240129-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7698742033)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.md)
- [📈time plot](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x slower (HPT: reliability of 96.94%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.md)
- [📈time plot](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.md)
- [📈time plot](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 98.64%, 1.00x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base-mem.png)
- [📄table](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.md)
- [📈time plot](bm-20240129-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7698742033)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.md)
- [📈time plot](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x slower (HPT: reliability of 86.47%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.md)
- [📈time plot](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.md)
- [📈time plot](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base-mem.png)
- [📄table](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.md)
- [📈time plot](bm-20240129-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7698742033)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.md)
- [📈time plot](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x faster (HPT: reliability of 99.81%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.md)
- [📈time plot](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 76.67%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.md)
- [📈time plot](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 93.41%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.md)
- [📈time plot](bm-20240129-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7698742033)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.md)
- [📈time plot](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.md)
- [📈time plot](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.md)
- [📈time plot](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 97.58%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.md)
- [📈time plot](bm-20240129-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7698742033)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit
- [raw results](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 1.12x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.md)
- [📈time plot](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.md)
- [📈time plot](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.md)
- [📈time plot](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base-mem.png)
- [📄table](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.md)
- [📈time plot](bm-20240129-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-fcdc84c-vs-base.png)

