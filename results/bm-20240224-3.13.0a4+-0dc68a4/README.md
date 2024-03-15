# Results

- fork: faster-cpython
- version: 3.13.0a4+
- tier 2: False
- jit: False
- commit hash: [0dc68a4](https://github.com/faster%2dcpython/cpython/commit/0dc68a4)
- commit date: 2024-02-24T02:11:49+00:00
- commit merge base: [e2a3e4b7488aff6fdc704a0f258bc315e96c1d6e](https://github.com/faster%2dcpython/cpython/commit/e2a3e4b7488aff6fdc704a0f258bc315e96c1d6e)
- ref: inline_values

## linux x86_64 (azure)

- [pystats raw](bm-20240224-azure-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-pystats.json)
- [pystats table](bm-20240224-azure-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-pystats.md)

### vs. base

- [pystats diff](bm-20240224-azure-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8094586089)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-3.10.4.md)
- [📈time plot](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-3.11.0.md)
- [📈time plot](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-3.12.0.md)
- [📈time plot](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 99.85%, 1.00x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-base-mem.png)
- [📄table](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-base.md)
- [📈time plot](bm-20240224-linux-x86_64-faster%252dcpython-inline_values-3.13.0a4%2B-0dc68a4-vs-base.png)

