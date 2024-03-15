# Results

- fork: faster-cpython
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [76389dd](https://github.com/faster%2dcpython/cpython/commit/76389dd)
- commit date: 2024-02-15T19:43:55+00:00
- commit merge base: [a2bb8ad14409c7ecb8dea437b0e281eb1f65b5d8](https://github.com/faster%2dcpython/cpython/commit/a2bb8ad14409c7ecb8dea437b0e281eb1f65b5d8)
- ref: load_attr_module_con

## linux x86_64 (azure)

- [pystats raw](bm-20240215-azure-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-pystats.json)
- [pystats table](bm-20240215-azure-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-pystats.md)

### vs. base

- [pystats diff](bm-20240215-azure-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7973053649)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.15x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-3.10.4.md)
- [📈time plot](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.83%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-3.11.0.md)
- [📈time plot](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-3.12.0.md)
- [📈time plot](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 80.94%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-base-mem.png)
- [📄table](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-base.md)
- [📈time plot](bm-20240215-linux-x86_64-faster%252dcpython-load_attr_module_con-3.13.0a4%2B-76389dd-vs-base.png)

