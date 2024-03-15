# Results

- fork: python
- version: 3.12.0a5
- tier 2: False
- jit: False
- commit hash: [3c67ec3](https://github.com/python/cpython/commit/3c67ec3)
- commit date: 2023-02-07T13:21:15+01:00
- commit merge base: [79903240480429a6e545177416a7b782b0e5b9bd](https://github.com/python/cpython/commit/79903240480429a6e545177416a7b782b0e5b9bd)
- ref: 3c67ec394faac79d2608

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546447055)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230207-linux-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json)

### vs. 3.10.4

- Geometric mean: 1.38x faster (HPT: reliability of 100.00%, 1.32x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-linux-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.md)
- [📈time plot](bm-20230207-linux-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-linux-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.md)
- [📈time plot](bm-20230207-linux-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230207-linux-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.md)
- [📈time plot](bm-20230207-linux-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546461361)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.md)
- [📈time plot](bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.md)
- [📈time plot](bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 97.24%, 1.00x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.md)
- [📈time plot](bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4511434995)
- cpu model: missing
- platform: Windows-11-10.0.22000-SP0
- [raw results](bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.md)
- [📈time plot](bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.md)
- [📈time plot](bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.md)
- [📈time plot](bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961754763)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json)

### vs. 3.10.4

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.md)
- [📈time plot](bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint
- [📄table](bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.md)
- [📈time plot](bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 95.35%, 1.00x slower at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: aiohttp, coverage, gunicorn, mypy2
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.md)
- [📈time plot](bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3-vs-3.12.0.png)

