
# Results vs. 3.11.0

- fork: python
- ref: v3.10.4
- machine: darwin-arm64
- commit hash: 9d38120
- commit date: 2022-03-23
- overall geometric mean: 1.23x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 192 ms: 1.24x slower                                   |
| chameleon      | 4.30 ms                                                | 6.26 ms: 1.46x slower                                  |
| docutils       | 1.43 sec                                               | 1.73 sec: 1.21x slower                                 |
| html5lib       | 33.0 ms                                                | 42.4 ms: 1.28x slower                                  |
| tornado_http   | 69.1 ms                                                | 86.7 ms: 1.26x slower                                  |
| Geometric mean | (ref)                                                  | 1.29x slower                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 519 ms                                                 | 649 ms: 1.25x slower                                   |
| async_tree_none         | 282 ms                                                 | 388 ms: 1.38x slower                                   |
| async_tree_io           | 697 ms                                                 | 980 ms: 1.40x slower                                   |
| async_tree_memoization  | 336 ms                                                 | 474 ms: 1.41x slower                                   |
| Geometric mean          | (ref)                                                  | 1.36x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                   |
| float          | 50.8 ms                                                | 69.0 ms: 1.36x slower                                  |
| nbody          | 61.7 ms                                                | 93.0 ms: 1.51x slower                                  |
| Geometric mean | (ref)                                                  | 1.27x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 2.43 ms                                                | 2.46 ms: 1.01x slower                                  |
| regex_v8       | 15.1 ms                                                | 17.1 ms: 1.13x slower                                  |
| regex_dna      | 148 ms                                                 | 174 ms: 1.18x slower                                   |
| regex_compile  | 72.8 ms                                                | 95.3 ms: 1.31x slower                                  |
| Geometric mean | (ref)                                                  | 1.15x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_dict          | 17.1 us                                                | 17.0 us: 1.01x faster                                  |
| unpickle_list        | 2.69 us                                                | 2.69 us: 1.00x slower                                  |
| pickle_list          | 2.70 us                                                | 2.74 us: 1.02x slower                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 72.1 ms: 1.06x slower                                  |
| unpickle             | 8.29 us                                                | 8.80 us: 1.06x slower                                  |
| json_loads           | 15.3 us                                                | 16.4 us: 1.07x slower                                  |
| xml_etree_parse      | 100 ms                                                 | 108 ms: 1.07x slower                                   |
| json_dumps           | 7.53 ms                                                | 8.11 ms: 1.08x slower                                  |
| xml_etree_generate   | 45.8 ms                                                | 53.5 ms: 1.17x slower                                  |
| unpickle_pure_python | 149 us                                                 | 194 us: 1.31x slower                                   |
| tomli_loads          | 1.27 sec                                               | 1.71 sec: 1.34x slower                                 |
| xml_etree_process    | 33.6 ms                                                | 46.5 ms: 1.39x slower                                  |
| pickle_pure_python   | 191 us                                                 | 281 us: 1.47x slower                                   |
| Geometric mean       | (ref)                                                  | 1.13x slower                                           |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 8.57 ms                                                | 7.91 ms: 1.08x faster                                  |
| Geometric mean         | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| genshi_xml      | 28.5 ms                                                | 33.8 ms: 1.19x slower                                  |
| genshi_text     | 14.4 ms                                                | 17.3 ms: 1.20x slower                                  |
| mako            | 7.93 ms                                                | 9.87 ms: 1.24x slower                                  |
| django_template | 20.1 ms                                                | 26.4 ms: 1.31x slower                                  |
| Geometric mean  | (ref)                                                  | 1.24x slower                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| bench_mp_pool            | 41.0 ms                                                | 37.4 ms: 1.10x faster                                  |
| python_startup_no_site   | 8.57 ms                                                | 7.91 ms: 1.08x faster                                  |
| coverage                 | 43.9 ms                                                | 41.5 ms: 1.06x faster                                  |
| gc_traversal             | 2.38 ms                                                | 2.36 ms: 1.01x faster                                  |
| pickle_dict              | 17.1 us                                                | 17.0 us: 1.01x faster                                  |
| unpickle_list            | 2.69 us                                                | 2.69 us: 1.00x slower                                  |
| pidigits                 | 280 ms                                                 | 282 ms: 1.01x slower                                   |
| regex_effbot             | 2.43 ms                                                | 2.46 ms: 1.01x slower                                  |
| pickle_list              | 2.70 us                                                | 2.74 us: 1.02x slower                                  |
| asyncio_tcp              | 643 ms                                                 | 659 ms: 1.02x slower                                   |
| pathlib                  | 23.2 ms                                                | 24.5 ms: 1.06x slower                                  |
| xml_etree_iterparse      | 68.3 ms                                                | 72.1 ms: 1.06x slower                                  |
| unpickle                 | 8.29 us                                                | 8.80 us: 1.06x slower                                  |
| generators               | 30.3 ms                                                | 32.3 ms: 1.07x slower                                  |
| json_loads               | 15.3 us                                                | 16.4 us: 1.07x slower                                  |
| typing_runtime_protocols | 301 us                                                 | 323 us: 1.07x slower                                   |
| xml_etree_parse          | 100 ms                                                 | 108 ms: 1.07x slower                                   |
| json_dumps               | 7.53 ms                                                | 8.11 ms: 1.08x slower                                  |
| meteor_contest           | 71.1 ms                                                | 77.7 ms: 1.09x slower                                  |
| pylint                   | 253 ms                                                 | 277 ms: 1.10x slower                                   |
| mdp                      | 1.48 sec                                               | 1.63 sec: 1.10x slower                                 |
| telco                    | 3.17 ms                                                | 3.49 ms: 1.10x slower                                  |
| json                     | 2.75 ms                                                | 3.08 ms: 1.12x slower                                  |
| flaskblogging            | 2.35 ms                                                | 2.65 ms: 1.13x slower                                  |
| regex_v8                 | 15.1 ms                                                | 17.1 ms: 1.13x slower                                  |
| bench_thread_pool        | 465 us                                                 | 527 us: 1.13x slower                                   |
| nqueens                  | 55.9 ms                                                | 63.8 ms: 1.14x slower                                  |
| asyncio_tcp_ssl          | 1.40 sec                                               | 1.60 sec: 1.15x slower                                 |
| sympy_sum                | 80.2 ms                                                | 92.2 ms: 1.15x slower                                  |
| sympy_str                | 144 ms                                                 | 165 ms: 1.15x slower                                   |
| dask                     | 219 ms                                                 | 253 ms: 1.16x slower                                   |
| unpack_sequence          | 33.6 ns                                                | 39.0 ns: 1.16x slower                                  |
| sqlite_synth             | 1.26 us                                                | 1.46 us: 1.16x slower                                  |
| sympy_integrate          | 11.3 ms                                                | 13.1 ms: 1.17x slower                                  |
| xml_etree_generate       | 45.8 ms                                                | 53.5 ms: 1.17x slower                                  |
| comprehensions           | 14.4 us                                                | 16.9 us: 1.17x slower                                  |
| sympy_expand             | 229 ms                                                 | 269 ms: 1.17x slower                                   |
| sqlglot_normalize        | 162 ms                                                 | 190 ms: 1.18x slower                                   |
| regex_dna                | 148 ms                                                 | 174 ms: 1.18x slower                                   |
| genshi_xml               | 28.5 ms                                                | 33.8 ms: 1.19x slower                                  |
| gunicorn                 | 1.10 ms                                                | 1.30 ms: 1.19x slower                                  |
| aiohttp                  | 1.02 ms                                                | 1.22 ms: 1.19x slower                                  |
| genshi_text              | 14.4 ms                                                | 17.3 ms: 1.20x slower                                  |
| async_generators         | 192 ms                                                 | 231 ms: 1.20x slower                                   |
| coroutines               | 17.2 ms                                                | 20.7 ms: 1.21x slower                                  |
| create_gc_cycles         | 711 us                                                 | 860 us: 1.21x slower                                   |
| docutils                 | 1.43 sec                                               | 1.73 sec: 1.21x slower                                 |
| scimark_sparse_mat_mult  | 2.81 ms                                                | 3.42 ms: 1.22x slower                                  |
| dulwich_log              | 28.6 ms                                                | 35.3 ms: 1.23x slower                                  |
| sqlalchemy_declarative   | 59.3 ms                                                | 73.3 ms: 1.24x slower                                  |
| sqlglot_optimize         | 29.6 ms                                                | 36.8 ms: 1.24x slower                                  |
| 2to3                     | 154 ms                                                 | 192 ms: 1.24x slower                                   |
| mako                     | 7.93 ms                                                | 9.87 ms: 1.24x slower                                  |
| async_tree_cpu_io_mixed  | 519 ms                                                 | 649 ms: 1.25x slower                                   |
| tornado_http             | 69.1 ms                                                | 86.7 ms: 1.26x slower                                  |
| deepcopy                 | 215 us                                                 | 272 us: 1.26x slower                                   |
| fannkuch                 | 240 ms                                                 | 303 ms: 1.26x slower                                   |
| sqlalchemy_imperative    | 6.98 ms                                                | 8.86 ms: 1.27x slower                                  |
| html5lib                 | 33.0 ms                                                | 42.4 ms: 1.28x slower                                  |
| deepcopy_reduce          | 1.79 us                                                | 2.33 us: 1.30x slower                                  |
| scimark_fft              | 173 ms                                                 | 224 ms: 1.30x slower                                   |
| logging_simple           | 3.41 us                                                | 4.45 us: 1.30x slower                                  |
| regex_compile            | 72.8 ms                                                | 95.3 ms: 1.31x slower                                  |
| unpickle_pure_python     | 149 us                                                 | 194 us: 1.31x slower                                   |
| django_template          | 20.1 ms                                                | 26.4 ms: 1.31x slower                                  |
| logging_format           | 3.67 us                                                | 4.83 us: 1.31x slower                                  |
| pycparser                | 659 ms                                                 | 877 ms: 1.33x slower                                   |
| pprint_pformat           | 979 ms                                                 | 1.30 sec: 1.33x slower                                 |
| pprint_safe_repr         | 478 ms                                                 | 641 ms: 1.34x slower                                   |
| tomli_loads              | 1.27 sec                                               | 1.71 sec: 1.34x slower                                 |
| deepcopy_memo            | 25.7 us                                                | 34.7 us: 1.35x slower                                  |
| hexiom                   | 4.58 ms                                                | 6.19 ms: 1.35x slower                                  |
| float                    | 50.8 ms                                                | 69.0 ms: 1.36x slower                                  |
| sqlglot_transpile        | 1.05 ms                                                | 1.44 ms: 1.37x slower                                  |
| async_tree_none          | 282 ms                                                 | 388 ms: 1.38x slower                                   |
| xml_etree_process        | 33.6 ms                                                | 46.5 ms: 1.39x slower                                  |
| chaos                    | 47.4 ms                                                | 65.8 ms: 1.39x slower                                  |
| thrift                   | 410 us                                                 | 572 us: 1.39x slower                                   |
| sqlglot_parse            | 890 us                                                 | 1.24 ms: 1.40x slower                                  |
| async_tree_io            | 697 ms                                                 | 980 ms: 1.40x slower                                   |
| async_tree_memoization   | 336 ms                                                 | 474 ms: 1.41x slower                                   |
| go                       | 105 ms                                                 | 151 ms: 1.43x slower                                   |
| spectral_norm            | 65.7 ms                                                | 94.8 ms: 1.44x slower                                  |
| chameleon                | 4.30 ms                                                | 6.26 ms: 1.46x slower                                  |
| raytrace                 | 206 ms                                                 | 301 ms: 1.46x slower                                   |
| pickle_pure_python       | 191 us                                                 | 281 us: 1.47x slower                                   |
| pyflate                  | 284 ms                                                 | 427 ms: 1.50x slower                                   |
| scimark_monte_carlo      | 43.5 ms                                                | 65.6 ms: 1.51x slower                                  |
| nbody                    | 61.7 ms                                                | 93.0 ms: 1.51x slower                                  |
| crypto_pyaes             | 47.5 ms                                                | 71.8 ms: 1.51x slower                                  |
| scimark_lu               | 67.7 ms                                                | 103 ms: 1.52x slower                                   |
| richards_super           | 37.3 ms                                                | 57.8 ms: 1.55x slower                                  |
| richards                 | 31.1 ms                                                | 48.7 ms: 1.57x slower                                  |
| scimark_sor              | 79.2 ms                                                | 128 ms: 1.62x slower                                   |
| mypy2                    | 372 ms                                                 | 607 ms: 1.63x slower                                   |
| logging_silent           | 66.5 ns                                                | 117 ns: 1.76x slower                                   |
| deltablue                | 2.75 ms                                                | 4.91 ms: 1.79x slower                                  |
| Geometric mean           | (ref)                                                  | 1.23x slower                                           |

Benchmark hidden because not significant (3): pickle, asyncio_websockets, python_startup
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.20x
- 95% likely to have a slowdown of 1.20x
- 99% likely to have a slowdown of 1.18x


# Memory

- memory change: 0.95x