# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [9f32fb0](https://github.com/faster%2dcpython/cpython/commit/9f32fb0)
- commit date: 2024-02-03T13:36:25+00:00
- commit merge base: [0e71a295e9530c939a5efcb45db23cf31e0303b4](https://github.com/faster%2dcpython/cpython/commit/0e71a295e9530c939a5efcb45db23cf31e0303b4)
- ref: abstract_interpreter

## linux x86_64 (azure)

- [pystats raw](bm-20240203-azure-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-pystats.json)
- [pystats table](bm-20240203-azure-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-pystats.md)

### vs. base

- [pystats diff](bm-20240203-azure-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7785913785)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-3.10.4.md)
- [📈time plot](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 89.85%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-3.11.0.md)
- [📈time plot](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.87%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-3.12.0.md)
- [📈time plot](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 99.54%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: 🔴 mypy2
- [🧠memory plot](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-base-mem.png)
- [📄table](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-base.md)
- [📈time plot](bm-20240203-linux-x86_64-faster%252dcpython-abstract_interpreter-3.13.0a3%2B-9f32fb0-vs-base.png)

