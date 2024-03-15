# Results

- fork: Fidget-Spinner
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [8915762](https://github.com/Fidget%2dSpinner/cpython/commit/8915762)
- commit date: 2024-01-20T12:02:23+08:00
- commit merge base: [68a7b78cd5185cbd9456f42c15ecf872a7c16f44](https://github.com/Fidget%2dSpinner/cpython/commit/68a7b78cd5185cbd9456f42c15ecf872a7c16f44)
- ref: tier2_abstract_inter

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7589857594)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.10.4.md)
- [📈time plot](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.93%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.11.0.md)
- [📈time plot](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 96.43%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.12.0.md)
- [📈time plot](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 77.62%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-base.md)
- [📈time plot](bm-20240120-pythonperf1-amd64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7589857594)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.10.4.md)
- [📈time plot](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.11.0.md)
- [📈time plot](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.12.0.md)
- [📈time plot](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 50.72%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-base.md)
- [📈time plot](bm-20240120-pythonperf1_win32-x86-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-8915762-vs-base.png)

