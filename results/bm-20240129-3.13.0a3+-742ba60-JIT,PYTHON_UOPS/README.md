# Results

- fork: python
- version: 3.13.0a3+
- tier 2: True
- jit: True
- commit hash: [742ba60](https://github.com/python/cpython/commit/742ba60)
- commit date: 2024-01-29T16:29:54-08:00
- commit merge base: [8612230c1cacab6d48bfbeb9e17d04ef5a9acf21](https://github.com/python/cpython/commit/8612230c1cacab6d48bfbeb9e17d04ef5a9acf21)
- ref: 742ba6081c92744ba30f

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7706998804)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.md)
- [📈time plot](bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 80.62%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.md)
- [📈time plot](bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 58.87%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.md)
- [📈time plot](bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7706998804)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.md)
- [📈time plot](bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 78.34%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.md)
- [📈time plot](bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.md)
- [📈time plot](bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7706998804)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.14x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.md)
- [📈time plot](bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.md)
- [📈time plot](bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.41%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.md)
- [📈time plot](bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7706998804)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60.json)

### vs. 3.10.4

- Geometric mean: 1.08x faster (HPT: reliability of 99.94%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.md)
- [📈time plot](bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.14x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.md)
- [📈time plot](bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.09x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.md)
- [📈time plot](bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7706998804)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit-Mach-O
- [raw results](bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.28x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.md)
- [📈time plot](bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.20x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.md)
- [📈time plot](bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 98.50%, 1.00x slower at 99th %ile)
- Memory usage: 1.15x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.md)
- [📈time plot](bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3%2B-742ba60-vs-3.12.0.png)

