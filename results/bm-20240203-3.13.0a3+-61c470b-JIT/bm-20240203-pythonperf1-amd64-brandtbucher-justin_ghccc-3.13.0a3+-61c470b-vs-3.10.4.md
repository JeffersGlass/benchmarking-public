
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-amd64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 219 ms: 1.12x faster                                                      |
| chameleon      | 5.79 ms                                                     | 4.81 ms: 1.20x faster                                                     |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                    |
| tornado_http   | 108 ms                                                      | 87.4 ms: 1.24x faster                                                     |
| Geometric mean | (ref)                                                       | 1.19x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 279 ms: 1.56x faster                                                      |
| async_tree_memoization  | 526 ms                                                      | 354 ms: 1.49x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 750 ms: 1.48x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 461 ms: 1.38x faster                                                      |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 71.3 ms                                                     | 55.3 ms: 1.29x faster                                                     |
| float          | 61.7 ms                                                     | 50.6 ms: 1.22x faster                                                     |
| pidigits       | 149 ms                                                      | 153 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                       | 1.15x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 81.6 ms: 1.30x faster                                                     |
| regex_dna      | 136 ms                                                      | 118 ms: 1.15x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                     |
| Geometric mean | (ref)                                                       | 1.10x faster                                                              |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.54 ms: 1.65x faster                                                     |
| pickle_pure_python   | 270 us                                                      | 177 us: 1.52x faster                                                      |
| unpickle_pure_python | 183 us                                                      | 130 us: 1.41x faster                                                      |
| tomli_loads          | 1.67 sec                                                    | 1.30 sec: 1.28x faster                                                    |
| xml_etree_process    | 44.5 ms                                                     | 36.0 ms: 1.24x faster                                                     |
| xml_etree_generate   | 55.5 ms                                                     | 53.1 ms: 1.05x faster                                                     |
| unpickle             | 9.09 us                                                     | 8.73 us: 1.04x faster                                                     |
| xml_etree_parse      | 96.8 ms                                                     | 94.3 ms: 1.03x faster                                                     |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                     |
| pickle_dict          | 17.2 us                                                     | 17.7 us: 1.03x slower                                                     |
| pickle_list          | 2.75 us                                                     | 2.86 us: 1.04x slower                                                     |
| unpickle_list        | 2.71 us                                                     | 2.84 us: 1.05x slower                                                     |
| pickle               | 6.85 us                                                     | 7.41 us: 1.08x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                              |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 21.1 ms: 1.03x slower                                                     |
| python_startup_no_site | 15.5 ms                                                     | 19.0 ms: 1.23x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.12x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.63 ms: 1.36x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.1 us: 4.79x faster                                                     |
| deltablue                | 4.19 ms                                                     | 2.08 ms: 2.01x faster                                                     |
| richards_super           | 52.2 ms                                                     | 28.6 ms: 1.82x faster                                                     |
| logging_silent           | 94.6 ns                                                     | 53.6 ns: 1.76x faster                                                     |
| richards                 | 42.4 ms                                                     | 25.2 ms: 1.68x faster                                                     |
| json_dumps               | 9.16 ms                                                     | 5.54 ms: 1.65x faster                                                     |
| raytrace                 | 273 ms                                                      | 167 ms: 1.64x faster                                                      |
| generators               | 32.4 ms                                                     | 20.0 ms: 1.62x faster                                                     |
| sqlglot_parse            | 1.22 ms                                                     | 768 us: 1.58x faster                                                      |
| async_tree_none          | 435 ms                                                      | 279 ms: 1.56x faster                                                      |
| scimark_lu               | 85.8 ms                                                     | 55.3 ms: 1.55x faster                                                     |
| pickle_pure_python       | 270 us                                                      | 177 us: 1.52x faster                                                      |
| asyncio_tcp              | 732 ms                                                      | 486 ms: 1.51x faster                                                      |
| sqlglot_transpile        | 1.48 ms                                                     | 988 us: 1.49x faster                                                      |
| chaos                    | 61.7 ms                                                     | 41.3 ms: 1.49x faster                                                     |
| async_tree_memoization   | 526 ms                                                      | 354 ms: 1.49x faster                                                      |
| async_tree_io            | 1.11 sec                                                    | 750 ms: 1.48x faster                                                      |
| comprehensions           | 16.5 us                                                     | 11.4 us: 1.44x faster                                                     |
| crypto_pyaes             | 62.5 ms                                                     | 43.6 ms: 1.44x faster                                                     |
| unpickle_pure_python     | 183 us                                                      | 130 us: 1.41x faster                                                      |
| go                       | 139 ms                                                      | 98.6 ms: 1.41x faster                                                     |
| scimark_sor              | 106 ms                                                      | 76.3 ms: 1.39x faster                                                     |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 461 ms: 1.38x faster                                                      |
| mako                     | 9.03 ms                                                     | 6.63 ms: 1.36x faster                                                     |
| pycparser                | 930 ms                                                      | 703 ms: 1.32x faster                                                      |
| pyflate                  | 409 ms                                                      | 310 ms: 1.32x faster                                                      |
| regex_compile            | 106 ms                                                      | 81.6 ms: 1.30x faster                                                     |
| deepcopy_memo            | 28.8 us                                                     | 22.2 us: 1.30x faster                                                     |
| nbody                    | 71.3 ms                                                     | 55.3 ms: 1.29x faster                                                     |
| tomli_loads              | 1.67 sec                                                    | 1.30 sec: 1.28x faster                                                    |
| mypy2                    | 555 ms                                                      | 436 ms: 1.27x faster                                                      |
| tornado_http             | 108 ms                                                      | 87.4 ms: 1.24x faster                                                     |
| coroutines               | 16.0 ms                                                     | 12.9 ms: 1.24x faster                                                     |
| spectral_norm            | 77.3 ms                                                     | 62.5 ms: 1.24x faster                                                     |
| xml_etree_process        | 44.5 ms                                                     | 36.0 ms: 1.24x faster                                                     |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.71 sec: 1.24x faster                                                    |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.23x faster                                                     |
| float                    | 61.7 ms                                                     | 50.6 ms: 1.22x faster                                                     |
| dulwich_log              | 50.5 ms                                                     | 41.8 ms: 1.21x faster                                                     |
| chameleon                | 5.79 ms                                                     | 4.81 ms: 1.20x faster                                                     |
| pprint_safe_repr         | 592 ms                                                      | 493 ms: 1.20x faster                                                      |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                    |
| pprint_pformat           | 1.22 sec                                                    | 1.03 sec: 1.19x faster                                                    |
| dask                     | 313 ms                                                      | 264 ms: 1.19x faster                                                      |
| sympy_sum                | 107 ms                                                      | 91.5 ms: 1.17x faster                                                     |
| deepcopy                 | 255 us                                                      | 220 us: 1.16x faster                                                      |
| regex_dna                | 136 ms                                                      | 118 ms: 1.15x faster                                                      |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                     |
| sqlglot_optimize         | 39.8 ms                                                     | 34.7 ms: 1.15x faster                                                     |
| deepcopy_reduce          | 2.20 us                                                     | 1.93 us: 1.14x faster                                                     |
| sqlglot_normalize        | 205 ms                                                      | 180 ms: 1.14x faster                                                      |
| sympy_str                | 194 ms                                                      | 172 ms: 1.13x faster                                                      |
| 2to3                     | 246 ms                                                      | 219 ms: 1.12x faster                                                      |
| mdp                      | 1.78 sec                                                    | 1.60 sec: 1.11x faster                                                    |
| nqueens                  | 66.6 ms                                                     | 61.0 ms: 1.09x faster                                                     |
| sympy_expand             | 314 ms                                                      | 288 ms: 1.09x faster                                                      |
| bench_thread_pool        | 958 us                                                      | 877 us: 1.09x faster                                                      |
| hexiom                   | 5.74 ms                                                     | 5.29 ms: 1.08x faster                                                     |
| fannkuch                 | 256 ms                                                      | 238 ms: 1.07x faster                                                      |
| create_gc_cycles         | 800 us                                                      | 757 us: 1.06x faster                                                      |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                     |
| logging_format           | 6.76 us                                                     | 6.41 us: 1.05x faster                                                     |
| xml_etree_generate       | 55.5 ms                                                     | 53.1 ms: 1.05x faster                                                     |
| unpickle                 | 9.09 us                                                     | 8.73 us: 1.04x faster                                                     |
| logging_simple           | 6.22 us                                                     | 5.98 us: 1.04x faster                                                     |
| xml_etree_parse          | 96.8 ms                                                     | 94.3 ms: 1.03x faster                                                     |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                     |
| scimark_monte_carlo      | 57.3 ms                                                     | 56.2 ms: 1.02x faster                                                     |
| unpack_sequence          | 39.6 ns                                                     | 40.1 ns: 1.01x slower                                                     |
| python_startup           | 20.6 ms                                                     | 21.1 ms: 1.03x slower                                                     |
| pidigits                 | 149 ms                                                      | 153 ms: 1.03x slower                                                      |
| meteor_contest           | 75.9 ms                                                     | 78.3 ms: 1.03x slower                                                     |
| pickle_dict              | 17.2 us                                                     | 17.7 us: 1.03x slower                                                     |
| pickle_list              | 2.75 us                                                     | 2.86 us: 1.04x slower                                                     |
| unpickle_list            | 2.71 us                                                     | 2.84 us: 1.05x slower                                                     |
| pathlib                  | 75.7 ms                                                     | 80.2 ms: 1.06x slower                                                     |
| pickle                   | 6.85 us                                                     | 7.41 us: 1.08x slower                                                     |
| gc_traversal             | 1.41 ms                                                     | 1.53 ms: 1.08x slower                                                     |
| async_generators         | 222 ms                                                      | 245 ms: 1.11x slower                                                      |
| bench_mp_pool            | 62.0 ms                                                     | 70.8 ms: 1.14x slower                                                     |
| telco                    | 3.94 ms                                                     | 4.50 ms: 1.14x slower                                                     |
| python_startup_no_site   | 15.5 ms                                                     | 19.0 ms: 1.23x slower                                                     |
| coverage                 | 39.0 ms                                                     | 47.8 ms: 1.23x slower                                                     |
| Geometric mean           | (ref)                                                       | 1.21x faster                                                              |

Benchmark hidden because not significant (5): json, scimark_sparse_mat_mult, xml_etree_iterparse, scimark_fft, regex_v8
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240203-3.13.0a3+-61c470b-JIT/bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown