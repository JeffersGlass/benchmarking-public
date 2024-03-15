# Results

- fork: python
- version: 3.11.0a2
- tier 2: False
- jit: False
- commit hash: [e2b4e4b](https://github.com/python/cpython/commit/e2b4e4b)
- commit date: 2021-11-05T19:04:04+00:00
- commit merge base: [3d42cd9461e60c7427f3793f640cd975fbd99289](https://github.com/python/cpython/commit/3d42cd9461e60c7427f3793f640cd975fbd99289)
- ref: e2b4e4bab90b69fbd361

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.md)
- [📈time plot](bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.md)
- [📈time plot](bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.97%, 1.01x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.md)
- [📈time plot](bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4513535196)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.md)
- [📈time plot](bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.md)
- [📈time plot](bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.13x slower (HPT: reliability of 100.00%, 1.10x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.md)
- [📈time plot](bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4491158300)
- cpu model: missing
- platform: Windows-10-10.0.22000
- [raw results](bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json)

### vs. 3.10.4

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.md)
- [📈time plot](bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x slower (HPT: reliability of 99.99%, 1.01x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.md)
- [📈time plot](bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.12x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.md)
- [📈time plot](bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961752383)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json)

### vs. 3.10.4

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.md)
- [📈time plot](bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.12x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.md)
- [📈time plot](bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 99.21%, 1.00x slower at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.md)
- [📈time plot](bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.12.0.png)

