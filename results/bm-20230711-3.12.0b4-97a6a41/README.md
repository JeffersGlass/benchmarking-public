# Results

- fork: python
- version: 3.12.0b4
- tier 2: False
- jit: False
- commit hash: [97a6a41](https://github.com/python/cpython/commit/97a6a41)
- commit date: 2023-07-11T14:23:30+02:00
- ref: 97a6a418167f1c8bbb01, v3.12.0b4

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/5977401451)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift
- [📄table](bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.10.4.md)
- [📈time plot](bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.82%, 1.00x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift
- [📄table](bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.11.0.md)
- [📈time plot](bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sympy_expand, sympy_integrate, sympy_str, sympy_sum
- [📄table](bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.12.0.md)
- [📈time plot](bm-20230711-linux-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/5977401451)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-76-generic-x86_64-with-glibc2.35
- [raw results](bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift
- [📄table](bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.10.4.md)
- [📈time plot](bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 99.96%, 1.01x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift
- [📄table](bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.11.0.md)
- [📈time plot](bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 55.42%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum
- [📄table](bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.12.0.md)
- [📈time plot](bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/5977401451)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift
- [📄table](bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.10.4.md)
- [📈time plot](bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift
- [📄table](bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.11.0.md)
- [📈time plot](bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum
- [📄table](bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.12.0.md)
- [📈time plot](bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961755556)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20230711-darwin-arm64-python-97a6a418167f1c8bbb01-3.12.0b4-97a6a41.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20230711-darwin-arm64-python-97a6a418167f1c8bbb01-3.12.0b4-97a6a41-vs-3.10.4.md)
- [📈time plot](bm-20230711-darwin-arm64-python-97a6a418167f1c8bbb01-3.12.0b4-97a6a41-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.91%, 1.00x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, thrift
- [📄table](bm-20230711-darwin-arm64-python-97a6a418167f1c8bbb01-3.12.0b4-97a6a41-vs-3.11.0.md)
- [📈time plot](bm-20230711-darwin-arm64-python-97a6a418167f1c8bbb01-3.12.0b4-97a6a41-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 98.73%, 1.00x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: mypy2
- [📄table](bm-20230711-darwin-arm64-python-97a6a418167f1c8bbb01-3.12.0b4-97a6a41-vs-3.12.0.md)
- [📈time plot](bm-20230711-darwin-arm64-python-97a6a418167f1c8bbb01-3.12.0b4-97a6a41-vs-3.12.0.png)

