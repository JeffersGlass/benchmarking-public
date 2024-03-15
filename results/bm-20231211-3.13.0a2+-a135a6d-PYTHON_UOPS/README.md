# Results

- fork: python
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [a135a6d](https://github.com/python/cpython/commit/a135a6d)
- commit date: 2023-12-11T11:44:22+00:00
- commit merge base: [4c5b9c107a1d158b245f21a1839a2bec97d05383](https://github.com/python/cpython/commit/4c5b9c107a1d158b245f21a1839a2bec97d05383)
- ref: a135a6d2c6d503b18669

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7583592652)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20231211-pythonperf1_win32-x86-python-a135a6d2c6d503b18669-3.13.0a2%2B-a135a6d.json)

### vs. 3.10.4

- Geometric mean: 1.08x faster (HPT: reliability of 100.00%, 1.03x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231211-pythonperf1_win32-x86-python-a135a6d2c6d503b18669-3.13.0a2%2B-a135a6d-vs-3.10.4.md)
- [📈time plot](bm-20231211-pythonperf1_win32-x86-python-a135a6d2c6d503b18669-3.13.0a2%2B-a135a6d-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.19x faster (HPT: reliability of 100.00%, 1.16x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231211-pythonperf1_win32-x86-python-a135a6d2c6d503b18669-3.13.0a2%2B-a135a6d-vs-3.11.0.md)
- [📈time plot](bm-20231211-pythonperf1_win32-x86-python-a135a6d2c6d503b18669-3.13.0a2%2B-a135a6d-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.09x faster (HPT: reliability of 100.00%, 1.08x faster at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231211-pythonperf1_win32-x86-python-a135a6d2c6d503b18669-3.13.0a2%2B-a135a6d-vs-3.12.0.md)
- [📈time plot](bm-20231211-pythonperf1_win32-x86-python-a135a6d2c6d503b18669-3.13.0a2%2B-a135a6d-vs-3.12.0.png)

