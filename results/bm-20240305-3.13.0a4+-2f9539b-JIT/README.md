# Results

- fork: gvanrossum
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [2f9539b](https://github.com/gvanrossum/cpython/commit/2f9539b)
- commit date: 2024-03-05T18:04:42-08:00
- commit merge base: [23db9c62272f7470aadf8f52fe3ebb42b5e5d380](https://github.com/gvanrossum/cpython/commit/23db9c62272f7470aadf8f52fe3ebb42b5e5d380)
- ref: kenjin_tier2_inliner

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8175263769)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.24x faster at 99th %ile)
- Memory usage: 1.34x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-3.10.4.md)
- [📈time plot](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.03x faster (HPT: reliability of 94.34%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-3.11.0.md)
- [📈time plot](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.00x faster (HPT: reliability of 98.99%, 1.00x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-3.12.0.md)
- [📈time plot](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x slower (HPT: reliability of 56.30%, 1.00x faster at 99th %ile)
- Memory usage: 1.00x
- [🧠memory plot](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-base-mem.png)
- [📄table](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-base.md)
- [📈time plot](bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4%2B-2f9539b-vs-base.png)

