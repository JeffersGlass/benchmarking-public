
# Results vs. 3.12.0

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: darwin-arm64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.08x slower \*
- HPT reliability: 99.21%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 165 ms: 1.03x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.87 ms: 1.04x slower                                                 |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.01x slower                                                |
| tornado_http   | 69.3 ms                                                | 77.9 ms: 1.12x slower                                                 |
| Geometric mean | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 526 ms                                                 | 568 ms: 1.08x slower                                                  |
| async_tree_none         | 266 ms                                                 | 288 ms: 1.09x slower                                                  |
| async_tree_memoization  | 312 ms                                                 | 359 ms: 1.15x slower                                                  |
| async_tree_io           | 668 ms                                                 | 786 ms: 1.18x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.12x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.4 ms: 1.05x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| nbody          | 68.8 ms                                                | 73.1 ms: 1.06x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.46 ms: 1.07x faster                                                 |
| regex_compile  | 77.9 ms                                                | 76.4 ms: 1.02x faster                                                 |
| regex_v8       | 16.0 ms                                                | 16.8 ms: 1.05x slower                                                 |
| regex_dna      | 154 ms                                                 | 174 ms: 1.13x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 48.3 ms: 1.16x faster                                                 |
| json_loads           | 17.2 us                                                | 15.4 us: 1.12x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 96.5 ms: 1.10x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.75 us: 1.10x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 36.3 ms: 1.09x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.64 us: 1.09x faster                                                 |
| pickle_dict          | 18.1 us                                                | 16.8 us: 1.08x faster                                                 |
| unpickle             | 9.12 us                                                | 8.57 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 70.5 ms: 1.05x faster                                                 |
| pickle               | 7.23 us                                                | 7.26 us: 1.01x slower                                                 |
| tomli_loads          | 1.39 sec                                               | 1.52 sec: 1.09x slower                                                |
| pickle_pure_python   | 200 us                                                 | 223 us: 1.12x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 169 us: 1.12x slower                                                  |
| json_dumps           | 6.22 ms                                                | 7.61 ms: 1.22x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 8.93 ms: 1.05x faster                                                 |
| python_startup         | 11.4 ms                                                | 15.3 ms: 1.34x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.13x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 22.2 ms: 1.01x faster                                                 |
| mako            | 7.71 ms                                                | 8.15 ms: 1.06x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.02x slower                                                          |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators         | 304 ms                                                 | 197 ms: 1.54x faster                                                  |
| xml_etree_generate       | 55.8 ms                                                | 48.3 ms: 1.16x faster                                                 |
| sqlite_synth             | 1.57 us                                                | 1.37 us: 1.15x faster                                                 |
| telco                    | 3.68 ms                                                | 3.21 ms: 1.14x faster                                                 |
| json_loads               | 17.2 us                                                | 15.4 us: 1.12x faster                                                 |
| bench_mp_pool            | 44.9 ms                                                | 40.6 ms: 1.11x faster                                                 |
| xml_etree_parse          | 106 ms                                                 | 96.5 ms: 1.10x faster                                                 |
| unpickle_list            | 3.02 us                                                | 2.75 us: 1.10x faster                                                 |
| xml_etree_process        | 39.7 ms                                                | 36.3 ms: 1.09x faster                                                 |
| pickle_list              | 2.89 us                                                | 2.64 us: 1.09x faster                                                 |
| sqlglot_normalize        | 186 ms                                                 | 171 ms: 1.08x faster                                                  |
| pickle_dict              | 18.1 us                                                | 16.8 us: 1.08x faster                                                 |
| regex_effbot             | 2.64 ms                                                | 2.46 ms: 1.07x faster                                                 |
| json                     | 3.09 ms                                                | 2.88 ms: 1.07x faster                                                 |
| logging_simple           | 3.69 us                                                | 3.44 us: 1.07x faster                                                 |
| logging_format           | 3.98 us                                                | 3.74 us: 1.06x faster                                                 |
| unpickle                 | 9.12 us                                                | 8.57 us: 1.06x faster                                                 |
| nqueens                  | 62.4 ms                                                | 59.1 ms: 1.06x faster                                                 |
| xml_etree_iterparse      | 74.0 ms                                                | 70.5 ms: 1.05x faster                                                 |
| python_startup_no_site   | 9.37 ms                                                | 8.93 ms: 1.05x faster                                                 |
| spectral_norm            | 76.4 ms                                                | 72.9 ms: 1.05x faster                                                 |
| generators               | 31.1 ms                                                | 29.7 ms: 1.05x faster                                                 |
| float                    | 55.8 ms                                                | 53.4 ms: 1.05x faster                                                 |
| deepcopy_reduce          | 2.07 us                                                | 1.99 us: 1.04x faster                                                 |
| coroutines               | 19.2 ms                                                | 18.6 ms: 1.03x faster                                                 |
| sqlglot_optimize         | 34.0 ms                                                | 33.0 ms: 1.03x faster                                                 |
| 2to3                     | 169 ms                                                 | 165 ms: 1.03x faster                                                  |
| scimark_fft              | 195 ms                                                 | 190 ms: 1.03x faster                                                  |
| pprint_safe_repr         | 497 ms                                                 | 487 ms: 1.02x faster                                                  |
| regex_compile            | 77.9 ms                                                | 76.4 ms: 1.02x faster                                                 |
| pathlib                  | 24.2 ms                                                | 23.8 ms: 1.02x faster                                                 |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.08 ms: 1.02x faster                                                 |
| pprint_pformat           | 1.01 sec                                               | 996 ms: 1.01x faster                                                  |
| django_template          | 22.3 ms                                                | 22.2 ms: 1.01x faster                                                 |
| deepcopy                 | 235 us                                                 | 233 us: 1.01x faster                                                  |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| gc_traversal             | 2.40 ms                                                | 2.40 ms: 1.00x faster                                                 |
| pickle                   | 7.23 us                                                | 7.26 us: 1.01x slower                                                 |
| docutils                 | 1.50 sec                                               | 1.51 sec: 1.01x slower                                                |
| deepcopy_memo            | 27.7 us                                                | 27.9 us: 1.01x slower                                                 |
| dulwich_log              | 29.8 ms                                                | 30.2 ms: 1.01x slower                                                 |
| bench_thread_pool        | 504 us                                                 | 516 us: 1.02x slower                                                  |
| meteor_contest           | 71.7 ms                                                | 73.7 ms: 1.03x slower                                                 |
| chameleon                | 4.70 ms                                                | 4.87 ms: 1.04x slower                                                 |
| unpack_sequence          | 31.5 ns                                                | 32.6 ns: 1.04x slower                                                 |
| create_gc_cycles         | 701 us                                                 | 732 us: 1.04x slower                                                  |
| sympy_integrate          | 11.4 ms                                                | 11.9 ms: 1.05x slower                                                 |
| regex_v8                 | 16.0 ms                                                | 16.8 ms: 1.05x slower                                                 |
| raytrace                 | 212 ms                                                 | 223 ms: 1.05x slower                                                  |
| sympy_expand             | 241 ms                                                 | 254 ms: 1.06x slower                                                  |
| mako                     | 7.71 ms                                                | 8.15 ms: 1.06x slower                                                 |
| sympy_str                | 148 ms                                                 | 156 ms: 1.06x slower                                                  |
| nbody                    | 68.8 ms                                                | 73.1 ms: 1.06x slower                                                 |
| scimark_monte_carlo      | 45.0 ms                                                | 47.9 ms: 1.06x slower                                                 |
| logging_silent           | 76.4 ns                                                | 81.4 ns: 1.06x slower                                                 |
| fannkuch                 | 248 ms                                                 | 268 ms: 1.08x slower                                                  |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 568 ms: 1.08x slower                                                  |
| async_tree_none          | 266 ms                                                 | 288 ms: 1.09x slower                                                  |
| gunicorn                 | 1.15 ms                                                | 1.25 ms: 1.09x slower                                                 |
| sympy_sum                | 77.6 ms                                                | 84.5 ms: 1.09x slower                                                 |
| hexiom                   | 4.54 ms                                                | 4.95 ms: 1.09x slower                                                 |
| tomli_loads              | 1.39 sec                                               | 1.52 sec: 1.09x slower                                                |
| pycparser                | 677 ms                                                 | 742 ms: 1.10x slower                                                  |
| crypto_pyaes             | 51.9 ms                                                | 56.9 ms: 1.10x slower                                                 |
| pickle_pure_python       | 200 us                                                 | 223 us: 1.12x slower                                                  |
| pyflate                  | 316 ms                                                 | 354 ms: 1.12x slower                                                  |
| tornado_http             | 69.3 ms                                                | 77.9 ms: 1.12x slower                                                 |
| unpickle_pure_python     | 151 us                                                 | 169 us: 1.12x slower                                                  |
| scimark_sor              | 87.4 ms                                                | 98.4 ms: 1.13x slower                                                 |
| regex_dna                | 154 ms                                                 | 174 ms: 1.13x slower                                                  |
| mdp                      | 1.58 sec                                               | 1.81 sec: 1.14x slower                                                |
| scimark_lu               | 76.0 ms                                                | 87.1 ms: 1.15x slower                                                 |
| async_tree_memoization   | 312 ms                                                 | 359 ms: 1.15x slower                                                  |
| chaos                    | 42.5 ms                                                | 49.5 ms: 1.16x slower                                                 |
| async_tree_io            | 668 ms                                                 | 786 ms: 1.18x slower                                                  |
| deltablue                | 2.71 ms                                                | 3.26 ms: 1.20x slower                                                 |
| richards                 | 32.1 ms                                                | 39.0 ms: 1.21x slower                                                 |
| comprehensions           | 14.5 us                                                | 17.7 us: 1.22x slower                                                 |
| json_dumps               | 6.22 ms                                                | 7.61 ms: 1.22x slower                                                 |
| go                       | 102 ms                                                 | 130 ms: 1.28x slower                                                  |
| richards_super           | 36.0 ms                                                | 48.0 ms: 1.33x slower                                                 |
| python_startup           | 11.4 ms                                                | 15.3 ms: 1.34x slower                                                 |
| dask                     | 222 ms                                                 | 298 ms: 1.34x slower                                                  |
| sqlglot_transpile        | 1.02 ms                                                | 1.44 ms: 1.41x slower                                                 |
| sqlglot_parse            | 848 us                                                 | 1.28 ms: 1.50x slower                                                 |
| typing_runtime_protocols | 93.0 us                                                | 328 us: 3.53x slower                                                  |
| coverage                 | 38.9 ms                                                | 330 ms: 8.50x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.08x slower                                                          |
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json: flaskblogging, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 99.21% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.96x