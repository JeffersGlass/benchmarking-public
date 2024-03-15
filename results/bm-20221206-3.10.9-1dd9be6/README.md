# Results

- fork: python
- version: 3.10.9
- tier 2: False
- jit: False
- commit hash: [1dd9be6](https://github.com/python/cpython/commit/1dd9be6)
- commit date: 2022-12-06T18:31:21+00:00
- ref: 1dd9be6584413fbfa823

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6.json)

### vs. 3.10.4

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.10.4.md)
- [📈time plot](bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.21x slower (HPT: reliability of 100.00%, 1.15x slower at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.11.0.md)
- [📈time plot](bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.20x slower (HPT: reliability of 100.00%, 1.13x slower at 99th %ile)
- Memory usage: 0.89x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift
- [📄table](bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.12.0.md)
- [📈time plot](bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.12.0.png)

## darwin arm64 (darwin)

- cpu model: missing
- platform: macOS-12.6-arm64-arm-64bit
- [raw results](bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6.json)

### vs. 3.10.4

- Geometric mean: 1.02x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.10.4.md)
- [📈time plot](bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.26x slower (HPT: reliability of 100.00%, 1.22x slower at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.11.0.md)
- [📈time plot](bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.19x slower (HPT: reliability of 100.00%, 1.14x slower at 99th %ile)
- Memory usage: 0.87x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift
- [📄table](bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.12.0.md)
- [📈time plot](bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.12.0.png)

