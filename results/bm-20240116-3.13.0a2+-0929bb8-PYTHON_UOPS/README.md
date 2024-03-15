# Results

- fork: Fidget-Spinner
- version: 3.13.0a2+
- tier 2: True
- jit: False
- commit hash: [0929bb8](https://github.com/Fidget%2dSpinner/cpython/commit/0929bb8)
- commit date: 2024-01-16T14:41:58+00:00
- commit merge base: [77b45fa6d0b8c0c14657b5117b21a3f3f2ce97d8](https://github.com/Fidget%2dSpinner/cpython/commit/77b45fa6d0b8c0c14657b5117b21a3f3f2ce97d8)
- ref: tier2_abstract_inter

## linux x86_64 (azure)

- [pystats raw](bm-20240116-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-pystats.json)
- [pystats table](bm-20240116-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-pystats.md)

### vs. base

- [pystats diff](bm-20240116-azure-x86_64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-pystats-vs-base.md)

## darwin arm64 (darwin)

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/7559538614)
- cpu model: missing
- platform: macOS-14.2.1-arm64-arm-64bit
- [raw results](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8.json)

### vs. 3.10.4

- Geometric mean: 1.12x faster (HPT: reliability of 100.00%, 1.04x faster at 99th %ile)
- Memory usage: 1.41x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- new benchmarks: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg
- [📄table](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-3.10.4.md)
- [📈time plot](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-3.10.4.png)

### vs. 3.11.0

- Geometric mean: 1.09x slower (HPT: reliability of 100.00%, 1.05x slower at 99th %ile)
- Memory usage: 1.31x
- missing benchmarks: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
- [📄table](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-3.11.0.md)
- [📈time plot](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-3.11.0.png)

### vs. 3.12.0

- Geometric mean: 1.06x slower (HPT: reliability of 100.00%, 1.02x slower at 99th %ile)
- Memory usage: 1.27x
- missing benchmarks: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
- [📄table](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-3.12.0.md)
- [📈time plot](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-3.12.0.png)

### vs. base

- Geometric mean: 1.01x slower (HPT: reliability of 98.63%, 1.00x slower at 99th %ile)
- Memory usage: 1.27x
- [🧠memory plot](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-base-mem.png)
- [📄table](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-base.md)
- [📈time plot](bm-20240116-darwin-arm64-Fidget%252dSpinner-tier2_abstract_inter-3.13.0a2%2B-0929bb8-vs-base.png)

