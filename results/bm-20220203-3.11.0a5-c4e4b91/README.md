# Results

- fork: python
- version: 3.11.0a5
- tier 2: False
- jit: False
- commit hash: [c4e4b91](https://github.com/python/cpython/commit/c4e4b91)
- commit date: 2022-02-03T18:37:08+00:00
- commit merge base: [2d080347d74078a55c47715d232d1ab8dc8cd603](https://github.com/python/cpython/commit/2d080347d74078a55c47715d232d1ab8dc8cd603)
- ref: c4e4b91557f18f881f39, main

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-91-generic-x86_64-with-glibc2.31
- [raw results](bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91.json)

### vs. 3.10.4

- Geometric mean: 1.31x faster (HPT: reliability of 100.00%, 1.23x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.10.4.md)
- [📈time plot](bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 81.74%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, djangocms, docutils, flaskblogging, gc_traversal, generators, genshi_text, genshi_xml, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.11.0.md)
- [📈time plot](bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 83.25%, 1.00x faster at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: aiohttp, async_generators, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, bench_mp_pool, bench_thread_pool, comprehensions, coroutines, coverage, create_gc_cycles, dask, deepcopy, deepcopy_memo, deepcopy_reduce, docutils, gc_traversal, generators, gunicorn, mdp, mypy2, pprint_pformat, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, sqlglot_normalize, sqlglot_optimize, sqlglot_parse, sqlglot_transpile, tomli_loads, typing_runtime_protocols
- new benchmarks: html5lib, thrift
- [📄table](bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.12.0.md)
- [📈time plot](bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4513535495)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-67-generic-x86_64-with-glibc2.35
- [raw results](bm-20220203-pythonperf2-x86_64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91.json)

### vs. 3.10.4

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220203-pythonperf2-x86_64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.10.4.md)
- [📈time plot](bm-20220203-pythonperf2-x86_64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols
- [📄table](bm-20220203-pythonperf2-x86_64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.11.0.md)
- [📈time plot](bm-20220203-pythonperf2-x86_64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.11x slower (HPT: reliability of 100.00%, 1.07x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, thrift
- [📄table](bm-20220203-pythonperf2-x86_64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.12.0.md)
- [📈time plot](bm-20220203-pythonperf2-x86_64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/6961752719)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91.json)

### vs. 3.10.4

- Geometric mean: 1.07x slower (HPT: reliability of 98.40%, 1.00x slower at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: asyncio_websockets, mypy2
- [📄table](bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.10.4.md)
- [📈time plot](bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.32x slower (HPT: reliability of 100.00%, 1.25x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, mypy2
- [📄table](bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.11.0.md)
- [📈time plot](bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.28x slower (HPT: reliability of 100.00%, 1.21x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, mypy2
- new benchmarks: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.12.0.md)
- [📈time plot](bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.12.0.png)

