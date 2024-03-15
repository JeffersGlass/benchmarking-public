# Results

- fork: python
- version: 3.12.0a6
- tier 2: False
- jit: False
- commit hash: [f9774e5](https://github.com/python/cpython/commit/f9774e5)
- commit date: 2023-03-07T22:48:18+01:00
- ref: f9774e57d84162ff0cba

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546447152)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230307-linux-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.15x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-linux-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.md)
- [📈time plot](bm-20230307-linux-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-linux-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.md)
- [📈time plot](bm-20230307-linux-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230307-linux-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.md)
- [📈time plot](bm-20230307-linux-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546461484)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.23x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.md)
- [📈time plot](bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 1.15x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.md)
- [📈time plot](bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 85.47%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.md)
- [📈time plot](bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4511434980)
- cpu model: missing
- platform: Windows-11-10.0.22000-SP0
- [raw results](bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.md)
- [📈time plot](bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.md)
- [📈time plot](bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.md)
- [📈time plot](bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546451869)
- cpu model: missing
- platform: macOS-13.2.1-arm64-arm-64bit
- [raw results](bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5.json)

### vs. 3.10.4

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.md)
- [📈time plot](bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.md)
- [📈time plot](bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 61.93%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.md)
- [📈time plot](bm-20230307-darwin-arm64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5-vs-3.12.0.png)

