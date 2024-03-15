# Results

- fork: python
- version: 3.12.0a4
- tier 2: False
- jit: False
- commit hash: [3d5d3f7](https://github.com/python/cpython/commit/3d5d3f7)
- commit date: 2023-01-10T13:09:15+01:00
- commit merge base: [f07daaf4f7a637f9f9324e7c8bf78e8a3faae7e0](https://github.com/python/cpython/commit/f07daaf4f7a637f9f9324e7c8bf78e8a3faae7e0)
- ref: 3d5d3f7af6498effbc60

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4747478381)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json)

### vs. 3.10.4

- Geometric mean: 1.38x faster (HPT: reliability of 100.00%, 1.33x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.md)
- [📈time plot](bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.md)
- [📈time plot](bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.md)
- [📈time plot](bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546461326)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.md)
- [📈time plot](bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 99.99%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.md)
- [📈time plot](bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.56%, 1.00x slower at 99th %ile)
- Memory usage: 0.89x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.md)
- [📈time plot](bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4747479725)
- cpu model: missing
- platform: Windows-11-10.0.22000-SP0
- [raw results](bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.md)
- [📈time plot](bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.md)
- [📈time plot](bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.md)
- [📈time plot](bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961754642)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json)

### vs. 3.10.4

- Geometric mean: 1.22x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.04x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.md)
- [📈time plot](bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 93.60%, 1.00x slower at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
- [📄table](bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.md)
- [📈time plot](bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.96%, 1.00x faster at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, coverage, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.md)
- [📈time plot](bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7-vs-3.12.0.png)

