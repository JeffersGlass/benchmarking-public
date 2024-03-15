
# Results vs. 3.11.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: windows-amd64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 193 ms: 1.11x faster                                                       |
| chameleon      | 5.26 ms                                                     | 4.59 ms: 1.15x faster                                                      |
| docutils       | 1.64 sec                                                    | 1.52 sec: 1.08x faster                                                     |
| html5lib       | 38.9 ms                                                     | 36.4 ms: 1.07x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 89.5 ms: 1.04x faster                                                      |
| Geometric mean | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 530 ms                                                      | 507 ms: 1.05x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 386 ms: 1.03x faster                                                       |
| async_tree_io           | 808 ms                                                      | 783 ms: 1.03x faster                                                       |
| async_tree_none         | 332 ms                                                      | 325 ms: 1.02x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.03x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 62.3 ms: 1.13x faster                                                      |
| float          | 54.4 ms                                                     | 48.7 ms: 1.12x faster                                                      |
| pidigits       | 150 ms                                                      | 146 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 82.3 ms: 1.11x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                                      |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.70 ms: 1.13x slower                                                      |
| Geometric mean | (ref)                                                       | 1.01x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.12 ms: 1.58x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 130 us: 1.20x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 180 us: 1.16x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 87.6 ms: 1.11x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 33.9 ms: 1.10x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 49.0 ms: 1.07x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 61.3 ms: 1.07x faster                                                      |
| pickle_list          | 2.70 us                                                     | 2.62 us: 1.03x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.3 us: 1.01x faster                                                      |
| pickle               | 6.64 us                                                     | 6.57 us: 1.01x faster                                                      |
| json_loads           | 13.0 us                                                     | 13.3 us: 1.02x slower                                                      |
| unpickle_list        | 2.59 us                                                     | 2.79 us: 1.08x slower                                                      |
| unpickle             | 7.57 us                                                     | 8.25 us: 1.09x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.08x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 14.4 ms: 1.28x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 32.2 ms: 1.24x faster                                                      |
| mako            | 7.58 ms                                                     | 6.25 ms: 1.21x faster                                                      |
| django_template | 24.4 ms                                                     | 21.6 ms: 1.13x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.21x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps              | 8.09 ms                                                     | 5.12 ms: 1.58x faster                                                      |
| unpack_sequence         | 46.9 ns                                                     | 30.8 ns: 1.52x faster                                                      |
| genshi_text             | 18.4 ms                                                     | 14.4 ms: 1.28x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 32.2 ms: 1.24x faster                                                      |
| mako                    | 7.58 ms                                                     | 6.25 ms: 1.21x faster                                                      |
| deltablue               | 2.70 ms                                                     | 2.24 ms: 1.20x faster                                                      |
| go                      | 101 ms                                                      | 84.0 ms: 1.20x faster                                                      |
| unpickle_pure_python    | 157 us                                                      | 130 us: 1.20x faster                                                       |
| logging_silent          | 71.8 ns                                                     | 59.9 ns: 1.20x faster                                                      |
| nqueens                 | 68.3 ms                                                     | 57.5 ms: 1.19x faster                                                      |
| richards                | 31.4 ms                                                     | 26.7 ms: 1.17x faster                                                      |
| deepcopy_memo           | 26.0 us                                                     | 22.2 us: 1.17x faster                                                      |
| pprint_pformat          | 1.09 sec                                                    | 934 ms: 1.16x faster                                                       |
| raytrace                | 213 ms                                                      | 184 ms: 1.16x faster                                                       |
| pickle_pure_python      | 208 us                                                      | 180 us: 1.16x faster                                                       |
| pprint_safe_repr        | 529 ms                                                      | 458 ms: 1.16x faster                                                       |
| pyflate                 | 312 ms                                                      | 272 ms: 1.15x faster                                                       |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.25 ms: 1.15x faster                                                      |
| chameleon               | 5.26 ms                                                     | 4.59 ms: 1.15x faster                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 39.8 ms: 1.14x faster                                                      |
| hexiom                  | 4.55 ms                                                     | 4.00 ms: 1.14x faster                                                      |
| deepcopy                | 246 us                                                      | 217 us: 1.14x faster                                                       |
| django_template         | 24.4 ms                                                     | 21.6 ms: 1.13x faster                                                      |
| nbody                   | 70.3 ms                                                     | 62.3 ms: 1.13x faster                                                      |
| scimark_sor             | 78.1 ms                                                     | 69.2 ms: 1.13x faster                                                      |
| chaos                   | 48.4 ms                                                     | 43.1 ms: 1.12x faster                                                      |
| float                   | 54.4 ms                                                     | 48.7 ms: 1.12x faster                                                      |
| fannkuch                | 253 ms                                                      | 227 ms: 1.12x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 87.6 ms: 1.11x faster                                                      |
| pycparser               | 720 ms                                                      | 650 ms: 1.11x faster                                                       |
| 2to3                    | 214 ms                                                      | 193 ms: 1.11x faster                                                       |
| regex_compile           | 91.0 ms                                                     | 82.3 ms: 1.11x faster                                                      |
| scimark_lu              | 62.8 ms                                                     | 56.9 ms: 1.10x faster                                                      |
| sqlglot_parse           | 953 us                                                      | 865 us: 1.10x faster                                                       |
| deepcopy_reduce         | 2.06 us                                                     | 1.87 us: 1.10x faster                                                      |
| xml_etree_process       | 37.2 ms                                                     | 33.9 ms: 1.10x faster                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.06 ms: 1.10x faster                                                      |
| python_startup_no_site  | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                      |
| logging_format          | 7.16 us                                                     | 6.56 us: 1.09x faster                                                      |
| sqlglot_normalize       | 190 ms                                                      | 174 ms: 1.09x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 12.9 ms: 1.09x faster                                                      |
| logging_simple          | 6.86 us                                                     | 6.31 us: 1.09x faster                                                      |
| meteor_contest          | 75.2 ms                                                     | 69.3 ms: 1.09x faster                                                      |
| python_startup          | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| spectral_norm           | 68.3 ms                                                     | 63.1 ms: 1.08x faster                                                      |
| docutils                | 1.64 sec                                                    | 1.52 sec: 1.08x faster                                                     |
| json                    | 2.98 ms                                                     | 2.75 ms: 1.08x faster                                                      |
| crypto_pyaes            | 48.9 ms                                                     | 45.4 ms: 1.08x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 43.1 ms: 1.08x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 32.1 ms: 1.07x faster                                                      |
| xml_etree_generate      | 52.5 ms                                                     | 49.0 ms: 1.07x faster                                                      |
| create_gc_cycles        | 713 us                                                      | 665 us: 1.07x faster                                                       |
| xml_etree_iterparse     | 65.6 ms                                                     | 61.3 ms: 1.07x faster                                                      |
| html5lib                | 38.9 ms                                                     | 36.4 ms: 1.07x faster                                                      |
| sympy_expand            | 299 ms                                                      | 282 ms: 1.06x faster                                                       |
| dask                    | 273 ms                                                      | 258 ms: 1.06x faster                                                       |
| sympy_str               | 185 ms                                                      | 175 ms: 1.06x faster                                                       |
| scimark_fft             | 179 ms                                                      | 170 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 507 ms: 1.05x faster                                                       |
| bench_thread_pool       | 872 us                                                      | 835 us: 1.04x faster                                                       |
| mdp                     | 1.59 sec                                                    | 1.53 sec: 1.04x faster                                                     |
| sympy_sum               | 100 ms                                                      | 96.1 ms: 1.04x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.44 ms: 1.04x faster                                                      |
| tornado_http            | 92.8 ms                                                     | 89.5 ms: 1.04x faster                                                      |
| async_tree_memoization  | 399 ms                                                      | 386 ms: 1.03x faster                                                       |
| bench_mp_pool           | 63.2 ms                                                     | 61.2 ms: 1.03x faster                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.71 us: 1.03x faster                                                      |
| async_tree_io           | 808 ms                                                      | 783 ms: 1.03x faster                                                       |
| pickle_list             | 2.70 us                                                     | 2.62 us: 1.03x faster                                                      |
| telco                   | 4.06 ms                                                     | 3.95 ms: 1.03x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                                      |
| pidigits                | 150 ms                                                      | 146 ms: 1.03x faster                                                       |
| async_generators        | 177 ms                                                      | 173 ms: 1.02x faster                                                       |
| async_tree_none         | 332 ms                                                      | 325 ms: 1.02x faster                                                       |
| comprehensions          | 15.6 us                                                     | 15.4 us: 1.02x faster                                                      |
| pickle_dict             | 18.5 us                                                     | 18.3 us: 1.01x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.57 us: 1.01x faster                                                      |
| json_loads              | 13.0 us                                                     | 13.3 us: 1.02x slower                                                      |
| pathlib                 | 70.9 ms                                                     | 72.6 ms: 1.02x slower                                                      |
| regex_dna               | 116 ms                                                      | 120 ms: 1.03x slower                                                       |
| generators              | 34.0 ms                                                     | 35.7 ms: 1.05x slower                                                      |
| unpickle_list           | 2.59 us                                                     | 2.79 us: 1.08x slower                                                      |
| unpickle                | 7.57 us                                                     | 8.25 us: 1.09x slower                                                      |
| thrift                  | 494 us                                                      | 558 us: 1.13x slower                                                       |
| regex_effbot            | 1.50 ms                                                     | 1.70 ms: 1.13x slower                                                      |
| coverage                | 43.4 ms                                                     | 52.0 ms: 1.20x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.08x faster                                                               |

Benchmark hidden because not significant (2): asyncio_tcp, coroutines
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown