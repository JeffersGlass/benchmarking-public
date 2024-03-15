# Results

- fork: python
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [f428c4d](https://github.com/python/cpython/commit/f428c4d)
- commit date: 2023-12-18T08:57:45+02:00
- commit merge base: [2b93f5224216d10f8119373e72b5c2b3984e0af6](https://github.com/python/cpython/commit/2b93f5224216d10f8119373e72b5c2b3984e0af6)
- ref: f428c4dafbfa2425ea05

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7583592680)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2%2B-f428c4d.json)

### vs. 3.10.4

- Geometric mean: 1.14x faster (HPT: reliability of 100.00%, 1.09x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2%2B-f428c4d-vs-3.10.4.md)
- [📈time plot](bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2%2B-f428c4d-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.25x faster (HPT: reliability of 100.00%, 1.21x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2%2B-f428c4d-vs-3.11.0.md)
- [📈time plot](bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2%2B-f428c4d-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.15x faster (HPT: reliability of 100.00%, 1.13x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2%2B-f428c4d-vs-3.12.0.md)
- [📈time plot](bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2%2B-f428c4d-vs-3.12.0.png)

