# Results

- fork: faster-cpython
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [4d59a84](https://github.com/faster%2dcpython/cpython/commit/4d59a84)
- commit date: 2024-02-09T07:44:44+00:00
- commit merge base: [35ef8cb25917bfd6cbbd7c2bb55dd4f82131c9cf](https://github.com/faster%2dcpython/cpython/commit/35ef8cb25917bfd6cbbd7c2bb55dd4f82131c9cf)
- ref: better_set_ip_check_

## linux x86_64 (azure)

- [pystats raw](bm-20240209-azure-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-pystats.json)
- [pystats table](bm-20240209-azure-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-pystats.md)

### vs. base

- [pystats diff](bm-20240209-azure-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7855691461)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-3.10.4.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 95.68%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-3.11.0.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.99%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-3.12.0.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-base-mem.png)
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-base.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-better_set_ip_check_-3.13.0a2%2B-4d59a84-vs-base.png)

