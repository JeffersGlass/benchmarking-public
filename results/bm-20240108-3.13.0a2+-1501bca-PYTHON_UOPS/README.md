# Results

- fork: faster-cpython
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [1501bca](https://github.com/faster%2dcpython/cpython/commit/1501bca)
- commit date: 2024-01-08T00:36:09+00:00
- commit merge base: [b3dba18eab96dc95653031863bb2a222af912f2b](https://github.com/faster%2dcpython/cpython/commit/b3dba18eab96dc95653031863bb2a222af912f2b)
- ref: guarantee_forward_pr

## linux x86_64 (azure)

- [pystats raw](bm-20240108-azure-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-pystats.json)
- [pystats table](bm-20240108-azure-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-pystats.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7459912480)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240108-linux-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca.json)

### vs. 3.10.4

- Geometric mean: 1.27x faster (HPT: reliability of 100.00%, 1.20x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240108-linux-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-vs-3.10.4.md)
- [📈time plot](bm-20240108-linux-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.00x faster (HPT: reliability of 97.27%, 1.00x slower at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240108-linux-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-vs-3.11.0.md)
- [📈time plot](bm-20240108-linux-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240108-linux-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-vs-3.12.0.md)
- [📈time plot](bm-20240108-linux-x86_64-faster%252dcpython-guarantee_forward_pr-3.13.0a2%2B-1501bca-vs-3.12.0.png)

