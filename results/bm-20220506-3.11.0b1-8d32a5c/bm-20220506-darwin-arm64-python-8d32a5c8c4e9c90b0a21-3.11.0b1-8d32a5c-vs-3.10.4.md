
# Results vs. 3.10.4

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: darwin-arm64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 152 ms: 1.26x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.32 ms: 1.45x faster                                                 |
| docutils       | 1.73 sec                                               | 1.39 sec: 1.25x faster                                                |
| html5lib       | 42.4 ms                                                | 31.0 ms: 1.36x faster                                                 |
| tornado_http   | 86.7 ms                                                | 69.4 ms: 1.25x faster                                                 |
| Geometric mean | (ref)                                                  | 1.31x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_io           | 980 ms                                                 | 690 ms: 1.42x faster                                                  |
| async_tree_none         | 388 ms                                                 | 277 ms: 1.40x faster                                                  |
| async_tree_memoization  | 474 ms                                                 | 353 ms: 1.34x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 514 ms: 1.26x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.35x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 65.6 ms: 1.42x faster                                                 |
| float          | 69.0 ms                                                | 53.3 ms: 1.30x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.23x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.1 ms: 1.30x faster                                                 |
| regex_dna      | 174 ms                                                 | 144 ms: 1.21x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.26 ms: 1.09x faster                                                 |
| regex_v8       | 17.1 ms                                                | 15.8 ms: 1.09x faster                                                 |
| Geometric mean | (ref)                                                  | 1.17x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 34.2 ms: 1.36x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.31 sec: 1.30x faster                                                |
| unpickle_pure_python | 194 us                                                 | 152 us: 1.28x faster                                                  |
| xml_etree_generate   | 53.5 ms                                                | 46.9 ms: 1.14x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 97.3 ms: 1.11x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.55 us: 1.07x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 67.2 ms: 1.07x faster                                                 |
| json_dumps           | 8.11 ms                                                | 7.57 ms: 1.07x faster                                                 |
| json_loads           | 16.4 us                                                | 15.5 us: 1.06x faster                                                 |
| unpickle             | 8.80 us                                                | 8.32 us: 1.06x faster                                                 |
| pickle_dict          | 17.0 us                                                | 16.2 us: 1.05x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.77 us: 1.03x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                          |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.27 ms: 1.17x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.11x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 19.6 ms: 1.35x faster                                                 |
| mako            | 9.87 ms                                                | 8.18 ms: 1.21x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.5 ms: 1.20x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 28.7 ms: 1.18x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.23x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.71 ms: 1.82x faster                                                 |
| logging_silent           | 117 ns                                                 | 65.8 ns: 1.78x faster                                                 |
| scimark_sor              | 128 ms                                                 | 78.2 ms: 1.64x faster                                                 |
| richards                 | 48.7 ms                                                | 31.1 ms: 1.56x faster                                                 |
| richards_super           | 57.8 ms                                                | 37.4 ms: 1.54x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 47.8 ms: 1.50x faster                                                 |
| scimark_lu               | 103 ms                                                 | 68.4 ms: 1.50x faster                                                 |
| pyflate                  | 427 ms                                                 | 286 ms: 1.49x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 44.1 ms: 1.49x faster                                                 |
| raytrace                 | 301 ms                                                 | 203 ms: 1.48x faster                                                  |
| go                       | 151 ms                                                 | 104 ms: 1.45x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.32 ms: 1.45x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                  |
| async_tree_io            | 980 ms                                                 | 690 ms: 1.42x faster                                                  |
| nbody                    | 93.0 ms                                                | 65.6 ms: 1.42x faster                                                 |
| async_tree_none          | 388 ms                                                 | 277 ms: 1.40x faster                                                  |
| thrift                   | 572 us                                                 | 411 us: 1.39x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 68.2 ms: 1.39x faster                                                 |
| chaos                    | 65.8 ms                                                | 48.2 ms: 1.37x faster                                                 |
| html5lib                 | 42.4 ms                                                | 31.0 ms: 1.36x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 34.2 ms: 1.36x faster                                                 |
| hexiom                   | 6.19 ms                                                | 4.59 ms: 1.35x faster                                                 |
| django_template          | 26.4 ms                                                | 19.6 ms: 1.35x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 353 ms: 1.34x faster                                                  |
| pycparser                | 877 ms                                                 | 659 ms: 1.33x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 482 ms: 1.33x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 985 ms: 1.32x faster                                                  |
| logging_format           | 4.83 us                                                | 3.68 us: 1.31x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.41 us: 1.31x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.31 sec: 1.30x faster                                                |
| regex_compile            | 95.3 ms                                                | 73.1 ms: 1.30x faster                                                 |
| float                    | 69.0 ms                                                | 53.3 ms: 1.30x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 152 us: 1.28x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 514 ms: 1.26x faster                                                  |
| 2to3                     | 192 ms                                                 | 152 ms: 1.26x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 27.8 us: 1.25x faster                                                 |
| tornado_http             | 86.7 ms                                                | 69.4 ms: 1.25x faster                                                 |
| docutils                 | 1.73 sec                                               | 1.39 sec: 1.25x faster                                                |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.14 ms: 1.24x faster                                                 |
| scimark_fft              | 224 ms                                                 | 182 ms: 1.23x faster                                                  |
| sqlalchemy_declarative   | 73.3 ms                                                | 59.7 ms: 1.23x faster                                                 |
| coroutines               | 20.7 ms                                                | 16.9 ms: 1.23x faster                                                 |
| fannkuch                 | 303 ms                                                 | 247 ms: 1.23x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 28.9 ms: 1.22x faster                                                 |
| async_generators         | 231 ms                                                 | 190 ms: 1.21x faster                                                  |
| regex_dna                | 174 ms                                                 | 144 ms: 1.21x faster                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 30.5 ms: 1.21x faster                                                 |
| mako                     | 9.87 ms                                                | 8.18 ms: 1.21x faster                                                 |
| deepcopy_reduce          | 2.33 us                                                | 1.93 us: 1.20x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 715 us: 1.20x faster                                                  |
| genshi_text              | 17.3 ms                                                | 14.5 ms: 1.20x faster                                                 |
| deepcopy                 | 272 us                                                 | 228 us: 1.19x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 32.9 ns: 1.19x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 78.1 ms: 1.18x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.18x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 28.7 ms: 1.18x faster                                                 |
| nqueens                  | 63.8 ms                                                | 54.5 ms: 1.17x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.95 ms: 1.16x faster                                                 |
| sympy_expand             | 269 ms                                                 | 232 ms: 1.16x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 164 ms: 1.16x faster                                                  |
| sympy_str                | 165 ms                                                 | 143 ms: 1.16x faster                                                  |
| dask                     | 253 ms                                                 | 220 ms: 1.15x faster                                                  |
| xml_etree_generate       | 53.5 ms                                                | 46.9 ms: 1.14x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.29 ms: 1.12x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.43 sec: 1.12x faster                                                |
| flaskblogging            | 2.65 ms                                                | 2.38 ms: 1.11x faster                                                 |
| json                     | 3.08 ms                                                | 2.77 ms: 1.11x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 97.3 ms: 1.11x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 1.12 ms: 1.11x faster                                                 |
| aiohttp                  | 1.22 ms                                                | 1.11 ms: 1.10x faster                                                 |
| gunicorn                 | 1.30 ms                                                | 1.18 ms: 1.10x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 480 us: 1.10x faster                                                  |
| telco                    | 3.49 ms                                                | 3.18 ms: 1.10x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.33 us: 1.10x faster                                                 |
| pylint                   | 277 ms                                                 | 253 ms: 1.09x faster                                                  |
| regex_effbot             | 2.46 ms                                                | 2.26 ms: 1.09x faster                                                 |
| regex_v8                 | 17.1 ms                                                | 15.8 ms: 1.09x faster                                                 |
| generators               | 32.3 ms                                                | 29.9 ms: 1.08x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.55 us: 1.07x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 67.2 ms: 1.07x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 72.5 ms: 1.07x faster                                                 |
| json_dumps               | 8.11 ms                                                | 7.57 ms: 1.07x faster                                                 |
| json_loads               | 16.4 us                                                | 15.5 us: 1.06x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.1 ms: 1.06x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.32 us: 1.06x faster                                                 |
| pickle_dict              | 17.0 us                                                | 16.2 us: 1.05x faster                                                 |
| asyncio_websockets       | 410 ms                                                 | 407 ms: 1.01x faster                                                  |
| pidigits                 | 282 ms                                                 | 281 ms: 1.01x faster                                                  |
| gc_traversal             | 2.36 ms                                                | 2.38 ms: 1.01x slower                                                 |
| comprehensions           | 16.9 us                                                | 17.1 us: 1.01x slower                                                 |
| typing_runtime_protocols | 323 us                                                 | 327 us: 1.01x slower                                                  |
| unpickle_list            | 2.69 us                                                | 2.77 us: 1.03x slower                                                 |
| python_startup           | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.73 sec: 1.06x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 41.7 ms: 1.11x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.27 ms: 1.17x slower                                                 |
| coverage                 | 41.5 ms                                                | 73.6 ms: 1.77x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.20x faster                                                          |

Benchmark hidden because not significant (2): pickle, asyncio_tcp
Ignored benchmarks (1) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: mypy2
Ignored benchmarks (4) of results/bm-20220506-3.11.0b1-8d32a5c/bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.06x