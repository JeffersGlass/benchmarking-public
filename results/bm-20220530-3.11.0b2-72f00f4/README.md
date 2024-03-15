# Results

- fork: python
- version: 3.11.0b2
- tier 2: False
- jit: False
- commit hash: [72f00f4](https://github.com/python/cpython/commit/72f00f4)
- commit date: 2022-05-30T22:18:15+01:00
- ref: 72f00f420afaba3bc873, v3.11.0b2

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4566178854)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4.json)

### vs. 3.10.4

- Geometric mean: 1.33x faster (HPT: reliability of 100.00%, 1.27x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.10.4.md)
- [📈time plot](bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.11.0.md)
- [📈time plot](bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.12.0.md)
- [📈time plot](bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4566178854)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.10.4.md)
- [📈time plot](bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.11.0.md)
- [📈time plot](bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.77%, 1.00x slower at 99th %ile)
- Memory usage: 0.90x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.12.0.md)
- [📈time plot](bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4566178854)
- cpu model: missing
- platform: Windows-10-10.0.22000-SP0
- [raw results](bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4.json)

### vs. 3.10.4

- Geometric mean: 1.09x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.10.4.md)
- [📈time plot](bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.11.0.md)
- [📈time plot](bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.12.0.md)
- [📈time plot](bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961753382)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: flaskblogging, mypy2
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.10.4.md)
- [📈time plot](bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 92.27%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: flaskblogging, mypy2
- [📄table](bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.11.0.md)
- [📈time plot](bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.82%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: mypy2
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.12.0.md)
- [📈time plot](bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.12.0.png)

