# Results

- fork: brandtbucher
- version: 3.13.0a2+
- tier 2: False
- jit: True
- commit hash: [b63610e](https://github.com/brandtbucher/cpython/commit/b63610e)
- commit date: 2023-12-19T15:28:31-08:00
- commit merge base: [2feec0fc7fd0b9caae7ab2e26e69311d3ed93e77](https://github.com/brandtbucher/cpython/commit/2feec0fc7fd0b9caae7ab2e26e69311d3ed93e77)
- ref: justin

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7269649687)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.10x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.md)
- [📈time plot](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 50.23%, 1.00x slower at 99th %ile)
- Memory usage: 1.02x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.md)
- [📈time plot](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x slower (HPT: reliability of 88.74%, 1.00x slower at 99th %ile)
- Memory usage: 0.96x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.md)
- [📈time plot](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.04x
- [🧠memory plot](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base-mem.png)
- [📄table](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base.md)
- [📈time plot](bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base.png)

## linux x86_64 (pythonperf2)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7269649687)
- cpu model: 12th Gen Intel(R) Core(TM) i9-12900
- platform: Linux-5.15.0-88-generic-x86_64-with-glibc2.35
- [raw results](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e.json)

### vs. 3.10.4

- Geometric mean: 1.24x faster (HPT: reliability of 100.00%, 1.17x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.md)
- [📈time plot](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.02x faster (HPT: reliability of 67.51%, 1.00x faster at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.md)
- [📈time plot](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.md)
- [📈time plot](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.04x
- [🧠memory plot](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base-mem.png)
- [📄table](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base.md)
- [📈time plot](bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base.png)

## windows amd64 (pythonperf1)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7269649687)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2%2B-b63610e.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.md)
- [📈time plot](bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.md)
- [📈time plot](bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x faster (HPT: reliability of 99.97%, 1.00x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.md)
- [📈time plot](bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7269649687)
- cpu model: missing
- platform: macOS-14.1.1-arm64-arm-64bit
- [raw results](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e.json)

### vs. 3.10.4

- Geometric mean: 1.13x faster (HPT: reliability of 100.00%, 1.07x faster at 99th %ile)
- Memory usage: 1.27x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.md)
- [📈time plot](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.06x slower at 99th %ile)
- Memory usage: 1.19x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.md)
- [📈time plot](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.15x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.md)
- [📈time plot](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 1.16x
- [🧠memory plot](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base-mem.png)
- [📄table](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base.md)
- [📈time plot](bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2%2B-b63610e-vs-base.png)

