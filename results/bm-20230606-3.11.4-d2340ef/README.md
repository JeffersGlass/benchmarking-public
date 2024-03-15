# Results

- fork: python
- version: 3.11.4
- tier 2: False
- jit: False
- commit hash: [d2340ef](https://github.com/python/cpython/commit/d2340ef)
- commit date: 2023-06-06T23:00:27+01:00
- ref: d2340ef25721b6a72d45, v3.11.4

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/5204077606)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef.json)

### vs. 3.10.4

- Geometric mean: 1.32x faster (HPT: reliability of 100.00%, 1.27x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: asyncio_websockets, coverage, mypy2
- [📄table](bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.10.4.md)
- [📈time plot](bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
- [📄table](bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.11.0.md)
- [📈time plot](bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
- new benchmarks: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.12.0.md)
- [📈time plot](bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/5204077606)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef.json)

### vs. 3.10.4

- Geometric mean: 1.22x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: asyncio_websockets, coverage, mypy2
- [📄table](bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.10.4.md)
- [📈time plot](bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 60.29%, 1.00x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
- [📄table](bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.11.0.md)
- [📈time plot](bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.12.0.md)
- [📈time plot](bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/5204077606)
- cpu model: missing
- platform: Windows-10-10.0.22621-SP0
- [raw results](bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef.json)

### vs. 3.10.4

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: mypy2
- [📄table](bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef-vs-3.10.4.md)
- [📈time plot](bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.32%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2
- [📄table](bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef-vs-3.11.0.md)
- [📈time plot](bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef-vs-3.12.0.md)
- [📈time plot](bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961755333)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20230606-darwin-arm64-python-d2340ef25721b6a72d45-3.11.4-d2340ef.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: mypy2
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20230606-darwin-arm64-python-d2340ef25721b6a72d45-3.11.4-d2340ef-vs-3.10.4.md)
- [📈time plot](bm-20230606-darwin-arm64-python-d2340ef25721b6a72d45-3.11.4-d2340ef-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: mypy2
- [📄table](bm-20230606-darwin-arm64-python-d2340ef25721b6a72d45-3.11.4-d2340ef-vs-3.11.0.md)
- [📈time plot](bm-20230606-darwin-arm64-python-d2340ef25721b6a72d45-3.11.4-d2340ef-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.32%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: mypy2
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20230606-darwin-arm64-python-d2340ef25721b6a72d45-3.11.4-d2340ef-vs-3.12.0.md)
- [📈time plot](bm-20230606-darwin-arm64-python-d2340ef25721b6a72d45-3.11.4-d2340ef-vs-3.12.0.png)

