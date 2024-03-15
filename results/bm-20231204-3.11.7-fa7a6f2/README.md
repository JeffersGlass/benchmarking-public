# Results

- fork: python
- version: 3.11.7
- tier 2: False
- jit: False
- commit hash: [fa7a6f2](https://github.com/python/cpython/commit/fa7a6f2)
- commit date: 2023-12-04T17:56:29+00:00
- ref: fa7a6f23036537567592, v3.11.7

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265497583)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.07x
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.md)
- [📈time plot](bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [📄table](bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.md)
- [📈time plot](bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 92.51%, 1.00x faster at 99th %ile)
- Memory usage: 0.95x
- new benchmarks: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.md)
- [📈time plot](bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265497583)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2.json)

### vs. 3.10.4

- Geometric mean: 1.22x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.08x
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.md)
- [📈time plot](bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.99%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [📄table](bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.md)
- [📈time plot](bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.90x
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.md)
- [📈time plot](bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265497583)
- cpu model: missing
- platform: Windows-10-10.0.22621-SP0
- [raw results](bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: unknown
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.md)
- [📈time plot](bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.md)
- [📈time plot](bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 98.71%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.md)
- [📈time plot](bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7583587711)
- cpu model: missing
- platform: Windows-10-10.0.22621-SP0
- [raw results](bm-20231204-pythonperf1_win32-x86-python-fa7a6f23036537567592-3.11.7-fa7a6f2.json)

### vs. 3.10.4

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: unknown
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231204-pythonperf1_win32-x86-python-fa7a6f23036537567592-3.11.7-fa7a6f2-vs-3.10.4.md)
- [📈time plot](bm-20231204-pythonperf1_win32-x86-python-fa7a6f23036537567592-3.11.7-fa7a6f2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20231204-pythonperf1_win32-x86-python-fa7a6f23036537567592-3.11.7-fa7a6f2-vs-3.11.0.md)
- [📈time plot](bm-20231204-pythonperf1_win32-x86-python-fa7a6f23036537567592-3.11.7-fa7a6f2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: unknown
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231204-pythonperf1_win32-x86-python-fa7a6f23036537567592-3.11.7-fa7a6f2-vs-3.12.0.md)
- [📈time plot](bm-20231204-pythonperf1_win32-x86-python-fa7a6f23036537567592-3.11.7-fa7a6f2-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265497583)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.06x
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.md)
- [📈time plot](bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- [📄table](bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.md)
- [📈time plot](bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.01%, 1.00x faster at 99th %ile)
- Memory usage: 0.97x
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.md)
- [📈time plot](bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2-vs-3.12.0.png)

