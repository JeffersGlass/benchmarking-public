# Results

- fork: python
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [841eacd](https://github.com/python/cpython/commit/841eacd)
- commit date: 2024-01-26T05:49:37+09:00
- commit merge base: [ac5e53e15057bc0326a03f56e400ce345d1cebeb](https://github.com/python/cpython/commit/ac5e53e15057bc0326a03f56e400ce345d1cebeb)
- ref: 841eacd07646e643f87d

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7674631038)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.10.4.md)
- [📈time plot](bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.11.0.md)
- [📈time plot](bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.12.0.md)
- [📈time plot](bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7674631038)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.10.4.md)
- [📈time plot](bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.97%, 1.00x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.11.0.md)
- [📈time plot](bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 84.18%, 1.00x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.12.0.md)
- [📈time plot](bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7674631038)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit
- [raw results](bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.10.4.md)
- [📈time plot](bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 99.95%, 1.00x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.11.0.md)
- [📈time plot](bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 82.16%, 1.00x faster at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.12.0.md)
- [📈time plot](bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3%2B-841eacd-vs-3.12.0.png)

