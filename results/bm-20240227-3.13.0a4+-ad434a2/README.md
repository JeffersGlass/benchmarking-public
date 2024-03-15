# Results

- fork: iritkatriel
- version: 3.13.0a4+
- tier 2: False
- jit: False
- commit hash: [ad434a2](https://github.com/iritkatriel/cpython/commit/ad434a2)
- commit date: 2024-02-27T15:17:56+00:00
- commit merge base: [e3dedeae7abbeda0cb3f1d872ebbb914635d64f2](https://github.com/iritkatriel/cpython/commit/e3dedeae7abbeda0cb3f1d872ebbb914635d64f2)
- ref: expected_attrs

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8067109362)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2.json)

### vs. 3.10.4

- Geometric mean: 1.38x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-3.10.4.md)
- [📈time plot](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-3.11.0.md)
- [📈time plot](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-3.12.0.md)
- [📈time plot](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 97.18%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-base-mem.png)
- [📄table](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-base.md)
- [📈time plot](bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4%2B-ad434a2-vs-base.png)

