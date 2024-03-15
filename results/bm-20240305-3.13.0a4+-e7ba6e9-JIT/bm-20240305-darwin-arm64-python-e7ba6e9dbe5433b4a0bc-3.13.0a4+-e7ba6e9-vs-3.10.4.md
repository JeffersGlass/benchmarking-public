# Results vs. 3.10.4

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: darwin-arm64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 2.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 189 ms: 1.01x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.83 ms: 1.30x faster                                                  |
| docutils       | 1.73 sec                                               | 1.53 sec: 1.13x faster                                                 |
| html5lib       | 42.4 ms                                                | 35.7 ms: 1.19x faster                                                  |
| tornado_http   | 86.7 ms                                                | 70.4 ms: 1.23x faster                                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 251 ms: 1.55x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 327 ms: 1.45x faster                                                   |
| async_tree_io           | 980 ms                                                 | 701 ms: 1.40x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 519 ms: 1.25x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 70.7 ms: 1.32x faster                                                  |
| float          | 69.0 ms                                                | 53.4 ms: 1.29x faster                                                  |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.19x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                   |
| regex_compile  | 95.3 ms                                                | 86.4 ms: 1.10x faster                                                  |
| regex_v8       | 17.1 ms                                                | 17.2 ms: 1.00x slower                                                  |
| regex_effbot   | 2.46 ms                                                | 2.62 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.42x faster                                                   |
| unpickle_pure_python | 194 us                                                 | 151 us: 1.29x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.47 ms: 1.25x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.37 sec: 1.24x faster                                                 |
| xml_etree_process    | 46.5 ms                                                | 38.8 ms: 1.20x faster                                                  |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| xml_etree_iterparse  | 72.1 ms                                                | 74.6 ms: 1.03x slower                                                  |
| json_loads           | 16.4 us                                                | 17.0 us: 1.04x slower                                                  |
| pickle               | 6.97 us                                                | 7.34 us: 1.05x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 56.4 ms: 1.05x slower                                                  |
| unpickle             | 8.80 us                                                | 9.27 us: 1.05x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.95 us: 1.08x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.11 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 18.7 ms: 1.72x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 17.0 ms: 2.15x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.92x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 6.82 ms: 1.45x faster                                                  |
| django_template | 26.4 ms                                                | 21.8 ms: 1.21x faster                                                  |
| genshi_text     | 17.3 ms                                                | 15.8 ms: 1.10x faster                                                  |
| genshi_xml      | 33.8 ms                                                | 37.3 ms: 1.10x slower                                                  |
| Geometric mean  | (ref)                                                  | 1.15x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 72.1 us: 4.48x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.54 ms: 1.93x faster                                                  |
| chaos                    | 65.8 ms                                                | 40.5 ms: 1.62x faster                                                  |
| logging_silent           | 117 ns                                                 | 73.0 ns: 1.61x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 414 ms: 1.59x faster                                                   |
| pylint                   | 277 ms                                                 | 176 ms: 1.57x faster                                                   |
| raytrace                 | 301 ms                                                 | 192 ms: 1.57x faster                                                   |
| async_tree_none          | 388 ms                                                 | 251 ms: 1.55x faster                                                   |
| crypto_pyaes             | 71.8 ms                                                | 47.7 ms: 1.51x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 835 us: 1.49x faster                                                   |
| async_tree_memoization   | 474 ms                                                 | 327 ms: 1.45x faster                                                   |
| mako                     | 9.87 ms                                                | 6.82 ms: 1.45x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 45.7 ms: 1.44x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.42x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.03 ms: 1.41x faster                                                  |
| async_tree_io            | 980 ms                                                 | 701 ms: 1.40x faster                                                   |
| richards_super           | 57.8 ms                                                | 42.7 ms: 1.35x faster                                                  |
| comprehensions           | 16.9 us                                                | 12.7 us: 1.33x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 26.2 us: 1.33x faster                                                  |
| nbody                    | 93.0 ms                                                | 70.7 ms: 1.32x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.83 ms: 1.30x faster                                                  |
| go                       | 151 ms                                                 | 117 ms: 1.29x faster                                                   |
| float                    | 69.0 ms                                                | 53.4 ms: 1.29x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 151 us: 1.29x faster                                                   |
| logging_format           | 4.83 us                                                | 3.77 us: 1.28x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.47 us: 1.28x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 74.6 ms: 1.27x faster                                                  |
| json_dumps               | 8.11 ms                                                | 6.47 ms: 1.25x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 519 ms: 1.25x faster                                                   |
| richards                 | 48.7 ms                                                | 39.1 ms: 1.25x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.37 sec: 1.24x faster                                                 |
| thrift                   | 572 us                                                 | 461 us: 1.24x faster                                                   |
| pprint_safe_repr         | 641 ms                                                 | 516 ms: 1.24x faster                                                   |
| pyflate                  | 427 ms                                                 | 344 ms: 1.24x faster                                                   |
| tornado_http             | 86.7 ms                                                | 70.4 ms: 1.23x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                                 |
| pprint_pformat           | 1.30 sec                                               | 1.06 sec: 1.23x faster                                                 |
| django_template          | 26.4 ms                                                | 21.8 ms: 1.21x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 76.3 ms: 1.21x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 714 us: 1.20x faster                                                   |
| scimark_lu               | 103 ms                                                 | 85.8 ms: 1.20x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 38.8 ms: 1.20x faster                                                  |
| pycparser                | 877 ms                                                 | 735 ms: 1.19x faster                                                   |
| html5lib                 | 42.4 ms                                                | 35.7 ms: 1.19x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.98 us: 1.18x faster                                                  |
| deepcopy                 | 272 us                                                 | 231 us: 1.18x faster                                                   |
| hexiom                   | 6.19 ms                                                | 5.26 ms: 1.18x faster                                                  |
| gunicorn                 | 1.30 ms                                                | 1.11 ms: 1.17x faster                                                  |
| aiohttp                  | 1.22 ms                                                | 1.05 ms: 1.16x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.4 ms: 1.15x faster                                                  |
| sympy_str                | 165 ms                                                 | 144 ms: 1.15x faster                                                   |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 30.8 ms: 1.15x faster                                                  |
| scimark_sor              | 128 ms                                                 | 112 ms: 1.14x faster                                                   |
| generators               | 32.3 ms                                                | 28.4 ms: 1.14x faster                                                  |
| docutils                 | 1.73 sec                                               | 1.53 sec: 1.13x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.3 ms: 1.13x faster                                                  |
| scimark_fft              | 224 ms                                                 | 199 ms: 1.12x faster                                                   |
| regex_compile            | 95.3 ms                                                | 86.4 ms: 1.10x faster                                                  |
| genshi_text              | 17.3 ms                                                | 15.8 ms: 1.10x faster                                                  |
| sympy_expand             | 269 ms                                                 | 245 ms: 1.10x faster                                                   |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.14 ms: 1.09x faster                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 35.4 ms: 1.04x faster                                                  |
| json                     | 3.08 ms                                                | 2.98 ms: 1.03x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 184 ms: 1.03x faster                                                   |
| meteor_contest           | 77.7 ms                                                | 75.4 ms: 1.03x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 516 us: 1.02x faster                                                   |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| 2to3                     | 192 ms                                                 | 189 ms: 1.01x faster                                                   |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.01x faster                                                 |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                   |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x faster                                                   |
| regex_v8                 | 17.1 ms                                                | 17.2 ms: 1.00x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                  |
| pathlib                  | 24.5 ms                                                | 25.2 ms: 1.03x slower                                                  |
| fannkuch                 | 303 ms                                                 | 312 ms: 1.03x slower                                                   |
| xml_etree_iterparse      | 72.1 ms                                                | 74.6 ms: 1.03x slower                                                  |
| json_loads               | 16.4 us                                                | 17.0 us: 1.04x slower                                                  |
| pickle                   | 6.97 us                                                | 7.34 us: 1.05x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 56.4 ms: 1.05x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.27 us: 1.05x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.62 ms: 1.07x slower                                                  |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.95 us: 1.08x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.58 us: 1.08x slower                                                  |
| genshi_xml               | 33.8 ms                                                | 37.3 ms: 1.10x slower                                                  |
| coverage                 | 41.5 ms                                                | 47.5 ms: 1.14x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.11 us: 1.15x slower                                                  |
| telco                    | 3.49 ms                                                | 4.46 ms: 1.28x slower                                                  |
| dask                     | 253 ms                                                 | 334 ms: 1.32x slower                                                   |
| async_generators         | 231 ms                                                 | 312 ms: 1.35x slower                                                   |
| bench_mp_pool            | 37.4 ms                                                | 53.4 ms: 1.43x slower                                                  |
| python_startup           | 10.9 ms                                                | 18.7 ms: 1.72x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 17.0 ms: 2.15x slower                                                  |
| unpack_sequence          | 39.0 ns                                                | 113 ns: 2.90x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.14x faster                                                           |

Benchmark hidden because not significant (2): mypy2, nqueens
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 2.06x