# Results

- fork: faster_cpython
- version: 3.9.10
- tier 2: False
- jit: False
- commit hash: [258cab1](https://github.com/faster_cpython/cpython/commit/258cab1)
- commit date: 2022-12-21T19:44:41-08:00
- ref: nogil

## linux x86_64 (linux)

- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1.json)

### vs. 3.10.4

- Geometric mean: 1.07x faster (HPT: reliability of 99.94%, 1.02x faster at 99th %ile)
- Memory usage: 1.47x
- missing benchmarks: asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1-vs-3.10.4.md)
- [📈time plot](bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.20x slower (HPT: reliability of 100.00%, 1.11x slower at 99th %ile)
- Memory usage: 1.42x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: mypy
- [📄table](bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1-vs-3.11.0.md)
- [📈time plot](bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.18x slower (HPT: reliability of 100.00%, 1.11x slower at 99th %ile)
- Memory usage: 1.36x
- missing benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
- new benchmarks: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift
- [📄table](bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1-vs-3.12.0.md)
- [📈time plot](bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1-vs-3.12.0.png)

