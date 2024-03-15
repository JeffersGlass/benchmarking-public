# Results

- fork: python
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [5a1b531](https://github.com/python/cpython/commit/5a1b531)
- commit date: 2023-12-03T23:45:56-05:00
- commit merge base: [09505c5c26d6a4c81b54786eb4196379e9cb223c](https://github.com/python/cpython/commit/09505c5c26d6a4c81b54786eb4196379e9cb223c)
- ref: 5a1b5316af648ae79bb9

## windows x86 (pythonperf1_win32)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7583592459)
- cpu model: missing
- platform: Windows-11-10.0.22621-SP0
- [raw results](bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2%2B-5a1b531.json)

### vs. 3.10.4

- Geometric mean: 1.15x slower (HPT: reliability of 100.00%, 1.07x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2%2B-5a1b531-vs-3.10.4.md)
- [📈time plot](bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2%2B-5a1b531-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x slower (HPT: reliability of 99.82%, 1.00x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2%2B-5a1b531-vs-3.11.0.md)
- [📈time plot](bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2%2B-5a1b531-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.14x slower (HPT: reliability of 100.00%, 1.07x slower at 99th %ile)
- Memory usage: unknown
- missing benchmarks: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2%2B-5a1b531-vs-3.12.0.md)
- [📈time plot](bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2%2B-5a1b531-vs-3.12.0.png)

