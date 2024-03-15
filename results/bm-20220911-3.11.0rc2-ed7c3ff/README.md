# Results

- fork: python
- version: 3.11.0rc2
- tier 2: False
- jit: False
- commit hash: [ed7c3ff](https://github.com/python/cpython/commit/ed7c3ff)
- commit date: 2022-09-11T20:23:30+01:00
- ref: ed7c3ff15680c1939fad

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json)

### vs. 3.10.4

- Geometric mean: 1.35x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.md)
- [📈time plot](bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.md)
- [📈time plot](bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift
- [📄table](bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.md)
- [📈time plot](bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4513536491)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.md)
- [📈time plot](bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x slower (HPT: reliability of 96.75%, 1.00x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.md)
- [📈time plot](bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.md)
- [📈time plot](bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4483411552)
- cpu model: missing
- platform: Windows-10-10.0.22000-SP0
- [raw results](bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json)

### vs. 3.10.4

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.md)
- [📈time plot](bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.md)
- [📈time plot](bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 87.08%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.md)
- [📈time plot](bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961753940)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: mypy2
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.md)
- [📈time plot](bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 87.32%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: mypy2
- [📄table](bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.md)
- [📈time plot](bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.62%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: mypy2
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.md)
- [📈time plot](bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.12.0.png)

