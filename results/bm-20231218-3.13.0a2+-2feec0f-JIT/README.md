# Results

- fork: python
- version: 3.13.0a2+
- tier 2: False
- jit: True
- commit hash: [2feec0f](https://github.com/python/cpython/commit/2feec0f)
- commit date: 2023-12-18T17:04:40+00:00
- commit merge base: [d00dbf541525fcb36c9c6ebb7b41a5637c5aa6c0](https://github.com/python/cpython/commit/d00dbf541525fcb36c9c6ebb7b41a5637c5aa6c0)
- ref: 2feec0fc7fd0b9caae7a

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7269649687)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.10.4.md)
- [📈time plot](bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.11.0.md)
- [📈time plot](bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.12.0.md)
- [📈time plot](bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.12.0.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7269649687)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f.json)

### vs. 3.10.4

- Geometric mean: 1.29x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.10.4.md)
- [📈time plot](bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 99.79%, 1.00x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.11.0.md)
- [📈time plot](bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 95.13%, 1.00x slower at 99th %ile)
- Memory usage: 0.88x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.12.0.md)
- [📈time plot](bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7269649687)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f.json)

### vs. 3.10.4

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.10.4.md)
- [📈time plot](bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.11.0.md)
- [📈time plot](bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.12.0.md)
- [📈time plot](bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2%2B-2feec0f-vs-3.12.0.png)

