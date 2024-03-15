
# Results vs. 3.10.4

- fork: python
- ref: 3c67ec394faac79d2608
- machine: darwin-arm64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 166 ms: 1.15x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.69 ms: 1.33x faster                                                 |
| docutils       | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                |
| html5lib       | 42.4 ms                                                | 34.6 ms: 1.22x faster                                                 |
| tornado_http   | 86.7 ms                                                | 72.3 ms: 1.20x faster                                                 |
| Geometric mean | (ref)                                                  | 1.21x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 336 ms: 1.41x faster                                                  |
| async_tree_none         | 388 ms                                                 | 290 ms: 1.34x faster                                                  |
| async_tree_io           | 980 ms                                                 | 753 ms: 1.30x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 533 ms: 1.22x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.31x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 68.5 ms: 1.36x faster                                                 |
| float          | 69.0 ms                                                | 57.5 ms: 1.20x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.18x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 76.0 ms: 1.25x faster                                                 |
| regex_dna      | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| regex_v8       | 17.1 ms                                                | 15.3 ms: 1.12x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.45 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.14x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 8.11 ms                                                | 6.08 ms: 1.33x faster                                                 |
| pickle_pure_python   | 281 us                                                 | 214 us: 1.31x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 37.1 ms: 1.25x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.38 sec: 1.24x faster                                                |
| unpickle_pure_python | 194 us                                                 | 161 us: 1.21x faster                                                  |
| xml_etree_parse      | 108 ms                                                 | 95.0 ms: 1.13x faster                                                 |
| xml_etree_generate   | 53.5 ms                                                | 48.7 ms: 1.10x faster                                                 |
| json_loads           | 16.4 us                                                | 15.7 us: 1.05x faster                                                 |
| unpickle             | 8.80 us                                                | 8.50 us: 1.04x faster                                                 |
| pickle_dict          | 17.0 us                                                | 16.8 us: 1.01x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.72 us: 1.01x faster                                                 |
| pickle               | 6.97 us                                                | 7.09 us: 1.02x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.85 us: 1.06x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                          |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.8 ms: 1.08x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.55 ms: 1.21x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.14x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 6.94 ms: 1.42x faster                                                 |
| django_template | 26.4 ms                                                | 22.5 ms: 1.17x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 30.7 ms: 1.10x faster                                                 |
| genshi_text     | 17.3 ms                                                | 16.3 ms: 1.06x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.18x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.81 ms: 1.75x faster                                                 |
| asyncio_tcp              | 659 ms                                                 | 437 ms: 1.51x faster                                                  |
| richards                 | 48.7 ms                                                | 33.5 ms: 1.45x faster                                                 |
| richards_super           | 57.8 ms                                                | 40.4 ms: 1.43x faster                                                 |
| mako                     | 9.87 ms                                                | 6.94 ms: 1.42x faster                                                 |
| scimark_sor              | 128 ms                                                 | 90.7 ms: 1.41x faster                                                 |
| logging_silent           | 117 ns                                                 | 83.0 ns: 1.41x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 336 ms: 1.41x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 51.6 ms: 1.39x faster                                                 |
| chaos                    | 65.8 ms                                                | 48.4 ms: 1.36x faster                                                 |
| nbody                    | 93.0 ms                                                | 68.5 ms: 1.36x faster                                                 |
| hexiom                   | 6.19 ms                                                | 4.61 ms: 1.34x faster                                                 |
| async_tree_none          | 388 ms                                                 | 290 ms: 1.34x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.69 ms: 1.33x faster                                                 |
| json_dumps               | 8.11 ms                                                | 6.08 ms: 1.33x faster                                                 |
| go                       | 151 ms                                                 | 113 ms: 1.33x faster                                                  |
| pyflate                  | 427 ms                                                 | 324 ms: 1.32x faster                                                  |
| raytrace                 | 301 ms                                                 | 229 ms: 1.32x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 214 us: 1.31x faster                                                  |
| pycparser                | 877 ms                                                 | 670 ms: 1.31x faster                                                  |
| async_tree_io            | 980 ms                                                 | 753 ms: 1.30x faster                                                  |
| thrift                   | 572 us                                                 | 443 us: 1.29x faster                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.70 ms: 1.27x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 37.1 ms: 1.25x faster                                                 |
| regex_compile            | 95.3 ms                                                | 76.0 ms: 1.25x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.28 sec: 1.25x faster                                                |
| create_gc_cycles         | 860 us                                                 | 687 us: 1.25x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 52.9 ms: 1.24x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.38 sec: 1.24x faster                                                |
| scimark_lu               | 103 ms                                                 | 83.3 ms: 1.23x faster                                                 |
| fannkuch                 | 303 ms                                                 | 246 ms: 1.23x faster                                                  |
| html5lib                 | 42.4 ms                                                | 34.6 ms: 1.22x faster                                                 |
| scimark_fft              | 224 ms                                                 | 183 ms: 1.22x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 524 ms: 1.22x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 533 ms: 1.22x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.07 sec: 1.22x faster                                                |
| deepcopy_memo            | 34.7 us                                                | 28.6 us: 1.21x faster                                                 |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.32 ms: 1.21x faster                                                 |
| dulwich_log              | 35.3 ms                                                | 29.2 ms: 1.21x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 161 us: 1.21x faster                                                  |
| float                    | 69.0 ms                                                | 57.5 ms: 1.20x faster                                                 |
| tornado_http             | 86.7 ms                                                | 72.3 ms: 1.20x faster                                                 |
| regex_dna                | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 1.05 ms: 1.18x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.23 ms: 1.18x faster                                                 |
| django_template          | 26.4 ms                                                | 22.5 ms: 1.17x faster                                                 |
| comprehensions           | 16.9 us                                                | 14.5 us: 1.17x faster                                                 |
| sqlalchemy_declarative   | 73.3 ms                                                | 62.6 ms: 1.17x faster                                                 |
| unpack_sequence          | 39.0 ns                                                | 33.4 ns: 1.17x faster                                                 |
| docutils                 | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                |
| spectral_norm            | 94.8 ms                                                | 81.8 ms: 1.16x faster                                                 |
| 2to3                     | 192 ms                                                 | 166 ms: 1.15x faster                                                  |
| logging_format           | 4.83 us                                                | 4.21 us: 1.15x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.89 us: 1.14x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 95.0 ms: 1.13x faster                                                 |
| regex_v8                 | 17.1 ms                                                | 15.3 ms: 1.12x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 82.4 ms: 1.12x faster                                                 |
| sympy_str                | 165 ms                                                 | 148 ms: 1.12x faster                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 33.1 ms: 1.11x faster                                                 |
| async_generators         | 231 ms                                                 | 209 ms: 1.11x faster                                                  |
| deepcopy                 | 272 us                                                 | 246 us: 1.11x faster                                                  |
| json                     | 3.08 ms                                                | 2.79 ms: 1.10x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 30.7 ms: 1.10x faster                                                 |
| xml_etree_generate       | 53.5 ms                                                | 48.7 ms: 1.10x faster                                                 |
| sympy_expand             | 269 ms                                                 | 245 ms: 1.10x faster                                                  |
| telco                    | 3.49 ms                                                | 3.18 ms: 1.10x faster                                                 |
| deepcopy_reduce          | 2.33 us                                                | 2.15 us: 1.09x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 495 us: 1.07x faster                                                  |
| nqueens                  | 63.8 ms                                                | 59.9 ms: 1.07x faster                                                 |
| genshi_text              | 17.3 ms                                                | 16.3 ms: 1.06x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.2 ms: 1.06x faster                                                 |
| json_loads               | 16.4 us                                                | 15.7 us: 1.05x faster                                                 |
| sqlglot_normalize        | 190 ms                                                 | 181 ms: 1.05x faster                                                  |
| sqlite_synth             | 1.46 us                                                | 1.40 us: 1.04x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.50 us: 1.04x faster                                                 |
| typing_runtime_protocols | 323 us                                                 | 319 us: 1.01x faster                                                  |
| pickle_dict              | 17.0 us                                                | 16.8 us: 1.01x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 77.2 ms: 1.01x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.72 us: 1.01x faster                                                 |
| regex_effbot             | 2.46 ms                                                | 2.45 ms: 1.01x faster                                                 |
| pidigits                 | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| coroutines               | 20.7 ms                                                | 20.6 ms: 1.00x faster                                                 |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                                 |
| pickle                   | 6.97 us                                                | 7.09 us: 1.02x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.85 us: 1.06x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.76 sec: 1.08x slower                                                |
| python_startup           | 10.9 ms                                                | 11.8 ms: 1.08x slower                                                 |
| bench_mp_pool            | 37.4 ms                                                | 43.7 ms: 1.17x slower                                                 |
| generators               | 32.3 ms                                                | 38.6 ms: 1.19x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.55 ms: 1.21x slower                                                 |
| dask                     | 253 ms                                                 | 327 ms: 1.29x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.16x faster                                                          |

Benchmark hidden because not significant (2): xml_etree_iterparse, asyncio_websockets
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint
Ignored benchmarks (4) of results/bm-20230207-3.12.0a5-3c67ec3/bm-20230207-darwin-arm64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.05x