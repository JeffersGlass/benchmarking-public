# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [42374f4](https://github.com/faster%2dcpython/cpython/commit/42374f4)
- commit date: 2024-01-17T23:40:23+00:00
- commit merge base: [d1b031cc58516e1aba823fd613528417a996f50d](https://github.com/faster%2dcpython/cpython/commit/d1b031cc58516e1aba823fd613528417a996f50d)
- ref: remove_pep_523_check

## linux x86_64 (azure)

- [pystats raw](bm-20240117-azure-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-pystats.json)
- [pystats table](bm-20240117-azure-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-pystats.md)

### vs. base

- [pystats diff](bm-20240117-azure-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7625605053)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-3.10.4.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 91.10%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-3.11.0.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.96%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-3.12.0.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 98.95%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-base-mem.png)
- [📄table](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-base.md)
- [📈time plot](bm-20240117-linux-x86_64-faster%252dcpython-remove_pep_523_check-3.13.0a3%2B-42374f4-vs-base.png)

