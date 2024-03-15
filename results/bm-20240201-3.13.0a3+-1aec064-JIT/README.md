# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [1aec064](https://github.com/python/cpython/commit/1aec064)
- commit date: 2024-02-01T17:44:01-08:00
- commit merge base: [618d7256e78da8200f6e2c6235094a1ef885dca4](https://github.com/python/cpython/commit/618d7256e78da8200f6e2c6235094a1ef885dca4)
- ref: 1aec0644447e69e981d5

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.md)
- [📈time plot](bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 79.55%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.md)
- [📈time plot](bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 78.11%, 1.00x faster at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.md)
- [📈time plot](bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.md)
- [📈time plot](bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 64.85%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.md)
- [📈time plot](bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.md)
- [📈time plot](bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.md)
- [📈time plot](bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 99.99%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.md)
- [📈time plot](bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.75%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.md)
- [📈time plot](bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064.json)

### vs. 3.10.4

- Geometric mean: 1.11x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.md)
- [📈time plot](bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.md)
- [📈time plot](bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.md)
- [📈time plot](bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7761915648)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.27x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.md)
- [📈time plot](bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.19x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.md)
- [📈time plot](bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 87.20%, 1.00x slower at 99th %ile)
- Memory usage: 1.15x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.md)
- [📈time plot](bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3%2B-1aec064-vs-3.12.0.png)

