# Results

- fork: mdboom
- version: 3.13.0a3+
- tier 2: False
- jit: False
- commit hash: [f5a8425](https://github.com/mdboom/cpython/commit/f5a8425)
- commit date: 2024-01-23T11:14:08-05:00
- commit merge base: [05e47202a34e6ae05e699af1083455f5b8b59496](https://github.com/mdboom/cpython/commit/05e47202a34e6ae05e699af1083455f5b8b59496)
- ref: rare_event_stats

## linux x86_64 (azure)

- [pystats raw](bm-20240123-azure-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-pystats.json)
- [pystats table](bm-20240123-azure-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-pystats.md)

### vs. base

- [pystats diff](bm-20240123-azure-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7628637062)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425.json)

### vs. 3.10.4

- Geometric mean: 1.36x faster (HPT: reliability of 100.00%, 1.29x faster at 99th %ile)
- Memory usage: 1.05x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-3.10.4.md)
- [📈time plot](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.07x faster (HPT: reliability of 100.00%, 1.01x faster at 99th %ile)
- Memory usage: 0.98x
- missing benchmarks: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-3.11.0.md)
- [📈time plot](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.04x faster (HPT: reliability of 100.00%, 1.02x faster at 99th %ile)
- Memory usage: 0.92x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-3.12.0.md)
- [📈time plot](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 52.52%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-base-mem.png)
- [📄table](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-base.md)
- [📈time plot](bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3%2B-f5a8425-vs-base.png)

