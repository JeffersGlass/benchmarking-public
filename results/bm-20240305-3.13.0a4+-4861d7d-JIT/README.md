# Results

- fork: Fidget-Spinner
- version: 3.13.0a4+
- tier 2: False
- jit: True
- commit hash: [4861d7d](https://github.com/Fidget%2dSpinner/cpython/commit/4861d7d)
- commit date: 2024-03-05T03:07:55+08:00
- commit merge base: [ffed8d985b57a97def2ec40c61b71a22a2af1b48](https://github.com/Fidget%2dSpinner/cpython/commit/ffed8d985b57a97def2ec40c61b71a22a2af1b48)
- ref: tier2_superinstructi

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8145868526)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d.json)

### vs. 3.10.4

- Geometric mean: 1.30x faster (HPT: reliability of 100.00%, 1.22x faster at 99th %ile)
- Memory usage: 1.34x
- missing benchmarks: 2to3, aiohttp, chameleon, django_template, djangocms, docutils, flaskblogging, generators, genshi_text, genshi_xml, gunicorn, html5lib, pickle_pure_python, pylint, scimark_fft, scimark_lu, scimark_monte_carlo, scimark_sor, scimark_sparse_mat_mult, sqlalchemy_declarative, sqlalchemy_imperative, telco, thrift, unpickle
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-3.10.4.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.04x faster (HPT: reliability of 99.76%, 1.00x faster at 99th %ile)
- Memory usage: 1.24x
- missing benchmarks: 2to3, aiohttp, chameleon, django_template, djangocms, docutils, flaskblogging, generators, genshi_text, genshi_xml, gunicorn, html5lib, pickle_pure_python, pylint, scimark_fft, scimark_lu, scimark_monte_carlo, scimark_sor, scimark_sparse_mat_mult, sqlalchemy_declarative, sqlalchemy_imperative, telco, thrift, unpickle
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-3.11.0.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.01x faster (HPT: reliability of 98.90%, 1.00x faster at 99th %ile)
- Memory usage: 1.17x
- missing benchmarks: 2to3, aiohttp, chameleon, django_template, docutils, generators, gunicorn, pickle_pure_python, scimark_fft, scimark_lu, scimark_monte_carlo, scimark_sor, scimark_sparse_mat_mult, sqlalchemy_declarative, sqlalchemy_imperative, telco, unpickle
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-3.12.0.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.00x faster (HPT: reliability of 94.61%, 1.00x faster at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: 🔴 2to3, chameleon, docutils, generators, pickle_pure_python, scimark_fft, scimark_lu, scimark_monte_carlo, scimark_sor, scimark_sparse_mat_mult, telco, unpickle
- [🧠memory plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-base-mem.png)
- [📄table](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-base.md)
- [📈time plot](bm-20240305-linux-x86_64-Fidget%252dSpinner-tier2_superinstructi-3.13.0a4%2B-4861d7d-vs-base.png)

