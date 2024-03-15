# Results

- fork: pvlkhn
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [3213e3a](https://github.com/pvlkhn/cpython/commit/3213e3a)
- commit date: 2024-02-11T03:04:59+02:00
- commit merge base: [b70a68fbd6b72a25b5ef430603e39c9e40f40d29](https://github.com/pvlkhn/cpython/commit/b70a68fbd6b72a25b5ef430603e39c9e40f40d29)
- ref: gh_115267

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7875687258)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a.json)

### vs. 3.10.4

- Geometric mean: 1.35x faster (HPT: reliability of 100.00%, 1.28x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-3.10.4.md)
- [📈time plot](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.06x faster (HPT: reliability of 99.99%, 1.01x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-3.11.0.md)
- [📈time plot](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-3.12.0.md)
- [📈time plot](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 100.00%, 1.00x slower at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-base-mem.png)
- [📄table](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-base.md)
- [📈time plot](bm-20240211-linux-x86_64-pvlkhn-gh_115267-3.13.0a3%2B-3213e3a-vs-base.png)

