
# Results vs. 3.10.4

- fork: python
- ref: 7c12e4835ebe52287acd
- machine: windows-amd64
- commit hash: 7c12e48
- commit date: 2021-10-05
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 222 ms: 1.11x faster                                                       |
| chameleon      | 5.79 ms                                                     | 5.68 ms: 1.02x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.73 sec: 1.11x faster                                                     |
| html5lib       | 51.0 ms                                                     | 41.5 ms: 1.23x faster                                                      |
| tornado_http   | 108 ms                                                      | 97.6 ms: 1.11x faster                                                      |
| Geometric mean | (ref)                                                       | 1.11x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 296 ms: 1.47x faster                                                       |
| async_tree_io           | 1.11 sec                                                    | 777 ms: 1.43x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 384 ms: 1.37x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 541 ms: 1.18x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.36x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                                      |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                                       |
| nbody          | 71.3 ms                                                     | 86.8 ms: 1.22x slower                                                      |
| Geometric mean | (ref)                                                       | 1.04x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 92.3 ms: 1.15x faster                                                      |
| regex_v8       | 15.4 ms                                                     | 14.4 ms: 1.07x faster                                                      |
| regex_dna      | 136 ms                                                      | 129 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.07x faster                                                               |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 8.03 ms: 1.14x faster                                                      |
| pickle_pure_python   | 270 us                                                      | 240 us: 1.12x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 40.3 ms: 1.10x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.48 us: 1.07x faster                                                      |
| unpickle_pure_python | 183 us                                                      | 172 us: 1.07x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.56 us: 1.06x faster                                                      |
| pickle               | 6.85 us                                                     | 6.58 us: 1.04x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.66 us: 1.03x faster                                                      |
| pickle_dict          | 17.2 us                                                     | 16.8 us: 1.02x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 54.8 ms: 1.01x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 65.6 ms: 1.01x slower                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 98.4 ms: 1.02x slower                                                      |
| json_loads           | 14.0 us                                                     | 14.4 us: 1.03x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup_no_site, python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 19.8 ms                                                     | 17.3 ms: 1.14x faster                                                      |
| django_template | 28.9 ms                                                     | 25.8 ms: 1.12x faster                                                      |
| mako            | 9.03 ms                                                     | 8.12 ms: 1.11x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 37.8 ms: 1.08x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.11x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 296 ms: 1.47x faster                                                       |
| async_tree_io           | 1.11 sec                                                    | 777 ms: 1.43x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 384 ms: 1.37x faster                                                       |
| deltablue               | 4.19 ms                                                     | 3.12 ms: 1.34x faster                                                      |
| go                      | 139 ms                                                      | 108 ms: 1.29x faster                                                       |
| html5lib                | 51.0 ms                                                     | 41.5 ms: 1.23x faster                                                      |
| richards                | 42.4 ms                                                     | 34.7 ms: 1.22x faster                                                      |
| raytrace                | 273 ms                                                      | 224 ms: 1.22x faster                                                       |
| sqlalchemy_declarative  | 103 ms                                                      | 86.3 ms: 1.20x faster                                                      |
| pycparser               | 930 ms                                                      | 777 ms: 1.20x faster                                                       |
| logging_format          | 6.76 us                                                     | 5.64 us: 1.20x faster                                                      |
| logging_simple          | 6.22 us                                                     | 5.24 us: 1.19x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 541 ms: 1.18x faster                                                       |
| asyncio_tcp             | 732 ms                                                      | 628 ms: 1.17x faster                                                       |
| thrift                  | 617 us                                                      | 535 us: 1.15x faster                                                       |
| regex_compile           | 106 ms                                                      | 92.3 ms: 1.15x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 17.3 ms: 1.14x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 8.03 ms: 1.14x faster                                                      |
| logging_silent          | 94.6 ns                                                     | 83.4 ns: 1.13x faster                                                      |
| mdp                     | 1.78 sec                                                    | 1.58 sec: 1.13x faster                                                     |
| chaos                   | 61.7 ms                                                     | 55.0 ms: 1.12x faster                                                      |
| pickle_pure_python      | 270 us                                                      | 240 us: 1.12x faster                                                       |
| pyflate                 | 409 ms                                                      | 365 ms: 1.12x faster                                                       |
| generators              | 32.4 ms                                                     | 28.9 ms: 1.12x faster                                                      |
| django_template         | 28.9 ms                                                     | 25.8 ms: 1.12x faster                                                      |
| async_generators        | 222 ms                                                      | 198 ms: 1.12x faster                                                       |
| mako                    | 9.03 ms                                                     | 8.12 ms: 1.11x faster                                                      |
| docutils                | 1.92 sec                                                    | 1.73 sec: 1.11x faster                                                     |
| hexiom                  | 5.74 ms                                                     | 5.17 ms: 1.11x faster                                                      |
| tornado_http            | 108 ms                                                      | 97.6 ms: 1.11x faster                                                      |
| 2to3                    | 246 ms                                                      | 222 ms: 1.11x faster                                                       |
| xml_etree_process       | 44.5 ms                                                     | 40.3 ms: 1.10x faster                                                      |
| pylint                  | 350 ms                                                      | 318 ms: 1.10x faster                                                       |
| dulwich_log             | 50.5 ms                                                     | 46.1 ms: 1.09x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 52.6 ms: 1.09x faster                                                      |
| genshi_xml              | 41.0 ms                                                     | 37.8 ms: 1.08x faster                                                      |
| crypto_pyaes            | 62.5 ms                                                     | 57.7 ms: 1.08x faster                                                      |
| float                   | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                                      |
| regex_v8                | 15.4 ms                                                     | 14.4 ms: 1.07x faster                                                      |
| unpickle                | 9.09 us                                                     | 8.48 us: 1.07x faster                                                      |
| unpickle_pure_python    | 183 us                                                      | 172 us: 1.07x faster                                                       |
| sympy_sum               | 107 ms                                                      | 100 ms: 1.07x faster                                                       |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.7 ms: 1.07x faster                                                      |
| sympy_integrate         | 15.3 ms                                                     | 14.4 ms: 1.06x faster                                                      |
| dask                    | 313 ms                                                      | 295 ms: 1.06x faster                                                       |
| sqlite_synth            | 1.91 us                                                     | 1.80 us: 1.06x faster                                                      |
| regex_dna               | 136 ms                                                      | 129 ms: 1.06x faster                                                       |
| unpickle_list           | 2.71 us                                                     | 2.56 us: 1.06x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 37.8 ms: 1.05x faster                                                      |
| pprint_pformat          | 1.22 sec                                                    | 1.16 sec: 1.05x faster                                                     |
| bench_thread_pool       | 958 us                                                      | 915 us: 1.05x faster                                                       |
| json                    | 3.14 ms                                                     | 3.01 ms: 1.04x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.58 us: 1.04x faster                                                      |
| pprint_safe_repr        | 592 ms                                                      | 570 ms: 1.04x faster                                                       |
| sympy_str               | 194 ms                                                      | 188 ms: 1.04x faster                                                       |
| pickle_list             | 2.75 us                                                     | 2.66 us: 1.03x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 73.4 ms: 1.03x faster                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.37 ms: 1.03x faster                                                      |
| scimark_lu              | 85.8 ms                                                     | 83.6 ms: 1.03x faster                                                      |
| pickle_dict             | 17.2 us                                                     | 16.8 us: 1.02x faster                                                      |
| sqlglot_normalize       | 205 ms                                                      | 201 ms: 1.02x faster                                                       |
| deepcopy_reduce         | 2.20 us                                                     | 2.16 us: 1.02x faster                                                      |
| chameleon               | 5.79 ms                                                     | 5.68 ms: 1.02x faster                                                      |
| sympy_expand            | 314 ms                                                      | 309 ms: 1.02x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 54.8 ms: 1.01x faster                                                      |
| scimark_sor             | 106 ms                                                      | 105 ms: 1.01x faster                                                       |
| meteor_contest          | 75.9 ms                                                     | 75.3 ms: 1.01x faster                                                      |
| deepcopy_memo           | 28.8 us                                                     | 28.6 us: 1.01x faster                                                      |
| pidigits                | 149 ms                                                      | 150 ms: 1.01x slower                                                       |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| telco                   | 3.94 ms                                                     | 3.98 ms: 1.01x slower                                                      |
| create_gc_cycles        | 800 us                                                      | 807 us: 1.01x slower                                                       |
| xml_etree_iterparse     | 65.0 ms                                                     | 65.6 ms: 1.01x slower                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 63.0 ms: 1.02x slower                                                      |
| xml_etree_parse         | 96.8 ms                                                     | 98.4 ms: 1.02x slower                                                      |
| nqueens                 | 66.6 ms                                                     | 67.7 ms: 1.02x slower                                                      |
| json_loads              | 14.0 us                                                     | 14.4 us: 1.03x slower                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.53 ms: 1.04x slower                                                      |
| unpack_sequence         | 39.6 ns                                                     | 41.7 ns: 1.05x slower                                                      |
| sqlglot_parse           | 1.22 ms                                                     | 1.32 ms: 1.08x slower                                                      |
| fannkuch                | 256 ms                                                      | 279 ms: 1.09x slower                                                       |
| spectral_norm           | 77.3 ms                                                     | 84.7 ms: 1.10x slower                                                      |
| coroutines              | 16.0 ms                                                     | 17.9 ms: 1.12x slower                                                      |
| scimark_fft             | 187 ms                                                      | 216 ms: 1.15x slower                                                       |
| comprehensions          | 16.5 us                                                     | 19.1 us: 1.16x slower                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 3.18 ms: 1.17x slower                                                      |
| nbody                   | 71.3 ms                                                     | 86.8 ms: 1.22x slower                                                      |
| coverage                | 39.0 ms                                                     | 261 ms: 6.70x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.04x faster                                                               |

Benchmark hidden because not significant (4): deepcopy, regex_effbot, python_startup_no_site, python_startup
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown