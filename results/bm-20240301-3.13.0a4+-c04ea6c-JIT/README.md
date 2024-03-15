# Results

- fork: Fidget-Spinner
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [c04ea6c](https://github.com/Fidget%2dSpinner/cpython/commit/c04ea6c)
- commit date: 2024-03-01T06:40:12+08:00
- commit merge base: [75c6c05fea212330f4b0259602ffae1b2cb91be3](https://github.com/Fidget%2dSpinner/cpython/commit/75c6c05fea212330f4b0259602ffae1b2cb91be3)
- ref: tier2_superinstructi

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8104150029)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.34x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-3.10.4.md)
- [📈time plot](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 53.41%, 1.00x slower at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-3.11.0.md)
- [📈time plot](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x slower (HPT: reliability of 70.45%, 1.00x slower at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-3.12.0.md)
- [📈time plot](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 100.00%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-base-mem.png)
- [📄table](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-base.md)
- [📈time plot](bm-20240301-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-c04ea6c-vs-base.png)

