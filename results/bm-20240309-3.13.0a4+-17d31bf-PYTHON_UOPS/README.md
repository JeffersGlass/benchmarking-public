# Results

- fork: python
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [17d31bf](https://github.com/python/cpython/commit/17d31bf)
- commit date: 2024-03-09T23:50:28+00:00
- commit merge base: [db8f423f58e336eb6180a70d9886b443d7203c2c](https://github.com/python/cpython/commit/db8f423f58e336eb6180a70d9886b443d7203c2c)
- ref: 17d31bf3843c38487399

## linux x86_64 (azure)

- [pystats raw](bm-20240309-azure-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-pystats.json)
- [pystats table](bm-20240309-azure-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-pystats.md)

### vs. base

- [pystats diff](bm-20240309-azure-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png)
- [📄table](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-linux-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-97-generic-x86_64-with-glibc2.35
- [raw results](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.06x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x slower (HPT: reliability of 99.96%, 1.02x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.14x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: 0.89x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.13x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png)
- [📄table](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: missing
- platform: Windows-11-10.0.22631-SP0
- [raw results](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.11x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x slower (HPT: reliability of 52.09%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.50%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: missing
- platform: Windows-11-10.0.22631-SP0
- [raw results](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: unknown
- [📄table](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8218012503)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf.json)

### vs. 3.10.4

- Geometric mean: 1.09x faster (HPT: reliability of 99.83%, 1.01x faster at 99th %ile)
- Memory usage: 1.13x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.12x slower (HPT: reliability of 100.00%, 1.07x slower at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png)
- [📄table](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)
- [📈time plot](bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)

