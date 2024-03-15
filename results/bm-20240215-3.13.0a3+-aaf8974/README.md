# Results

- fork: mdboom
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [aaf8974](https://github.com/mdboom/cpython/commit/aaf8974)
- commit date: 2024-02-15T17:19:06-05:00
- commit merge base: [ae460d450ab854ca66d509ef6971cfe1b6312405](https://github.com/mdboom/cpython/commit/ae460d450ab854ca66d509ef6971cfe1b6312405)
- ref: aa_test

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7933466342)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974.json)

### vs. 3.10.4

- Geometric mean: 1.37x faster (HPT: reliability of 100.00%, 1.30x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-3.10.4.md)
- [📈time plot](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-3.11.0.md)
- [📈time plot](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.05x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-3.12.0.md)
- [📈time plot](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 99.12%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-base-mem.png)
- [📄table](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-base.md)
- [📈time plot](bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3%2B-aaf8974-vs-base.png)

