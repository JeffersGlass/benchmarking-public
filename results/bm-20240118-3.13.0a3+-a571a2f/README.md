# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [a571a2f](https://github.com/python/cpython/commit/a571a2f)
- commit date: 2024-01-18T13:27:44+02:00
- commit merge base: [311d1e2701037952eaf75f993be76f3092c1f01c](https://github.com/python/cpython/commit/311d1e2701037952eaf75f993be76f3092c1f01c)
- ref: a571a2fd3fdaeafdfd71

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7572385965)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3%2B-a571a2f.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3%2B-a571a2f-vs-3.10.4.md)
- [📈time plot](bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3%2B-a571a2f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3%2B-a571a2f-vs-3.11.0.md)
- [📈time plot](bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3%2B-a571a2f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3%2B-a571a2f-vs-3.12.0.md)
- [📈time plot](bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3%2B-a571a2f-vs-3.12.0.png)

