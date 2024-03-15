# Results

- fork: python
- version: 3.11.0b1
- tier 2: False
- jit: False
- commit hash: [8d32a5c](https://github.com/python/cpython/commit/8d32a5c)
- commit date: 2022-05-06T23:56:26+01:00
- commit merge base: [0e5fe7f9e9d3b995a7ccc4fae498e6eaf01027a0](https://github.com/python/cpython/commit/0e5fe7f9e9d3b995a7ccc4fae498e6eaf01027a0)
- commit date: 2022-05-06T22:56:26+00:00
- ref: 8d32a5c8c4e9c90b0a21, main

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-91-generic-x86_64-with-glibc2.31
- [raw results](bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c.json)

### vs. 3.10.4

- Geometric mean: 1.38x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.04x
- missing benchmarks: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.10.4.md)
- [📈time plot](bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 0.95x
- missing benchmarks: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.11.0.md)
- [📈time plot](bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.09x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 0.87x
- missing benchmarks: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
- new benchmarks: html5lib, thrift
- [📄table](bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.12.0.md)
- [📈time plot](bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4513535796)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c.json)

### vs. 3.10.4

- Geometric mean: 1.23x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.09x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.10.4.md)
- [📈time plot](bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.67%, 1.00x faster at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.11.0.md)
- [📈time plot](bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.91%, 1.00x slower at 99th %ile)
- Memory usage: 0.90x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.12.0.md)
- [📈time plot](bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4483411100)
- cpu model: missing
- platform: Windows-10-10.0.22000-SP0
- [raw results](bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c.json)

### vs. 3.10.4

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.10.4.md)
- [📈time plot](bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 99.91%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.11.0.md)
- [📈time plot](bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 99.60%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.12.0.md)
- [📈time plot](bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961753238)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c.json)

### vs. 3.10.4

- Geometric mean: 1.20x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: mypy2
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.10.4.md)
- [📈time plot](bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.94%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: mypy2
- [📄table](bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.11.0.md)
- [📈time plot](bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 99.68%, 1.00x faster at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: mypy2
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.12.0.md)
- [📈time plot](bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.12.0.png)

