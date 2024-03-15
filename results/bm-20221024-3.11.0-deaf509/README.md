# Results

- fork: python
- version: 3.11.0
- tier 2: False
- jit: False
- commit hash: [deaf509](https://github.com/python/cpython/commit/deaf509)
- commit date: 2022-10-24T18:35:39+01:00
- ref: v3.11.0

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7646927066)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.07x
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.md)
- [📈time plot](bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 79.60%, 1.00x faster at 99th %ile)
- Memory usage: 0.95x
- new benchmarks: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.md)
- [📈time plot](bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7646927066)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.08x
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.md)
- [📈time plot](bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.90x
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.md)
- [📈time plot](bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7646927066)
- cpu model: missing
- platform: Windows-10-10.0.22621-SP0
- [raw results](bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json)

### vs. 3.10.4

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.md)
- [📈time plot](bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: unknown
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.md)
- [📈time plot](bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7646927066)
- cpu model: missing
- platform: Windows-10-10.0.22621-SP0
- [raw results](bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json)

### vs. 3.10.4

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: unknown
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.md)
- [📈time plot](bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.png)

### vs. 3.12.0

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: unknown
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.md)
- [📈time plot](bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7646927066)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit
- [raw results](bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.07x
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.md)
- [📈time plot](bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.md)
- [📈time plot](bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509-vs-3.12.0.png)

