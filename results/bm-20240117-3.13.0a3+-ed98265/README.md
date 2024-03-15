# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [ed98265](https://github.com/faster%2dcpython/cpython/commit/ed98265)
- commit date: 2024-01-17T05:09:42+00:00
- commit merge base: [a571a2fd3fdaeafdfd71f3d80ed5a3b22b63d0f7](https://github.com/faster%2dcpython/cpython/commit/a571a2fd3fdaeafdfd71f3d80ed5a3b22b63d0f7)
- ref: split_end_for

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7572385965)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-3.10.4.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-3.11.0.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-3.12.0.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 76.26%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-base-mem.png)
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-base.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-split_end_for-3.13.0a3%2B-ed98265-vs-base.png)

