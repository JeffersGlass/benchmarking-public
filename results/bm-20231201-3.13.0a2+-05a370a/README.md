# Results

- fork: python
- version: 3.13.0a2+
- tier 2: False
- jit: False
- commit hash: [05a370a](https://github.com/python/cpython/commit/05a370a)
- commit date: 2023-12-01T17:05:56+01:00
- commit merge base: [a9073564ee50bc610e1fd36e45b0a5204618883a](https://github.com/python/cpython/commit/a9073564ee50bc610e1fd36e45b0a5204618883a)
- ref: 05a370abd6cdfe4b54be

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7290755702)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a.json)

### vs. 3.10.4

- Geometric mean: 1.35x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.md)
- [📈time plot](bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.98%, 1.01x faster at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.md)
- [📈time plot](bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.91x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.md)
- [📈time plot](bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7290755702)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.md)
- [📈time plot](bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.99%, 1.01x faster at 99th %ile)
- Memory usage: 0.97x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.md)
- [📈time plot](bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 94.60%, 1.00x slower at 99th %ile)
- Memory usage: 0.86x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.md)
- [📈time plot](bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7290755702)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.10x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.md)
- [📈time plot](bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.69%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.md)
- [📈time plot](bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 89.00%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.md)
- [📈time plot](bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7290755702)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a.json)

### vs. 3.10.4

- Geometric mean: 1.16x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.md)
- [📈time plot](bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.md)
- [📈time plot](bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.md)
- [📈time plot](bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2%2B-05a370a-vs-3.12.0.png)

