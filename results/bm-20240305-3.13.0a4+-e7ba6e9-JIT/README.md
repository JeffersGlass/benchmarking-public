# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [e7ba6e9](https://github.com/python/cpython/commit/e7ba6e9)
- commit date: 2024-03-05T09:05:52-07:00
- commit merge base: [4402b3cbcf8323bfa908ef86a687a5a7d46d27f3](https://github.com/python/cpython/commit/4402b3cbcf8323bfa908ef86a687a5a7d46d27f3)
- ref: e7ba6e9dbe5433b4a0bc

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8160546330)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.34x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.md)
- [📈time plot](bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 98.05%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.md)
- [📈time plot](bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 98.67%, 1.00x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.md)
- [📈time plot](bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-97-generic-x86_64-with-glibc2.35
- [raw results](bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.35x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.md)
- [📈time plot](bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 80.66%, 1.00x faster at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.md)
- [📈time plot](bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.12x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.md)
- [📈time plot](bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.md)
- [📈time plot](bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.md)
- [📈time plot](bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.md)
- [📈time plot](bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9.json)

### vs. 3.10.4

- Geometric mean: 1.02x faster (HPT: reliability of 99.33%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.md)
- [📈time plot](bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.md)
- [📈time plot](bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.md)
- [📈time plot](bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8164027985)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: 2.06x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.md)
- [📈time plot](bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.90x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.md)
- [📈time plot](bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 98.37%, 1.00x slower at 99th %ile)
- Memory usage: 1.82x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.md)
- [📈time plot](bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4%2B-e7ba6e9-vs-3.12.0.png)

