# Results

- fork: python
- version: 3.11.0rc1
- tier 2: False
- jit: False
- commit hash: [41cb071](https://github.com/python/cpython/commit/41cb071)
- commit date: 2022-08-05T15:45:18+01:00
- ref: 41cb07120b7792eac641

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.md)
- [📈time plot](bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.md)
- [📈time plot](bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, create_gc_cycles, dask, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift
- [📄table](bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.md)
- [📈time plot](bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4513536357)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20220805-pythonperf2-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220805-pythonperf2-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.md)
- [📈time plot](bm-20220805-pythonperf2-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.97%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220805-pythonperf2-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.md)
- [📈time plot](bm-20220805-pythonperf2-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.66%, 1.00x slower at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220805-pythonperf2-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.md)
- [📈time plot](bm-20220805-pythonperf2-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4483411487)
- cpu model: missing
- platform: Windows-10-10.0.22000-SP0
- [raw results](bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.md)
- [📈time plot](bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.md)
- [📈time plot](bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 90.74%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.md)
- [📈time plot](bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961753819)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: dask, mypy2
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.md)
- [📈time plot](bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 75.05%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: dask, mypy2
- [📄table](bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.md)
- [📈time plot](bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.34%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: dask, mypy2
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.md)
- [📈time plot](bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.12.0.png)

