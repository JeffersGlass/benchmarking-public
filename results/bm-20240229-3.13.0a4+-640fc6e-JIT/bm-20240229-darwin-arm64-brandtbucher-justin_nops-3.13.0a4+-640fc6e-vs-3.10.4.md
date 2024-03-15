# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_nops
- machine: darwin-arm64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 2.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 188 ms: 1.02x faster                                                |
| chameleon      | 6.26 ms                                                | 4.82 ms: 1.30x faster                                               |
| docutils       | 1.73 sec                                               | 1.52 sec: 1.14x faster                                              |
| html5lib       | 42.4 ms                                                | 35.6 ms: 1.19x faster                                               |
| tornado_http   | 86.7 ms                                                | 70.5 ms: 1.23x faster                                               |
| Geometric mean | (ref)                                                  | 1.17x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 251 ms: 1.55x faster                                                |
| async_tree_memoization  | 474 ms                                                 | 328 ms: 1.45x faster                                                |
| async_tree_io           | 980 ms                                                 | 701 ms: 1.40x faster                                                |
| async_tree_cpu_io_mixed | 649 ms                                                 | 518 ms: 1.25x faster                                                |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 71.3 ms: 1.30x faster                                               |
| float          | 69.0 ms                                                | 53.1 ms: 1.30x faster                                               |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                |
| Geometric mean | (ref)                                                  | 1.19x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                |
| regex_compile  | 95.3 ms                                                | 86.8 ms: 1.10x faster                                               |
| regex_v8       | 17.1 ms                                                | 17.2 ms: 1.00x slower                                               |
| regex_effbot   | 2.46 ms                                                | 2.62 ms: 1.07x slower                                               |
| Geometric mean | (ref)                                                  | 1.04x faster                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                |
| unpickle_pure_python | 194 us                                                 | 155 us: 1.26x faster                                                |
| tomli_loads          | 1.71 sec                                               | 1.37 sec: 1.25x faster                                              |
| json_dumps           | 8.11 ms                                                | 6.50 ms: 1.25x faster                                               |
| xml_etree_process    | 46.5 ms                                                | 39.2 ms: 1.19x faster                                               |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 74.5 ms: 1.03x slower                                               |
| json_loads           | 16.4 us                                                | 17.0 us: 1.03x slower                                               |
| unpickle             | 8.80 us                                                | 9.13 us: 1.04x slower                                               |
| xml_etree_generate   | 53.5 ms                                                | 55.8 ms: 1.04x slower                                               |
| pickle               | 6.97 us                                                | 7.29 us: 1.05x slower                                               |
| pickle_list          | 2.74 us                                                | 2.93 us: 1.07x slower                                               |
| pickle_dict          | 17.0 us                                                | 18.2 us: 1.07x slower                                               |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                               |
| Geometric mean       | (ref)                                                  | 1.06x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 18.4 ms: 1.69x slower                                               |
| python_startup_no_site | 7.91 ms                                                | 16.8 ms: 2.13x slower                                               |
| Geometric mean         | (ref)                                                  | 1.90x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 6.82 ms: 1.45x faster                                               |
| django_template | 26.4 ms                                                | 21.8 ms: 1.21x faster                                               |
| genshi_text     | 17.3 ms                                                | 15.7 ms: 1.11x faster                                               |
| genshi_xml      | 33.8 ms                                                | 37.1 ms: 1.10x slower                                               |
| Geometric mean  | (ref)                                                  | 1.15x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.3 us: 4.53x faster                                               |
| deltablue                | 4.91 ms                                                | 2.54 ms: 1.94x faster                                               |
| chaos                    | 65.8 ms                                                | 40.5 ms: 1.63x faster                                               |
| logging_silent           | 117 ns                                                 | 72.8 ns: 1.61x faster                                               |
| asyncio_tcp              | 659 ms                                                 | 411 ms: 1.60x faster                                                |
| raytrace                 | 301 ms                                                 | 191 ms: 1.57x faster                                                |
| pylint                   | 277 ms                                                 | 177 ms: 1.57x faster                                                |
| async_tree_none          | 388 ms                                                 | 251 ms: 1.55x faster                                                |
| crypto_pyaes             | 71.8 ms                                                | 47.7 ms: 1.51x faster                                               |
| sqlglot_parse            | 1.24 ms                                                | 834 us: 1.49x faster                                                |
| mako                     | 9.87 ms                                                | 6.82 ms: 1.45x faster                                               |
| async_tree_memoization   | 474 ms                                                 | 328 ms: 1.45x faster                                                |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                |
| scimark_monte_carlo      | 65.6 ms                                                | 46.0 ms: 1.42x faster                                               |
| sqlglot_transpile        | 1.44 ms                                                | 1.03 ms: 1.40x faster                                               |
| async_tree_io            | 980 ms                                                 | 701 ms: 1.40x faster                                                |
| deepcopy_memo            | 34.7 us                                                | 26.1 us: 1.33x faster                                               |
| richards_super           | 57.8 ms                                                | 43.5 ms: 1.33x faster                                               |
| comprehensions           | 16.9 us                                                | 13.0 us: 1.31x faster                                               |
| nbody                    | 93.0 ms                                                | 71.3 ms: 1.30x faster                                               |
| float                    | 69.0 ms                                                | 53.1 ms: 1.30x faster                                               |
| chameleon                | 6.26 ms                                                | 4.82 ms: 1.30x faster                                               |
| go                       | 151 ms                                                 | 116 ms: 1.30x faster                                                |
| logging_simple           | 4.45 us                                                | 3.49 us: 1.28x faster                                               |
| logging_format           | 4.83 us                                                | 3.80 us: 1.27x faster                                               |
| thrift                   | 572 us                                                 | 454 us: 1.26x faster                                                |
| unpickle_pure_python     | 194 us                                                 | 155 us: 1.26x faster                                                |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 518 ms: 1.25x faster                                                |
| tomli_loads              | 1.71 sec                                               | 1.37 sec: 1.25x faster                                              |
| json_dumps               | 8.11 ms                                                | 6.50 ms: 1.25x faster                                               |
| pprint_safe_repr         | 641 ms                                                 | 515 ms: 1.24x faster                                                |
| richards                 | 48.7 ms                                                | 39.3 ms: 1.24x faster                                               |
| pyflate                  | 427 ms                                                 | 346 ms: 1.23x faster                                                |
| pprint_pformat           | 1.30 sec                                               | 1.06 sec: 1.23x faster                                              |
| tornado_http             | 86.7 ms                                                | 70.5 ms: 1.23x faster                                               |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                              |
| django_template          | 26.4 ms                                                | 21.8 ms: 1.21x faster                                               |
| pycparser                | 877 ms                                                 | 727 ms: 1.21x faster                                                |
| create_gc_cycles         | 860 us                                                 | 716 us: 1.20x faster                                                |
| scimark_lu               | 103 ms                                                 | 85.7 ms: 1.20x faster                                               |
| sympy_sum                | 92.2 ms                                                | 76.9 ms: 1.20x faster                                               |
| deepcopy                 | 272 us                                                 | 228 us: 1.19x faster                                                |
| html5lib                 | 42.4 ms                                                | 35.6 ms: 1.19x faster                                               |
| xml_etree_process        | 46.5 ms                                                | 39.2 ms: 1.19x faster                                               |
| gunicorn                 | 1.30 ms                                                | 1.10 ms: 1.19x faster                                               |
| deepcopy_reduce          | 2.33 us                                                | 1.98 us: 1.18x faster                                               |
| hexiom                   | 6.19 ms                                                | 5.32 ms: 1.16x faster                                               |
| spectral_norm            | 94.8 ms                                                | 81.6 ms: 1.16x faster                                               |
| aiohttp                  | 1.22 ms                                                | 1.05 ms: 1.16x faster                                               |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                               |
| sympy_str                | 165 ms                                                 | 145 ms: 1.14x faster                                                |
| coroutines               | 20.7 ms                                                | 18.1 ms: 1.14x faster                                               |
| dulwich_log              | 35.3 ms                                                | 31.0 ms: 1.14x faster                                               |
| generators               | 32.3 ms                                                | 28.4 ms: 1.14x faster                                               |
| scimark_sor              | 128 ms                                                 | 113 ms: 1.14x faster                                                |
| docutils                 | 1.73 sec                                               | 1.52 sec: 1.14x faster                                              |
| scimark_fft              | 224 ms                                                 | 200 ms: 1.12x faster                                                |
| genshi_text              | 17.3 ms                                                | 15.7 ms: 1.11x faster                                               |
| regex_compile            | 95.3 ms                                                | 86.8 ms: 1.10x faster                                               |
| sympy_expand             | 269 ms                                                 | 247 ms: 1.09x faster                                                |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.14 ms: 1.09x faster                                               |
| json                     | 3.08 ms                                                | 2.95 ms: 1.05x faster                                               |
| meteor_contest           | 77.7 ms                                                | 75.0 ms: 1.04x faster                                               |
| sqlglot_normalize        | 190 ms                                                 | 183 ms: 1.04x faster                                                |
| sqlglot_optimize         | 36.8 ms                                                | 35.6 ms: 1.03x faster                                               |
| bench_thread_pool        | 527 us                                                 | 514 us: 1.03x faster                                                |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                                |
| 2to3                     | 192 ms                                                 | 188 ms: 1.02x faster                                                |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x faster                                                |
| mdp                      | 1.63 sec                                               | 1.63 sec: 1.00x faster                                              |
| regex_v8                 | 17.1 ms                                                | 17.2 ms: 1.00x slower                                               |
| nqueens                  | 63.8 ms                                                | 64.1 ms: 1.00x slower                                               |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                               |
| xml_etree_iterparse      | 72.1 ms                                                | 74.5 ms: 1.03x slower                                               |
| json_loads               | 16.4 us                                                | 17.0 us: 1.03x slower                                               |
| pathlib                  | 24.5 ms                                                | 25.3 ms: 1.03x slower                                               |
| unpickle                 | 8.80 us                                                | 9.13 us: 1.04x slower                                               |
| xml_etree_generate       | 53.5 ms                                                | 55.8 ms: 1.04x slower                                               |
| pickle                   | 6.97 us                                                | 7.29 us: 1.05x slower                                               |
| regex_effbot             | 2.46 ms                                                | 2.62 ms: 1.07x slower                                               |
| fannkuch                 | 303 ms                                                 | 323 ms: 1.07x slower                                                |
| pickle_list              | 2.74 us                                                | 2.93 us: 1.07x slower                                               |
| pickle_dict              | 17.0 us                                                | 18.2 us: 1.07x slower                                               |
| sqlite_synth             | 1.46 us                                                | 1.59 us: 1.09x slower                                               |
| genshi_xml               | 33.8 ms                                                | 37.1 ms: 1.10x slower                                               |
| coverage                 | 41.5 ms                                                | 47.2 ms: 1.14x slower                                               |
| unpickle_list            | 2.69 us                                                | 3.07 us: 1.14x slower                                               |
| telco                    | 3.49 ms                                                | 4.47 ms: 1.28x slower                                               |
| dask                     | 253 ms                                                 | 334 ms: 1.32x slower                                                |
| async_generators         | 231 ms                                                 | 311 ms: 1.35x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 52.9 ms: 1.42x slower                                               |
| python_startup           | 10.9 ms                                                | 18.4 ms: 1.69x slower                                               |
| python_startup_no_site   | 7.91 ms                                                | 16.8 ms: 2.13x slower                                               |
| unpack_sequence          | 39.0 ns                                                | 114 ns: 2.91x slower                                                |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                        |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 2.07x