# Results

- fork: faster-cpython
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [1054202](https://github.com/faster%2dcpython/cpython/commit/1054202)
- commit date: 2024-02-09T04:18:31+00:00
- commit merge base: [17689e3c41d9f61bcd1928b24d3c50c37ceaf3f2](https://github.com/faster%2dcpython/cpython/commit/17689e3c41d9f61bcd1928b24d3c50c37ceaf3f2)
- ref: watched_dict_stats

## linux x86_64 (azure)

- [pystats raw](bm-20240209-azure-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-pystats.json)
- [pystats table](bm-20240209-azure-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-pystats.md)

### vs. base

- [pystats diff](bm-20240209-azure-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7848013504)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.19x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-3.10.4.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 90.46%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-3.11.0.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.98%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-3.12.0.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-base-mem.png)
- [📄table](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-base.md)
- [📈time plot](bm-20240209-linux-x86_64-faster%252dcpython-watched_dict_stats-3.13.0a3%2B-1054202-vs-base.png)

