# Results

- fork: Fidget-Spinner
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [27ce303](https://github.com/Fidget%2dSpinner/cpython/commit/27ce303)
- commit date: 2024-01-20T06:18:19+08:00
- commit merge base: [68a7b78cd5185cbd9456f42c15ecf872a7c16f44](https://github.com/Fidget%2dSpinner/cpython/commit/68a7b78cd5185cbd9456f42c15ecf872a7c16f44)
- ref: tier2_abstract_inter

## linux x86_64 (azure)

- [pystats raw](bm-20240120-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-pystats.json)
- [pystats table](bm-20240120-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-pystats.md)

### vs. base

- [pystats diff](bm-20240120-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7589857594)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.37x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.10.4.md)
- [📈time plot](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x slower (HPT: reliability of 94.89%, 1.00x slower at 99th %ile)
- Memory usage: 1.28x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.11.0.md)
- [📈time plot](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: 1.19x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.12.0.md)
- [📈time plot](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 69.82%, 1.00x faster at 99th %ile)
- Memory usage: 1.27x
- [🧠memory plot](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base-mem.png)
- [📄table](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base.md)
- [📈time plot](bm-20240120-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7589857594)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: 1.39x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.10.4.md)
- [📈time plot](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 93.94%, 1.00x slower at 99th %ile)
- Memory usage: 1.28x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.11.0.md)
- [📈time plot](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.12.0.md)
- [📈time plot](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 1.28x
- [🧠memory plot](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base-mem.png)
- [📄table](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base.md)
- [📈time plot](bm-20240120-pythonperf2-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7589857594)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit
- [raw results](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.41x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.10.4.md)
- [📈time plot](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.31x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.11.0.md)
- [📈time plot](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.12.0.md)
- [📈time plot](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 99.73%, 1.00x faster at 99th %ile)
- Memory usage: 1.27x
- [🧠memory plot](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base-mem.png)
- [📄table](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base.md)
- [📈time plot](bm-20240120-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-27ce303-vs-base.png)

