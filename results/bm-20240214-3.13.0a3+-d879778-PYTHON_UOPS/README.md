# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [d879778](https://github.com/faster%2dcpython/cpython/commit/d879778)
- commit date: 2024-02-14T21:08:25+00:00
- commit merge base: [32f8ab1ab65c13ed70f047ffd780ec1fe303ff1e](https://github.com/faster%2dcpython/cpython/commit/32f8ab1ab65c13ed70f047ffd780ec1fe303ff1e)
- ref: split_on_oparg_1

## linux x86_64 (azure)

- [pystats raw](bm-20240214-azure-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-pystats.json)

### vs. base

- [pystats diff](bm-20240214-azure-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7918451871)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-3.10.4.md)
- [📈time plot](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 89.45%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-3.11.0.md)
- [📈time plot](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.94%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-3.12.0.md)
- [📈time plot](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-base-mem.png)
- [📄table](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-base.md)
- [📈time plot](bm-20240214-linux-x86_64-faster%252dcpython-split_on_oparg_1-3.13.0a3%2B-d879778-vs-base.png)

