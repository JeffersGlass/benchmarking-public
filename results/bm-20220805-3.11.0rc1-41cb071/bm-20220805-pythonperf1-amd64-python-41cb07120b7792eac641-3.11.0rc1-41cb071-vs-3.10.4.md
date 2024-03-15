
# Results vs. 3.10.4

- fork: python
- ref: 41cb07120b7792eac641
- machine: windows-amd64
- commit hash: 41cb071
- commit date: 2022-08-05
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 202 ms: 1.21x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.05 ms: 1.15x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| html5lib       | 51.0 ms                                                     | 38.4 ms: 1.33x faster                                                       |
| tornado_http   | 108 ms                                                      | 90.9 ms: 1.19x faster                                                       |
| Geometric mean | (ref)                                                       | 1.22x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 739 ms: 1.50x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 368 ms: 1.43x faster                                                        |
| async_tree_none         | 435 ms                                                      | 310 ms: 1.41x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 491 ms: 1.30x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.41x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 52.9 ms: 1.17x faster                                                       |
| nbody          | 71.3 ms                                                     | 68.3 ms: 1.04x faster                                                       |
| pidigits       | 149 ms                                                      | 146 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.08x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 89.4 ms: 1.19x faster                                                       |
| regex_dna      | 136 ms                                                      | 123 ms: 1.11x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 14.1 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                       | 1.09x faster                                                                |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 202 us: 1.33x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 150 us: 1.22x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                                       |
| json_dumps           | 9.16 ms                                                     | 7.73 ms: 1.18x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.11 us: 1.12x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.57 us: 1.07x faster                                                       |
| pickle               | 6.85 us                                                     | 6.44 us: 1.06x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.9 ms: 1.03x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.64 us: 1.03x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 94.8 ms: 1.02x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.09x faster                                                                |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| Geometric mean         | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.26 ms: 1.24x faster                                                       |
| django_template | 28.9 ms                                                     | 23.7 ms: 1.22x faster                                                       |
| genshi_text     | 19.8 ms                                                     | 16.7 ms: 1.18x faster                                                       |
| genshi_xml      | 41.0 ms                                                     | 37.7 ms: 1.09x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.18x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.63 ms: 1.59x faster                                                       |
| async_tree_io           | 1.11 sec                                                    | 739 ms: 1.50x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 368 ms: 1.43x faster                                                        |
| async_tree_none         | 435 ms                                                      | 310 ms: 1.41x faster                                                        |
| go                      | 139 ms                                                      | 101 ms: 1.38x faster                                                        |
| scimark_sor             | 106 ms                                                      | 77.3 ms: 1.37x faster                                                       |
| richards                | 42.4 ms                                                     | 31.3 ms: 1.36x faster                                                       |
| pyflate                 | 409 ms                                                      | 303 ms: 1.35x faster                                                        |
| pycparser               | 930 ms                                                      | 689 ms: 1.35x faster                                                        |
| scimark_lu              | 85.8 ms                                                     | 63.7 ms: 1.35x faster                                                       |
| raytrace                | 273 ms                                                      | 204 ms: 1.34x faster                                                        |
| pickle_pure_python      | 270 us                                                      | 202 us: 1.33x faster                                                        |
| html5lib                | 51.0 ms                                                     | 38.4 ms: 1.33x faster                                                       |
| logging_silent          | 94.6 ns                                                     | 71.9 ns: 1.32x faster                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 925 us: 1.31x faster                                                        |
| sqlglot_transpile       | 1.48 ms                                                     | 1.13 ms: 1.30x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 491 ms: 1.30x faster                                                        |
| scimark_monte_carlo     | 57.3 ms                                                     | 44.4 ms: 1.29x faster                                                       |
| hexiom                  | 5.74 ms                                                     | 4.46 ms: 1.29x faster                                                       |
| crypto_pyaes            | 62.5 ms                                                     | 48.7 ms: 1.28x faster                                                       |
| thrift                  | 617 us                                                      | 482 us: 1.28x faster                                                        |
| async_generators        | 222 ms                                                      | 176 ms: 1.26x faster                                                        |
| mako                    | 9.03 ms                                                     | 7.26 ms: 1.24x faster                                                       |
| chaos                   | 61.7 ms                                                     | 49.6 ms: 1.24x faster                                                       |
| sqlalchemy_declarative  | 103 ms                                                      | 83.4 ms: 1.24x faster                                                       |
| unpickle_pure_python    | 183 us                                                      | 150 us: 1.22x faster                                                        |
| django_template         | 28.9 ms                                                     | 23.7 ms: 1.22x faster                                                       |
| 2to3                    | 246 ms                                                      | 202 ms: 1.21x faster                                                        |
| xml_etree_process       | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                                       |
| docutils                | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 665 us: 1.20x faster                                                        |
| tornado_http            | 108 ms                                                      | 90.9 ms: 1.19x faster                                                       |
| regex_compile           | 106 ms                                                      | 89.4 ms: 1.19x faster                                                       |
| json_dumps              | 9.16 ms                                                     | 7.73 ms: 1.18x faster                                                       |
| genshi_text             | 19.8 ms                                                     | 16.7 ms: 1.18x faster                                                       |
| dask                    | 313 ms                                                      | 267 ms: 1.17x faster                                                        |
| pprint_pformat          | 1.22 sec                                                    | 1.04 sec: 1.17x faster                                                      |
| float                   | 61.7 ms                                                     | 52.9 ms: 1.17x faster                                                       |
| dulwich_log             | 50.5 ms                                                     | 43.3 ms: 1.17x faster                                                       |
| aiohttp                 | 995 us                                                      | 861 us: 1.16x faster                                                        |
| sqlglot_optimize        | 39.8 ms                                                     | 34.5 ms: 1.15x faster                                                       |
| pprint_safe_repr        | 592 ms                                                      | 513 ms: 1.15x faster                                                        |
| chameleon               | 5.79 ms                                                     | 5.05 ms: 1.15x faster                                                       |
| sqlite_synth            | 1.91 us                                                     | 1.68 us: 1.14x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 25.3 us: 1.14x faster                                                       |
| sympy_integrate         | 15.3 ms                                                     | 13.5 ms: 1.13x faster                                                       |
| python_startup          | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                       |
| unpickle                | 9.09 us                                                     | 8.11 us: 1.12x faster                                                       |
| bench_thread_pool       | 958 us                                                      | 856 us: 1.12x faster                                                        |
| mdp                     | 1.78 sec                                                    | 1.60 sec: 1.11x faster                                                      |
| asyncio_tcp             | 732 ms                                                      | 659 ms: 1.11x faster                                                        |
| regex_dna               | 136 ms                                                      | 123 ms: 1.11x faster                                                        |
| pylint                  | 350 ms                                                      | 318 ms: 1.10x faster                                                        |
| sympy_sum               | 107 ms                                                      | 97.0 ms: 1.10x faster                                                       |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.4 ms: 1.10x faster                                                       |
| regex_v8                | 15.4 ms                                                     | 14.1 ms: 1.09x faster                                                       |
| genshi_xml              | 41.0 ms                                                     | 37.7 ms: 1.09x faster                                                       |
| comprehensions          | 16.5 us                                                     | 15.2 us: 1.09x faster                                                       |
| sqlglot_normalize       | 205 ms                                                      | 189 ms: 1.09x faster                                                        |
| sympy_expand            | 314 ms                                                      | 290 ms: 1.08x faster                                                        |
| coroutines              | 16.0 ms                                                     | 14.8 ms: 1.08x faster                                                       |
| sympy_str               | 194 ms                                                      | 180 ms: 1.08x faster                                                        |
| deepcopy_reduce         | 2.20 us                                                     | 2.05 us: 1.08x faster                                                       |
| spectral_norm           | 77.3 ms                                                     | 71.8 ms: 1.08x faster                                                       |
| deepcopy                | 255 us                                                      | 238 us: 1.07x faster                                                        |
| pickle_list             | 2.75 us                                                     | 2.57 us: 1.07x faster                                                       |
| json                    | 3.14 ms                                                     | 2.94 ms: 1.07x faster                                                       |
| pickle                  | 6.85 us                                                     | 6.44 us: 1.06x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.61 ms: 1.04x faster                                                       |
| nbody                   | 71.3 ms                                                     | 68.3 ms: 1.04x faster                                                       |
| pathlib                 | 75.7 ms                                                     | 72.6 ms: 1.04x faster                                                       |
| nqueens                 | 66.6 ms                                                     | 64.2 ms: 1.04x faster                                                       |
| meteor_contest          | 75.9 ms                                                     | 73.3 ms: 1.04x faster                                                       |
| fannkuch                | 256 ms                                                      | 247 ms: 1.03x faster                                                        |
| xml_etree_iterparse     | 65.0 ms                                                     | 62.9 ms: 1.03x faster                                                       |
| unpickle_list           | 2.71 us                                                     | 2.64 us: 1.03x faster                                                       |
| scimark_fft             | 187 ms                                                      | 182 ms: 1.03x faster                                                        |
| pidigits                | 149 ms                                                      | 146 ms: 1.02x faster                                                        |
| xml_etree_parse         | 96.8 ms                                                     | 94.8 ms: 1.02x faster                                                       |
| telco                   | 3.94 ms                                                     | 3.87 ms: 1.02x faster                                                       |
| python_startup_no_site  | 15.5 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| bench_mp_pool           | 62.0 ms                                                     | 61.4 ms: 1.01x faster                                                       |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                      |
| logging_format          | 6.76 us                                                     | 6.90 us: 1.02x slower                                                       |
| logging_simple          | 6.22 us                                                     | 6.37 us: 1.02x slower                                                       |
| generators              | 32.4 ms                                                     | 33.8 ms: 1.04x slower                                                       |
| unpack_sequence         | 39.6 ns                                                     | 41.9 ns: 1.06x slower                                                       |
| pickle_dict             | 17.2 us                                                     | 18.4 us: 1.07x slower                                                       |
| coverage                | 39.0 ms                                                     | 53.6 ms: 1.38x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.14x faster                                                                |

Benchmark hidden because not significant (3): gc_traversal, json_loads, regex_effbot
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown