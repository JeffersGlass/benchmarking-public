# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [d5b3dec](https://github.com/brandtbucher/cpython/commit/d5b3dec)
- commit date: 2024-02-14T16:07:23-08:00
- commit merge base: [4297d7301b97aba2e0df9f9cc5fa4010e53a8950](https://github.com/brandtbucher/cpython/commit/4297d7301b97aba2e0df9f9cc5fa4010e53a8950)
- ref: justin_relax

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7910716457)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec.json)

### vs. 3.10.4

- Geometric mean: 1.34x faster (HPT: reliability of 100.00%, 1.26x faster at 99th %ile)
- Memory usage: 1.11x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.10.4.md)
- [📈time plot](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.99%, 1.01x faster at 99th %ile)
- Memory usage: 1.03x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.11.0.md)
- [📈time plot](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.03x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.12.0.md)
- [📈time plot](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.02x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-base-mem.png)
- [📄table](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-base.md)
- [📈time plot](bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-base.png)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7924830831)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.10.4.md)
- [📈time plot](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.11.0.md)
- [📈time plot](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 73.20%, 1.00x slower at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.12.0.md)
- [📈time plot](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 97.90%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-base-mem.png)
- [📄table](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-base.md)
- [📈time plot](bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-d5b3dec-vs-base.png)

