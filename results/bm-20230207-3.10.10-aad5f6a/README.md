# Results

- fork: python
- version: 3.10.10
- tier 2: False
- jit: False
- commit hash: [aad5f6a](https://github.com/python/cpython/commit/aad5f6a)
- commit date: 2023-02-07T12:05:45+00:00
- ref: aad5f6a89125ad4529ab, v3.10.10

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a.json)

### vs. 3.10.4

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a-vs-3.10.4.md)
- [📈time plot](bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.20x slower (HPT: reliability of 100.00%, 1.15x slower at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a-vs-3.11.0.md)
- [📈time plot](bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.20x slower (HPT: reliability of 100.00%, 1.13x slower at 99th %ile)
- Memory usage: 0.90x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a-vs-3.12.0.md)
- [📈time plot](bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4513537895)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a.json)

### vs. 3.10.4

- Geometric mean: 1.01x slower (HPT: reliability of 99.49%, 1.00x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.10.4.md)
- [📈time plot](bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.23x slower (HPT: reliability of 100.00%, 1.16x slower at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.11.0.md)
- [📈time plot](bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.29x slower (HPT: reliability of 100.00%, 1.23x slower at 99th %ile)
- Memory usage: 0.84x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.12.0.md)
- [📈time plot](bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4500951050)
- cpu model: missing
- platform: Windows-10-10.0.22000-SP0
- [raw results](bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a.json)

### vs. 3.10.4

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.10.4.md)
- [📈time plot](bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.11.0.md)
- [📈time plot](bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.15x slower (HPT: reliability of 100.00%, 1.09x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.12.0.md)
- [📈time plot](bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4494505736)
- cpu model: missing
- platform: macOS-13.2.1-arm64-arm-64bit
- [raw results](bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a.json)

### vs. 3.10.4

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.10.4.md)
- [📈time plot](bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.28x slower (HPT: reliability of 100.00%, 1.23x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.11.0.md)
- [📈time plot](bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.21x slower (HPT: reliability of 100.00%, 1.17x slower at 99th %ile)
- Memory usage: 0.90x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.12.0.md)
- [📈time plot](bm-20230207-darwin-arm64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a-vs-3.12.0.png)

