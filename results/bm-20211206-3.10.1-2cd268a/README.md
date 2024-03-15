# Results

- fork: python
- version: 3.10.1
- tier 2: False
- jit: False
- commit hash: [2cd268a](https://github.com/python/cpython/commit/2cd268a)
- commit date: 2021-12-06T18:23:39+00:00
- ref: 2cd268a3a9340346dd86

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4500950957)
- cpu model: missing
- platform: Windows-10-10.0.22000-SP0
- [raw results](bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a.json)

### vs. 3.10.4

- Geometric mean: 1.01x faster (HPT: reliability of 99.95%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a-vs-3.10.4.md)
- [📈time plot](bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.07x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a-vs-3.11.0.md)
- [📈time plot](bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.15x slower (HPT: reliability of 100.00%, 1.09x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a-vs-3.12.0.md)
- [📈time plot](bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a-vs-3.12.0.png)

