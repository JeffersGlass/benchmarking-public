# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_mprotect
- machine: darwin-arm64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: 2.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 205 ms: 1.07x slower                                                    |
| chameleon      | 6.26 ms                                                | 4.87 ms: 1.29x faster                                                   |
| docutils       | 1.73 sec                                               | 1.53 sec: 1.13x faster                                                  |
| tornado_http   | 86.7 ms                                                | 71.0 ms: 1.22x faster                                                   |
| Geometric mean | (ref)                                                  | 1.14x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 252 ms: 1.54x faster                                                    |
| async_tree_memoization  | 474 ms                                                 | 327 ms: 1.45x faster                                                    |
| async_tree_io           | 980 ms                                                 | 700 ms: 1.40x faster                                                    |
| async_tree_cpu_io_mixed | 649 ms                                                 | 519 ms: 1.25x faster                                                    |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 70.3 ms: 1.32x faster                                                   |
| float          | 69.0 ms                                                | 53.0 ms: 1.30x faster                                                   |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                    |
| Geometric mean | (ref)                                                  | 1.20x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                    |
| regex_compile  | 95.3 ms                                                | 86.8 ms: 1.10x faster                                                   |
| regex_v8       | 17.1 ms                                                | 17.3 ms: 1.01x slower                                                   |
| regex_effbot   | 2.46 ms                                                | 2.65 ms: 1.08x slower                                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                    |
| unpickle_pure_python | 194 us                                                 | 151 us: 1.29x faster                                                    |
| json_dumps           | 8.11 ms                                                | 6.49 ms: 1.25x faster                                                   |
| tomli_loads          | 1.71 sec                                               | 1.38 sec: 1.23x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 39.3 ms: 1.18x faster                                                   |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                                    |
| xml_etree_iterparse  | 72.1 ms                                                | 74.3 ms: 1.03x slower                                                   |
| json_loads           | 16.4 us                                                | 17.0 us: 1.03x slower                                                   |
| xml_etree_generate   | 53.5 ms                                                | 55.7 ms: 1.04x slower                                                   |
| unpickle             | 8.80 us                                                | 9.21 us: 1.05x slower                                                   |
| pickle               | 6.97 us                                                | 7.32 us: 1.05x slower                                                   |
| pickle_list          | 2.74 us                                                | 2.94 us: 1.07x slower                                                   |
| pickle_dict          | 17.0 us                                                | 18.2 us: 1.07x slower                                                   |
| unpickle_list        | 2.69 us                                                | 3.05 us: 1.13x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.06x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 17.9 ms: 1.64x slower                                                   |
| python_startup_no_site | 7.91 ms                                                | 16.3 ms: 2.06x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.84x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 6.80 ms: 1.45x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.5 us: 4.52x faster                                                   |
| deltablue                | 4.91 ms                                                | 2.55 ms: 1.93x faster                                                   |
| logging_silent           | 117 ns                                                 | 72.2 ns: 1.62x faster                                                   |
| chaos                    | 65.8 ms                                                | 40.5 ms: 1.62x faster                                                   |
| raytrace                 | 301 ms                                                 | 191 ms: 1.57x faster                                                    |
| asyncio_tcp              | 659 ms                                                 | 420 ms: 1.57x faster                                                    |
| async_tree_none          | 388 ms                                                 | 252 ms: 1.54x faster                                                    |
| crypto_pyaes             | 71.8 ms                                                | 48.1 ms: 1.49x faster                                                   |
| sqlglot_parse            | 1.24 ms                                                | 840 us: 1.48x faster                                                    |
| mako                     | 9.87 ms                                                | 6.80 ms: 1.45x faster                                                   |
| async_tree_memoization   | 474 ms                                                 | 327 ms: 1.45x faster                                                    |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                    |
| scimark_monte_carlo      | 65.6 ms                                                | 46.0 ms: 1.42x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.02 ms: 1.41x faster                                                   |
| async_tree_io            | 980 ms                                                 | 700 ms: 1.40x faster                                                    |
| nbody                    | 93.0 ms                                                | 70.3 ms: 1.32x faster                                                   |
| deepcopy_memo            | 34.7 us                                                | 26.3 us: 1.32x faster                                                   |
| comprehensions           | 16.9 us                                                | 12.8 us: 1.32x faster                                                   |
| richards_super           | 57.8 ms                                                | 44.2 ms: 1.31x faster                                                   |
| float                    | 69.0 ms                                                | 53.0 ms: 1.30x faster                                                   |
| go                       | 151 ms                                                 | 116 ms: 1.29x faster                                                    |
| unpickle_pure_python     | 194 us                                                 | 151 us: 1.29x faster                                                    |
| chameleon                | 6.26 ms                                                | 4.87 ms: 1.29x faster                                                   |
| logging_format           | 4.83 us                                                | 3.79 us: 1.27x faster                                                   |
| logging_simple           | 4.45 us                                                | 3.50 us: 1.27x faster                                                   |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 519 ms: 1.25x faster                                                    |
| json_dumps               | 8.11 ms                                                | 6.49 ms: 1.25x faster                                                   |
| pprint_safe_repr         | 641 ms                                                 | 517 ms: 1.24x faster                                                    |
| tomli_loads              | 1.71 sec                                               | 1.38 sec: 1.23x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.06 sec: 1.23x faster                                                  |
| tornado_http             | 86.7 ms                                                | 71.0 ms: 1.22x faster                                                   |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.22x faster                                                  |
| pyflate                  | 427 ms                                                 | 350 ms: 1.22x faster                                                    |
| sympy_sum                | 92.2 ms                                                | 76.3 ms: 1.21x faster                                                   |
| create_gc_cycles         | 860 us                                                 | 712 us: 1.21x faster                                                    |
| pycparser                | 877 ms                                                 | 726 ms: 1.21x faster                                                    |
| richards                 | 48.7 ms                                                | 40.5 ms: 1.20x faster                                                   |
| scimark_lu               | 103 ms                                                 | 85.7 ms: 1.20x faster                                                   |
| spectral_norm            | 94.8 ms                                                | 79.3 ms: 1.20x faster                                                   |
| xml_etree_process        | 46.5 ms                                                | 39.3 ms: 1.18x faster                                                   |
| deepcopy                 | 272 us                                                 | 230 us: 1.18x faster                                                    |
| deepcopy_reduce          | 2.33 us                                                | 2.00 us: 1.17x faster                                                   |
| hexiom                   | 6.19 ms                                                | 5.31 ms: 1.17x faster                                                   |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                    |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.15x faster                                                   |
| sympy_str                | 165 ms                                                 | 144 ms: 1.14x faster                                                    |
| dulwich_log              | 35.3 ms                                                | 30.9 ms: 1.14x faster                                                   |
| generators               | 32.3 ms                                                | 28.3 ms: 1.14x faster                                                   |
| scimark_sor              | 128 ms                                                 | 113 ms: 1.14x faster                                                    |
| coroutines               | 20.7 ms                                                | 18.3 ms: 1.13x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.53 sec: 1.13x faster                                                  |
| scimark_fft              | 224 ms                                                 | 200 ms: 1.12x faster                                                    |
| regex_compile            | 95.3 ms                                                | 86.8 ms: 1.10x faster                                                   |
| sympy_expand             | 269 ms                                                 | 246 ms: 1.09x faster                                                    |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.17 ms: 1.08x faster                                                   |
| json                     | 3.08 ms                                                | 2.96 ms: 1.04x faster                                                   |
| sqlglot_normalize        | 190 ms                                                 | 183 ms: 1.04x faster                                                    |
| meteor_contest           | 77.7 ms                                                | 75.0 ms: 1.04x faster                                                   |
| bench_thread_pool        | 527 us                                                 | 511 us: 1.03x faster                                                    |
| sqlglot_optimize         | 36.8 ms                                                | 35.6 ms: 1.03x faster                                                   |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                                    |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                    |
| nqueens                  | 63.8 ms                                                | 64.1 ms: 1.01x slower                                                   |
| fannkuch                 | 303 ms                                                 | 305 ms: 1.01x slower                                                    |
| regex_v8                 | 17.1 ms                                                | 17.3 ms: 1.01x slower                                                   |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                   |
| xml_etree_iterparse      | 72.1 ms                                                | 74.3 ms: 1.03x slower                                                   |
| json_loads               | 16.4 us                                                | 17.0 us: 1.03x slower                                                   |
| xml_etree_generate       | 53.5 ms                                                | 55.7 ms: 1.04x slower                                                   |
| pathlib                  | 24.5 ms                                                | 25.5 ms: 1.04x slower                                                   |
| unpickle                 | 8.80 us                                                | 9.21 us: 1.05x slower                                                   |
| pickle                   | 6.97 us                                                | 7.32 us: 1.05x slower                                                   |
| 2to3                     | 192 ms                                                 | 205 ms: 1.07x slower                                                    |
| pickle_list              | 2.74 us                                                | 2.94 us: 1.07x slower                                                   |
| pickle_dict              | 17.0 us                                                | 18.2 us: 1.07x slower                                                   |
| regex_effbot             | 2.46 ms                                                | 2.65 ms: 1.08x slower                                                   |
| sqlite_synth             | 1.46 us                                                | 1.58 us: 1.08x slower                                                   |
| unpickle_list            | 2.69 us                                                | 3.05 us: 1.13x slower                                                   |
| coverage                 | 41.5 ms                                                | 47.6 ms: 1.15x slower                                                   |
| dask                     | 253 ms                                                 | 332 ms: 1.31x slower                                                    |
| telco                    | 3.49 ms                                                | 4.60 ms: 1.32x slower                                                   |
| async_generators         | 231 ms                                                 | 310 ms: 1.34x slower                                                    |
| bench_mp_pool            | 37.4 ms                                                | 52.6 ms: 1.41x slower                                                   |
| python_startup           | 10.9 ms                                                | 17.9 ms: 1.64x slower                                                   |
| python_startup_no_site   | 7.91 ms                                                | 16.3 ms: 2.06x slower                                                   |
| unpack_sequence          | 39.0 ns                                                | 113 ns: 2.90x slower                                                    |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                            |

Benchmark hidden because not significant (3): mypy2, asyncio_websockets, mdp
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-84bbac4-JIT/bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: 2.06x