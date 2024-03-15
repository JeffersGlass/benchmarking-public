
# Results vs. 3.10.4

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: darwin-arm64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 160 ms: 1.20x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.29 ms: 1.46x faster                                                 |
| docutils       | 1.73 sec                                               | 1.43 sec: 1.21x faster                                                |
| html5lib       | 42.4 ms                                                | 33.4 ms: 1.27x faster                                                 |
| tornado_http   | 86.7 ms                                                | 70.7 ms: 1.23x faster                                                 |
| Geometric mean | (ref)                                                  | 1.27x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 329 ms: 1.44x faster                                                  |
| async_tree_none         | 388 ms                                                 | 281 ms: 1.38x faster                                                  |
| async_tree_io           | 980 ms                                                 | 725 ms: 1.35x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 522 ms: 1.24x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.35x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 68.8 ms: 1.35x faster                                                 |
| float          | 69.0 ms                                                | 56.0 ms: 1.23x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.19x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 72.7 ms: 1.31x faster                                                 |
| regex_dna      | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| regex_v8       | 17.1 ms                                                | 15.0 ms: 1.15x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.44 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.16x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 200 us: 1.40x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 34.2 ms: 1.36x faster                                                 |
| json_dumps           | 8.11 ms                                                | 5.97 ms: 1.36x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 149 us: 1.30x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.40 sec: 1.22x faster                                                |
| xml_etree_generate   | 53.5 ms                                                | 46.0 ms: 1.16x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 95.4 ms: 1.13x faster                                                 |
| json_loads           | 16.4 us                                                | 15.6 us: 1.05x faster                                                 |
| unpickle             | 8.80 us                                                | 8.39 us: 1.05x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 69.2 ms: 1.04x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.64 us: 1.04x faster                                                 |
| pickle_dict          | 17.0 us                                                | 17.1 us: 1.01x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.73 us: 1.01x slower                                                 |
| pickle               | 6.97 us                                                | 7.14 us: 1.02x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.43 ms: 1.19x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.12x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 19.7 ms: 1.34x faster                                                 |
| mako            | 9.87 ms                                                | 7.55 ms: 1.31x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 28.3 ms: 1.19x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.9 ms: 1.17x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.25x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.67 ms: 1.84x faster                                                 |
| logging_silent           | 117 ns                                                 | 65.2 ns: 1.80x faster                                                 |
| richards                 | 48.7 ms                                                | 30.2 ms: 1.61x faster                                                 |
| richards_super           | 57.8 ms                                                | 36.7 ms: 1.58x faster                                                 |
| scimark_lu               | 103 ms                                                 | 67.0 ms: 1.54x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 49.0 ms: 1.47x faster                                                 |
| chameleon                | 6.26 ms                                                | 4.29 ms: 1.46x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 329 ms: 1.44x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 200 us: 1.40x faster                                                  |
| async_tree_none          | 388 ms                                                 | 281 ms: 1.38x faster                                                  |
| raytrace                 | 301 ms                                                 | 220 ms: 1.37x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 34.2 ms: 1.36x faster                                                 |
| json_dumps               | 8.11 ms                                                | 5.97 ms: 1.36x faster                                                 |
| nbody                    | 93.0 ms                                                | 68.8 ms: 1.35x faster                                                 |
| async_tree_io            | 980 ms                                                 | 725 ms: 1.35x faster                                                  |
| thrift                   | 572 us                                                 | 424 us: 1.35x faster                                                  |
| django_template          | 26.4 ms                                                | 19.7 ms: 1.34x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 70.9 ms: 1.34x faster                                                 |
| pycparser                | 877 ms                                                 | 660 ms: 1.33x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 483 ms: 1.33x faster                                                  |
| chaos                    | 65.8 ms                                                | 49.7 ms: 1.32x faster                                                 |
| go                       | 151 ms                                                 | 115 ms: 1.31x faster                                                  |
| regex_compile            | 95.3 ms                                                | 72.7 ms: 1.31x faster                                                 |
| mako                     | 9.87 ms                                                | 7.55 ms: 1.31x faster                                                 |
| pprint_pformat           | 1.30 sec                                               | 998 ms: 1.31x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 954 us: 1.30x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 149 us: 1.30x faster                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.64 ms: 1.30x faster                                                 |
| pyflate                  | 427 ms                                                 | 329 ms: 1.30x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 1.12 ms: 1.29x faster                                                 |
| hexiom                   | 6.19 ms                                                | 4.83 ms: 1.28x faster                                                 |
| deepcopy_memo            | 34.7 us                                                | 27.1 us: 1.28x faster                                                 |
| html5lib                 | 42.4 ms                                                | 33.4 ms: 1.27x faster                                                 |
| logging_format           | 4.83 us                                                | 3.82 us: 1.26x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.53 us: 1.26x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 683 us: 1.26x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 52.5 ms: 1.25x faster                                                 |
| scimark_sor              | 128 ms                                                 | 103 ms: 1.24x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 522 ms: 1.24x faster                                                  |
| float                    | 69.0 ms                                                | 56.0 ms: 1.23x faster                                                 |
| dulwich_log              | 35.3 ms                                                | 28.7 ms: 1.23x faster                                                 |
| tornado_http             | 86.7 ms                                                | 70.7 ms: 1.23x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.40 sec: 1.22x faster                                                |
| deepcopy_reduce          | 2.33 us                                                | 1.92 us: 1.21x faster                                                 |
| docutils                 | 1.73 sec                                               | 1.43 sec: 1.21x faster                                                |
| scimark_fft              | 224 ms                                                 | 186 ms: 1.21x faster                                                  |
| deepcopy                 | 272 us                                                 | 225 us: 1.20x faster                                                  |
| 2to3                     | 192 ms                                                 | 160 ms: 1.20x faster                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 30.7 ms: 1.20x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 28.3 ms: 1.19x faster                                                 |
| regex_dna                | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.2 ms: 1.17x faster                                                 |
| genshi_text              | 17.3 ms                                                | 14.9 ms: 1.17x faster                                                 |
| fannkuch                 | 303 ms                                                 | 260 ms: 1.16x faster                                                  |
| xml_etree_generate       | 53.5 ms                                                | 46.0 ms: 1.16x faster                                                 |
| unpack_sequence          | 39.0 ns                                                | 33.8 ns: 1.15x faster                                                 |
| regex_v8                 | 17.1 ms                                                | 15.0 ms: 1.15x faster                                                 |
| async_generators         | 231 ms                                                 | 203 ms: 1.14x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 463 us: 1.14x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 167 ms: 1.14x faster                                                  |
| xml_etree_parse          | 108 ms                                                 | 95.4 ms: 1.13x faster                                                 |
| sympy_str                | 165 ms                                                 | 146 ms: 1.13x faster                                                  |
| sympy_expand             | 269 ms                                                 | 238 ms: 1.13x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.43 sec: 1.12x faster                                                |
| sympy_sum                | 92.2 ms                                                | 82.6 ms: 1.12x faster                                                 |
| telco                    | 3.49 ms                                                | 3.15 ms: 1.11x faster                                                 |
| json                     | 3.08 ms                                                | 2.79 ms: 1.10x faster                                                 |
| nqueens                  | 63.8 ms                                                | 58.8 ms: 1.08x faster                                                 |
| coroutines               | 20.7 ms                                                | 19.3 ms: 1.07x faster                                                 |
| comprehensions           | 16.9 us                                                | 15.9 us: 1.06x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.1 ms: 1.06x faster                                                 |
| json_loads               | 16.4 us                                                | 15.6 us: 1.05x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.39 us: 1.05x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 69.2 ms: 1.04x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.64 us: 1.04x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.42 us: 1.03x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 75.6 ms: 1.03x faster                                                 |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| regex_effbot             | 2.46 ms                                                | 2.44 ms: 1.01x faster                                                 |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                  |
| typing_runtime_protocols | 323 us                                                 | 325 us: 1.01x slower                                                  |
| pickle_dict              | 17.0 us                                                | 17.1 us: 1.01x slower                                                 |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.73 us: 1.01x slower                                                 |
| pickle                   | 6.97 us                                                | 7.14 us: 1.02x slower                                                 |
| python_startup           | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.74 sec: 1.07x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 42.2 ms: 1.13x slower                                                 |
| generators               | 32.3 ms                                                | 36.6 ms: 1.13x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.43 ms: 1.19x slower                                                 |
| dask                     | 253 ms                                                 | 320 ms: 1.26x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.19x faster                                                          |

Benchmark hidden because not significant (1): asyncio_tcp
Ignored benchmarks (8) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20221114-3.12.0a2-3b9d793/bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.05x