
# Results vs. 3.10.4

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: darwin-arm64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 153 ms: 1.25x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.17 ms: 1.50x faster                                                  |
| docutils       | 1.73 sec                                               | 1.43 sec: 1.21x faster                                                 |
| html5lib       | 42.4 ms                                                | 33.3 ms: 1.27x faster                                                  |
| tornado_http   | 86.7 ms                                                | 70.3 ms: 1.23x faster                                                  |
| Geometric mean | (ref)                                                  | 1.29x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_io           | 980 ms                                                 | 690 ms: 1.42x faster                                                   |
| async_tree_none         | 388 ms                                                 | 277 ms: 1.40x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 347 ms: 1.36x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 515 ms: 1.26x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 68.4 ms: 1.36x faster                                                  |
| float          | 69.0 ms                                                | 55.7 ms: 1.24x faster                                                  |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.19x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.6 ms: 1.29x faster                                                  |
| regex_dna      | 174 ms                                                 | 150 ms: 1.16x faster                                                   |
| regex_v8       | 17.1 ms                                                | 15.5 ms: 1.10x faster                                                  |
| Geometric mean | (ref)                                                  | 1.14x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| xml_etree_process    | 46.5 ms                                                | 34.0 ms: 1.37x faster                                                  |
| pickle_pure_python   | 281 us                                                 | 210 us: 1.34x faster                                                   |
| tomli_loads          | 1.71 sec                                               | 1.31 sec: 1.31x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 163 us: 1.20x faster                                                   |
| xml_etree_generate   | 53.5 ms                                                | 46.7 ms: 1.14x faster                                                  |
| xml_etree_parse      | 108 ms                                                 | 96.9 ms: 1.11x faster                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 67.1 ms: 1.08x faster                                                  |
| json_dumps           | 8.11 ms                                                | 7.56 ms: 1.07x faster                                                  |
| json_loads           | 16.4 us                                                | 15.5 us: 1.06x faster                                                  |
| unpickle             | 8.80 us                                                | 8.37 us: 1.05x faster                                                  |
| pickle_list          | 2.74 us                                                | 2.66 us: 1.03x faster                                                  |
| unpickle_list        | 2.69 us                                                | 2.77 us: 1.03x slower                                                  |
| pickle               | 6.97 us                                                | 7.17 us: 1.03x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                           |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.0 ms: 1.11x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 9.94 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.18x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 19.8 ms: 1.33x faster                                                  |
| genshi_xml      | 33.8 ms                                                | 28.1 ms: 1.20x faster                                                  |
| mako            | 9.87 ms                                                | 8.22 ms: 1.20x faster                                                  |
| genshi_text     | 17.3 ms                                                | 14.5 ms: 1.20x faster                                                  |
| Geometric mean  | (ref)                                                  | 1.23x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.68 ms: 1.83x faster                                                  |
| logging_silent           | 117 ns                                                 | 64.4 ns: 1.82x faster                                                  |
| scimark_sor              | 128 ms                                                 | 74.8 ms: 1.71x faster                                                  |
| richards                 | 48.7 ms                                                | 30.8 ms: 1.58x faster                                                  |
| richards_super           | 57.8 ms                                                | 36.8 ms: 1.57x faster                                                  |
| scimark_lu               | 103 ms                                                 | 67.9 ms: 1.52x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.17 ms: 1.50x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 48.1 ms: 1.49x faster                                                  |
| go                       | 151 ms                                                 | 102 ms: 1.47x faster                                                   |
| raytrace                 | 301 ms                                                 | 206 ms: 1.46x faster                                                   |
| pyflate                  | 427 ms                                                 | 294 ms: 1.45x faster                                                   |
| sqlglot_parse            | 1.24 ms                                                | 874 us: 1.42x faster                                                   |
| async_tree_io            | 980 ms                                                 | 690 ms: 1.42x faster                                                   |
| async_tree_none          | 388 ms                                                 | 277 ms: 1.40x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.03 ms: 1.40x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 47.2 ms: 1.39x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 69.2 ms: 1.37x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 34.0 ms: 1.37x faster                                                  |
| chaos                    | 65.8 ms                                                | 48.2 ms: 1.37x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.54 ms: 1.37x faster                                                  |
| thrift                   | 572 us                                                 | 419 us: 1.36x faster                                                   |
| async_tree_memoization   | 474 ms                                                 | 347 ms: 1.36x faster                                                   |
| nbody                    | 93.0 ms                                                | 68.4 ms: 1.36x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 477 ms: 1.34x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 210 us: 1.34x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 977 ms: 1.33x faster                                                   |
| django_template          | 26.4 ms                                                | 19.8 ms: 1.33x faster                                                  |
| pycparser                | 877 ms                                                 | 663 ms: 1.32x faster                                                   |
| tomli_loads              | 1.71 sec                                               | 1.31 sec: 1.31x faster                                                 |
| logging_format           | 4.83 us                                                | 3.72 us: 1.30x faster                                                  |
| regex_compile            | 95.3 ms                                                | 73.6 ms: 1.29x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.45 us: 1.29x faster                                                  |
| html5lib                 | 42.4 ms                                                | 33.3 ms: 1.27x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 515 ms: 1.26x faster                                                   |
| coroutines               | 20.7 ms                                                | 16.4 ms: 1.26x faster                                                  |
| 2to3                     | 192 ms                                                 | 153 ms: 1.25x faster                                                   |
| sqlglot_optimize         | 36.8 ms                                                | 29.5 ms: 1.25x faster                                                  |
| float                    | 69.0 ms                                                | 55.7 ms: 1.24x faster                                                  |
| tornado_http             | 86.7 ms                                                | 70.3 ms: 1.23x faster                                                  |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.19 ms: 1.23x faster                                                  |
| fannkuch                 | 303 ms                                                 | 247 ms: 1.23x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.43 sec: 1.21x faster                                                 |
| sqlalchemy_declarative   | 73.3 ms                                                | 60.5 ms: 1.21x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 28.7 us: 1.21x faster                                                  |
| async_generators         | 231 ms                                                 | 191 ms: 1.21x faster                                                   |
| scimark_fft              | 224 ms                                                 | 186 ms: 1.21x faster                                                   |
| unpack_sequence          | 39.0 ns                                                | 32.3 ns: 1.21x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 712 us: 1.21x faster                                                   |
| genshi_xml               | 33.8 ms                                                | 28.1 ms: 1.20x faster                                                  |
| mako                     | 9.87 ms                                                | 8.22 ms: 1.20x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 29.5 ms: 1.20x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 163 us: 1.20x faster                                                   |
| genshi_text              | 17.3 ms                                                | 14.5 ms: 1.20x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 160 ms: 1.19x faster                                                   |
| gunicorn                 | 1.30 ms                                                | 1.10 ms: 1.19x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.97 us: 1.19x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.2 ms: 1.18x faster                                                  |
| nqueens                  | 63.8 ms                                                | 54.3 ms: 1.17x faster                                                  |
| deepcopy                 | 272 us                                                 | 233 us: 1.16x faster                                                   |
| regex_dna                | 174 ms                                                 | 150 ms: 1.16x faster                                                   |
| comprehensions           | 16.9 us                                                | 14.6 us: 1.16x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 457 us: 1.15x faster                                                   |
| dask                     | 253 ms                                                 | 220 ms: 1.15x faster                                                   |
| sympy_str                | 165 ms                                                 | 144 ms: 1.15x faster                                                   |
| sympy_expand             | 269 ms                                                 | 235 ms: 1.15x faster                                                   |
| xml_etree_generate       | 53.5 ms                                                | 46.7 ms: 1.14x faster                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.00 ms: 1.14x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 81.0 ms: 1.14x faster                                                  |
| json                     | 3.08 ms                                                | 2.75 ms: 1.12x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.44 sec: 1.12x faster                                                 |
| generators               | 32.3 ms                                                | 29.0 ms: 1.11x faster                                                  |
| xml_etree_parse          | 108 ms                                                 | 96.9 ms: 1.11x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 15.5 ms: 1.10x faster                                                  |
| pylint                   | 277 ms                                                 | 251 ms: 1.10x faster                                                   |
| telco                    | 3.49 ms                                                | 3.18 ms: 1.10x faster                                                  |
| aiohttp                  | 1.22 ms                                                | 1.12 ms: 1.09x faster                                                  |
| flaskblogging            | 2.65 ms                                                | 2.45 ms: 1.08x faster                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 67.1 ms: 1.08x faster                                                  |
| sqlite_synth             | 1.46 us                                                | 1.36 us: 1.07x faster                                                  |
| json_dumps               | 8.11 ms                                                | 7.56 ms: 1.07x faster                                                  |
| json_loads               | 16.4 us                                                | 15.5 us: 1.06x faster                                                  |
| unpickle                 | 8.80 us                                                | 8.37 us: 1.05x faster                                                  |
| pathlib                  | 24.5 ms                                                | 23.4 ms: 1.05x faster                                                  |
| meteor_contest           | 77.7 ms                                                | 75.0 ms: 1.04x faster                                                  |
| pickle_list              | 2.74 us                                                | 2.66 us: 1.03x faster                                                  |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                   |
| asyncio_websockets       | 410 ms                                                 | 407 ms: 1.01x faster                                                   |
| typing_runtime_protocols | 323 us                                                 | 322 us: 1.00x faster                                                   |
| coverage                 | 41.5 ms                                                | 41.3 ms: 1.00x faster                                                  |
| gc_traversal             | 2.36 ms                                                | 2.38 ms: 1.01x slower                                                  |
| unpickle_list            | 2.69 us                                                | 2.77 us: 1.03x slower                                                  |
| pickle                   | 6.97 us                                                | 7.17 us: 1.03x slower                                                  |
| mdp                      | 1.63 sec                                               | 1.74 sec: 1.06x slower                                                 |
| python_startup           | 10.9 ms                                                | 12.0 ms: 1.11x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 41.8 ms: 1.12x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 9.94 ms: 1.26x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.21x faster                                                           |

Benchmark hidden because not significant (3): pickle_dict, regex_effbot, asyncio_tcp
Ignored benchmarks (1) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: mypy2
Ignored benchmarks (4) of results/bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.06x