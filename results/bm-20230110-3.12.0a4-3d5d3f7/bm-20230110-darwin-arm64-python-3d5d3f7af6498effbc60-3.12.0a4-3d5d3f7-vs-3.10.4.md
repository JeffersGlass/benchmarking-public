
# Results vs. 3.10.4

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: darwin-arm64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.22x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 158 ms: 1.22x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.21 ms: 1.49x faster                                                 |
| docutils       | 1.73 sec                                               | 1.41 sec: 1.23x faster                                                |
| html5lib       | 42.4 ms                                                | 32.3 ms: 1.31x faster                                                 |
| Geometric mean | (ref)                                                  | 1.31x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 322 ms: 1.47x faster                                                  |
| async_tree_none         | 388 ms                                                 | 280 ms: 1.39x faster                                                  |
| async_tree_io           | 980 ms                                                 | 728 ms: 1.35x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 521 ms: 1.25x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.36x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 67.7 ms: 1.37x faster                                                 |
| float          | 69.0 ms                                                | 55.5 ms: 1.24x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.20x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 72.1 ms: 1.32x faster                                                 |
| regex_dna      | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| regex_v8       | 17.1 ms                                                | 15.0 ms: 1.14x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.44 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.16x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 190 us: 1.48x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 137 us: 1.42x faster                                                  |
| json_dumps           | 8.11 ms                                                | 5.84 ms: 1.39x faster                                                 |
| xml_etree_process    | 46.5 ms                                                | 33.8 ms: 1.38x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.28 sec: 1.33x faster                                                |
| xml_etree_generate   | 53.5 ms                                                | 46.9 ms: 1.14x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 96.4 ms: 1.12x faster                                                 |
| json_loads           | 16.4 us                                                | 15.5 us: 1.06x faster                                                 |
| unpickle             | 8.80 us                                                | 8.43 us: 1.04x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 70.0 ms: 1.03x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.70 us: 1.01x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.81 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                          |

