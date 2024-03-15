# Results

- fork: Fidget-Spinner
- version: 3.13.0a3+
- tier 2: True
- jit: False
- commit hash: [6e55480](https://github.com/Fidget%2dSpinner/cpython/commit/6e55480)
- commit date: 2024-01-24T21:04:34+08:00
- commit merge base: [384429d1c0cf011dcf88d4043e0328de8b063c24](https://github.com/Fidget%2dSpinner/cpython/commit/384429d1c0cf011dcf88d4043e0328de8b063c24)
- ref: tier2_abstract_inter

## linux x86_64 (azure)

- [pystats raw](bm-20240124-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-pystats.json)
- [pystats table](bm-20240124-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-pystats.md)

### vs. base

- [pystats diff](bm-20240124-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7648665033)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480.json)

### vs. 3.10.4

- Geometric mean: 1.28x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: 1.06x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-3.10.4.md)
- [📈time plot](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.01x faster (HPT: reliability of 96.18%, 1.00x slower at 99th %ile)
- Memory usage: 0.99x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-3.11.0.md)
- [📈time plot](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.02x slower (HPT: reliability of 99.97%, 1.00x slower at 99th %ile)
- Memory usage: 0.93x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-3.12.0.md)
- [📈time plot](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x faster (HPT: reliability of 99.99%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-base-mem.png)
- [📄table](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-base.md)
- [📈time plot](bm-20240124-linux-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a3%2B-6e55480-vs-base.png)

