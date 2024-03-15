
# Results vs. 3.10.4

- fork: python
- ref: f9774e57d84162ff0cba
- machine: windows-amd64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 194 ms: 1.27x faster                                                       |
| chameleon      | 5.79 ms                                                     | 4.76 ms: 1.21x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.51 sec: 1.27x faster                                                     |
| html5lib       | 51.0 ms                                                     | 34.8 ms: 1.46x faster                                                      |
| tornado_http   | 108 ms                                                      | 90.6 ms: 1.20x faster                                                      |
| Geometric mean | (ref)                                                       | 1.28x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 744 ms: 1.49x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 356 ms: 1.48x faster                                                       |
| async_tree_none         | 435 ms                                                      | 304 ms: 1.43x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 479 ms: 1.33x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.43x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 47.4 ms: 1.30x faster                                                      |
| nbody          | 71.3 ms                                                     | 63.3 ms: 1.13x faster                                                      |
| pidigits       | 149 ms                                                      | 147 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 83.5 ms: 1.27x faster                                                      |
| regex_dna      | 136 ms                                                      | 115 ms: 1.18x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 13.4 ms: 1.16x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.50 ms: 1.11x faster                                                      |
| Geometric mean | (ref)                                                       | 1.18x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.51 ms: 1.66x faster                                                      |
| pickle_pure_python   | 270 us                                                      | 175 us: 1.54x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 124 us: 1.48x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 35.6 ms: 1.25x faster                                                      |
| unpickle             | 9.09 us                                                     | 7.98 us: 1.14x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 88.4 ms: 1.10x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 52.1 ms: 1.07x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| json_loads           | 14.0 us                                                     | 13.4 us: 1.04x faster                                                      |
| pickle               | 6.85 us                                                     | 6.96 us: 1.02x slower                                                      |
| pickle_list          | 2.75 us                                                     | 2.80 us: 1.02x slower                                                      |
| pickle_dict          | 17.2 us                                                     | 18.7 us: 1.09x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.15x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| Geometric mean | (ref)                                                       | 1.06x faster                                                               |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 6.20 ms: 1.46x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 13.9 ms: 1.42x faster                                                      |
| django_template | 28.9 ms                                                     | 20.9 ms: 1.38x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 30.9 ms: 1.33x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.40x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 1.92 ms: 2.18x faster                                                      |
| richards                | 42.4 ms                                                     | 24.5 ms: 1.73x faster                                                      |
| go                      | 139 ms                                                      | 82.6 ms: 1.68x faster                                                      |
| logging_silent          | 94.6 ns                                                     | 56.5 ns: 1.67x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 5.51 ms: 1.66x faster                                                      |
| asyncio_tcp             | 732 ms                                                      | 463 ms: 1.58x faster                                                       |
| pickle_pure_python      | 270 us                                                      | 175 us: 1.54x faster                                                       |
| pyflate                 | 409 ms                                                      | 270 ms: 1.51x faster                                                       |
| raytrace                | 273 ms                                                      | 180 ms: 1.51x faster                                                       |
| hexiom                  | 5.74 ms                                                     | 3.83 ms: 1.50x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 744 ms: 1.49x faster                                                       |
| scimark_sor             | 106 ms                                                      | 71.6 ms: 1.48x faster                                                      |
| unpickle_pure_python    | 183 us                                                      | 124 us: 1.48x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 356 ms: 1.48x faster                                                       |
| generators              | 32.4 ms                                                     | 21.9 ms: 1.48x faster                                                      |
| chaos                   | 61.7 ms                                                     | 42.0 ms: 1.47x faster                                                      |
| html5lib                | 51.0 ms                                                     | 34.8 ms: 1.46x faster                                                      |
| scimark_lu              | 85.8 ms                                                     | 58.7 ms: 1.46x faster                                                      |
| mako                    | 9.03 ms                                                     | 6.20 ms: 1.46x faster                                                      |
| crypto_pyaes            | 62.5 ms                                                     | 43.3 ms: 1.45x faster                                                      |
| async_tree_none         | 435 ms                                                      | 304 ms: 1.43x faster                                                       |
| genshi_text             | 19.8 ms                                                     | 13.9 ms: 1.42x faster                                                      |
| unpack_sequence         | 39.6 ns                                                     | 27.9 ns: 1.42x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 40.4 ms: 1.42x faster                                                      |
| pycparser               | 930 ms                                                      | 663 ms: 1.40x faster                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 871 us: 1.40x faster                                                       |
| sqlglot_transpile       | 1.48 ms                                                     | 1.06 ms: 1.39x faster                                                      |
| django_template         | 28.9 ms                                                     | 20.9 ms: 1.38x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 479 ms: 1.33x faster                                                       |
| genshi_xml              | 41.0 ms                                                     | 30.9 ms: 1.33x faster                                                      |
| float                   | 61.7 ms                                                     | 47.4 ms: 1.30x faster                                                      |
| thrift                  | 617 us                                                      | 476 us: 1.30x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 22.6 us: 1.28x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 31.2 ms: 1.27x faster                                                      |
| docutils                | 1.92 sec                                                    | 1.51 sec: 1.27x faster                                                     |
| regex_compile           | 106 ms                                                      | 83.5 ms: 1.27x faster                                                      |
| 2to3                    | 246 ms                                                      | 194 ms: 1.27x faster                                                       |
| pprint_pformat          | 1.22 sec                                                    | 977 ms: 1.25x faster                                                       |
| xml_etree_process       | 44.5 ms                                                     | 35.6 ms: 1.25x faster                                                      |
| mdp                     | 1.78 sec                                                    | 1.43 sec: 1.24x faster                                                     |
| pprint_safe_repr        | 592 ms                                                      | 478 ms: 1.24x faster                                                       |
| sqlglot_normalize       | 205 ms                                                      | 168 ms: 1.22x faster                                                       |
| chameleon               | 5.79 ms                                                     | 4.76 ms: 1.21x faster                                                      |
| tornado_http            | 108 ms                                                      | 90.6 ms: 1.20x faster                                                      |
| dulwich_log             | 50.5 ms                                                     | 42.2 ms: 1.19x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 671 us: 1.19x faster                                                       |
| fannkuch                | 256 ms                                                      | 216 ms: 1.19x faster                                                       |
| regex_dna               | 136 ms                                                      | 115 ms: 1.18x faster                                                       |
| deepcopy_reduce         | 2.20 us                                                     | 1.88 us: 1.17x faster                                                      |
| nqueens                 | 66.6 ms                                                     | 56.9 ms: 1.17x faster                                                      |
| sympy_integrate         | 15.3 ms                                                     | 13.1 ms: 1.17x faster                                                      |
| deepcopy                | 255 us                                                      | 219 us: 1.17x faster                                                       |
| bench_thread_pool       | 958 us                                                      | 827 us: 1.16x faster                                                       |
| regex_v8                | 15.4 ms                                                     | 13.4 ms: 1.16x faster                                                      |
| spectral_norm           | 77.3 ms                                                     | 67.2 ms: 1.15x faster                                                      |
| json                    | 3.14 ms                                                     | 2.74 ms: 1.14x faster                                                      |
| coroutines              | 16.0 ms                                                     | 14.0 ms: 1.14x faster                                                      |
| unpickle                | 9.09 us                                                     | 7.98 us: 1.14x faster                                                      |
| sympy_expand            | 314 ms                                                      | 277 ms: 1.14x faster                                                       |
| python_startup          | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| sympy_str               | 194 ms                                                      | 173 ms: 1.13x faster                                                       |
| nbody                   | 71.3 ms                                                     | 63.3 ms: 1.13x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 68.0 ms: 1.12x faster                                                      |
| scimark_fft             | 187 ms                                                      | 169 ms: 1.11x faster                                                       |
| regex_effbot            | 1.66 ms                                                     | 1.50 ms: 1.11x faster                                                      |
| sympy_sum               | 107 ms                                                      | 96.6 ms: 1.11x faster                                                      |
| xml_etree_parse         | 96.8 ms                                                     | 88.4 ms: 1.10x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.79 us: 1.07x faster                                                      |
| xml_etree_generate      | 55.5 ms                                                     | 52.1 ms: 1.07x faster                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.56 ms: 1.06x faster                                                      |
| xml_etree_iterparse     | 65.0 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| json_loads              | 14.0 us                                                     | 13.4 us: 1.04x faster                                                      |
| comprehensions          | 16.5 us                                                     | 15.9 us: 1.04x faster                                                      |
| logging_format          | 6.76 us                                                     | 6.55 us: 1.03x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 73.9 ms: 1.02x faster                                                      |
| telco                   | 3.94 ms                                                     | 3.86 ms: 1.02x faster                                                      |
| logging_simple          | 6.22 us                                                     | 6.10 us: 1.02x faster                                                      |
| pidigits                | 149 ms                                                      | 147 ms: 1.02x faster                                                       |
| async_generators        | 222 ms                                                      | 223 ms: 1.01x slower                                                       |
| pickle                  | 6.85 us                                                     | 6.96 us: 1.02x slower                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 63.1 ms: 1.02x slower                                                      |
| pickle_list             | 2.75 us                                                     | 2.80 us: 1.02x slower                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.44 ms: 1.02x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 18.7 us: 1.09x slower                                                      |
| dask                    | 313 ms                                                      | 352 ms: 1.13x slower                                                       |
| coverage                | 39.0 ms                                                     | 49.9 ms: 1.28x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.23x faster                                                               |

Benchmark hidden because not significant (2): python_startup_no_site, unpickle_list
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: unknown