Benchmark hidden because not significant (2): pickle, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.54 ms: 1.21x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.13x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.76 ms: 1.27x faster                                                 |
| django_template | 26.4 ms                                                | 20.8 ms: 1.27x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 27.3 ms: 1.24x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.2 ms: 1.23x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.25x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.51 ms: 1.96x faster                                                 |
| logging_silent           | 117 ns                                                 | 63.9 ns: 1.83x faster                                                 |
| richards                 | 48.7 ms                                                | 29.8 ms: 1.63x faster                                                 |
| richards_super           | 57.8 ms                                                | 36.0 ms: 1.61x faster                                                 |
| scimark_sor              | 128 ms                                                 | 83.4 ms: 1.54x faster                                                 |
| asyncio_tcp              | 659 ms                                                 | 430 ms: 1.53x faster                                                  |
| scimark_lu               | 103 ms                                                 | 67.3 ms: 1.53x faster                                                 |
| chameleon                | 6.26 ms                                                | 4.21 ms: 1.49x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 190 us: 1.48x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 322 ms: 1.47x faster                                                  |
| raytrace                 | 301 ms                                                 | 208 ms: 1.45x faster                                                  |
| go                       | 151 ms                                                 | 106 ms: 1.43x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 50.4 ms: 1.43x faster                                                 |
| pyflate                  | 427 ms                                                 | 301 ms: 1.42x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 137 us: 1.42x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 46.8 ms: 1.40x faster                                                 |
| async_tree_none          | 388 ms                                                 | 280 ms: 1.39x faster                                                  |
| json_dumps               | 8.11 ms                                                | 5.84 ms: 1.39x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 33.8 ms: 1.38x faster                                                 |
| nbody                    | 93.0 ms                                                | 67.7 ms: 1.37x faster                                                 |
| thrift                   | 572 us                                                 | 419 us: 1.36x faster                                                  |
| pycparser                | 877 ms                                                 | 643 ms: 1.36x faster                                                  |
| async_tree_io            | 980 ms                                                 | 728 ms: 1.35x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 70.6 ms: 1.34x faster                                                 |
| logging_format           | 4.83 us                                                | 3.60 us: 1.34x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 480 ms: 1.34x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 977 ms: 1.33x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.28 sec: 1.33x faster                                                |
| logging_simple           | 4.45 us                                                | 3.34 us: 1.33x faster                                                 |
| chaos                    | 65.8 ms                                                | 49.5 ms: 1.33x faster                                                 |
| hexiom                   | 6.19 ms                                                | 4.66 ms: 1.33x faster                                                 |
| regex_compile            | 95.3 ms                                                | 72.1 ms: 1.32x faster                                                 |
| html5lib                 | 42.4 ms                                                | 32.3 ms: 1.31x faster                                                 |
| unpack_sequence          | 39.0 ns                                                | 30.2 ns: 1.29x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.66 ms: 1.29x faster                                                 |
| mako                     | 9.87 ms                                                | 7.76 ms: 1.27x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.26 sec: 1.27x faster                                                |
| django_template          | 26.4 ms                                                | 20.8 ms: 1.27x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 985 us: 1.26x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 1.15 ms: 1.26x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 686 us: 1.25x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 28.2 ms: 1.25x faster                                                 |
| deepcopy_memo            | 34.7 us                                                | 27.7 us: 1.25x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 521 ms: 1.25x faster                                                  |
| float                    | 69.0 ms                                                | 55.5 ms: 1.24x faster                                                 |
| fannkuch                 | 303 ms                                                 | 244 ms: 1.24x faster                                                  |
| genshi_xml               | 33.8 ms                                                | 27.3 ms: 1.24x faster                                                 |
| scimark_fft              | 224 ms                                                 | 182 ms: 1.23x faster                                                  |
| docutils                 | 1.73 sec                                               | 1.41 sec: 1.23x faster                                                |
| sqlglot_optimize         | 36.8 ms                                                | 30.0 ms: 1.23x faster                                                 |
| genshi_text              | 17.3 ms                                                | 14.2 ms: 1.23x faster                                                 |
| 2to3                     | 192 ms                                                 | 158 ms: 1.22x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.94 us: 1.20x faster                                                 |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                                  |
| regex_dna                | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| coroutines               | 20.7 ms                                                | 17.5 ms: 1.19x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.18x faster                                                 |
| sympy_expand             | 269 ms                                                 | 230 ms: 1.17x faster                                                  |
| async_generators         | 231 ms                                                 | 200 ms: 1.16x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 165 ms: 1.15x faster                                                  |
| sympy_str                | 165 ms                                                 | 144 ms: 1.15x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 460 us: 1.15x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 15.0 ms: 1.14x faster                                                 |
| xml_etree_generate       | 53.5 ms                                                | 46.9 ms: 1.14x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 81.7 ms: 1.13x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 96.4 ms: 1.12x faster                                                 |
| nqueens                  | 63.8 ms                                                | 57.2 ms: 1.11x faster                                                 |
| json                     | 3.08 ms                                                | 2.79 ms: 1.11x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 71.1 ms: 1.09x faster                                                 |
| telco                    | 3.49 ms                                                | 3.22 ms: 1.08x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.36 us: 1.07x faster                                                 |
| json_loads               | 16.4 us                                                | 15.5 us: 1.06x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.1 ms: 1.06x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.43 us: 1.04x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 70.0 ms: 1.03x faster                                                 |
| comprehensions           | 16.9 us                                                | 16.6 us: 1.02x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.70 us: 1.01x faster                                                 |
| typing_runtime_protocols | 323 us                                                 | 320 us: 1.01x faster                                                  |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| regex_effbot             | 2.46 ms                                                | 2.44 ms: 1.01x faster                                                 |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                  |
| gc_traversal             | 2.36 ms                                                | 2.38 ms: 1.01x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.70 sec: 1.04x slower                                                |
| unpickle_list            | 2.69 us                                                | 2.81 us: 1.04x slower                                                 |
| python_startup           | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| generators               | 32.3 ms                                                | 35.1 ms: 1.09x slower                                                 |
| bench_mp_pool            | 37.4 ms                                                | 42.5 ms: 1.14x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.54 ms: 1.21x slower                                                 |
| dask                     | 253 ms                                                 | 309 ms: 1.22x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.22x faster                                                          |

Benchmark hidden because not significant (2): pickle, pickle_dict
Ignored benchmarks (9) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
Ignored benchmarks (4) of results/bm-20230110-3.12.0a4-3d5d3f7/bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.04x