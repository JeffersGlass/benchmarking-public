
# Results vs. 3.10.4

- fork: python
- ref: 3c67ec394faac79d2608
- machine: windows-amd64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 192 ms: 1.28x faster                                                       |
| chameleon      | 5.79 ms                                                     | 4.41 ms: 1.31x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.50 sec: 1.28x faster                                                     |
| html5lib       | 51.0 ms                                                     | 34.1 ms: 1.50x faster                                                      |
| tornado_http   | 108 ms                                                      | 90.5 ms: 1.20x faster                                                      |
| Geometric mean | (ref)                                                       | 1.31x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 748 ms: 1.48x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 356 ms: 1.48x faster                                                       |
| async_tree_none         | 435 ms                                                      | 302 ms: 1.44x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 480 ms: 1.33x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.43x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 47.3 ms: 1.30x faster                                                      |
| nbody          | 71.3 ms                                                     | 59.1 ms: 1.21x faster                                                      |
| pidigits       | 149 ms                                                      | 146 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.17x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 78.8 ms: 1.35x faster                                                      |
| regex_v8       | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                                      |
| regex_dna      | 136 ms                                                      | 121 ms: 1.12x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.68 ms: 1.02x slower                                                      |
| Geometric mean | (ref)                                                       | 1.14x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.38 ms: 1.70x faster                                                      |
| pickle_pure_python   | 270 us                                                      | 166 us: 1.62x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 120 us: 1.53x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 33.5 ms: 1.33x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 49.5 ms: 1.12x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 88.5 ms: 1.09x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.3 ms: 1.04x faster                                                      |
| unpickle_list        | 2.71 us                                                     | 2.65 us: 1.02x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.70 us: 1.02x faster                                                      |
| pickle               | 6.85 us                                                     | 6.77 us: 1.01x faster                                                      |
| json_loads           | 14.0 us                                                     | 14.2 us: 1.01x slower                                                      |
| unpickle             | 9.09 us                                                     | 9.39 us: 1.03x slower                                                      |
| pickle_dict          | 17.2 us                                                     | 18.5 us: 1.08x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.16x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| Geometric mean | (ref)                                                       | 1.06x faster                                                               |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 6.15 ms: 1.47x faster                                                      |
| django_template | 28.9 ms                                                     | 20.2 ms: 1.43x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 14.2 ms: 1.39x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 32.6 ms: 1.26x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.39x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 1.96 ms: 2.14x faster                                                      |
| richards                | 42.4 ms                                                     | 23.9 ms: 1.77x faster                                                      |
| go                      | 139 ms                                                      | 78.8 ms: 1.76x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 5.38 ms: 1.70x faster                                                      |
| logging_silent          | 94.6 ns                                                     | 58.1 ns: 1.63x faster                                                      |
| pickle_pure_python      | 270 us                                                      | 166 us: 1.62x faster                                                       |
| raytrace                | 273 ms                                                      | 170 ms: 1.60x faster                                                       |
| scimark_sor             | 106 ms                                                      | 67.0 ms: 1.59x faster                                                      |
| asyncio_tcp             | 732 ms                                                      | 466 ms: 1.57x faster                                                       |
| chaos                   | 61.7 ms                                                     | 39.6 ms: 1.56x faster                                                      |
| unpack_sequence         | 39.6 ns                                                     | 25.6 ns: 1.55x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 3.73 ms: 1.54x faster                                                      |
| unpickle_pure_python    | 183 us                                                      | 120 us: 1.53x faster                                                       |
| pyflate                 | 409 ms                                                      | 267 ms: 1.53x faster                                                       |
| scimark_monte_carlo     | 57.3 ms                                                     | 37.9 ms: 1.51x faster                                                      |
| html5lib                | 51.0 ms                                                     | 34.1 ms: 1.50x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 748 ms: 1.48x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 356 ms: 1.48x faster                                                       |
| pycparser               | 930 ms                                                      | 633 ms: 1.47x faster                                                       |
| mako                    | 9.03 ms                                                     | 6.15 ms: 1.47x faster                                                      |
| scimark_lu              | 85.8 ms                                                     | 58.7 ms: 1.46x faster                                                      |
| async_tree_none         | 435 ms                                                      | 302 ms: 1.44x faster                                                       |
| django_template         | 28.9 ms                                                     | 20.2 ms: 1.43x faster                                                      |
| sqlglot_parse           | 1.22 ms                                                     | 851 us: 1.43x faster                                                       |
| crypto_pyaes            | 62.5 ms                                                     | 44.0 ms: 1.42x faster                                                      |
| comprehensions          | 16.5 us                                                     | 11.7 us: 1.41x faster                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.05 ms: 1.40x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 14.2 ms: 1.39x faster                                                      |
| thrift                  | 617 us                                                      | 452 us: 1.37x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 21.1 us: 1.36x faster                                                      |
| regex_compile           | 106 ms                                                      | 78.8 ms: 1.35x faster                                                      |
| pprint_pformat          | 1.22 sec                                                    | 907 ms: 1.34x faster                                                       |
| pprint_safe_repr        | 592 ms                                                      | 445 ms: 1.33x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 480 ms: 1.33x faster                                                       |
| async_generators        | 222 ms                                                      | 167 ms: 1.33x faster                                                       |
| xml_etree_process       | 44.5 ms                                                     | 33.5 ms: 1.33x faster                                                      |
| chameleon               | 5.79 ms                                                     | 4.41 ms: 1.31x faster                                                      |
| float                   | 61.7 ms                                                     | 47.3 ms: 1.30x faster                                                      |
| 2to3                    | 246 ms                                                      | 192 ms: 1.28x faster                                                       |
| docutils                | 1.92 sec                                                    | 1.50 sec: 1.28x faster                                                     |
| genshi_xml              | 41.0 ms                                                     | 32.6 ms: 1.26x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 31.6 ms: 1.26x faster                                                      |
| spectral_norm           | 77.3 ms                                                     | 61.5 ms: 1.26x faster                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.18 ms: 1.25x faster                                                      |
| sympy_integrate         | 15.3 ms                                                     | 12.4 ms: 1.23x faster                                                      |
| nqueens                 | 66.6 ms                                                     | 54.6 ms: 1.22x faster                                                      |
| deepcopy                | 255 us                                                      | 211 us: 1.21x faster                                                       |
| nbody                   | 71.3 ms                                                     | 59.1 ms: 1.21x faster                                                      |
| dulwich_log             | 50.5 ms                                                     | 41.9 ms: 1.20x faster                                                      |
| sqlglot_normalize       | 205 ms                                                      | 171 ms: 1.20x faster                                                       |
| mdp                     | 1.78 sec                                                    | 1.48 sec: 1.20x faster                                                     |
| fannkuch                | 256 ms                                                      | 213 ms: 1.20x faster                                                       |
| tornado_http            | 108 ms                                                      | 90.5 ms: 1.20x faster                                                      |
| sympy_sum               | 107 ms                                                      | 89.5 ms: 1.20x faster                                                      |
| sympy_str               | 194 ms                                                      | 164 ms: 1.19x faster                                                       |
| create_gc_cycles        | 800 us                                                      | 676 us: 1.18x faster                                                       |
| deepcopy_reduce         | 2.20 us                                                     | 1.88 us: 1.17x faster                                                      |
| sympy_expand            | 314 ms                                                      | 269 ms: 1.17x faster                                                       |
| bench_thread_pool       | 958 us                                                      | 823 us: 1.16x faster                                                       |
| scimark_fft             | 187 ms                                                      | 166 ms: 1.13x faster                                                       |
| regex_v8                | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| regex_dna               | 136 ms                                                      | 121 ms: 1.12x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 49.5 ms: 1.12x faster                                                      |
| json                    | 3.14 ms                                                     | 2.81 ms: 1.11x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 69.1 ms: 1.10x faster                                                      |
| xml_etree_parse         | 96.8 ms                                                     | 88.5 ms: 1.09x faster                                                      |
| coroutines              | 16.0 ms                                                     | 14.8 ms: 1.08x faster                                                      |
| logging_format          | 6.76 us                                                     | 6.28 us: 1.08x faster                                                      |
| telco                   | 3.94 ms                                                     | 3.72 ms: 1.06x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.82 us: 1.05x faster                                                      |
| xml_etree_iterparse     | 65.0 ms                                                     | 62.3 ms: 1.04x faster                                                      |
| logging_simple          | 6.22 us                                                     | 6.01 us: 1.04x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 73.7 ms: 1.03x faster                                                      |
| unpickle_list           | 2.71 us                                                     | 2.65 us: 1.02x faster                                                      |
| pidigits                | 149 ms                                                      | 146 ms: 1.02x faster                                                       |
| pickle_list             | 2.75 us                                                     | 2.70 us: 1.02x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.77 us: 1.01x faster                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 61.7 ms: 1.01x faster                                                      |
| json_loads              | 14.0 us                                                     | 14.2 us: 1.01x slower                                                      |
| regex_effbot            | 1.66 ms                                                     | 1.68 ms: 1.02x slower                                                      |
| generators              | 32.4 ms                                                     | 33.0 ms: 1.02x slower                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.45 ms: 1.03x slower                                                      |
| unpickle                | 9.09 us                                                     | 9.39 us: 1.03x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 18.5 us: 1.08x slower                                                      |
| dask                    | 313 ms                                                      | 349 ms: 1.12x slower                                                       |
| coverage                | 39.0 ms                                                     | 51.8 ms: 1.33x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.25x faster                                                               |

Benchmark hidden because not significant (1): python_startup_no_site
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: unknown