
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0
- machine: darwin-arm64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.23x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 154 ms: 1.24x faster                                   |
| chameleon      | 6.26 ms                                                | 4.30 ms: 1.46x faster                                  |
| docutils       | 1.73 sec                                               | 1.43 sec: 1.21x faster                                 |
| html5lib       | 42.4 ms                                                | 33.0 ms: 1.28x faster                                  |
| tornado_http   | 86.7 ms                                                | 69.1 ms: 1.26x faster                                  |
| Geometric mean | (ref)                                                  | 1.29x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 336 ms: 1.41x faster                                   |
| async_tree_io           | 980 ms                                                 | 697 ms: 1.40x faster                                   |
| async_tree_none         | 388 ms                                                 | 282 ms: 1.38x faster                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 519 ms: 1.25x faster                                   |
| Geometric mean          | (ref)                                                  | 1.36x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 61.7 ms: 1.51x faster                                  |
| float          | 69.0 ms                                                | 50.8 ms: 1.36x faster                                  |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                   |
| Geometric mean | (ref)                                                  | 1.27x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 72.8 ms: 1.31x faster                                  |
| regex_dna      | 174 ms                                                 | 148 ms: 1.18x faster                                   |
| regex_v8       | 17.1 ms                                                | 15.1 ms: 1.13x faster                                  |
| regex_effbot   | 2.46 ms                                                | 2.43 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.15x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 191 us: 1.47x faster                                   |
| xml_etree_process    | 46.5 ms                                                | 33.6 ms: 1.39x faster                                  |
| tomli_loads          | 1.71 sec                                               | 1.27 sec: 1.34x faster                                 |
| unpickle_pure_python | 194 us                                                 | 149 us: 1.31x faster                                   |
| xml_etree_generate   | 53.5 ms                                                | 45.8 ms: 1.17x faster                                  |
| json_dumps           | 8.11 ms                                                | 7.53 ms: 1.08x faster                                  |
| xml_etree_parse      | 108 ms                                                 | 100 ms: 1.07x faster                                   |
| json_loads           | 16.4 us                                                | 15.3 us: 1.07x faster                                  |
| unpickle             | 8.80 us                                                | 8.29 us: 1.06x faster                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 68.3 ms: 1.06x faster                                  |
| pickle_list          | 2.74 us                                                | 2.70 us: 1.02x faster                                  |
| unpickle_list        | 2.69 us                                                | 2.69 us: 1.00x faster                                  |
| pickle_dict          | 17.0 us                                                | 17.1 us: 1.01x slower                                  |
| Geometric mean       | (ref)                                                  | 1.13x faster                                           |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 7.91 ms                                                | 8.57 ms: 1.08x slower                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                           |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 26.4 ms                                                | 20.1 ms: 1.31x faster                                  |
| mako            | 9.87 ms                                                | 7.93 ms: 1.24x faster                                  |
| genshi_text     | 17.3 ms                                                | 14.4 ms: 1.20x faster                                  |
| genshi_xml      | 33.8 ms                                                | 28.5 ms: 1.19x faster                                  |
| Geometric mean  | (ref)                                                  | 1.24x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.75 ms: 1.79x faster                                  |
| logging_silent           | 117 ns                                                 | 66.5 ns: 1.76x faster                                  |
| mypy2                    | 607 ms                                                 | 372 ms: 1.63x faster                                   |
| scimark_sor              | 128 ms                                                 | 79.2 ms: 1.62x faster                                  |
| richards                 | 48.7 ms                                                | 31.1 ms: 1.57x faster                                  |
| richards_super           | 57.8 ms                                                | 37.3 ms: 1.55x faster                                  |
| scimark_lu               | 103 ms                                                 | 67.7 ms: 1.52x faster                                  |
| crypto_pyaes             | 71.8 ms                                                | 47.5 ms: 1.51x faster                                  |
| nbody                    | 93.0 ms                                                | 61.7 ms: 1.51x faster                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 43.5 ms: 1.51x faster                                  |
| pyflate                  | 427 ms                                                 | 284 ms: 1.50x faster                                   |
| pickle_pure_python       | 281 us                                                 | 191 us: 1.47x faster                                   |
| raytrace                 | 301 ms                                                 | 206 ms: 1.46x faster                                   |
| chameleon                | 6.26 ms                                                | 4.30 ms: 1.46x faster                                  |
| spectral_norm            | 94.8 ms                                                | 65.7 ms: 1.44x faster                                  |
| go                       | 151 ms                                                 | 105 ms: 1.43x faster                                   |
| async_tree_memoization   | 474 ms                                                 | 336 ms: 1.41x faster                                   |
| async_tree_io            | 980 ms                                                 | 697 ms: 1.40x faster                                   |
| sqlglot_parse            | 1.24 ms                                                | 890 us: 1.40x faster                                   |
| thrift                   | 572 us                                                 | 410 us: 1.39x faster                                   |
| chaos                    | 65.8 ms                                                | 47.4 ms: 1.39x faster                                  |
| xml_etree_process        | 46.5 ms                                                | 33.6 ms: 1.39x faster                                  |
| async_tree_none          | 388 ms                                                 | 282 ms: 1.38x faster                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.05 ms: 1.37x faster                                  |
| float                    | 69.0 ms                                                | 50.8 ms: 1.36x faster                                  |
| hexiom                   | 6.19 ms                                                | 4.58 ms: 1.35x faster                                  |
| deepcopy_memo            | 34.7 us                                                | 25.7 us: 1.35x faster                                  |
| tomli_loads              | 1.71 sec                                               | 1.27 sec: 1.34x faster                                 |
| pprint_safe_repr         | 641 ms                                                 | 478 ms: 1.34x faster                                   |
| pprint_pformat           | 1.30 sec                                               | 979 ms: 1.33x faster                                   |
| pycparser                | 877 ms                                                 | 659 ms: 1.33x faster                                   |
| logging_format           | 4.83 us                                                | 3.67 us: 1.31x faster                                  |
| django_template          | 26.4 ms                                                | 20.1 ms: 1.31x faster                                  |
| unpickle_pure_python     | 194 us                                                 | 149 us: 1.31x faster                                   |
| regex_compile            | 95.3 ms                                                | 72.8 ms: 1.31x faster                                  |
| logging_simple           | 4.45 us                                                | 3.41 us: 1.30x faster                                  |
| scimark_fft              | 224 ms                                                 | 173 ms: 1.30x faster                                   |
| deepcopy_reduce          | 2.33 us                                                | 1.79 us: 1.30x faster                                  |
| html5lib                 | 42.4 ms                                                | 33.0 ms: 1.28x faster                                  |
| sqlalchemy_imperative    | 8.86 ms                                                | 6.98 ms: 1.27x faster                                  |
| fannkuch                 | 303 ms                                                 | 240 ms: 1.26x faster                                   |
| deepcopy                 | 272 us                                                 | 215 us: 1.26x faster                                   |
| tornado_http             | 86.7 ms                                                | 69.1 ms: 1.26x faster                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 519 ms: 1.25x faster                                   |
| mako                     | 9.87 ms                                                | 7.93 ms: 1.24x faster                                  |
| 2to3                     | 192 ms                                                 | 154 ms: 1.24x faster                                   |
| sqlglot_optimize         | 36.8 ms                                                | 29.6 ms: 1.24x faster                                  |
| sqlalchemy_declarative   | 73.3 ms                                                | 59.3 ms: 1.24x faster                                  |
| dulwich_log              | 35.3 ms                                                | 28.6 ms: 1.23x faster                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.81 ms: 1.22x faster                                  |
| docutils                 | 1.73 sec                                               | 1.43 sec: 1.21x faster                                 |
| create_gc_cycles         | 860 us                                                 | 711 us: 1.21x faster                                   |
| coroutines               | 20.7 ms                                                | 17.2 ms: 1.21x faster                                  |
| async_generators         | 231 ms                                                 | 192 ms: 1.20x faster                                   |
| genshi_text              | 17.3 ms                                                | 14.4 ms: 1.20x faster                                  |
| aiohttp                  | 1.22 ms                                                | 1.02 ms: 1.19x faster                                  |
| gunicorn                 | 1.30 ms                                                | 1.10 ms: 1.19x faster                                  |
| genshi_xml               | 33.8 ms                                                | 28.5 ms: 1.19x faster                                  |
| regex_dna                | 174 ms                                                 | 148 ms: 1.18x faster                                   |
| sqlglot_normalize        | 190 ms                                                 | 162 ms: 1.18x faster                                   |
| sympy_expand             | 269 ms                                                 | 229 ms: 1.17x faster                                   |
| comprehensions           | 16.9 us                                                | 14.4 us: 1.17x faster                                  |
| xml_etree_generate       | 53.5 ms                                                | 45.8 ms: 1.17x faster                                  |
| sympy_integrate          | 13.1 ms                                                | 11.3 ms: 1.17x faster                                  |
| sqlite_synth             | 1.46 us                                                | 1.26 us: 1.16x faster                                  |
| unpack_sequence          | 39.0 ns                                                | 33.6 ns: 1.16x faster                                  |
| dask                     | 253 ms                                                 | 219 ms: 1.16x faster                                   |
| sympy_str                | 165 ms                                                 | 144 ms: 1.15x faster                                   |
| sympy_sum                | 92.2 ms                                                | 80.2 ms: 1.15x faster                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.40 sec: 1.15x faster                                 |
| nqueens                  | 63.8 ms                                                | 55.9 ms: 1.14x faster                                  |
| bench_thread_pool        | 527 us                                                 | 465 us: 1.13x faster                                   |
| regex_v8                 | 17.1 ms                                                | 15.1 ms: 1.13x faster                                  |
| flaskblogging            | 2.65 ms                                                | 2.35 ms: 1.13x faster                                  |
| json                     | 3.08 ms                                                | 2.75 ms: 1.12x faster                                  |
| telco                    | 3.49 ms                                                | 3.17 ms: 1.10x faster                                  |
| mdp                      | 1.63 sec                                               | 1.48 sec: 1.10x faster                                 |
| pylint                   | 277 ms                                                 | 253 ms: 1.10x faster                                   |
| meteor_contest           | 77.7 ms                                                | 71.1 ms: 1.09x faster                                  |
| json_dumps               | 8.11 ms                                                | 7.53 ms: 1.08x faster                                  |
| xml_etree_parse          | 108 ms                                                 | 100 ms: 1.07x faster                                   |
| typing_runtime_protocols | 323 us                                                 | 301 us: 1.07x faster                                   |
| json_loads               | 16.4 us                                                | 15.3 us: 1.07x faster                                  |
| generators               | 32.3 ms                                                | 30.3 ms: 1.07x faster                                  |
| unpickle                 | 8.80 us                                                | 8.29 us: 1.06x faster                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 68.3 ms: 1.06x faster                                  |
| pathlib                  | 24.5 ms                                                | 23.2 ms: 1.06x faster                                  |
| asyncio_tcp              | 659 ms                                                 | 643 ms: 1.02x faster                                   |
| pickle_list              | 2.74 us                                                | 2.70 us: 1.02x faster                                  |
| regex_effbot             | 2.46 ms                                                | 2.43 ms: 1.01x faster                                  |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                   |
| unpickle_list            | 2.69 us                                                | 2.69 us: 1.00x faster                                  |
| pickle_dict              | 17.0 us                                                | 17.1 us: 1.01x slower                                  |
| gc_traversal             | 2.36 ms                                                | 2.38 ms: 1.01x slower                                  |
| coverage                 | 41.5 ms                                                | 43.9 ms: 1.06x slower                                  |
| python_startup_no_site   | 7.91 ms                                                | 8.57 ms: 1.08x slower                                  |
| bench_mp_pool            | 37.4 ms                                                | 41.0 ms: 1.10x slower                                  |
| Geometric mean           | (ref)                                                  | 1.23x faster                                           |

Benchmark hidden because not significant (3): python_startup, asyncio_websockets, pickle
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.07x