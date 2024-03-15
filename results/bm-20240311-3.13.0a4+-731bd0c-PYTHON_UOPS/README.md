# Results

- fork: faster-cpython
- version: 3.13.0a4+
- tier 2: True
- jit: False
- commit hash: [731bd0c](https://github.com/faster%2dcpython/cpython/commit/731bd0c)
- commit date: 2024-03-11T11:37:23+00:00
- commit merge base: [fdb2d90a274158aee23b526d972172bf41bd4b7e](https://github.com/faster%2dcpython/cpython/commit/fdb2d90a274158aee23b526d972172bf41bd4b7e)
- ref: fewer_escapes

## linux x86_64 (azure)

- [pystats raw](bm-20240311-azure-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-pystats.json)
- [pystats table](bm-20240311-azure-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-pystats.md)

### vs. base

- [pystats diff](bm-20240311-azure-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-pystats-vs-base.md)

## linux x86_64 (linux)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/8232643215)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-164-generic-x86_64-with-glibc2.31
- [raw results](bm-20240311-linux-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c.json)

### vs. 3.10.4

- Geometric mean: 1.21x faster (HPT: reliability of 100.00%, 1.12x faster at 99th %ile)
- Memory usage: 1.08x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240311-linux-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-vs-3.10.4.md)
- [📈time plot](bm-20240311-linux-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.05x slower (HPT: reliability of 100.00%, 1.03x slower at 99th %ile)
- Memory usage: 1.01x
- missing benchmarks: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240311-linux-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-vs-3.11.0.md)
- [📈time plot](bm-20240311-linux-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.08x slower (HPT: reliability of 100.00%, 1.04x slower at 99th %ile)
- Memory usage: 0.94x
- missing benchmarks: sqlalchemy_declarative, sqlalchemy_imperative
- new benchmarks: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift
- [📄table](bm-20240311-linux-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-vs-3.12.0.md)
- [📈time plot](bm-20240311-linux-x86_64-faster%252dcpython-fewer_escapes-3.13.0a4%2B-731bd0c-vs-3.12.0.png)

