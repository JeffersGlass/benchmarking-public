# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [7f5e3f0](https://github.com/python/cpython/commit/7f5e3f0)
- commit date: 2024-02-21T23:18:57+00:00
- commit merge base: [113687a8381d6dde179aeede607bcbca5c09d182](https://github.com/python/cpython/commit/113687a8381d6dde179aeede607bcbca5c09d182)
- ref: 7f5e3f04f838686d65f1

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.22x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.md)
- [📈time plot](bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 93.26%, 1.00x slower at 99th %ile)
- Memory usage: 1.13x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.md)
- [📈time plot](bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.81%, 1.00x slower at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.md)
- [📈time plot](bm-20240221-linux-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-92-generic-x86_64-with-glibc2.35
- [raw results](bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: 1.23x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.md)
- [📈time plot](bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 79.66%, 1.00x slower at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.md)
- [📈time plot](bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.md)
- [📈time plot](bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0.json)

### vs. 3.10.4

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.md)
- [📈time plot](bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 97.82%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.md)
- [📈time plot](bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 87.12%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.md)
- [📈time plot](bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0.json)

### vs. 3.10.4

- Geometric mean: 1.03x faster (HPT: reliability of 91.52%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.md)
- [📈time plot](bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.md)
- [📈time plot](bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.md)
- [📈time plot](bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7998838640)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 2.08x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.md)
- [📈time plot](bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.90x
- missing benchmarks: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.md)
- [📈time plot](bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 99.75%, 1.00x slower at 99th %ile)
- Memory usage: 1.83x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.md)
- [📈time plot](bm-20240221-darwin-arm64-python-7f5e3f04f838686d65f1-3.13.0a4%2B-7f5e3f0-vs-3.12.0.png)

