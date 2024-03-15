# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [9d22a48](https://github.com/faster%2dcpython/cpython/commit/9d22a48)
- commit date: 2024-01-17T22:32:47+00:00
- commit merge base: [d1b031cc58516e1aba823fd613528417a996f50d](https://github.com/faster%2dcpython/cpython/commit/d1b031cc58516e1aba823fd613528417a996f50d)
- ref: tier_2_inline_consts

## linux x86_64 (azure)

- [pystats raw](bm-20240117-azure-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-pystats.json)
- [pystats table](bm-20240117-azure-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-pystats.md)

### vs. base

- [pystats diff](bm-20240117-azure-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7610631691)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-3.10.4.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 94.21%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-3.11.0.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-3.12.0.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 90.27%, 1.00x faster at 99th %ile)
- Memory usage: 1.03x
- [🧠memory plot](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-base-mem.png)
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-base.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-tier_2_inline_consts-3.13.0a3%2B-9d22a48-vs-base.png)

