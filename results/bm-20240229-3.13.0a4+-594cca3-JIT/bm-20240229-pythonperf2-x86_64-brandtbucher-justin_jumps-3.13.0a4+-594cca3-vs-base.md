# Results vs. base

- fork: brandtbucher
- ref: justin_jumps
- machine: linux-x86_64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 310 ms                                                                       | 307 ms: 1.01x faster                                                       |
| chameleon      | 7.45 ms                                                                      | 7.48 ms: 1.00x slower                                                      |
| docutils       | 2.96 sec                                                                     | 2.92 sec: 1.01x faster                                                     |
| tornado_http   | 127 ms                                                                       | 124 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|--------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io      | 1.10 sec                                                                     | 1.10 sec: 1.00x faster                                                     |
| async_tree_none_tg | 444 ms                                                                       | 446 ms: 1.00x slower                                                       |
| Geometric mean     | (ref)                                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (6): async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 102 ms                                                                       | 101 ms: 1.01x faster                                                       |
| float          | 78.8 ms                                                                      | 78.4 ms: 1.01x faster                                                      |
| pidigits       | 262 ms                                                                       | 262 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 154 ms                                                                       | 148 ms: 1.04x faster                                                       |
| regex_dna      | 239 ms                                                                       | 237 ms: 1.01x faster                                                       |
| regex_effbot   | 3.50 ms                                                                      | 3.63 ms: 1.04x slower                                                      |
| Geometric mean | (ref)                                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| tomli_loads          | 2.39 sec                                                                     | 2.14 sec: 1.11x faster                                                     |
| pickle_list          | 4.51 us                                                                      | 4.28 us: 1.05x faster                                                      |
| unpickle_pure_python | 243 us                                                                       | 233 us: 1.04x faster                                                       |
| xml_etree_parse      | 151 ms                                                                       | 146 ms: 1.03x faster                                                       |
| xml_etree_generate   | 86.8 ms                                                                      | 84.4 ms: 1.03x faster                                                      |
| xml_etree_iterparse  | 106 ms                                                                       | 103 ms: 1.03x faster                                                       |
| xml_etree_process    | 59.5 ms                                                                      | 58.0 ms: 1.03x faster                                                      |
| json_dumps           | 10.4 ms                                                                      | 10.5 ms: 1.00x slower                                                      |
| pickle_dict          | 30.4 us                                                                      | 30.5 us: 1.01x slower                                                      |
| pickle               | 10.2 us                                                                      | 10.3 us: 1.01x slower                                                      |
| json_loads           | 25.0 us                                                                      | 25.5 us: 1.02x slower                                                      |
| unpickle_list        | 4.60 us                                                                      | 4.72 us: 1.02x slower                                                      |
| unpickle             | 14.6 us                                                                      | 15.5 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 15.7 ms                                                                      | 15.5 ms: 1.01x faster                                                      |
| python_startup_no_site | 14.1 ms                                                                      | 14.1 ms: 1.01x faster                                                      |
| Geometric mean         | (ref)                                                                        | 1.01x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                                      | 10.00 ms: 1.07x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|--------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence          | 81.5 ns                                                                      | 61.5 ns: 1.33x faster                                                      |
| gc_traversal             | 3.89 ms                                                                      | 3.47 ms: 1.12x faster                                                      |
| fannkuch                 | 440 ms                                                                       | 394 ms: 1.12x faster                                                       |
| tomli_loads              | 2.39 sec                                                                     | 2.14 sec: 1.11x faster                                                     |
| scimark_monte_carlo      | 84.3 ms                                                                      | 77.7 ms: 1.08x faster                                                      |
| coverage                 | 84.7 ms                                                                      | 78.8 ms: 1.08x faster                                                      |
| mako                     | 10.7 ms                                                                      | 10.00 ms: 1.07x faster                                                     |
| spectral_norm            | 99.6 ms                                                                      | 92.9 ms: 1.07x faster                                                      |
| scimark_fft              | 341 ms                                                                       | 322 ms: 1.06x faster                                                       |
| pickle_list              | 4.51 us                                                                      | 4.28 us: 1.05x faster                                                      |
| crypto_pyaes             | 80.9 ms                                                                      | 77.0 ms: 1.05x faster                                                      |
| pprint_safe_repr         | 886 ms                                                                       | 843 ms: 1.05x faster                                                       |
| hexiom                   | 7.69 ms                                                                      | 7.34 ms: 1.05x faster                                                      |
| scimark_sparse_mat_mult  | 4.45 ms                                                                      | 4.25 ms: 1.05x faster                                                      |
| nqueens                  | 104 ms                                                                       | 99.1 ms: 1.05x faster                                                      |
| pprint_pformat           | 1.83 sec                                                                     | 1.76 sec: 1.04x faster                                                     |
| regex_compile            | 154 ms                                                                       | 148 ms: 1.04x faster                                                       |
| unpickle_pure_python     | 243 us                                                                       | 233 us: 1.04x faster                                                       |
| deepcopy_reduce          | 3.48 us                                                                      | 3.35 us: 1.04x faster                                                      |
| xml_etree_parse          | 151 ms                                                                       | 146 ms: 1.03x faster                                                       |
| telco                    | 8.32 ms                                                                      | 8.06 ms: 1.03x faster                                                      |
| pyflate                  | 544 ms                                                                       | 529 ms: 1.03x faster                                                       |
| xml_etree_generate       | 86.8 ms                                                                      | 84.4 ms: 1.03x faster                                                      |
| comprehensions           | 19.2 us                                                                      | 18.7 us: 1.03x faster                                                      |
| chaos                    | 69.2 ms                                                                      | 67.2 ms: 1.03x faster                                                      |
| dulwich_log              | 71.1 ms                                                                      | 69.1 ms: 1.03x faster                                                      |
| xml_etree_iterparse      | 106 ms                                                                       | 103 ms: 1.03x faster                                                       |
| sympy_sum                | 163 ms                                                                       | 159 ms: 1.03x faster                                                       |
| xml_etree_process        | 59.5 ms                                                                      | 58.0 ms: 1.03x faster                                                      |
| sympy_integrate          | 25.1 ms                                                                      | 24.5 ms: 1.03x faster                                                      |
| sqlglot_optimize         | 64.3 ms                                                                      | 62.8 ms: 1.02x faster                                                      |
| sqlglot_normalize        | 120 ms                                                                       | 118 ms: 1.02x faster                                                       |
| tornado_http             | 127 ms                                                                       | 124 ms: 1.02x faster                                                       |
| richards                 | 52.2 ms                                                                      | 51.2 ms: 1.02x faster                                                      |
| pathlib                  | 19.5 ms                                                                      | 19.2 ms: 1.02x faster                                                      |
| docutils                 | 2.96 sec                                                                     | 2.92 sec: 1.01x faster                                                     |
| nbody                    | 102 ms                                                                       | 101 ms: 1.01x faster                                                       |
| raytrace                 | 304 ms                                                                       | 300 ms: 1.01x faster                                                       |
| sympy_expand             | 523 ms                                                                       | 517 ms: 1.01x faster                                                       |
| sympy_str                | 306 ms                                                                       | 302 ms: 1.01x faster                                                       |
| sqlglot_transpile        | 1.88 ms                                                                      | 1.86 ms: 1.01x faster                                                      |
| 2to3                     | 310 ms                                                                       | 307 ms: 1.01x faster                                                       |
| sqlglot_parse            | 1.45 ms                                                                      | 1.43 ms: 1.01x faster                                                      |
| json                     | 5.33 ms                                                                      | 5.28 ms: 1.01x faster                                                      |
| logging_silent           | 100 ns                                                                       | 99.0 ns: 1.01x faster                                                      |
| bench_mp_pool            | 6.93 ms                                                                      | 6.86 ms: 1.01x faster                                                      |
| regex_dna                | 239 ms                                                                       | 237 ms: 1.01x faster                                                       |
| python_startup           | 15.7 ms                                                                      | 15.5 ms: 1.01x faster                                                      |
| async_generators         | 388 ms                                                                       | 385 ms: 1.01x faster                                                       |
| scimark_sor              | 156 ms                                                                       | 155 ms: 1.01x faster                                                       |
| deepcopy_memo            | 39.8 us                                                                      | 39.6 us: 1.01x faster                                                      |
| python_startup_no_site   | 14.1 ms                                                                      | 14.1 ms: 1.01x faster                                                      |
| meteor_contest           | 132 ms                                                                       | 131 ms: 1.01x faster                                                       |
| float                    | 78.8 ms                                                                      | 78.4 ms: 1.01x faster                                                      |
| coroutines               | 22.4 ms                                                                      | 22.3 ms: 1.00x faster                                                      |
| asyncio_tcp              | 378 ms                                                                       | 376 ms: 1.00x faster                                                       |
| go                       | 176 ms                                                                       | 176 ms: 1.00x faster                                                       |
| async_tree_io            | 1.10 sec                                                                     | 1.10 sec: 1.00x faster                                                     |
| pidigits                 | 262 ms                                                                       | 262 ms: 1.00x faster                                                       |
| asyncio_tcp_ssl          | 1.59 sec                                                                     | 1.58 sec: 1.00x faster                                                     |
| generators               | 33.4 ms                                                                      | 33.4 ms: 1.00x slower                                                      |
| async_tree_none_tg       | 444 ms                                                                       | 446 ms: 1.00x slower                                                       |
| logging_simple           | 6.58 us                                                                      | 6.60 us: 1.00x slower                                                      |
| chameleon                | 7.45 ms                                                                      | 7.48 ms: 1.00x slower                                                      |
| json_dumps               | 10.4 ms                                                                      | 10.5 ms: 1.00x slower                                                      |
| pickle_dict              | 30.4 us                                                                      | 30.5 us: 1.01x slower                                                      |
| mdp                      | 2.61 sec                                                                     | 2.62 sec: 1.01x slower                                                     |
| pickle                   | 10.2 us                                                                      | 10.3 us: 1.01x slower                                                      |
| deltablue                | 3.80 ms                                                                      | 3.83 ms: 1.01x slower                                                      |
| asyncio_websockets       | 385 ms                                                                       | 389 ms: 1.01x slower                                                       |
| logging_format           | 7.15 us                                                                      | 7.28 us: 1.02x slower                                                      |
| json_loads               | 25.0 us                                                                      | 25.5 us: 1.02x slower                                                      |
| scimark_lu               | 121 ms                                                                       | 124 ms: 1.02x slower                                                       |
| unpickle_list            | 4.60 us                                                                      | 4.72 us: 1.02x slower                                                      |
| typing_runtime_protocols | 120 us                                                                       | 123 us: 1.03x slower                                                       |
| regex_effbot             | 3.50 ms                                                                      | 3.63 ms: 1.04x slower                                                      |
| unpickle                 | 14.6 us                                                                      | 15.5 us: 1.06x slower                                                      |
| Geometric mean           | (ref)                                                                        | 1.02x faster                                                               |

Benchmark hidden because not significant (15): bench_thread_pool, mypy2, async_tree_cpu_io_mixed, richards_super, pickle_pure_python, async_tree_none, sqlite_synth, async_tree_cpu_io_mixed_tg, pycparser, async_tree_io_tg, regex_v8, async_tree_memoization, create_gc_cycles, deepcopy, async_tree_memoization_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x