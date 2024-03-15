# Results

- fork: Fidget-Spinner
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [b04215f](https://github.com/Fidget%2dSpinner/cpython/commit/b04215f)
- commit date: 2024-03-05T03:07:34+08:00
- commit merge base: [ffed8d985b57a97def2ec40c61b71a22a2af1b48](https://github.com/Fidget%2dSpinner/cpython/commit/ffed8d985b57a97def2ec40c61b71a22a2af1b48)
- ref: tier2_inliner_redux

## linux x86_64 (azure)

- [pystats raw](bm-20240305-azure-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-pystats.json)
- [pystats table](bm-20240305-azure-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-pystats.md)

### vs. base

- [pystats diff](bm-20240305-azure-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8145881148)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f.json)

### vs. 3.10.4

- Geometric mean: 1.18x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: 1.07x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-3.10.4.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.00x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-3.11.0.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.10x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-3.12.0.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.04x slower (HPT: reliability of 100.00%, 1.01x slower at 99th %ile)
- Memory usage: 1.01x
- [🧠memory plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-base-mem.png)
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-base.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_inliner_redux-3.13.0a4%2B-b04215f-vs-base.png)

