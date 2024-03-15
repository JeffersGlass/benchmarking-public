# Results

- fork: faster-cpython
- version: 3.12.0a4
- tier 2: False
- jit: False
- commit hash: [1d39009](https://github.com/faster%2dcpython/cpython/commit/1d39009)
- commit date: 2023-04-16T13:41:10-07:00
- commit merge base: [3d5d3f7af6498effbc60a3db1d2b5f41ae6c0a75](https://github.com/faster%2dcpython/cpython/commit/3d5d3f7af6498effbc60a3db1d2b5f41ae6c0a75)
- ref: nogil_latest

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4744083530)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009.json)

### vs. 3.10.4

- Geometric mean: 1.26x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.44x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, dask, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.10.4.md)
- [📈time plot](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 99.82%, 1.00x slower at 99th %ile)
- Memory usage: 1.35x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, dask, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.11.0.md)
- [📈time plot](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 87.85%, 1.00x slower at 99th %ile)
- Memory usage: 1.27x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, dask, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.12.0.md)
- [📈time plot](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.08x slower at 99th %ile)
- Memory usage: 1.33x
- missing benchmarks: 🔴 dask
- [🧠memory plot](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-base-mem.png)
- [📄table](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-base.md)
- [📈time plot](bm-20230416-linux-x86_64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4744088784)
- cpu model: missing
- platform: Windows-11-10.0.22000-SP0
- [raw results](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009.json)

### vs. 3.10.4

- Geometric mean: 1.09x faster (HPT: reliability of 99.99%, 1.02x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, dask, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.10.4.md)
- [📈time plot](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.95%, 1.01x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, dask, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.11.0.md)
- [📈time plot](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 99.99%, 1.03x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, dask, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.12.0.md)
- [📈time plot](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.17x slower (HPT: reliability of 100.00%, 1.14x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: 🔴 dask
- [📄table](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-base.md)
- [📈time plot](bm-20230416-pythonperf1-amd64-faster%252dcpython-nogil_latest-3.12.0a4-1d39009-vs-base.png)

