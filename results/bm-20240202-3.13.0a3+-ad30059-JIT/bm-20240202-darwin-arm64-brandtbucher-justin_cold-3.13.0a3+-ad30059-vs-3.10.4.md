
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_cold
- machine: darwin-arm64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.18x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.35x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 177 ms: 1.08x faster                                                |
| chameleon      | 6.26 ms                                                | 4.86 ms: 1.29x faster                                               |
| docutils       | 1.73 sec                                               | 1.48 sec: 1.17x faster                                              |
| tornado_http   | 86.7 ms                                                | 69.8 ms: 1.24x faster                                               |
| Geometric mean | (ref)                                                  | 1.19x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 250 ms: 1.55x faster                                                |
| async_tree_memoization  | 474 ms                                                 | 327 ms: 1.45x faster                                                |
| async_tree_io           | 980 ms                                                 | 693 ms: 1.41x faster                                                |
| async_tree_cpu_io_mixed | 649 ms                                                 | 518 ms: 1.25x faster                                                |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 55.7 ms: 1.24x faster                                               |
| nbody          | 93.0 ms                                                | 76.6 ms: 1.21x faster                                               |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                |
| Geometric mean | (ref)                                                  | 1.15x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 76.6 ms: 1.24x faster                                               |
| regex_dna      | 174 ms                                                 | 153 ms: 1.14x faster                                                |
| regex_v8       | 17.1 ms                                                | 17.2 ms: 1.00x slower                                               |
| regex_effbot   | 2.46 ms                                                | 2.56 ms: 1.04x slower                                               |
| Geometric mean | (ref)                                                  | 1.08x faster                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                |
| json_dumps           | 8.11 ms                                                | 6.49 ms: 1.25x faster                                               |
| unpickle_pure_python | 194 us                                                 | 158 us: 1.23x faster                                                |
| tomli_loads          | 1.71 sec                                               | 1.41 sec: 1.21x faster                                              |
| xml_etree_process    | 46.5 ms                                                | 39.3 ms: 1.18x faster                                               |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.01x faster                                                |
| unpickle             | 8.80 us                                                | 8.99 us: 1.02x slower                                               |
| json_loads           | 16.4 us                                                | 17.0 us: 1.03x slower                                               |
| pickle               | 6.97 us                                                | 7.29 us: 1.05x slower                                               |
| xml_etree_iterparse  | 72.1 ms                                                | 76.0 ms: 1.05x slower                                               |
| pickle_dict          | 17.0 us                                                | 18.0 us: 1.06x slower                                               |
| xml_etree_generate   | 53.5 ms                                                | 56.9 ms: 1.06x slower                                               |
| pickle_list          | 2.74 us                                                | 3.00 us: 1.09x slower                                               |
| unpickle_list        | 2.69 us                                                | 3.08 us: 1.14x slower                                               |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.6 ms: 1.07x slower                                               |
| python_startup_no_site | 7.91 ms                                                | 10.2 ms: 1.28x slower                                               |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.94 ms: 1.24x faster                                               |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.2 us: 4.54x faster                                               |
| deltablue                | 4.91 ms                                                | 2.51 ms: 1.96x faster                                               |
| raytrace                 | 301 ms                                                 | 177 ms: 1.70x faster                                                |
| logging_silent           | 117 ns                                                 | 70.3 ns: 1.67x faster                                               |
| asyncio_tcp              | 659 ms                                                 | 405 ms: 1.63x faster                                                |
| richards_super           | 57.8 ms                                                | 35.9 ms: 1.61x faster                                               |
| chaos                    | 65.8 ms                                                | 41.8 ms: 1.57x faster                                               |
| sqlglot_parse            | 1.24 ms                                                | 794 us: 1.57x faster                                                |
| async_tree_none          | 388 ms                                                 | 250 ms: 1.55x faster                                                |
| richards                 | 48.7 ms                                                | 32.0 ms: 1.52x faster                                               |
| crypto_pyaes             | 71.8 ms                                                | 49.0 ms: 1.47x faster                                               |
| sqlglot_transpile        | 1.44 ms                                                | 985 us: 1.46x faster                                                |
| async_tree_memoization   | 474 ms                                                 | 327 ms: 1.45x faster                                                |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                |
| async_tree_io            | 980 ms                                                 | 693 ms: 1.41x faster                                                |
| unpack_sequence          | 39.0 ns                                                | 28.2 ns: 1.38x faster                                               |
| go                       | 151 ms                                                 | 109 ms: 1.38x faster                                                |
| scimark_lu               | 103 ms                                                 | 75.2 ms: 1.37x faster                                               |
| deepcopy_memo            | 34.7 us                                                | 26.0 us: 1.34x faster                                               |
| comprehensions           | 16.9 us                                                | 12.7 us: 1.33x faster                                               |
| scimark_monte_carlo      | 65.6 ms                                                | 49.3 ms: 1.33x faster                                               |
| pyflate                  | 427 ms                                                 | 328 ms: 1.30x faster                                                |
| chameleon                | 6.26 ms                                                | 4.86 ms: 1.29x faster                                               |
| logging_simple           | 4.45 us                                                | 3.48 us: 1.28x faster                                               |
| logging_format           | 4.83 us                                                | 3.80 us: 1.27x faster                                               |
| pycparser                | 877 ms                                                 | 696 ms: 1.26x faster                                                |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 518 ms: 1.25x faster                                                |
| json_dumps               | 8.11 ms                                                | 6.49 ms: 1.25x faster                                               |
| pprint_safe_repr         | 641 ms                                                 | 515 ms: 1.24x faster                                                |
| regex_compile            | 95.3 ms                                                | 76.6 ms: 1.24x faster                                               |
| hexiom                   | 6.19 ms                                                | 4.98 ms: 1.24x faster                                               |
| mako                     | 9.87 ms                                                | 7.94 ms: 1.24x faster                                               |
| tornado_http             | 86.7 ms                                                | 69.8 ms: 1.24x faster                                               |
| float                    | 69.0 ms                                                | 55.7 ms: 1.24x faster                                               |
| pprint_pformat           | 1.30 sec                                               | 1.05 sec: 1.24x faster                                              |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                              |
| unpickle_pure_python     | 194 us                                                 | 158 us: 1.23x faster                                                |
| create_gc_cycles         | 860 us                                                 | 701 us: 1.23x faster                                                |
| scimark_sor              | 128 ms                                                 | 105 ms: 1.22x faster                                                |
| nbody                    | 93.0 ms                                                | 76.6 ms: 1.21x faster                                               |
| tomli_loads              | 1.71 sec                                               | 1.41 sec: 1.21x faster                                              |
| sympy_sum                | 92.2 ms                                                | 76.5 ms: 1.20x faster                                               |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                                |
| xml_etree_process        | 46.5 ms                                                | 39.3 ms: 1.18x faster                                               |
| dulwich_log              | 35.3 ms                                                | 30.0 ms: 1.18x faster                                               |
| docutils                 | 1.73 sec                                               | 1.48 sec: 1.17x faster                                              |
| spectral_norm            | 94.8 ms                                                | 81.1 ms: 1.17x faster                                               |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                               |
| sympy_integrate          | 13.1 ms                                                | 11.3 ms: 1.16x faster                                               |
| sympy_str                | 165 ms                                                 | 142 ms: 1.16x faster                                                |
| mypy2                    | 607 ms                                                 | 526 ms: 1.15x faster                                                |
| regex_dna                | 174 ms                                                 | 153 ms: 1.14x faster                                                |
| generators               | 32.3 ms                                                | 28.4 ms: 1.14x faster                                               |
| dask                     | 253 ms                                                 | 225 ms: 1.12x faster                                                |
| coroutines               | 20.7 ms                                                | 18.5 ms: 1.12x faster                                               |
| sympy_expand             | 269 ms                                                 | 242 ms: 1.11x faster                                                |
| fannkuch                 | 303 ms                                                 | 278 ms: 1.09x faster                                                |
| 2to3                     | 192 ms                                                 | 177 ms: 1.08x faster                                                |
| sqlglot_optimize         | 36.8 ms                                                | 34.7 ms: 1.06x faster                                               |
| json                     | 3.08 ms                                                | 2.94 ms: 1.05x faster                                               |
| meteor_contest           | 77.7 ms                                                | 74.1 ms: 1.05x faster                                               |
| bench_thread_pool        | 527 us                                                 | 508 us: 1.04x faster                                                |
| sqlglot_normalize        | 190 ms                                                 | 184 ms: 1.03x faster                                                |
| scimark_fft              | 224 ms                                                 | 218 ms: 1.03x faster                                                |
| pathlib                  | 24.5 ms                                                | 23.9 ms: 1.02x faster                                               |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.35 ms: 1.02x faster                                               |
| nqueens                  | 63.8 ms                                                | 62.5 ms: 1.02x faster                                               |
| mdp                      | 1.63 sec                                               | 1.60 sec: 1.02x faster                                              |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.01x faster                                                |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x faster                                                |
| regex_v8                 | 17.1 ms                                                | 17.2 ms: 1.00x slower                                               |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                               |
| unpickle                 | 8.80 us                                                | 8.99 us: 1.02x slower                                               |
| json_loads               | 16.4 us                                                | 17.0 us: 1.03x slower                                               |
| regex_effbot             | 2.46 ms                                                | 2.56 ms: 1.04x slower                                               |
| pickle                   | 6.97 us                                                | 7.29 us: 1.05x slower                                               |
| xml_etree_iterparse      | 72.1 ms                                                | 76.0 ms: 1.05x slower                                               |
| pickle_dict              | 17.0 us                                                | 18.0 us: 1.06x slower                                               |
| xml_etree_generate       | 53.5 ms                                                | 56.9 ms: 1.06x slower                                               |
| python_startup           | 10.9 ms                                                | 11.6 ms: 1.07x slower                                               |
| pickle_list              | 2.74 us                                                | 3.00 us: 1.09x slower                                               |
| sqlite_synth             | 1.46 us                                                | 1.60 us: 1.09x slower                                               |
| coverage                 | 41.5 ms                                                | 46.8 ms: 1.13x slower                                               |
| unpickle_list            | 2.69 us                                                | 3.08 us: 1.14x slower                                               |
| bench_mp_pool            | 37.4 ms                                                | 45.7 ms: 1.22x slower                                               |
| python_startup_no_site   | 7.91 ms                                                | 10.2 ms: 1.28x slower                                               |
| async_generators         | 231 ms                                                 | 304 ms: 1.32x slower                                                |
| telco                    | 3.49 ms                                                | 4.61 ms: 1.32x slower                                               |
| Geometric mean           | (ref)                                                  | 1.18x faster                                                        |
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240202-3.13.0a3+-ad30059-JIT/bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.35x