
# Results vs. 3.10.4

- fork: python
- ref: v3.11.7
- machine: darwin-arm64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.20x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 153 ms: 1.25x faster                                   |
| chameleon      | 6.26 ms                                                | 4.36 ms: 1.44x faster                                  |
| docutils       | 1.73 sec                                               | 1.41 sec: 1.23x faster                                 |
| html5lib       | 42.4 ms                                                | 33.8 ms: 1.25x faster                                  |
| tornado_http   | 86.7 ms                                                | 70.3 ms: 1.23x faster                                  |
| Geometric mean | (ref)                                                  | 1.28x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 315 ms: 1.50x faster                                   |
| async_tree_io           | 980 ms                                                 | 697 ms: 1.40x faster                                   |
| async_tree_none         | 388 ms                                                 | 282 ms: 1.38x faster                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 516 ms: 1.26x faster                                   |
| Geometric mean          | (ref)                                                  | 1.38x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 68.9 ms: 1.35x faster                                  |
| float          | 69.0 ms                                                | 53.5 ms: 1.29x faster                                  |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.20x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 72.8 ms: 1.31x faster                                  |
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                   |
| regex_v8       | 17.1 ms                                                | 15.7 ms: 1.09x faster                                  |
| regex_effbot   | 2.46 ms                                                | 2.61 ms: 1.06x slower                                  |
| Geometric mean | (ref)                                                  | 1.11x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 193 us: 1.46x faster                                   |
| xml_etree_process    | 46.5 ms                                                | 34.4 ms: 1.35x faster                                  |
| tomli_loads          | 1.71 sec                                               | 1.32 sec: 1.29x faster                                 |
| unpickle_pure_python | 194 us                                                 | 151 us: 1.29x faster                                   |
| xml_etree_generate   | 53.5 ms                                                | 47.2 ms: 1.13x faster                                  |
| xml_etree_parse      | 108 ms                                                 | 97.1 ms: 1.11x faster                                  |
| json_loads           | 16.4 us                                                | 15.4 us: 1.07x faster                                  |
| json_dumps           | 8.11 ms                                                | 7.60 ms: 1.07x faster                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 67.8 ms: 1.06x faster                                  |
| unpickle             | 8.80 us                                                | 8.32 us: 1.06x faster                                  |
| pickle_list          | 2.74 us                                                | 2.69 us: 1.02x faster                                  |
| unpickle_list        | 2.69 us                                                | 2.78 us: 1.03x slower                                  |
| pickle               | 6.97 us                                                | 7.26 us: 1.04x slower                                  |
| Geometric mean       | (ref)                                                  | 1.12x faster                                           |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.9 ms: 1.09x slower                                  |
| python_startup_no_site | 7.91 ms                                                | 9.93 ms: 1.26x slower                                  |
| Geometric mean         | (ref)                                                  | 1.17x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 26.4 ms                                                | 19.7 ms: 1.34x faster                                  |
| mako            | 9.87 ms                                                | 8.19 ms: 1.21x faster                                  |
| genshi_xml      | 33.8 ms                                                | 28.9 ms: 1.17x faster                                  |
| genshi_text     | 17.3 ms                                                | 14.8 ms: 1.17x faster                                  |
| Geometric mean  | (ref)                                                  | 1.22x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.77 ms: 1.78x faster                                  |
| logging_silent           | 117 ns                                                 | 66.2 ns: 1.77x faster                                  |
| scimark_sor              | 128 ms                                                 | 76.4 ms: 1.68x faster                                  |
| richards                 | 48.7 ms                                                | 31.9 ms: 1.52x faster                                  |
| async_tree_memoization   | 474 ms                                                 | 315 ms: 1.50x faster                                   |
| scimark_lu               | 103 ms                                                 | 68.7 ms: 1.50x faster                                  |
| crypto_pyaes             | 71.8 ms                                                | 48.0 ms: 1.50x faster                                  |
| richards_super           | 57.8 ms                                                | 38.8 ms: 1.49x faster                                  |
| pyflate                  | 427 ms                                                 | 292 ms: 1.46x faster                                   |
| pickle_pure_python       | 281 us                                                 | 193 us: 1.46x faster                                   |
| raytrace                 | 301 ms                                                 | 209 ms: 1.44x faster                                   |
| chameleon                | 6.26 ms                                                | 4.36 ms: 1.44x faster                                  |
| async_tree_io            | 980 ms                                                 | 697 ms: 1.40x faster                                   |
| go                       | 151 ms                                                 | 108 ms: 1.40x faster                                   |
| thrift                   | 572 us                                                 | 411 us: 1.39x faster                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 47.6 ms: 1.38x faster                                  |
| async_tree_none          | 388 ms                                                 | 282 ms: 1.38x faster                                   |
| sqlglot_parse            | 1.24 ms                                                | 904 us: 1.38x faster                                   |
| deepcopy_memo            | 34.7 us                                                | 25.5 us: 1.36x faster                                  |
| xml_etree_process        | 46.5 ms                                                | 34.4 ms: 1.35x faster                                  |
| chaos                    | 65.8 ms                                                | 48.6 ms: 1.35x faster                                  |
| sqlglot_transpile        | 1.44 ms                                                | 1.07 ms: 1.35x faster                                  |
| nbody                    | 93.0 ms                                                | 68.9 ms: 1.35x faster                                  |
| spectral_norm            | 94.8 ms                                                | 70.5 ms: 1.34x faster                                  |
| django_template          | 26.4 ms                                                | 19.7 ms: 1.34x faster                                  |
| hexiom                   | 6.19 ms                                                | 4.65 ms: 1.33x faster                                  |
| pycparser                | 877 ms                                                 | 659 ms: 1.33x faster                                   |
| pprint_safe_repr         | 641 ms                                                 | 483 ms: 1.33x faster                                   |
| pprint_pformat           | 1.30 sec                                               | 986 ms: 1.32x faster                                   |
| regex_compile            | 95.3 ms                                                | 72.8 ms: 1.31x faster                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.80 us: 1.29x faster                                  |
| tomli_loads              | 1.71 sec                                               | 1.32 sec: 1.29x faster                                 |
| unpickle_pure_python     | 194 us                                                 | 151 us: 1.29x faster                                   |
| float                    | 69.0 ms                                                | 53.5 ms: 1.29x faster                                  |
| deepcopy                 | 272 us                                                 | 211 us: 1.29x faster                                   |
| logging_format           | 4.83 us                                                | 3.79 us: 1.27x faster                                  |
| logging_simple           | 4.45 us                                                | 3.50 us: 1.27x faster                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 516 ms: 1.26x faster                                   |
| 2to3                     | 192 ms                                                 | 153 ms: 1.25x faster                                   |
| html5lib                 | 42.4 ms                                                | 33.8 ms: 1.25x faster                                  |
| async_generators         | 231 ms                                                 | 187 ms: 1.24x faster                                   |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.16 ms: 1.24x faster                                  |
| tornado_http             | 86.7 ms                                                | 70.3 ms: 1.23x faster                                  |
| dulwich_log              | 35.3 ms                                                | 28.7 ms: 1.23x faster                                  |
| docutils                 | 1.73 sec                                               | 1.41 sec: 1.23x faster                                 |
| coroutines               | 20.7 ms                                                | 16.9 ms: 1.23x faster                                  |
| sqlglot_optimize         | 36.8 ms                                                | 30.0 ms: 1.22x faster                                  |
| sqlalchemy_declarative   | 73.3 ms                                                | 60.4 ms: 1.21x faster                                  |
| fannkuch                 | 303 ms                                                 | 250 ms: 1.21x faster                                   |
| create_gc_cycles         | 860 us                                                 | 713 us: 1.21x faster                                   |
| mako                     | 9.87 ms                                                | 8.19 ms: 1.21x faster                                  |
| scimark_fft              | 224 ms                                                 | 188 ms: 1.19x faster                                   |
| comprehensions           | 16.9 us                                                | 14.3 us: 1.18x faster                                  |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.18x faster                                  |
| genshi_xml               | 33.8 ms                                                | 28.9 ms: 1.17x faster                                  |
| genshi_text              | 17.3 ms                                                | 14.8 ms: 1.17x faster                                  |
| sqlglot_normalize        | 190 ms                                                 | 163 ms: 1.17x faster                                   |
| sqlite_synth             | 1.46 us                                                | 1.26 us: 1.16x faster                                  |
| gunicorn                 | 1.30 ms                                                | 1.12 ms: 1.16x faster                                  |
| aiohttp                  | 1.22 ms                                                | 1.06 ms: 1.16x faster                                  |
| sympy_sum                | 92.2 ms                                                | 80.0 ms: 1.15x faster                                  |
| unpack_sequence          | 39.0 ns                                                | 33.9 ns: 1.15x faster                                  |
| sympy_str                | 165 ms                                                 | 144 ms: 1.15x faster                                   |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                   |
| nqueens                  | 63.8 ms                                                | 55.7 ms: 1.15x faster                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.99 ms: 1.14x faster                                  |
| sympy_expand             | 269 ms                                                 | 235 ms: 1.14x faster                                   |
| dask                     | 253 ms                                                 | 222 ms: 1.14x faster                                   |
| bench_thread_pool        | 527 us                                                 | 464 us: 1.14x faster                                   |
| xml_etree_generate       | 53.5 ms                                                | 47.2 ms: 1.13x faster                                  |
| pylint                   | 277 ms                                                 | 246 ms: 1.12x faster                                   |
| json                     | 3.08 ms                                                | 2.77 ms: 1.11x faster                                  |
| xml_etree_parse          | 108 ms                                                 | 97.1 ms: 1.11x faster                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.45 sec: 1.11x faster                                 |
| telco                    | 3.49 ms                                                | 3.17 ms: 1.10x faster                                  |
| regex_v8                 | 17.1 ms                                                | 15.7 ms: 1.09x faster                                  |
| generators               | 32.3 ms                                                | 29.8 ms: 1.09x faster                                  |
| meteor_contest           | 77.7 ms                                                | 72.3 ms: 1.08x faster                                  |
| flaskblogging            | 2.65 ms                                                | 2.47 ms: 1.07x faster                                  |
| json_loads               | 16.4 us                                                | 15.4 us: 1.07x faster                                  |
| json_dumps               | 8.11 ms                                                | 7.60 ms: 1.07x faster                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 67.8 ms: 1.06x faster                                  |
| unpickle                 | 8.80 us                                                | 8.32 us: 1.06x faster                                  |
| pathlib                  | 24.5 ms                                                | 23.9 ms: 1.03x faster                                  |
| pickle_list              | 2.74 us                                                | 2.69 us: 1.02x faster                                  |
| asyncio_websockets       | 410 ms                                                 | 407 ms: 1.01x faster                                   |
| pidigits                 | 282 ms                                                 | 281 ms: 1.00x faster                                   |
| typing_runtime_protocols | 323 us                                                 | 328 us: 1.02x slower                                   |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                  |
| unpickle_list            | 2.69 us                                                | 2.78 us: 1.03x slower                                  |
| pickle                   | 6.97 us                                                | 7.26 us: 1.04x slower                                  |
| coverage                 | 41.5 ms                                                | 43.5 ms: 1.05x slower                                  |
| regex_effbot             | 2.46 ms                                                | 2.61 ms: 1.06x slower                                  |
| mdp                      | 1.63 sec                                               | 1.75 sec: 1.07x slower                                 |
| python_startup           | 10.9 ms                                                | 11.9 ms: 1.09x slower                                  |
| bench_mp_pool            | 37.4 ms                                                | 41.2 ms: 1.10x slower                                  |
| python_startup_no_site   | 7.91 ms                                                | 9.93 ms: 1.26x slower                                  |
| Geometric mean           | (ref)                                                  | 1.20x faster                                           |

Benchmark hidden because not significant (3): mypy2, asyncio_tcp, pickle_dict
Ignored benchmarks (4) of results/bm-20231204-3.11.7-fa7a6f2/bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.06x