
# Results vs. 3.10.4

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: windows-amd64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.15x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 202 ms: 1.22x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.09 ms: 1.14x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                      |
| html5lib       | 51.0 ms                                                     | 37.2 ms: 1.37x faster                                                       |
| tornado_http   | 108 ms                                                      | 92.1 ms: 1.18x faster                                                       |
| Geometric mean | (ref)                                                       | 1.22x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 740 ms: 1.50x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 368 ms: 1.43x faster                                                        |
| async_tree_none         | 435 ms                                                      | 310 ms: 1.40x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 488 ms: 1.31x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.41x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.9 ms: 1.14x faster                                                       |
| nbody          | 71.3 ms                                                     | 68.6 ms: 1.04x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 115 ms: 1.19x faster                                                        |
| regex_compile  | 106 ms                                                      | 89.5 ms: 1.19x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 13.4 ms: 1.15x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 197 us: 1.37x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 35.9 ms: 1.24x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 149 us: 1.23x faster                                                        |
| json_dumps           | 9.16 ms                                                     | 7.66 ms: 1.20x faster                                                       |
| unpickle             | 9.09 us                                                     | 7.70 us: 1.18x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 51.2 ms: 1.08x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.55 us: 1.06x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 91.6 ms: 1.06x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 61.9 ms: 1.05x faster                                                       |
| pickle               | 6.85 us                                                     | 6.60 us: 1.04x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.65 us: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.03x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 18.2 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.5 ms: 1.11x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 15.3 ms: 1.01x faster                                                       |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.22 ms: 1.25x faster                                                       |
| django_template | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                                       |
| genshi_text     | 19.8 ms                                                     | 16.7 ms: 1.19x faster                                                       |
| genshi_xml      | 41.0 ms                                                     | 38.3 ms: 1.07x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.18x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.61 ms: 1.60x faster                                                       |
| async_tree_io           | 1.11 sec                                                    | 740 ms: 1.50x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 368 ms: 1.43x faster                                                        |
| go                      | 139 ms                                                      | 97.5 ms: 1.43x faster                                                       |
| async_tree_none         | 435 ms                                                      | 310 ms: 1.40x faster                                                        |
| richards                | 42.4 ms                                                     | 30.6 ms: 1.39x faster                                                       |
| scimark_sor             | 106 ms                                                      | 77.3 ms: 1.37x faster                                                       |
| html5lib                | 51.0 ms                                                     | 37.2 ms: 1.37x faster                                                       |
| pickle_pure_python      | 270 us                                                      | 197 us: 1.37x faster                                                        |
| pycparser               | 930 ms                                                      | 683 ms: 1.36x faster                                                        |
| scimark_lu              | 85.8 ms                                                     | 63.4 ms: 1.35x faster                                                       |
| pyflate                 | 409 ms                                                      | 303 ms: 1.35x faster                                                        |
| logging_silent          | 94.6 ns                                                     | 70.9 ns: 1.33x faster                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 920 us: 1.32x faster                                                        |
| sqlglot_transpile       | 1.48 ms                                                     | 1.12 ms: 1.32x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 488 ms: 1.31x faster                                                        |
| raytrace                | 273 ms                                                      | 211 ms: 1.30x faster                                                        |
| crypto_pyaes            | 62.5 ms                                                     | 48.5 ms: 1.29x faster                                                       |
| scimark_monte_carlo     | 57.3 ms                                                     | 44.6 ms: 1.29x faster                                                       |
| chaos                   | 61.7 ms                                                     | 48.0 ms: 1.28x faster                                                       |
| hexiom                  | 5.74 ms                                                     | 4.48 ms: 1.28x faster                                                       |
| sqlalchemy_declarative  | 103 ms                                                      | 81.7 ms: 1.27x faster                                                       |
| async_generators        | 222 ms                                                      | 176 ms: 1.26x faster                                                        |
| thrift                  | 617 us                                                      | 491 us: 1.26x faster                                                        |
| mako                    | 9.03 ms                                                     | 7.22 ms: 1.25x faster                                                       |
| xml_etree_process       | 44.5 ms                                                     | 35.9 ms: 1.24x faster                                                       |
| unpickle_pure_python    | 183 us                                                      | 149 us: 1.23x faster                                                        |
| docutils                | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                      |
| 2to3                    | 246 ms                                                      | 202 ms: 1.22x faster                                                        |
| django_template         | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                                       |
| create_gc_cycles        | 800 us                                                      | 667 us: 1.20x faster                                                        |
| json_dumps              | 9.16 ms                                                     | 7.66 ms: 1.20x faster                                                       |
| genshi_text             | 19.8 ms                                                     | 16.7 ms: 1.19x faster                                                       |
| regex_dna               | 136 ms                                                      | 115 ms: 1.19x faster                                                        |
| regex_compile           | 106 ms                                                      | 89.5 ms: 1.19x faster                                                       |
| unpickle                | 9.09 us                                                     | 7.70 us: 1.18x faster                                                       |
| tornado_http            | 108 ms                                                      | 92.1 ms: 1.18x faster                                                       |
| dask                    | 313 ms                                                      | 267 ms: 1.17x faster                                                        |
| sqlglot_optimize        | 39.8 ms                                                     | 34.0 ms: 1.17x faster                                                       |
| aiohttp                 | 995 us                                                      | 857 us: 1.16x faster                                                        |
| pprint_pformat          | 1.22 sec                                                    | 1.05 sec: 1.16x faster                                                      |
| dulwich_log             | 50.5 ms                                                     | 43.6 ms: 1.16x faster                                                       |
| pprint_safe_repr        | 592 ms                                                      | 512 ms: 1.16x faster                                                        |
| regex_v8                | 15.4 ms                                                     | 13.4 ms: 1.15x faster                                                       |
| float                   | 61.7 ms                                                     | 53.9 ms: 1.14x faster                                                       |
| sqlite_synth            | 1.91 us                                                     | 1.67 us: 1.14x faster                                                       |
| chameleon               | 5.79 ms                                                     | 5.09 ms: 1.14x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 25.4 us: 1.13x faster                                                       |
| sympy_integrate         | 15.3 ms                                                     | 13.5 ms: 1.13x faster                                                       |
| bench_thread_pool       | 958 us                                                      | 849 us: 1.13x faster                                                        |
| mdp                     | 1.78 sec                                                    | 1.59 sec: 1.12x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.5 ms: 1.11x faster                                                       |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.3 ms: 1.11x faster                                                       |
| pylint                  | 350 ms                                                      | 316 ms: 1.11x faster                                                        |
| sqlglot_normalize       | 205 ms                                                      | 186 ms: 1.10x faster                                                        |
| deepcopy_reduce         | 2.20 us                                                     | 2.00 us: 1.10x faster                                                       |
| sympy_sum               | 107 ms                                                      | 98.2 ms: 1.09x faster                                                       |
| comprehensions          | 16.5 us                                                     | 15.2 us: 1.09x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 51.2 ms: 1.08x faster                                                       |
| coroutines              | 16.0 ms                                                     | 14.9 ms: 1.08x faster                                                       |
| genshi_xml              | 41.0 ms                                                     | 38.3 ms: 1.07x faster                                                       |
| deepcopy                | 255 us                                                      | 239 us: 1.07x faster                                                        |
| sympy_expand            | 314 ms                                                      | 294 ms: 1.07x faster                                                        |
| sympy_str               | 194 ms                                                      | 182 ms: 1.07x faster                                                        |
| unpickle_list           | 2.71 us                                                     | 2.55 us: 1.06x faster                                                       |
| asyncio_tcp             | 732 ms                                                      | 688 ms: 1.06x faster                                                        |
| xml_etree_parse         | 96.8 ms                                                     | 91.6 ms: 1.06x faster                                                       |
| spectral_norm           | 77.3 ms                                                     | 73.2 ms: 1.06x faster                                                       |
| xml_etree_iterparse     | 65.0 ms                                                     | 61.9 ms: 1.05x faster                                                       |
| pathlib                 | 75.7 ms                                                     | 72.1 ms: 1.05x faster                                                       |
| nbody                   | 71.3 ms                                                     | 68.6 ms: 1.04x faster                                                       |
| pickle                  | 6.85 us                                                     | 6.60 us: 1.04x faster                                                       |
| regex_effbot            | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                       |
| pickle_list             | 2.75 us                                                     | 2.65 us: 1.04x faster                                                       |
| nqueens                 | 66.6 ms                                                     | 64.6 ms: 1.03x faster                                                       |
| json_loads              | 14.0 us                                                     | 13.7 us: 1.03x faster                                                       |
| meteor_contest          | 75.9 ms                                                     | 74.3 ms: 1.02x faster                                                       |
| pidigits                | 149 ms                                                      | 147 ms: 1.02x faster                                                        |
| bench_mp_pool           | 62.0 ms                                                     | 61.2 ms: 1.01x faster                                                       |
| python_startup_no_site  | 15.5 ms                                                     | 15.3 ms: 1.01x faster                                                       |
| telco                   | 3.94 ms                                                     | 3.91 ms: 1.01x faster                                                       |
| flaskblogging           | 2.03 sec                                                    | 2.04 sec: 1.01x slower                                                      |
| scimark_fft             | 187 ms                                                      | 189 ms: 1.01x slower                                                        |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.81 ms: 1.03x slower                                                       |
| logging_format          | 6.76 us                                                     | 6.97 us: 1.03x slower                                                       |
| generators              | 32.4 ms                                                     | 33.5 ms: 1.04x slower                                                       |
| logging_simple          | 6.22 us                                                     | 6.57 us: 1.06x slower                                                       |
| pickle_dict             | 17.2 us                                                     | 18.2 us: 1.06x slower                                                       |
| unpack_sequence         | 39.6 ns                                                     | 42.7 ns: 1.08x slower                                                       |
| coverage                | 39.0 ms                                                     | 53.2 ms: 1.36x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.15x faster                                                                |

Benchmark hidden because not significant (3): json, gc_traversal, fannkuch
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown