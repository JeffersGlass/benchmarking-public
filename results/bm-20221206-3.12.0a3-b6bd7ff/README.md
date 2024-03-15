# Results

- fork: python
- version: 3.12.0a3
- tier 2: False
- jit: False
- commit hash: [b6bd7ff](https://github.com/python/cpython/commit/b6bd7ff)
- commit date: 2022-12-06T19:33:02+01:00
- commit merge base: [fd38a2f0ec03b4eec5e3cfd41241d198b1ee555a](https://github.com/python/cpython/commit/fd38a2f0ec03b4eec5e3cfd41241d198b1ee555a)
- ref: b6bd7ffcbc1ffaa68e34

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4556038398)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.md)
- [📈time plot](bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.md)
- [📈time plot](bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.md)
- [📈time plot](bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4556038398)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.18x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.md)
- [📈time plot](bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.50%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.md)
- [📈time plot](bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.88%, 1.00x slower at 99th %ile)
- Memory usage: 0.90x
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.md)
- [📈time plot](bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4556038398)
- cpu model: missing
- platform: Windows-11-10.0.22000-SP0
- [raw results](bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json)

### vs. 3.10.4

- Geometric mean: 1.22x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.md)
- [📈time plot](bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.09x faster (HPT: reliability of 100.00%, 1.05x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- [📄table](bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.md)
- [📈time plot](bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.md)
- [📈time plot](bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961754461)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json)

### vs. 3.10.4

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.11x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.md)
- [📈time plot](bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
- [📄table](bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.md)
- [📈time plot](bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.32%, 1.00x slower at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, coverage, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
- new benchmarks: genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.md)
- [📈time plot](bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff-vs-3.12.0.png)

