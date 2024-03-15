
# Results vs. 3.10.4

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: windows-amd64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 193 ms: 1.27x faster                                                       |
| chameleon      | 5.79 ms                                                     | 4.59 ms: 1.26x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.52 sec: 1.27x faster                                                     |
| html5lib       | 51.0 ms                                                     | 36.4 ms: 1.40x faster                                                      |
| tornado_http   | 108 ms                                                      | 89.5 ms: 1.21x faster                                                      |
| Geometric mean | (ref)                                                       | 1.28x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 783 ms: 1.42x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 386 ms: 1.36x faster                                                       |
| async_tree_none         | 435 ms                                                      | 325 ms: 1.34x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 507 ms: 1.26x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.34x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 48.7 ms: 1.27x faster                                                      |
| nbody          | 71.3 ms                                                     | 62.3 ms: 1.15x faster                                                      |
| pidigits       | 149 ms                                                      | 146 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 82.3 ms: 1.29x faster                                                      |
| regex_dna      | 136 ms                                                      | 120 ms: 1.14x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 13.8 ms: 1.12x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.70 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                       | 1.12x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.12 ms: 1.79x faster                                                      |
| pickle_pure_python   | 270 us                                                      | 180 us: 1.50x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 130 us: 1.40x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 33.9 ms: 1.31x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 49.0 ms: 1.13x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 87.6 ms: 1.11x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.25 us: 1.10x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| json_loads           | 14.0 us                                                     | 13.3 us: 1.06x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.62 us: 1.05x faster                                                      |
| pickle               | 6.85 us                                                     | 6.57 us: 1.04x faster                                                      |
| unpickle_list        | 2.71 us                                                     | 2.79 us: 1.03x slower                                                      |
| pickle_dict          | 17.2 us                                                     | 18.3 us: 1.07x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.17x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| Geometric mean | (ref)                                                       | 1.07x faster                                                               |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 6.25 ms: 1.45x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 14.4 ms: 1.37x faster                                                      |
| django_template | 28.9 ms                                                     | 21.6 ms: 1.34x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 32.2 ms: 1.27x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.36x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.24 ms: 1.87x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 5.12 ms: 1.79x faster                                                      |
| go                      | 139 ms                                                      | 84.0 ms: 1.65x faster                                                      |
| richards                | 42.4 ms                                                     | 26.7 ms: 1.59x faster                                                      |
| logging_silent          | 94.6 ns                                                     | 59.9 ns: 1.58x faster                                                      |
| scimark_sor             | 106 ms                                                      | 69.2 ms: 1.53x faster                                                      |
| scimark_lu              | 85.8 ms                                                     | 56.9 ms: 1.51x faster                                                      |
| pyflate                 | 409 ms                                                      | 272 ms: 1.50x faster                                                       |
| pickle_pure_python      | 270 us                                                      | 180 us: 1.50x faster                                                       |
| raytrace                | 273 ms                                                      | 184 ms: 1.48x faster                                                       |
| mako                    | 9.03 ms                                                     | 6.25 ms: 1.45x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 39.8 ms: 1.44x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 4.00 ms: 1.44x faster                                                      |
| pycparser               | 930 ms                                                      | 650 ms: 1.43x faster                                                       |
| chaos                   | 61.7 ms                                                     | 43.1 ms: 1.43x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 783 ms: 1.42x faster                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 865 us: 1.40x faster                                                       |
| unpickle_pure_python    | 183 us                                                      | 130 us: 1.40x faster                                                       |
| html5lib                | 51.0 ms                                                     | 36.4 ms: 1.40x faster                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.06 ms: 1.39x faster                                                      |
| crypto_pyaes            | 62.5 ms                                                     | 45.4 ms: 1.38x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 14.4 ms: 1.37x faster                                                      |
| async_tree_memoization  | 526 ms                                                      | 386 ms: 1.36x faster                                                       |
| async_tree_none         | 435 ms                                                      | 325 ms: 1.34x faster                                                       |
| django_template         | 28.9 ms                                                     | 21.6 ms: 1.34x faster                                                      |
| xml_etree_process       | 44.5 ms                                                     | 33.9 ms: 1.31x faster                                                      |
| pprint_pformat          | 1.22 sec                                                    | 934 ms: 1.30x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 22.2 us: 1.29x faster                                                      |
| pprint_safe_repr        | 592 ms                                                      | 458 ms: 1.29x faster                                                       |
| regex_compile           | 106 ms                                                      | 82.3 ms: 1.29x faster                                                      |
| unpack_sequence         | 39.6 ns                                                     | 30.8 ns: 1.29x faster                                                      |
| async_generators        | 222 ms                                                      | 173 ms: 1.28x faster                                                       |
| genshi_xml              | 41.0 ms                                                     | 32.2 ms: 1.27x faster                                                      |
| 2to3                    | 246 ms                                                      | 193 ms: 1.27x faster                                                       |
| float                   | 61.7 ms                                                     | 48.7 ms: 1.27x faster                                                      |
| docutils                | 1.92 sec                                                    | 1.52 sec: 1.27x faster                                                     |
| chameleon               | 5.79 ms                                                     | 4.59 ms: 1.26x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 507 ms: 1.26x faster                                                       |
| sqlglot_optimize        | 39.8 ms                                                     | 32.1 ms: 1.24x faster                                                      |
| spectral_norm           | 77.3 ms                                                     | 63.1 ms: 1.22x faster                                                      |
| dask                    | 313 ms                                                      | 258 ms: 1.21x faster                                                       |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.25 ms: 1.21x faster                                                      |
| tornado_http            | 108 ms                                                      | 89.5 ms: 1.21x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 665 us: 1.20x faster                                                       |
| sympy_integrate         | 15.3 ms                                                     | 12.9 ms: 1.19x faster                                                      |
| deepcopy                | 255 us                                                      | 217 us: 1.18x faster                                                       |
| sqlglot_normalize       | 205 ms                                                      | 174 ms: 1.18x faster                                                       |
| deepcopy_reduce         | 2.20 us                                                     | 1.87 us: 1.18x faster                                                      |
| dulwich_log             | 50.5 ms                                                     | 43.1 ms: 1.17x faster                                                      |
| mdp                     | 1.78 sec                                                    | 1.53 sec: 1.16x faster                                                     |
| nqueens                 | 66.6 ms                                                     | 57.5 ms: 1.16x faster                                                      |
| bench_thread_pool       | 958 us                                                      | 835 us: 1.15x faster                                                       |
| nbody                   | 71.3 ms                                                     | 62.3 ms: 1.15x faster                                                      |
| json                    | 3.14 ms                                                     | 2.75 ms: 1.14x faster                                                      |
| regex_dna               | 136 ms                                                      | 120 ms: 1.14x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 49.0 ms: 1.13x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| fannkuch                | 256 ms                                                      | 227 ms: 1.13x faster                                                       |
| regex_v8                | 15.4 ms                                                     | 13.8 ms: 1.12x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.71 us: 1.12x faster                                                      |
| sympy_sum               | 107 ms                                                      | 96.1 ms: 1.11x faster                                                      |
| sympy_expand            | 314 ms                                                      | 282 ms: 1.11x faster                                                       |
| sympy_str               | 194 ms                                                      | 175 ms: 1.11x faster                                                       |
| thrift                  | 617 us                                                      | 558 us: 1.11x faster                                                       |
| xml_etree_parse         | 96.8 ms                                                     | 87.6 ms: 1.11x faster                                                      |
| scimark_fft             | 187 ms                                                      | 170 ms: 1.10x faster                                                       |
| unpickle                | 9.09 us                                                     | 8.25 us: 1.10x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 69.3 ms: 1.10x faster                                                      |
| comprehensions          | 16.5 us                                                     | 15.4 us: 1.07x faster                                                      |
| coroutines              | 16.0 ms                                                     | 15.0 ms: 1.07x faster                                                      |
| xml_etree_iterparse     | 65.0 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| json_loads              | 14.0 us                                                     | 13.3 us: 1.06x faster                                                      |
| pickle_list             | 2.75 us                                                     | 2.62 us: 1.05x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 72.6 ms: 1.04x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.57 us: 1.04x faster                                                      |
| logging_format          | 6.76 us                                                     | 6.56 us: 1.03x faster                                                      |
| pidigits                | 149 ms                                                      | 146 ms: 1.02x faster                                                       |
| bench_mp_pool           | 62.0 ms                                                     | 61.2 ms: 1.01x faster                                                      |
| logging_simple          | 6.22 us                                                     | 6.31 us: 1.01x slower                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.44 ms: 1.02x slower                                                      |
| regex_effbot            | 1.66 ms                                                     | 1.70 ms: 1.03x slower                                                      |
| unpickle_list           | 2.71 us                                                     | 2.79 us: 1.03x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 18.3 us: 1.07x slower                                                      |
| generators              | 32.4 ms                                                     | 35.7 ms: 1.10x slower                                                      |
| coverage                | 39.0 ms                                                     | 52.0 ms: 1.33x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.21x faster                                                               |

Benchmark hidden because not significant (3): asyncio_tcp, python_startup_no_site, telco
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown