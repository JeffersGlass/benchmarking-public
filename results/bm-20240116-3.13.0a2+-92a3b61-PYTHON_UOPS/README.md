# Results

- fork: faster-cpython
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [92a3b61](https://github.com/faster%2dcpython/cpython/commit/92a3b61)
- commit date: 2024-01-16T16:39:33+00:00
- commit merge base: [ac10947ba79a15bfdaa3ca92c6864214648ab364](https://github.com/faster%2dcpython/cpython/commit/ac10947ba79a15bfdaa3ca92c6864214648ab364)
- ref: cold_exits

## linux x86_64 (azure)

- [pystats raw](bm-20240116-azure-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-pystats.json)
- [pystats table](bm-20240116-azure-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-pystats.md)

### vs. base

- [pystats diff](bm-20240116-azure-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7544748039)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-3.10.4.md)
- [📈time plot](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 97.95%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-3.11.0.md)
- [📈time plot](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-3.12.0.md)
- [📈time plot](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 90.27%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-base-mem.png)
- [📄table](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-base.md)
- [📈time plot](bm-20240116-linux-x86_64-faster%252dcpython-cold_exits-3.13.0a2%2B-92a3b61-vs-base.png)

