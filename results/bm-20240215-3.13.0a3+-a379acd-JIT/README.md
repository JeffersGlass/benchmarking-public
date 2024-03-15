# Results

- fork: brandtbucher
- version: 3.13.0a3+
- tier 2: False
- jit: True
- commit hash: [a379acd](https://github.com/brandtbucher/cpython/commit/a379acd)
- commit date: 2024-02-15T16:57:53-08:00
- commit merge base: [4297d7301b97aba2e0df9f9cc5fa4010e53a8950](https://github.com/brandtbucher/cpython/commit/4297d7301b97aba2e0df9f9cc5fa4010e53a8950)
- ref: justin_relax

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7936250670)
- cpu model: missing
- platform: macOS-14.3-arm64-arm-64bit-Mach-O
- [raw results](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd.json)

### vs. 3.10.4

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.26x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-3.10.4.md)
- [📈time plot](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.18x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-3.11.0.md)
- [📈time plot](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 70.75%, 1.00x faster at 99th %ile)
- Memory usage: 1.14x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-3.12.0.md)
- [📈time plot](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 0.99x
- [🧠memory plot](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-base-mem.png)
- [📄table](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-base.md)
- [📈time plot](bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3%2B-a379acd-vs-base.png)

