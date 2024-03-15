
# Results vs. 3.10.4

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: darwin-arm64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 165 ms: 1.16x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.87 ms: 1.29x faster                                                 |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.14x faster                                                |
| html5lib       | 42.4 ms                                                | 36.4 ms: 1.16x faster                                                 |
| tornado_http   | 86.7 ms                                                | 77.9 ms: 1.11x faster                                                 |
| Geometric mean | (ref)                                                  | 1.17x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 288 ms: 1.35x faster                                                  |
| async_tree_memoization  | 474 ms                                                 | 359 ms: 1.32x faster                                                  |
| async_tree_io           | 980 ms                                                 | 786 ms: 1.25x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 568 ms: 1.14x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.26x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 53.4 ms: 1.29x faster                                                 |
| nbody          | 93.0 ms                                                | 73.1 ms: 1.27x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.18x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 76.4 ms: 1.25x faster                                                 |
| regex_v8       | 17.1 ms                                                | 16.8 ms: 1.02x faster                                                 |
| regex_dna      | 174 ms                                                 | 174 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_process    | 46.5 ms                                                | 36.3 ms: 1.28x faster                                                 |
| pickle_pure_python   | 281 us                                                 | 223 us: 1.26x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 169 us: 1.15x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.52 sec: 1.12x faster                                                |
| xml_etree_parse      | 108 ms                                                 | 96.5 ms: 1.12x faster                                                 |
| xml_etree_generate   | 53.5 ms                                                | 48.3 ms: 1.11x faster                                                 |
| json_loads           | 16.4 us                                                | 15.4 us: 1.07x faster                                                 |
| json_dumps           | 8.11 ms                                                | 7.61 ms: 1.07x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.64 us: 1.04x faster                                                 |
| unpickle             | 8.80 us                                                | 8.57 us: 1.03x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 70.5 ms: 1.02x faster                                                 |
| pickle_dict          | 17.0 us                                                | 16.8 us: 1.01x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| pickle               | 6.97 us                                                | 7.26 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 7.91 ms                                                | 8.93 ms: 1.13x slower                                                 |
| python_startup         | 10.9 ms                                                | 15.3 ms: 1.40x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.26x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 8.15 ms: 1.21x faster                                                 |
| django_template | 26.4 ms                                                | 22.2 ms: 1.19x faster                                                 |
| genshi_text     | 17.3 ms                                                | 15.4 ms: 1.13x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 30.6 ms: 1.11x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.16x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 3.26 ms: 1.51x faster                                                 |
| logging_silent           | 117 ns                                                 | 81.4 ns: 1.44x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 47.9 ms: 1.37x faster                                                 |
| raytrace                 | 301 ms                                                 | 223 ms: 1.35x faster                                                  |
| async_tree_none          | 388 ms                                                 | 288 ms: 1.35x faster                                                  |
| chaos                    | 65.8 ms                                                | 49.5 ms: 1.33x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 359 ms: 1.32x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 487 ms: 1.32x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 996 ms: 1.31x faster                                                  |
| scimark_sor              | 128 ms                                                 | 98.4 ms: 1.30x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 72.9 ms: 1.30x faster                                                 |
| float                    | 69.0 ms                                                | 53.4 ms: 1.29x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.44 us: 1.29x faster                                                 |
| logging_format           | 4.83 us                                                | 3.74 us: 1.29x faster                                                 |
| chameleon                | 6.26 ms                                                | 4.87 ms: 1.29x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 36.3 ms: 1.28x faster                                                 |
| nbody                    | 93.0 ms                                                | 73.1 ms: 1.27x faster                                                 |
| thrift                   | 572 us                                                 | 453 us: 1.26x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 56.9 ms: 1.26x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 223 us: 1.26x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.95 ms: 1.25x faster                                                 |
| richards                 | 48.7 ms                                                | 39.0 ms: 1.25x faster                                                 |
| regex_compile            | 95.3 ms                                                | 76.4 ms: 1.25x faster                                                 |
| async_tree_io            | 980 ms                                                 | 786 ms: 1.25x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 27.9 us: 1.24x faster                                                 |
| mako                     | 9.87 ms                                                | 8.15 ms: 1.21x faster                                                 |
| richards_super           | 57.8 ms                                                | 48.0 ms: 1.21x faster                                                 |
| pyflate                  | 427 ms                                                 | 354 ms: 1.21x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 32.6 ns: 1.20x faster                                                 |
| django_template          | 26.4 ms                                                | 22.2 ms: 1.19x faster                                                 |
| pycparser                | 877 ms                                                 | 742 ms: 1.18x faster                                                  |
| scimark_lu               | 103 ms                                                 | 87.1 ms: 1.18x faster                                                 |
| scimark_fft              | 224 ms                                                 | 190 ms: 1.18x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 732 us: 1.17x faster                                                  |
| async_generators         | 231 ms                                                 | 197 ms: 1.17x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                                 |
| dulwich_log              | 35.3 ms                                                | 30.2 ms: 1.17x faster                                                 |
| deepcopy                 | 272 us                                                 | 233 us: 1.17x faster                                                  |
| html5lib                 | 42.4 ms                                                | 36.4 ms: 1.16x faster                                                 |
| 2to3                     | 192 ms                                                 | 165 ms: 1.16x faster                                                  |
| go                       | 151 ms                                                 | 130 ms: 1.16x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 169 us: 1.15x faster                                                  |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.14x faster                                                |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 568 ms: 1.14x faster                                                  |
| fannkuch                 | 303 ms                                                 | 268 ms: 1.13x faster                                                  |
| genshi_text              | 17.3 ms                                                | 15.4 ms: 1.13x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.52 sec: 1.12x faster                                                |
| xml_etree_parse          | 108 ms                                                 | 96.5 ms: 1.12x faster                                                 |
| tornado_http             | 86.7 ms                                                | 77.9 ms: 1.11x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 33.0 ms: 1.11x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.08 ms: 1.11x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.6 ms: 1.11x faster                                                 |
| sqlglot_normalize        | 190 ms                                                 | 171 ms: 1.11x faster                                                  |
| xml_etree_generate       | 53.5 ms                                                | 48.3 ms: 1.11x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 30.6 ms: 1.11x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.9 ms: 1.10x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 84.5 ms: 1.09x faster                                                 |
| generators               | 32.3 ms                                                | 29.7 ms: 1.09x faster                                                 |
| telco                    | 3.49 ms                                                | 3.21 ms: 1.09x faster                                                 |
| nqueens                  | 63.8 ms                                                | 59.1 ms: 1.08x faster                                                 |
| json                     | 3.08 ms                                                | 2.88 ms: 1.07x faster                                                 |
| json_loads               | 16.4 us                                                | 15.4 us: 1.07x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.37 us: 1.07x faster                                                 |
| json_dumps               | 8.11 ms                                                | 7.61 ms: 1.07x faster                                                 |
| sympy_str                | 165 ms                                                 | 156 ms: 1.06x faster                                                  |
| sympy_expand             | 269 ms                                                 | 254 ms: 1.06x faster                                                  |
| meteor_contest           | 77.7 ms                                                | 73.7 ms: 1.06x faster                                                 |
| gunicorn                 | 1.30 ms                                                | 1.25 ms: 1.04x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.64 us: 1.04x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.8 ms: 1.03x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.57 us: 1.03x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 70.5 ms: 1.02x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 516 us: 1.02x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 16.8 ms: 1.02x faster                                                 |
| pickle_dict              | 17.0 us                                                | 16.8 us: 1.01x faster                                                 |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| regex_dna                | 174 ms                                                 | 174 ms: 1.00x faster                                                  |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.01x slower                                                 |
| typing_runtime_protocols | 323 us                                                 | 328 us: 1.02x slower                                                  |
| unpickle_list            | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| sqlglot_parse            | 1.24 ms                                                | 1.28 ms: 1.03x slower                                                 |
| pickle                   | 6.97 us                                                | 7.26 us: 1.04x slower                                                 |
| comprehensions           | 16.9 us                                                | 17.7 us: 1.05x slower                                                 |
| flaskblogging            | 2.65 ms                                                | 2.84 ms: 1.07x slower                                                 |
| bench_mp_pool            | 37.4 ms                                                | 40.6 ms: 1.08x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.81 sec: 1.11x slower                                                |
| python_startup_no_site   | 7.91 ms                                                | 8.93 ms: 1.13x slower                                                 |
| dask                     | 253 ms                                                 | 298 ms: 1.18x slower                                                  |
| python_startup           | 10.9 ms                                                | 15.3 ms: 1.40x slower                                                 |
| coverage                 | 41.5 ms                                                | 330 ms: 7.96x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.10x faster                                                          |

Benchmark hidden because not significant (2): regex_effbot, sqlglot_transpile
Ignored benchmarks (8) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 1.08x