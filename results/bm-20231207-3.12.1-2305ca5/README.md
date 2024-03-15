# Results

- fork: python
- version: 3.12.1
- tier 2: False
- jit: False
- commit hash: [2305ca5](https://github.com/python/cpython/commit/2305ca5)
- commit date: 2023-12-07T21:46:47+01:00
- ref: 2305ca51448552542b24, v3.12.1

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265490302)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.md)
- [📈time plot](bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 74.91%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.md)
- [📈time plot](bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.10%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- [📄table](bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.md)
- [📈time plot](bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265490302)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.md)
- [📈time plot](bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.md)
- [📈time plot](bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 0.91x
- [📄table](bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.md)
- [📈time plot](bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265490302)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.md)
- [📈time plot](bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.md)
- [📈time plot](bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.md)
- [📈time plot](bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7583587818)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20231207-pythonperf1_win32-x86-python-2305ca51448552542b24-3.12.1-2305ca5.json)

### vs. 3.10.4

- Geometric mean: 1.01x faster (HPT: reliability of 72.17%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231207-pythonperf1_win32-x86-python-2305ca51448552542b24-3.12.1-2305ca5-vs-3.10.4.md)
- [📈time plot](bm-20231207-pythonperf1_win32-x86-python-2305ca51448552542b24-3.12.1-2305ca5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.11x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231207-pythonperf1_win32-x86-python-2305ca51448552542b24-3.12.1-2305ca5-vs-3.11.0.md)
- [📈time plot](bm-20231207-pythonperf1_win32-x86-python-2305ca51448552542b24-3.12.1-2305ca5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20231207-pythonperf1_win32-x86-python-2305ca51448552542b24-3.12.1-2305ca5-vs-3.12.0.md)
- [📈time plot](bm-20231207-pythonperf1_win32-x86-python-2305ca51448552542b24-3.12.1-2305ca5-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7265490302)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.md)
- [📈time plot](bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.93%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.md)
- [📈time plot](bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.92%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- [📄table](bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.md)
- [📈time plot](bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5-vs-3.12.0.png)

