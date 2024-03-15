# Results

- fork: python
- version: 3.11.0a1
- tier 2: False
- jit: False
- commit hash: [7c12e48](https://github.com/python/cpython/commit/7c12e48)
- commit date: 2021-10-05T13:44:05+01:00
- ref: 7c12e4835ebe52287acd

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.10.4.md)
- [📈time plot](bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.11.0.md)
- [📈time plot](bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.12.0.md)
- [📈time plot](bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4513535079)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48.json)

### vs. 3.10.4

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.10.4.md)
- [📈time plot](bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.11x slower (HPT: reliability of 100.00%, 1.07x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.11.0.md)
- [📈time plot](bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.16x slower (HPT: reliability of 100.00%, 1.12x slower at 99th %ile)
- Memory usage: 0.87x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.12.0.md)
- [📈time plot](bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4483410660)
- cpu model: missing
- platform: Windows-10-10.0.22000-SP0
- [raw results](bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48.json)

### vs. 3.10.4

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.10.4.md)
- [📈time plot](bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.11.0.md)
- [📈time plot](bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.13x slower (HPT: reliability of 100.00%, 1.07x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.12.0.md)
- [📈time plot](bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.12.0.png)

