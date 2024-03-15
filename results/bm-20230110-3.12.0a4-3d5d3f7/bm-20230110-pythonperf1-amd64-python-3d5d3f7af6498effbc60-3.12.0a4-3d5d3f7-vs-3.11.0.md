
# Results vs. 3.11.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: windows-amd64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 193 ms: 1.11x faster                                                       |
| chameleon      | 5.26 ms                                                     | 4.39 ms: 1.20x faster                                                      |
| docutils       | 1.64 sec                                                    | 1.48 sec: 1.11x faster                                                     |
| html5lib       | 38.9 ms                                                     | 33.7 ms: 1.15x faster                                                      |
| Geometric mean | (ref)                                                       | 1.14x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 342 ms: 1.17x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 465 ms: 1.14x faster                                                       |
| async_tree_none         | 332 ms                                                      | 295 ms: 1.13x faster                                                       |
| async_tree_io           | 808 ms                                                      | 742 ms: 1.09x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.13x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.5 ms: 1.18x faster                                                      |
| float          | 54.4 ms                                                     | 47.2 ms: 1.15x faster                                                      |
| pidigits       | 150 ms                                                      | 145 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 78.8 ms: 1.15x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 13.6 ms: 1.04x faster                                                      |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.10 ms: 1.59x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 119 us: 1.32x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 169 us: 1.23x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 86.5 ms: 1.13x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 33.8 ms: 1.10x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 60.1 ms: 1.09x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 48.3 ms: 1.09x faster                                                      |
| json_loads           | 13.0 us                                                     | 12.4 us: 1.04x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.2 us: 1.01x faster                                                      |
| pickle               | 6.64 us                                                     | 6.55 us: 1.01x faster                                                      |
| pickle_list          | 2.70 us                                                     | 2.81 us: 1.04x slower                                                      |
| unpickle             | 7.57 us                                                     | 8.70 us: 1.15x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.2 ms: 1.11x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.1 ms: 1.09x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.10x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 13.3 ms: 1.39x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 30.5 ms: 1.31x faster                                                      |
| mako            | 7.58 ms                                                     | 6.05 ms: 1.25x faster                                                      |
| django_template | 24.4 ms                                                     | 20.7 ms: 1.18x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.28x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 26.2 ns: 1.79x faster                                                      |
| json_dumps              | 8.09 ms                                                     | 5.10 ms: 1.59x faster                                                      |
| asyncio_tcp             | 726 ms                                                      | 466 ms: 1.56x faster                                                       |
| genshi_text             | 18.4 ms                                                     | 13.3 ms: 1.39x faster                                                      |
| deltablue               | 2.70 ms                                                     | 1.94 ms: 1.39x faster                                                      |
| logging_silent          | 71.8 ns                                                     | 54.2 ns: 1.33x faster                                                      |
| unpickle_pure_python    | 157 us                                                      | 119 us: 1.32x faster                                                       |
| genshi_xml              | 39.9 ms                                                     | 30.5 ms: 1.31x faster                                                      |
| richards                | 31.4 ms                                                     | 24.0 ms: 1.31x faster                                                      |
| deepcopy_memo           | 26.0 us                                                     | 20.4 us: 1.27x faster                                                      |
| go                      | 101 ms                                                      | 80.4 ms: 1.26x faster                                                      |
| mako                    | 7.58 ms                                                     | 6.05 ms: 1.25x faster                                                      |
| raytrace                | 213 ms                                                      | 171 ms: 1.25x faster                                                       |
| deepcopy                | 246 us                                                      | 199 us: 1.24x faster                                                       |
| pickle_pure_python      | 208 us                                                      | 169 us: 1.23x faster                                                       |
| scimark_sor             | 78.1 ms                                                     | 63.7 ms: 1.23x faster                                                      |
| hexiom                  | 4.55 ms                                                     | 3.77 ms: 1.21x faster                                                      |
| chameleon               | 5.26 ms                                                     | 4.39 ms: 1.20x faster                                                      |
| nqueens                 | 68.3 ms                                                     | 57.3 ms: 1.19x faster                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 38.0 ms: 1.19x faster                                                      |
| pyflate                 | 312 ms                                                      | 263 ms: 1.19x faster                                                       |
| pprint_pformat          | 1.09 sec                                                    | 918 ms: 1.18x faster                                                       |
| nbody                   | 70.3 ms                                                     | 59.5 ms: 1.18x faster                                                      |
| django_template         | 24.4 ms                                                     | 20.7 ms: 1.18x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 448 ms: 1.18x faster                                                       |
| logging_simple          | 6.86 us                                                     | 5.84 us: 1.18x faster                                                      |
| fannkuch                | 253 ms                                                      | 217 ms: 1.17x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 342 ms: 1.17x faster                                                       |
| deepcopy_reduce         | 2.06 us                                                     | 1.78 us: 1.16x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 40.1 ms: 1.16x faster                                                      |
| regex_compile           | 91.0 ms                                                     | 78.8 ms: 1.15x faster                                                      |
| float                   | 54.4 ms                                                     | 47.2 ms: 1.15x faster                                                      |
| html5lib                | 38.9 ms                                                     | 33.7 ms: 1.15x faster                                                      |
| chaos                   | 48.4 ms                                                     | 42.1 ms: 1.15x faster                                                      |
| pycparser               | 720 ms                                                      | 628 ms: 1.15x faster                                                       |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.25 ms: 1.15x faster                                                      |
| json                    | 2.98 ms                                                     | 2.61 ms: 1.14x faster                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 465 ms: 1.14x faster                                                       |
| logging_format          | 7.16 us                                                     | 6.29 us: 1.14x faster                                                      |
| telco                   | 4.06 ms                                                     | 3.59 ms: 1.13x faster                                                      |
| sqlglot_normalize       | 190 ms                                                      | 168 ms: 1.13x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 86.5 ms: 1.13x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 30.6 ms: 1.13x faster                                                      |
| async_tree_none         | 332 ms                                                      | 295 ms: 1.13x faster                                                       |
| sqlglot_parse           | 953 us                                                      | 848 us: 1.12x faster                                                       |
| scimark_lu              | 62.8 ms                                                     | 56.0 ms: 1.12x faster                                                      |
| sympy_integrate         | 14.0 ms                                                     | 12.6 ms: 1.12x faster                                                      |
| dask                    | 273 ms                                                      | 246 ms: 1.11x faster                                                       |
| sympy_expand            | 299 ms                                                      | 269 ms: 1.11x faster                                                       |
| docutils                | 1.64 sec                                                    | 1.48 sec: 1.11x faster                                                     |
| meteor_contest          | 75.2 ms                                                     | 67.9 ms: 1.11x faster                                                      |
| 2to3                    | 214 ms                                                      | 193 ms: 1.11x faster                                                       |
| python_startup_no_site  | 16.8 ms                                                     | 15.2 ms: 1.11x faster                                                      |
| sympy_str               | 185 ms                                                      | 168 ms: 1.10x faster                                                       |
| xml_etree_process       | 37.2 ms                                                     | 33.8 ms: 1.10x faster                                                      |
| bench_thread_pool       | 872 us                                                      | 798 us: 1.09x faster                                                       |
| python_startup          | 19.8 ms                                                     | 18.1 ms: 1.09x faster                                                      |
| xml_etree_iterparse     | 65.6 ms                                                     | 60.1 ms: 1.09x faster                                                      |
| spectral_norm           | 68.3 ms                                                     | 62.8 ms: 1.09x faster                                                      |
| async_tree_io           | 808 ms                                                      | 742 ms: 1.09x faster                                                       |
| sympy_sum               | 100 ms                                                      | 92.0 ms: 1.09x faster                                                      |
| xml_etree_generate      | 52.5 ms                                                     | 48.3 ms: 1.09x faster                                                      |
| create_gc_cycles        | 713 us                                                      | 661 us: 1.08x faster                                                       |
| coroutines              | 15.0 ms                                                     | 13.9 ms: 1.08x faster                                                      |
| scimark_fft             | 179 ms                                                      | 167 ms: 1.08x faster                                                       |
| thrift                  | 494 us                                                      | 463 us: 1.07x faster                                                       |
| crypto_pyaes            | 48.9 ms                                                     | 45.9 ms: 1.07x faster                                                      |
| mdp                     | 1.59 sec                                                    | 1.51 sec: 1.05x faster                                                     |
| async_generators        | 177 ms                                                      | 169 ms: 1.05x faster                                                       |
| json_loads              | 13.0 us                                                     | 12.4 us: 1.04x faster                                                      |
| comprehensions          | 15.6 us                                                     | 15.0 us: 1.04x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.43 ms: 1.04x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.6 ms: 1.04x faster                                                      |
| bench_mp_pool           | 63.2 ms                                                     | 61.1 ms: 1.03x faster                                                      |
| pidigits                | 150 ms                                                      | 145 ms: 1.03x faster                                                       |
| sqlite_synth            | 1.77 us                                                     | 1.72 us: 1.03x faster                                                      |
| generators              | 34.0 ms                                                     | 33.1 ms: 1.03x faster                                                      |
| pickle_dict             | 18.5 us                                                     | 18.2 us: 1.01x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.55 us: 1.01x faster                                                      |
| pathlib                 | 70.9 ms                                                     | 73.2 ms: 1.03x slower                                                      |
| regex_dna               | 116 ms                                                      | 120 ms: 1.03x slower                                                       |
| pickle_list             | 2.70 us                                                     | 2.81 us: 1.04x slower                                                      |
| regex_effbot            | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                      |
| unpickle                | 7.57 us                                                     | 8.70 us: 1.15x slower                                                      |
| coverage                | 43.4 ms                                                     | 52.5 ms: 1.21x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.14x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (15) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown