# Results vs. 3.10.4

- fork: gvanrossum
- ref: kenjin_tier2_inliner
- machine: linux-x86_64
- commit hash: 2f9539b
- commit date: 2024-03-05
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.34x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 277 ms: 1.26x faster                                                       |
| chameleon      | 9.68 ms                                                | 6.86 ms: 1.41x faster                                                      |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                     |
| html5lib       | 88.9 ms                                                | 66.5 ms: 1.34x faster                                                      |
| tornado_http   | 136 ms                                                 | 96.9 ms: 1.41x faster                                                      |
| Geometric mean | (ref)                                                  | 1.32x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 437 ms: 1.67x faster                                                       |
| async_tree_memoization  | 870 ms                                                 | 562 ms: 1.55x faster                                                       |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                     |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 707 ms: 1.44x faster                                                       |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.8 ms: 1.60x faster                                                      |
| float          | 117 ms                                                 | 78.2 ms: 1.50x faster                                                      |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                  | 1.35x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 142 ms: 1.33x faster                                                       |
| regex_v8       | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                      |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                       |
| regex_effbot   | 3.63 ms                                                | 3.73 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                  | 1.09x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 298 us: 1.62x faster                                                       |
| tomli_loads          | 3.14 sec                                               | 2.02 sec: 1.55x faster                                                     |
| unpickle_pure_python | 331 us                                                 | 238 us: 1.39x faster                                                       |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                      |
| xml_etree_process    | 79.1 ms                                                | 59.0 ms: 1.34x faster                                                      |
| xml_etree_generate   | 99.4 ms                                                | 86.8 ms: 1.15x faster                                                      |
| json_loads           | 31.2 us                                                | 27.5 us: 1.13x faster                                                      |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                       |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                       |
| unpickle_list        | 5.20 us                                                | 4.97 us: 1.05x faster                                                      |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                                      |
| unpickle             | 14.4 us                                                | 15.2 us: 1.06x slower                                                      |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                      |
| pickle_dict          | 29.6 us                                                | 34.6 us: 1.17x slower                                                      |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.4 ms: 1.18x faster                                                      |
| python_startup_no_site | 5.93 ms                                                | 11.0 ms: 1.85x slower                                                      |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.7 ms: 1.52x faster                                                      |
| django_template | 48.2 ms                                                | 33.9 ms: 1.42x faster                                                      |
| genshi_text     | 31.8 ms                                                | 24.0 ms: 1.33x faster                                                      |
| genshi_xml      | 66.0 ms                                                | 54.6 ms: 1.21x faster                                                      |
| Geometric mean  | (ref)                                                  | 1.37x faster                                                               |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.85x faster                                                       |
| generators               | 80.1 ms                                                | 29.5 ms: 2.71x faster                                                      |
| deltablue                | 7.91 ms                                                | 3.39 ms: 2.33x faster                                                      |
| asyncio_tcp              | 922 ms                                                 | 487 ms: 1.89x faster                                                       |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                                       |
| chaos                    | 115 ms                                                 | 62.5 ms: 1.85x faster                                                      |
| richards_super           | 94.7 ms                                                | 51.8 ms: 1.83x faster                                                      |
| raytrace                 | 507 ms                                                 | 288 ms: 1.76x faster                                                       |
| crypto_pyaes             | 128 ms                                                 | 73.3 ms: 1.74x faster                                                      |
| richards                 | 79.3 ms                                                | 45.5 ms: 1.74x faster                                                      |
| pylint                   | 551 ms                                                 | 319 ms: 1.73x faster                                                       |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.70x faster                                                      |
| scimark_sor              | 220 ms                                                 | 130 ms: 1.69x faster                                                       |
| scimark_monte_carlo      | 118 ms                                                 | 70.6 ms: 1.67x faster                                                      |
| async_tree_none          | 728 ms                                                 | 437 ms: 1.67x faster                                                       |
| comprehensions           | 28.8 us                                                | 17.5 us: 1.65x faster                                                      |
| pickle_pure_python       | 484 us                                                 | 298 us: 1.62x faster                                                       |
| nbody                    | 154 ms                                                 | 95.8 ms: 1.60x faster                                                      |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                      |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                                      |
| tomli_loads              | 3.14 sec                                               | 2.02 sec: 1.55x faster                                                     |
| async_tree_memoization   | 870 ms                                                 | 562 ms: 1.55x faster                                                       |
| go                       | 240 ms                                                 | 156 ms: 1.54x faster                                                       |
| mako                     | 16.3 ms                                                | 10.7 ms: 1.52x faster                                                      |
| spectral_norm            | 170 ms                                                 | 113 ms: 1.50x faster                                                       |
| float                    | 117 ms                                                 | 78.2 ms: 1.50x faster                                                      |
| pyflate                  | 716 ms                                                 | 480 ms: 1.49x faster                                                       |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                     |
| deepcopy_memo            | 58.5 us                                                | 39.3 us: 1.49x faster                                                      |
| hexiom                   | 10.4 ms                                                | 7.00 ms: 1.49x faster                                                      |
| logging_simple           | 8.30 us                                                | 5.64 us: 1.47x faster                                                      |
| logging_format           | 9.09 us                                                | 6.23 us: 1.46x faster                                                      |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 707 ms: 1.44x faster                                                       |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                     |
| django_template          | 48.2 ms                                                | 33.9 ms: 1.42x faster                                                      |
| chameleon                | 9.68 ms                                                | 6.86 ms: 1.41x faster                                                      |
| tornado_http             | 136 ms                                                 | 96.9 ms: 1.41x faster                                                      |
| unpickle_pure_python     | 331 us                                                 | 238 us: 1.39x faster                                                       |
| pprint_safe_repr         | 1.02 sec                                               | 745 ms: 1.37x faster                                                       |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                      |
| scimark_fft              | 466 ms                                                 | 342 ms: 1.36x faster                                                       |
| pprint_pformat           | 2.10 sec                                               | 1.54 sec: 1.36x faster                                                     |
| deepcopy                 | 479 us                                                 | 353 us: 1.36x faster                                                       |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                                      |
| thrift                   | 1.07 ms                                                | 793 us: 1.35x faster                                                       |
| scimark_lu               | 176 ms                                                 | 130 ms: 1.35x faster                                                       |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                                       |
| xml_etree_process        | 79.1 ms                                                | 59.0 ms: 1.34x faster                                                      |
| html5lib                 | 88.9 ms                                                | 66.5 ms: 1.34x faster                                                      |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                       |
| genshi_text              | 31.8 ms                                                | 24.0 ms: 1.33x faster                                                      |
| regex_compile            | 188 ms                                                 | 142 ms: 1.33x faster                                                       |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                                     |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.02 ms: 1.29x faster                                                      |
| 2to3                     | 348 ms                                                 | 277 ms: 1.26x faster                                                       |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                                       |
| sqlglot_optimize         | 69.2 ms                                                | 55.6 ms: 1.24x faster                                                      |
| sympy_str                | 346 ms                                                 | 279 ms: 1.24x faster                                                       |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.24x faster                                                      |
| aiohttp                  | 1.44 ms                                                | 1.16 ms: 1.24x faster                                                      |
| dulwich_log              | 84.3 ms                                                | 68.9 ms: 1.22x faster                                                      |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                     |
| genshi_xml               | 66.0 ms                                                | 54.6 ms: 1.21x faster                                                      |
| gunicorn                 | 1.53 ms                                                | 1.27 ms: 1.21x faster                                                      |
| sympy_expand             | 566 ms                                                 | 474 ms: 1.19x faster                                                       |
| djangocms                | 38.4 us                                                | 32.4 us: 1.19x faster                                                      |
| python_startup           | 14.6 ms                                                | 12.4 ms: 1.18x faster                                                      |
| nqueens                  | 106 ms                                                 | 89.7 ms: 1.18x faster                                                      |
| bench_thread_pool        | 986 us                                                 | 846 us: 1.17x faster                                                       |
| xml_etree_generate       | 99.4 ms                                                | 86.8 ms: 1.15x faster                                                      |
| json_loads               | 31.2 us                                                | 27.5 us: 1.13x faster                                                      |
| json                     | 5.69 ms                                                | 5.11 ms: 1.11x faster                                                      |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.11x faster                                                       |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                      |
| mdp                      | 2.85 sec                                               | 2.60 sec: 1.10x faster                                                     |
| regex_v8                 | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                      |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                       |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                      |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                                      |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                       |
| unpickle_list            | 5.20 us                                                | 4.97 us: 1.05x faster                                                      |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                       |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                       |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                       |
| regex_effbot             | 3.63 ms                                                | 3.73 ms: 1.03x slower                                                      |
| pickle_list              | 5.08 us                                                | 5.23 us: 1.03x slower                                                      |
| async_generators         | 444 ms                                                 | 463 ms: 1.04x slower                                                       |
| unpickle                 | 14.4 us                                                | 15.2 us: 1.06x slower                                                      |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                      |
| gc_traversal             | 3.62 ms                                                | 4.03 ms: 1.11x slower                                                      |
| telco                    | 7.27 ms                                                | 8.48 ms: 1.17x slower                                                      |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                      |
| pickle_dict              | 29.6 us                                                | 34.6 us: 1.17x slower                                                      |
| dask                     | 441 ms                                                 | 533 ms: 1.21x slower                                                       |
| coverage                 | 79.4 ms                                                | 97.1 ms: 1.22x slower                                                      |
| unpack_sequence          | 60.0 ns                                                | 96.7 ns: 1.61x slower                                                      |
| python_startup_no_site   | 5.93 ms                                                | 11.0 ms: 1.85x slower                                                      |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                               |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-2f9539b-JIT/bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.34x