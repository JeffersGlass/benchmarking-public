
# Results vs. 3.10.4

- fork: python
- ref: v3.12.1
- machine: darwin-arm64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.20x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 167 ms: 1.15x faster                                   |
| chameleon      | 6.26 ms                                                | 4.50 ms: 1.39x faster                                  |
| docutils       | 1.73 sec                                               | 1.48 sec: 1.17x faster                                 |
| tornado_http   | 86.7 ms                                                | 68.1 ms: 1.27x faster                                  |
| Geometric mean | (ref)                                                  | 1.24x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 306 ms: 1.55x faster                                   |
| async_tree_io           | 980 ms                                                 | 655 ms: 1.50x faster                                   |
| async_tree_none         | 388 ms                                                 | 260 ms: 1.49x faster                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 523 ms: 1.24x faster                                   |
| Geometric mean          | (ref)                                                  | 1.44x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 69.1 ms: 1.35x faster                                  |
| float          | 69.0 ms                                                | 56.5 ms: 1.22x faster                                  |
| Geometric mean | (ref)                                                  | 1.18x faster                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.7 ms: 1.29x faster                                  |
| regex_dna      | 174 ms                                                 | 152 ms: 1.14x faster                                   |
| regex_v8       | 17.1 ms                                                | 16.3 ms: 1.05x faster                                  |
| regex_effbot   | 2.46 ms                                                | 2.69 ms: 1.10x slower                                  |
| Geometric mean | (ref)                                                  | 1.09x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 188 us: 1.49x faster                                   |
| unpickle_pure_python | 194 us                                                 | 142 us: 1.37x faster                                   |
| json_dumps           | 8.11 ms                                                | 6.31 ms: 1.28x faster                                  |
| tomli_loads          | 1.71 sec                                               | 1.40 sec: 1.22x faster                                 |
| xml_etree_process    | 46.5 ms                                                | 38.7 ms: 1.20x faster                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 74.0 ms: 1.03x slower                                  |
| pickle_list          | 2.74 us                                                | 2.85 us: 1.04x slower                                  |
| xml_etree_generate   | 53.5 ms                                                | 55.8 ms: 1.04x slower                                  |
| pickle               | 6.97 us                                                | 7.27 us: 1.04x slower                                  |
| json_loads           | 16.4 us                                                | 17.2 us: 1.05x slower                                  |
| unpickle             | 8.80 us                                                | 9.24 us: 1.05x slower                                  |
| pickle_dict          | 17.0 us                                                | 18.0 us: 1.06x slower                                  |
| unpickle_list        | 2.69 us                                                | 3.25 us: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.06x faster                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.9 ms: 1.19x slower                                  |
| python_startup_no_site | 7.91 ms                                                | 11.0 ms: 1.39x slower                                  |
| Geometric mean         | (ref)                                                  | 1.29x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.59 ms: 1.30x faster                                  |
| django_template | 26.4 ms                                                | 21.2 ms: 1.25x faster                                  |
| Geometric mean  | (ref)                                                  | 1.27x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 72.5 us: 4.46x faster                                  |
| deltablue                | 4.91 ms                                                | 2.40 ms: 2.05x faster                                  |
| logging_silent           | 117 ns                                                 | 67.7 ns: 1.73x faster                                  |
| richards_super           | 57.8 ms                                                | 33.8 ms: 1.71x faster                                  |
| richards                 | 48.7 ms                                                | 30.2 ms: 1.61x faster                                  |
| go                       | 151 ms                                                 | 94.3 ms: 1.60x faster                                  |
| asyncio_tcp              | 659 ms                                                 | 418 ms: 1.58x faster                                   |
| chaos                    | 65.8 ms                                                | 41.8 ms: 1.58x faster                                  |
| async_tree_memoization   | 474 ms                                                 | 306 ms: 1.55x faster                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 43.2 ms: 1.52x faster                                  |
| sqlglot_parse            | 1.24 ms                                                | 823 us: 1.51x faster                                   |
| scimark_sor              | 128 ms                                                 | 85.1 ms: 1.51x faster                                  |
| async_tree_io            | 980 ms                                                 | 655 ms: 1.50x faster                                   |
| pickle_pure_python       | 281 us                                                 | 188 us: 1.49x faster                                   |
| async_tree_none          | 388 ms                                                 | 260 ms: 1.49x faster                                   |
| hexiom                   | 6.19 ms                                                | 4.23 ms: 1.47x faster                                  |
| raytrace                 | 301 ms                                                 | 206 ms: 1.46x faster                                   |
| sqlglot_transpile        | 1.44 ms                                                | 995 us: 1.45x faster                                   |
| scimark_lu               | 103 ms                                                 | 71.5 ms: 1.44x faster                                  |
| deepcopy_memo            | 34.7 us                                                | 24.9 us: 1.39x faster                                  |
| crypto_pyaes             | 71.8 ms                                                | 51.5 ms: 1.39x faster                                  |
| chameleon                | 6.26 ms                                                | 4.50 ms: 1.39x faster                                  |
| pyflate                  | 427 ms                                                 | 309 ms: 1.38x faster                                   |
| unpickle_pure_python     | 194 us                                                 | 142 us: 1.37x faster                                   |
| unpack_sequence          | 39.0 ns                                                | 29.0 ns: 1.35x faster                                  |
| nbody                    | 93.0 ms                                                | 69.1 ms: 1.35x faster                                  |
| pycparser                | 877 ms                                                 | 670 ms: 1.31x faster                                   |
| pprint_pformat           | 1.30 sec                                               | 999 ms: 1.31x faster                                   |
| pprint_safe_repr         | 641 ms                                                 | 492 ms: 1.30x faster                                   |
| mako                     | 9.87 ms                                                | 7.59 ms: 1.30x faster                                  |
| mypy2                    | 607 ms                                                 | 469 ms: 1.29x faster                                   |
| regex_compile            | 95.3 ms                                                | 73.7 ms: 1.29x faster                                  |
| json_dumps               | 8.11 ms                                                | 6.31 ms: 1.28x faster                                  |
| sqlalchemy_imperative    | 8.86 ms                                                | 6.93 ms: 1.28x faster                                  |
| tornado_http             | 86.7 ms                                                | 68.1 ms: 1.27x faster                                  |
| spectral_norm            | 94.8 ms                                                | 75.0 ms: 1.26x faster                                  |
| logging_format           | 4.83 us                                                | 3.86 us: 1.25x faster                                  |
| generators               | 32.3 ms                                                | 25.9 ms: 1.25x faster                                  |
| logging_simple           | 4.45 us                                                | 3.57 us: 1.25x faster                                  |
| django_template          | 26.4 ms                                                | 21.2 ms: 1.25x faster                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 523 ms: 1.24x faster                                   |
| create_gc_cycles         | 860 us                                                 | 693 us: 1.24x faster                                   |
| tomli_loads              | 1.71 sec                                               | 1.40 sec: 1.22x faster                                 |
| float                    | 69.0 ms                                                | 56.5 ms: 1.22x faster                                  |
| deepcopy                 | 272 us                                                 | 224 us: 1.22x faster                                   |
| dulwich_log              | 35.3 ms                                                | 29.1 ms: 1.21x faster                                  |
| xml_etree_process        | 46.5 ms                                                | 38.7 ms: 1.20x faster                                  |
| sympy_sum                | 92.2 ms                                                | 77.8 ms: 1.18x faster                                  |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.18x faster                                  |
| docutils                 | 1.73 sec                                               | 1.48 sec: 1.17x faster                                 |
| deepcopy_reduce          | 2.33 us                                                | 2.01 us: 1.16x faster                                  |
| comprehensions           | 16.9 us                                                | 14.7 us: 1.16x faster                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.39 sec: 1.15x faster                                 |
| 2to3                     | 192 ms                                                 | 167 ms: 1.15x faster                                   |
| regex_dna                | 174 ms                                                 | 152 ms: 1.14x faster                                   |
| fannkuch                 | 303 ms                                                 | 265 ms: 1.14x faster                                   |
| dask                     | 253 ms                                                 | 222 ms: 1.14x faster                                   |
| sqlalchemy_declarative   | 73.3 ms                                                | 64.7 ms: 1.13x faster                                  |
| scimark_fft              | 224 ms                                                 | 200 ms: 1.12x faster                                   |
| sympy_str                | 165 ms                                                 | 148 ms: 1.11x faster                                   |
| sympy_expand             | 269 ms                                                 | 247 ms: 1.09x faster                                   |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.15 ms: 1.09x faster                                  |
| coroutines               | 20.7 ms                                                | 19.1 ms: 1.09x faster                                  |
| sqlglot_optimize         | 36.8 ms                                                | 34.0 ms: 1.08x faster                                  |
| meteor_contest           | 77.7 ms                                                | 72.5 ms: 1.07x faster                                  |
| aiohttp                  | 1.22 ms                                                | 1.15 ms: 1.06x faster                                  |
| bench_thread_pool        | 527 us                                                 | 497 us: 1.06x faster                                   |
| nqueens                  | 63.8 ms                                                | 60.4 ms: 1.06x faster                                  |
| regex_v8                 | 17.1 ms                                                | 16.3 ms: 1.05x faster                                  |
| coverage                 | 41.5 ms                                                | 39.6 ms: 1.05x faster                                  |
| json                     | 3.08 ms                                                | 2.97 ms: 1.04x faster                                  |
| gunicorn                 | 1.30 ms                                                | 1.26 ms: 1.04x faster                                  |
| sqlglot_normalize        | 190 ms                                                 | 184 ms: 1.03x faster                                   |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.00x faster                                 |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 74.0 ms: 1.03x slower                                  |
| pickle_list              | 2.74 us                                                | 2.85 us: 1.04x slower                                  |
| xml_etree_generate       | 53.5 ms                                                | 55.8 ms: 1.04x slower                                  |
| pickle                   | 6.97 us                                                | 7.27 us: 1.04x slower                                  |
| json_loads               | 16.4 us                                                | 17.2 us: 1.05x slower                                  |
| unpickle                 | 8.80 us                                                | 9.24 us: 1.05x slower                                  |
| pickle_dict              | 17.0 us                                                | 18.0 us: 1.06x slower                                  |
| telco                    | 3.49 ms                                                | 3.82 ms: 1.09x slower                                  |
| regex_effbot             | 2.46 ms                                                | 2.69 ms: 1.10x slower                                  |
| sqlite_synth             | 1.46 us                                                | 1.61 us: 1.10x slower                                  |
| python_startup           | 10.9 ms                                                | 12.9 ms: 1.19x slower                                  |
| unpickle_list            | 2.69 us                                                | 3.25 us: 1.21x slower                                  |
| bench_mp_pool            | 37.4 ms                                                | 45.8 ms: 1.22x slower                                  |
| async_generators         | 231 ms                                                 | 303 ms: 1.31x slower                                   |
| python_startup_no_site   | 7.91 ms                                                | 11.0 ms: 1.39x slower                                  |
| Geometric mean           | (ref)                                                  | 1.20x faster                                           |

Benchmark hidden because not significant (4): xml_etree_parse, asyncio_websockets, pathlib, pidigits
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20231207-3.12.1-2305ca5/bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.06x