
# Results vs. 3.10.4

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: windows-amd64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 210 ms: 1.17x faster                                                       |
| chameleon      | 5.79 ms                                                     | 5.53 ms: 1.05x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                                     |
| html5lib       | 51.0 ms                                                     | 41.4 ms: 1.23x faster                                                      |
| tornado_http   | 108 ms                                                      | 98.3 ms: 1.10x faster                                                      |
| Geometric mean | (ref)                                                       | 1.14x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 307 ms: 1.42x faster                                                       |
| async_tree_io           | 1.11 sec                                                    | 793 ms: 1.40x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 395 ms: 1.33x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 530 ms: 1.20x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.33x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.1 ms: 1.10x faster                                                      |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                                       |
| nbody          | 71.3 ms                                                     | 90.3 ms: 1.27x slower                                                      |
| Geometric mean | (ref)                                                       | 1.04x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 90.4 ms: 1.17x faster                                                      |
| regex_dna      | 136 ms                                                      | 131 ms: 1.04x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.82 ms: 1.10x slower                                                      |
| Geometric mean | (ref)                                                       | 1.01x faster                                                               |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 228 us: 1.18x faster                                                       |
| unpickle             | 9.09 us                                                     | 7.81 us: 1.16x faster                                                      |
| json_dumps           | 9.16 ms                                                     | 7.94 ms: 1.15x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 39.7 ms: 1.12x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.49 us: 1.11x faster                                                      |
| unpickle_pure_python | 183 us                                                      | 168 us: 1.09x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.54 us: 1.07x faster                                                      |
| pickle_dict          | 17.2 us                                                     | 16.2 us: 1.06x faster                                                      |
| pickle               | 6.85 us                                                     | 6.61 us: 1.04x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 54.7 ms: 1.01x faster                                                      |
| json_loads           | 14.0 us                                                     | 14.9 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.07x faster                                                               |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.8 ms: 1.09x faster                                                      |
| python_startup_no_site | 15.5 ms                                                     | 15.1 ms: 1.03x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 19.8 ms                                                     | 17.5 ms: 1.13x faster                                                      |
| mako            | 9.03 ms                                                     | 8.07 ms: 1.12x faster                                                      |
| django_template | 28.9 ms                                                     | 26.0 ms: 1.11x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 38.5 ms: 1.07x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.11x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.86 ms: 1.47x faster                                                      |
| async_tree_none         | 435 ms                                                      | 307 ms: 1.42x faster                                                       |
| async_tree_io           | 1.11 sec                                                    | 793 ms: 1.40x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 395 ms: 1.33x faster                                                       |
| logging_silent          | 94.6 ns                                                     | 72.1 ns: 1.31x faster                                                      |
| go                      | 139 ms                                                      | 106 ms: 1.31x faster                                                       |
| raytrace                | 273 ms                                                      | 214 ms: 1.28x faster                                                       |
| richards                | 42.4 ms                                                     | 34.0 ms: 1.25x faster                                                      |
| html5lib                | 51.0 ms                                                     | 41.4 ms: 1.23x faster                                                      |
| pycparser               | 930 ms                                                      | 769 ms: 1.21x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 530 ms: 1.20x faster                                                       |
| pickle_pure_python      | 270 us                                                      | 228 us: 1.18x faster                                                       |
| regex_compile           | 106 ms                                                      | 90.4 ms: 1.17x faster                                                      |
| thrift                  | 617 us                                                      | 528 us: 1.17x faster                                                       |
| sqlalchemy_declarative  | 103 ms                                                      | 88.5 ms: 1.17x faster                                                      |
| 2to3                    | 246 ms                                                      | 210 ms: 1.17x faster                                                       |
| create_gc_cycles        | 800 us                                                      | 686 us: 1.17x faster                                                       |
| unpickle                | 9.09 us                                                     | 7.81 us: 1.16x faster                                                      |
| async_generators        | 222 ms                                                      | 192 ms: 1.16x faster                                                       |
| json_dumps              | 9.16 ms                                                     | 7.94 ms: 1.15x faster                                                      |
| docutils                | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                                     |
| chaos                   | 61.7 ms                                                     | 53.9 ms: 1.15x faster                                                      |
| dulwich_log             | 50.5 ms                                                     | 44.1 ms: 1.14x faster                                                      |
| pyflate                 | 409 ms                                                      | 358 ms: 1.14x faster                                                       |
| logging_simple          | 6.22 us                                                     | 5.45 us: 1.14x faster                                                      |
| logging_format          | 6.76 us                                                     | 5.92 us: 1.14x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 5.06 ms: 1.14x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 17.5 ms: 1.13x faster                                                      |
| mako                    | 9.03 ms                                                     | 8.07 ms: 1.12x faster                                                      |
| xml_etree_process       | 44.5 ms                                                     | 39.7 ms: 1.12x faster                                                      |
| django_template         | 28.9 ms                                                     | 26.0 ms: 1.11x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 51.7 ms: 1.11x faster                                                      |
| pickle_list             | 2.75 us                                                     | 2.49 us: 1.11x faster                                                      |
| mdp                     | 1.78 sec                                                    | 1.61 sec: 1.10x faster                                                     |
| tornado_http            | 108 ms                                                      | 98.3 ms: 1.10x faster                                                      |
| float                   | 61.7 ms                                                     | 56.1 ms: 1.10x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.8 ms: 1.09x faster                                                      |
| unpickle_pure_python    | 183 us                                                      | 168 us: 1.09x faster                                                       |
| pylint                  | 350 ms                                                      | 321 ms: 1.09x faster                                                       |
| pprint_pformat          | 1.22 sec                                                    | 1.13 sec: 1.08x faster                                                     |
| pprint_safe_repr        | 592 ms                                                      | 547 ms: 1.08x faster                                                       |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.6 ms: 1.07x faster                                                      |
| unpickle_list           | 2.71 us                                                     | 2.54 us: 1.07x faster                                                      |
| genshi_xml              | 41.0 ms                                                     | 38.5 ms: 1.07x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.80 us: 1.06x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 37.5 ms: 1.06x faster                                                      |
| crypto_pyaes            | 62.5 ms                                                     | 58.9 ms: 1.06x faster                                                      |
| dask                    | 313 ms                                                      | 295 ms: 1.06x faster                                                       |
| sympy_integrate         | 15.3 ms                                                     | 14.4 ms: 1.06x faster                                                      |
| pickle_dict             | 17.2 us                                                     | 16.2 us: 1.06x faster                                                      |
| bench_thread_pool       | 958 us                                                      | 906 us: 1.06x faster                                                       |
| asyncio_tcp             | 732 ms                                                      | 695 ms: 1.05x faster                                                       |
| scimark_lu              | 85.8 ms                                                     | 81.5 ms: 1.05x faster                                                      |
| sympy_sum               | 107 ms                                                      | 102 ms: 1.05x faster                                                       |
| scimark_sor             | 106 ms                                                      | 101 ms: 1.05x faster                                                       |
| generators              | 32.4 ms                                                     | 31.0 ms: 1.05x faster                                                      |
| sqlglot_normalize       | 205 ms                                                      | 196 ms: 1.05x faster                                                       |
| chameleon               | 5.79 ms                                                     | 5.53 ms: 1.05x faster                                                      |
| regex_dna               | 136 ms                                                      | 131 ms: 1.04x faster                                                       |
| pickle                  | 6.85 us                                                     | 6.61 us: 1.04x faster                                                      |
| xml_etree_parse         | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 73.4 ms: 1.03x faster                                                      |
| python_startup_no_site  | 15.5 ms                                                     | 15.1 ms: 1.03x faster                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.37 ms: 1.03x faster                                                      |
| json                    | 3.14 ms                                                     | 3.06 ms: 1.02x faster                                                      |
| deepcopy_memo           | 28.8 us                                                     | 28.1 us: 1.02x faster                                                      |
| sympy_str               | 194 ms                                                      | 191 ms: 1.02x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 54.7 ms: 1.01x faster                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 61.4 ms: 1.01x faster                                                      |
| sympy_expand            | 314 ms                                                      | 311 ms: 1.01x faster                                                       |
| pidigits                | 149 ms                                                      | 148 ms: 1.01x faster                                                       |
| telco                   | 3.94 ms                                                     | 3.91 ms: 1.01x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 76.2 ms: 1.00x slower                                                      |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| nqueens                 | 66.6 ms                                                     | 67.3 ms: 1.01x slower                                                      |
| deepcopy_reduce         | 2.20 us                                                     | 2.23 us: 1.01x slower                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.50 ms: 1.01x slower                                                      |
| deepcopy                | 255 us                                                      | 266 us: 1.04x slower                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 1.29 ms: 1.06x slower                                                      |
| json_loads              | 14.0 us                                                     | 14.9 us: 1.06x slower                                                      |
| spectral_norm           | 77.3 ms                                                     | 82.7 ms: 1.07x slower                                                      |
| fannkuch                | 256 ms                                                      | 275 ms: 1.08x slower                                                       |
| regex_effbot            | 1.66 ms                                                     | 1.82 ms: 1.10x slower                                                      |
| coroutines              | 16.0 ms                                                     | 18.1 ms: 1.13x slower                                                      |
| scimark_fft             | 187 ms                                                      | 212 ms: 1.13x slower                                                       |
| comprehensions          | 16.5 us                                                     | 19.1 us: 1.16x slower                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 3.18 ms: 1.17x slower                                                      |
| nbody                   | 71.3 ms                                                     | 90.3 ms: 1.27x slower                                                      |
| unpack_sequence         | 39.6 ns                                                     | 51.9 ns: 1.31x slower                                                      |
| coverage                | 39.0 ms                                                     | 262 ms: 6.72x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.05x faster                                                               |

Benchmark hidden because not significant (2): xml_etree_iterparse, regex_v8
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown