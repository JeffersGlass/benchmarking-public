# Results

- fork: python
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [17d31bf](https://github.com/python/cpython/commit/17d31bf)
- commit date: 2024-03-09T23:50:28+00:00
- commit merge base: [db8f423f58e336eb6180a70d9886b443d7203c2c](https://github.com/python/cpython/commit/db8f423f58e336eb6180a70d9886b443d7203c2c)
- ref: 17d31bf3843c38487399

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 66.72%, 1.00x slower at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 94.65%, 1.00x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.24x
- [🧠memory plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png)
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-97-generic-x86_64-with-glibc2.35
- [raw results](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.35x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 69.25%, 1.00x faster at 99th %ile)
- Memory usage: 1.25x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.25x
- [🧠memory plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png)
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: missing
- platform: Windows-11-10.0.22631-SP0
- [raw results](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 97.99%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: missing
- platform: Windows-11-10.0.22631-SP0
- [raw results](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.06x faster (HPT: reliability of 99.97%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: 2.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.89x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 98.97%, 1.00x slower at 99th %ile)
- Memory usage: 1.82x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.03x slower (HPT: reliability of 80.10%, 1.00x slower at 99th %ile)
- Memory usage: 1.80x
- [🧠memory plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png)
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

