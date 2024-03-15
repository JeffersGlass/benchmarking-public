
# Results vs. 3.10.4

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: darwin-arm64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 159 ms: 1.21x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.35 ms: 1.44x faster                                                 |
| docutils       | 1.73 sec                                               | 1.45 sec: 1.19x faster                                                |
| html5lib       | 42.4 ms                                                | 33.9 ms: 1.25x faster                                                 |
| tornado_http   | 86.7 ms                                                | 69.3 ms: 1.25x faster                                                 |
| Geometric mean | (ref)                                                  | 1.27x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 322 ms: 1.47x faster                                                  |
| async_tree_none         | 388 ms                                                 | 281 ms: 1.38x faster                                                  |
| async_tree_io           | 980 ms                                                 | 723 ms: 1.35x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 523 ms: 1.24x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.36x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 69.0 ms: 1.35x faster                                                 |
| float          | 69.0 ms                                                | 55.9 ms: 1.24x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.19x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.0 ms: 1.30x faster                                                 |
| regex_dna      | 174 ms                                                 | 148 ms: 1.18x faster                                                  |
| regex_v8       | 17.1 ms                                                | 15.0 ms: 1.14x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.44 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.15x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 201 us: 1.39x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 33.8 ms: 1.38x faster                                                 |
| json_dumps           | 8.11 ms                                                | 6.04 ms: 1.34x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 154 us: 1.26x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.42 sec: 1.21x faster                                                |
| xml_etree_parse      | 108 ms                                                 | 90.9 ms: 1.19x faster                                                 |
| xml_etree_generate   | 53.5 ms                                                | 46.0 ms: 1.16x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.52 us: 1.07x faster                                                 |
| unpickle             | 8.80 us                                                | 8.27 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 67.9 ms: 1.06x faster                                                 |
| json_loads           | 16.4 us                                                | 15.6 us: 1.05x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.70 us: 1.01x faster                                                 |
| pickle_dict          | 17.0 us                                                | 16.9 us: 1.00x faster                                                 |
| pickle               | 6.97 us                                                | 7.13 us: 1.02x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.3 ms: 1.04x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.36 ms: 1.18x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.11x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 20.0 ms: 1.32x faster                                                 |
| mako            | 9.87 ms                                                | 7.66 ms: 1.29x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 28.4 ms: 1.19x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.6 ms: 1.19x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.25x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| logging_silent           | 117 ns                                                 | 63.1 ns: 1.86x faster                                                 |
| deltablue                | 4.91 ms                                                | 2.75 ms: 1.79x faster                                                 |
| scimark_lu               | 103 ms                                                 | 67.4 ms: 1.53x faster                                                 |
| richards_super           | 57.8 ms                                                | 38.6 ms: 1.50x faster                                                 |
| richards                 | 48.7 ms                                                | 32.5 ms: 1.50x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 48.4 ms: 1.49x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 322 ms: 1.47x faster                                                  |
| raytrace                 | 301 ms                                                 | 207 ms: 1.46x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.35 ms: 1.44x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 201 us: 1.39x faster                                                  |
| async_tree_none          | 388 ms                                                 | 281 ms: 1.38x faster                                                  |
| thrift                   | 572 us                                                 | 415 us: 1.38x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 33.8 ms: 1.38x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 69.5 ms: 1.36x faster                                                 |
| async_tree_io            | 980 ms                                                 | 723 ms: 1.35x faster                                                  |
| chaos                    | 65.8 ms                                                | 48.6 ms: 1.35x faster                                                 |
| nbody                    | 93.0 ms                                                | 69.0 ms: 1.35x faster                                                 |
| json_dumps               | 8.11 ms                                                | 6.04 ms: 1.34x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 484 ms: 1.32x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 940 us: 1.32x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.68 ms: 1.32x faster                                                 |
| django_template          | 26.4 ms                                                | 20.0 ms: 1.32x faster                                                 |
| pprint_pformat           | 1.30 sec                                               | 990 ms: 1.32x faster                                                  |
| go                       | 151 ms                                                 | 114 ms: 1.32x faster                                                  |
| pycparser                | 877 ms                                                 | 668 ms: 1.31x faster                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.61 ms: 1.31x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.10 ms: 1.31x faster                                                 |
| regex_compile            | 95.3 ms                                                | 73.0 ms: 1.30x faster                                                 |
| pyflate                  | 427 ms                                                 | 331 ms: 1.29x faster                                                  |
| mako                     | 9.87 ms                                                | 7.66 ms: 1.29x faster                                                 |
| scimark_sor              | 128 ms                                                 | 100 ms: 1.28x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 27.3 us: 1.27x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 154 us: 1.26x faster                                                  |
| logging_format           | 4.83 us                                                | 3.85 us: 1.25x faster                                                 |
| tornado_http             | 86.7 ms                                                | 69.3 ms: 1.25x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 687 us: 1.25x faster                                                  |
| html5lib                 | 42.4 ms                                                | 33.9 ms: 1.25x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.58 us: 1.24x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 523 ms: 1.24x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 52.9 ms: 1.24x faster                                                 |
| float                    | 69.0 ms                                                | 55.9 ms: 1.24x faster                                                 |
| dulwich_log              | 35.3 ms                                                | 28.8 ms: 1.23x faster                                                 |
| deepcopy_reduce          | 2.33 us                                                | 1.92 us: 1.22x faster                                                 |
| scimark_fft              | 224 ms                                                 | 185 ms: 1.22x faster                                                  |
| 2to3                     | 192 ms                                                 | 159 ms: 1.21x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.42 sec: 1.21x faster                                                |
| sqlglot_optimize         | 36.8 ms                                                | 30.5 ms: 1.20x faster                                                 |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                                  |
| docutils                 | 1.73 sec                                               | 1.45 sec: 1.19x faster                                                |
| genshi_xml               | 33.8 ms                                                | 28.4 ms: 1.19x faster                                                 |
| genshi_text              | 17.3 ms                                                | 14.6 ms: 1.19x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.19x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 90.9 ms: 1.19x faster                                                 |
| async_generators         | 231 ms                                                 | 195 ms: 1.19x faster                                                  |
| regex_dna                | 174 ms                                                 | 148 ms: 1.18x faster                                                  |
| xml_etree_generate       | 53.5 ms                                                | 46.0 ms: 1.16x faster                                                 |
| fannkuch                 | 303 ms                                                 | 260 ms: 1.16x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 457 us: 1.16x faster                                                  |
| coroutines               | 20.7 ms                                                | 18.0 ms: 1.15x faster                                                 |
| nqueens                  | 63.8 ms                                                | 55.6 ms: 1.15x faster                                                 |
| unpack_sequence          | 39.0 ns                                                | 34.1 ns: 1.15x faster                                                 |
| sympy_expand             | 269 ms                                                 | 235 ms: 1.15x faster                                                  |
| sympy_str                | 165 ms                                                 | 144 ms: 1.14x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 167 ms: 1.14x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 15.0 ms: 1.14x faster                                                 |
| comprehensions           | 16.9 us                                                | 14.8 us: 1.14x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 81.5 ms: 1.13x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.43 sec: 1.12x faster                                                |
| json                     | 3.08 ms                                                | 2.82 ms: 1.09x faster                                                 |
| telco                    | 3.49 ms                                                | 3.20 ms: 1.09x faster                                                 |
| pylint                   | 277 ms                                                 | 255 ms: 1.08x faster                                                  |
| generators               | 32.3 ms                                                | 30.2 ms: 1.07x faster                                                 |
| unpickle_list            | 2.69 us                                                | 2.52 us: 1.07x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.27 us: 1.06x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 67.9 ms: 1.06x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.1 ms: 1.06x faster                                                 |
| json_loads               | 16.4 us                                                | 15.6 us: 1.05x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.42 us: 1.03x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 76.4 ms: 1.02x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.70 us: 1.01x faster                                                 |
| regex_effbot             | 2.46 ms                                                | 2.44 ms: 1.01x faster                                                 |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| typing_runtime_protocols | 323 us                                                 | 321 us: 1.01x faster                                                  |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                  |
| pickle_dict              | 17.0 us                                                | 16.9 us: 1.00x faster                                                 |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                 |
| pickle                   | 6.97 us                                                | 7.13 us: 1.02x slower                                                 |
| python_startup           | 10.9 ms                                                | 11.3 ms: 1.04x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.71 sec: 1.05x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 41.7 ms: 1.12x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.36 ms: 1.18x slower                                                 |
| dask                     | 253 ms                                                 | 322 ms: 1.27x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.20x faster                                                          |

Benchmark hidden because not significant (1): asyncio_tcp
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20221025-3.12.0a1-4ae1a0e/bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.05x