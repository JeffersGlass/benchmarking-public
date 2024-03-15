# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [939c26f](https://github.com/faster%2dcpython/cpython/commit/939c26f)
- commit date: 2024-02-01T15:28:16+00:00
- commit merge base: [4dbb198d279a06fed74ea4c38f93d658baf38170](https://github.com/faster%2dcpython/cpython/commit/4dbb198d279a06fed74ea4c38f93d658baf38170)
- ref: abstract_interpreter

## linux x86_64 (azure)

- [pystats raw](bm-20240201-azure-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-pystats.json)
- [pystats table](bm-20240201-azure-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-pystats.md)

### vs. base

- [pystats diff](bm-20240201-azure-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7745893450)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f.json)

### vs. 3.10.4

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-3.10.4.md)
- [📈time plot](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x slower (HPT: reliability of 98.98%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-3.11.0.md)
- [📈time plot](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-3.12.0.md)
- [📈time plot](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 99.62%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-base-mem.png)
- [📄table](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-base.md)
- [📈time plot](bm-20240201-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-939c26f-vs-base.png)

