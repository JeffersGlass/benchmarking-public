# Results

- fork: python
- version: 3.12.0a1
- tier 2: False
- jit: False
- commit hash: [4ae1a0e](https://github.com/python/cpython/commit/4ae1a0e)
- commit date: 2022-10-25T00:08:22+02:00
- commit merge base: [ad1dc3ebb6aadaeeeacde13d4ed2d62bf302bf62](https://github.com/python/cpython/commit/ad1dc3ebb6aadaeeeacde13d4ed2d62bf302bf62)
- ref: 4ae1a0ecaffe4320fe97

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546446990)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.31x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.md)
- [📈time plot](bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.md)
- [📈time plot](bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.md)
- [📈time plot](bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4546461065)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.md)
- [📈time plot](bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.md)
- [📈time plot](bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 94.17%, 1.00x slower at 99th %ile)
- Memory usage: 0.90x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.md)
- [📈time plot](bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4511435250)
- cpu model: missing
- platform: Windows-11-10.0.22000-SP0
- [raw results](bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json)

### vs. 3.10.4

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.md)
- [📈time plot](bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.md)
- [📈time plot](bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 56.20%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.md)
- [📈time plot](bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961754182)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.md)
- [📈time plot](bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.md)
- [📈time plot](bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 88.33%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, coverage, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.md)
- [📈time plot](bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e-vs-3.12.0.png)

