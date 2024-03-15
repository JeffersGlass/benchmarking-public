
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.17x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.28x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 175 ms: 1.09x faster                                                             |
| chameleon      | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                            |
| docutils       | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                           |
| tornado_http   | 86.7 ms                                                | 71.0 ms: 1.22x faster                                                            |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 252 ms: 1.54x faster                                                             |
| async_tree_memoization  | 474 ms                                                 | 328 ms: 1.44x faster                                                             |
| async_tree_io           | 980 ms                                                 | 698 ms: 1.40x faster                                                             |
| async_tree_cpu_io_mixed | 649 ms                                                 | 519 ms: 1.25x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 74.8 ms: 1.24x faster                                                            |
| float          | 69.0 ms                                                | 55.7 ms: 1.24x faster                                                            |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                  | 1.15x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 76.2 ms: 1.25x faster                                                            |
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                             |
| regex_effbot   | 2.46 ms                                                | 2.57 ms: 1.05x slower                                                            |
| Geometric mean | (ref)                                                  | 1.08x faster                                                                     |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.43x faster                                                             |
| json_dumps           | 8.11 ms                                                | 6.58 ms: 1.23x faster                                                            |
| unpickle_pure_python | 194 us                                                 | 160 us: 1.21x faster                                                             |
| tomli_loads          | 1.71 sec                                               | 1.41 sec: 1.21x faster                                                           |
| xml_etree_process    | 46.5 ms                                                | 39.4 ms: 1.18x faster                                                            |
| unpickle             | 8.80 us                                                | 9.07 us: 1.03x slower                                                            |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                                            |
| xml_etree_generate   | 53.5 ms                                                | 55.7 ms: 1.04x slower                                                            |
| pickle               | 6.97 us                                                | 7.36 us: 1.05x slower                                                            |
| xml_etree_iterparse  | 72.1 ms                                                | 76.4 ms: 1.06x slower                                                            |
| pickle_dict          | 17.0 us                                                | 18.2 us: 1.07x slower                                                            |
| pickle_list          | 2.74 us                                                | 2.99 us: 1.09x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.09 us: 1.15x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                                     |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.1 ms: 1.21x slower                                                            |
| python_startup_no_site | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.34x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.94 ms: 1.24x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 72.0 us: 4.48x faster                                                            |
| deltablue                | 4.91 ms                                                | 2.52 ms: 1.95x faster                                                            |
| raytrace                 | 301 ms                                                 | 177 ms: 1.70x faster                                                             |
| logging_silent           | 117 ns                                                 | 70.0 ns: 1.67x faster                                                            |
| asyncio_tcp              | 659 ms                                                 | 404 ms: 1.63x faster                                                             |
| richards_super           | 57.8 ms                                                | 35.7 ms: 1.62x faster                                                            |
| chaos                    | 65.8 ms                                                | 41.9 ms: 1.57x faster                                                            |
| sqlglot_parse            | 1.24 ms                                                | 796 us: 1.56x faster                                                             |
| async_tree_none          | 388 ms                                                 | 252 ms: 1.54x faster                                                             |
| richards                 | 48.7 ms                                                | 31.9 ms: 1.53x faster                                                            |
| sqlglot_transpile        | 1.44 ms                                                | 980 us: 1.47x faster                                                             |
| crypto_pyaes             | 71.8 ms                                                | 49.3 ms: 1.46x faster                                                            |
| async_tree_memoization   | 474 ms                                                 | 328 ms: 1.44x faster                                                             |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.43x faster                                                             |
| async_tree_io            | 980 ms                                                 | 698 ms: 1.40x faster                                                             |
| unpack_sequence          | 39.0 ns                                                | 28.3 ns: 1.38x faster                                                            |
| go                       | 151 ms                                                 | 110 ms: 1.37x faster                                                             |
| scimark_lu               | 103 ms                                                 | 75.1 ms: 1.37x faster                                                            |
| deepcopy_memo            | 34.7 us                                                | 25.9 us: 1.34x faster                                                            |
| comprehensions           | 16.9 us                                                | 12.7 us: 1.33x faster                                                            |
| scimark_monte_carlo      | 65.6 ms                                                | 49.4 ms: 1.33x faster                                                            |
| pyflate                  | 427 ms                                                 | 328 ms: 1.30x faster                                                             |
| chameleon                | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                            |
| logging_simple           | 4.45 us                                                | 3.49 us: 1.28x faster                                                            |
| logging_format           | 4.83 us                                                | 3.80 us: 1.27x faster                                                            |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.27 sec: 1.26x faster                                                           |
| pycparser                | 877 ms                                                 | 697 ms: 1.26x faster                                                             |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 519 ms: 1.25x faster                                                             |
| regex_compile            | 95.3 ms                                                | 76.2 ms: 1.25x faster                                                            |
| nbody                    | 93.0 ms                                                | 74.8 ms: 1.24x faster                                                            |
| mako                     | 9.87 ms                                                | 7.94 ms: 1.24x faster                                                            |
| float                    | 69.0 ms                                                | 55.7 ms: 1.24x faster                                                            |
| json_dumps               | 8.11 ms                                                | 6.58 ms: 1.23x faster                                                            |
| tornado_http             | 86.7 ms                                                | 71.0 ms: 1.22x faster                                                            |
| create_gc_cycles         | 860 us                                                 | 706 us: 1.22x faster                                                             |
| pprint_safe_repr         | 641 ms                                                 | 526 ms: 1.22x faster                                                             |
| unpickle_pure_python     | 194 us                                                 | 160 us: 1.21x faster                                                             |
| pprint_pformat           | 1.30 sec                                               | 1.07 sec: 1.21x faster                                                           |
| tomli_loads              | 1.71 sec                                               | 1.41 sec: 1.21x faster                                                           |
| hexiom                   | 6.19 ms                                                | 5.14 ms: 1.20x faster                                                            |
| deepcopy                 | 272 us                                                 | 226 us: 1.20x faster                                                             |
| sympy_sum                | 92.2 ms                                                | 76.7 ms: 1.20x faster                                                            |
| scimark_sor              | 128 ms                                                 | 107 ms: 1.20x faster                                                             |
| xml_etree_process        | 46.5 ms                                                | 39.4 ms: 1.18x faster                                                            |
| deepcopy_reduce          | 2.33 us                                                | 1.98 us: 1.18x faster                                                            |
| spectral_norm            | 94.8 ms                                                | 80.7 ms: 1.18x faster                                                            |
| docutils                 | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                           |
| dulwich_log              | 35.3 ms                                                | 30.1 ms: 1.17x faster                                                            |
| sympy_integrate          | 13.1 ms                                                | 11.3 ms: 1.16x faster                                                            |
| sympy_str                | 165 ms                                                 | 143 ms: 1.16x faster                                                             |
| generators               | 32.3 ms                                                | 28.1 ms: 1.15x faster                                                            |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                             |
| mypy2                    | 607 ms                                                 | 529 ms: 1.15x faster                                                             |
| dask                     | 253 ms                                                 | 226 ms: 1.12x faster                                                             |
| sympy_expand             | 269 ms                                                 | 241 ms: 1.11x faster                                                             |
| 2to3                     | 192 ms                                                 | 175 ms: 1.09x faster                                                             |
| coroutines               | 20.7 ms                                                | 19.3 ms: 1.07x faster                                                            |
| sqlglot_optimize         | 36.8 ms                                                | 34.9 ms: 1.05x faster                                                            |
| meteor_contest           | 77.7 ms                                                | 74.3 ms: 1.05x faster                                                            |
| scimark_fft              | 224 ms                                                 | 215 ms: 1.04x faster                                                             |
| bench_thread_pool        | 527 us                                                 | 506 us: 1.04x faster                                                             |
| json                     | 3.08 ms                                                | 2.97 ms: 1.04x faster                                                            |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.32 ms: 1.03x faster                                                            |
| sqlglot_normalize        | 190 ms                                                 | 185 ms: 1.03x faster                                                             |
| fannkuch                 | 303 ms                                                 | 295 ms: 1.02x faster                                                             |
| nqueens                  | 63.8 ms                                                | 62.8 ms: 1.02x faster                                                            |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                             |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                            |
| unpickle                 | 8.80 us                                                | 9.07 us: 1.03x slower                                                            |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                                            |
| xml_etree_generate       | 53.5 ms                                                | 55.7 ms: 1.04x slower                                                            |
| regex_effbot             | 2.46 ms                                                | 2.57 ms: 1.05x slower                                                            |
| pickle                   | 6.97 us                                                | 7.36 us: 1.05x slower                                                            |
| xml_etree_iterparse      | 72.1 ms                                                | 76.4 ms: 1.06x slower                                                            |
| pickle_dict              | 17.0 us                                                | 18.2 us: 1.07x slower                                                            |
| pickle_list              | 2.74 us                                                | 2.99 us: 1.09x slower                                                            |
| sqlite_synth             | 1.46 us                                                | 1.59 us: 1.09x slower                                                            |
| unpickle_list            | 2.69 us                                                | 3.09 us: 1.15x slower                                                            |
| coverage                 | 41.5 ms                                                | 48.0 ms: 1.16x slower                                                            |
| python_startup           | 10.9 ms                                                | 13.1 ms: 1.21x slower                                                            |
| bench_mp_pool            | 37.4 ms                                                | 47.4 ms: 1.27x slower                                                            |
| telco                    | 3.49 ms                                                | 4.59 ms: 1.32x slower                                                            |
| async_generators         | 231 ms                                                 | 306 ms: 1.32x slower                                                             |
| python_startup_no_site   | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.17x faster                                                                     |

Benchmark hidden because not significant (5): pathlib, xml_etree_parse, asyncio_websockets, regex_v8, mdp
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240130-3.13.0a3+-913d95b-JIT,PYTHON_UOPS/bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.28x