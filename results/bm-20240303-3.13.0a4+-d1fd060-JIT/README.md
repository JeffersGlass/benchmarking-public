# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [d1fd060](https://github.com/python/cpython/commit/d1fd060)
- commit date: 2024-03-03T07:04:29+09:00
- commit merge base: [2e91578a76d38fa8895fce95e2661618c3de892c](https://github.com/python/cpython/commit/2e91578a76d38fa8895fce95e2661618c3de892c)
- ref: d1fd0606591e1258eb08

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8126244758)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.md)
- [📈time plot](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 51.30%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.md)
- [📈time plot](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 77.08%, 1.00x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.md)
- [📈time plot](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.24x
- [🧠memory plot](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base-mem.png)
- [📄table](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.md)
- [📈time plot](bm-20240303-linux-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8126244758)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-97-generic-x86_64-with-glibc2.35
- [raw results](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.36x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.md)
- [📈time plot](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 77.54%, 1.00x slower at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.md)
- [📈time plot](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.md)
- [📈time plot](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.26x
- [🧠memory plot](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base-mem.png)
- [📄table](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.md)
- [📈time plot](bm-20240303-pythonperf2-x86_64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8126244758)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.14x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.md)
- [📈time plot](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.md)
- [📈time plot](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 97.75%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.md)
- [📈time plot](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x slower (HPT: reliability of 99.80%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.md)
- [📈time plot](bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8126244758)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060.json)

### vs. 3.10.4

- Geometric mean: 1.09x faster (HPT: reliability of 99.98%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.md)
- [📈time plot](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.14x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.md)
- [📈time plot](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.09x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.md)
- [📈time plot](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.md)
- [📈time plot](bm-20240303-pythonperf1_win32-x86-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8126244758)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 2.05x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.md)
- [📈time plot](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.88x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.md)
- [📈time plot](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 99.96%, 1.00x slower at 99th %ile)
- Memory usage: 1.81x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.md)
- [📈time plot](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 98.22%, 1.00x slower at 99th %ile)
- Memory usage: 1.81x
- [🧠memory plot](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base-mem.png)
- [📄table](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.md)
- [📈time plot](bm-20240303-darwin-arm64-python-d1fd0606591e1258eb08-3.13.0a4%2B-d1fd060-vs-base.png)

