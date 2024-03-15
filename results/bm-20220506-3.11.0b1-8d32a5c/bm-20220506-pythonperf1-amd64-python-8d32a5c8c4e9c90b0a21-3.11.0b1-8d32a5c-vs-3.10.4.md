
# Results vs. 3.10.4

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: windows-amd64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 203 ms: 1.21x faster                                                       |
| chameleon      | 5.79 ms                                                     | 5.45 ms: 1.06x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                     |
| html5lib       | 51.0 ms                                                     | 38.3 ms: 1.33x faster                                                      |
| tornado_http   | 108 ms                                                      | 89.7 ms: 1.21x faster                                                      |
| Geometric mean | (ref)                                                       | 1.20x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 751 ms: 1.48x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 370 ms: 1.42x faster                                                       |
| async_tree_none         | 435 ms                                                      | 311 ms: 1.40x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 499 ms: 1.28x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.39x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.5 ms: 1.15x faster                                                      |
| nbody          | 71.3 ms                                                     | 67.9 ms: 1.05x faster                                                      |
| pidigits       | 149 ms                                                      | 147 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 90.5 ms: 1.17x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.47 ms: 1.13x faster                                                      |
| regex_dna      | 136 ms                                                      | 121 ms: 1.13x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                                      |
| Geometric mean | (ref)                                                       | 1.13x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 204 us: 1.32x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 152 us: 1.20x faster                                                       |
| json_dumps           | 9.16 ms                                                     | 7.72 ms: 1.19x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 37.6 ms: 1.18x faster                                                      |
| unpickle             | 9.09 us                                                     | 7.87 us: 1.16x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 61.1 ms: 1.06x faster                                                      |
| unpickle_list        | 2.71 us                                                     | 2.58 us: 1.05x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 53.0 ms: 1.05x faster                                                      |
| json_loads           | 14.0 us                                                     | 13.4 us: 1.04x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 93.1 ms: 1.04x faster                                                      |
| pickle               | 6.85 us                                                     | 6.59 us: 1.04x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.67 us: 1.03x faster                                                      |
| pickle_dict          | 17.2 us                                                     | 17.1 us: 1.01x faster                                                      |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                      |
| python_startup_no_site | 15.5 ms                                                     | 15.2 ms: 1.02x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.13 ms: 1.27x faster                                                      |
| django_template | 28.9 ms                                                     | 24.0 ms: 1.20x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 17.7 ms: 1.12x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 39.8 ms: 1.03x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.15x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.66 ms: 1.57x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 751 ms: 1.48x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 370 ms: 1.42x faster                                                       |
| go                      | 139 ms                                                      | 97.9 ms: 1.42x faster                                                      |
| richards                | 42.4 ms                                                     | 30.1 ms: 1.41x faster                                                      |
| async_tree_none         | 435 ms                                                      | 311 ms: 1.40x faster                                                       |
| scimark_sor             | 106 ms                                                      | 77.1 ms: 1.38x faster                                                      |
| scimark_lu              | 85.8 ms                                                     | 62.7 ms: 1.37x faster                                                      |
| pyflate                 | 409 ms                                                      | 303 ms: 1.35x faster                                                       |
| logging_silent          | 94.6 ns                                                     | 70.2 ns: 1.35x faster                                                      |
| raytrace                | 273 ms                                                      | 203 ms: 1.34x faster                                                       |
| html5lib                | 51.0 ms                                                     | 38.3 ms: 1.33x faster                                                      |
| pickle_pure_python      | 270 us                                                      | 204 us: 1.32x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 499 ms: 1.28x faster                                                       |
| crypto_pyaes            | 62.5 ms                                                     | 49.1 ms: 1.27x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 45.0 ms: 1.27x faster                                                      |
| mako                    | 9.03 ms                                                     | 7.13 ms: 1.27x faster                                                      |
| chaos                   | 61.7 ms                                                     | 48.9 ms: 1.26x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 4.59 ms: 1.25x faster                                                      |
| pycparser               | 930 ms                                                      | 748 ms: 1.24x faster                                                       |
| thrift                  | 617 us                                                      | 504 us: 1.22x faster                                                       |
| docutils                | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                     |
| async_generators        | 222 ms                                                      | 182 ms: 1.21x faster                                                       |
| 2to3                    | 246 ms                                                      | 203 ms: 1.21x faster                                                       |
| tornado_http            | 108 ms                                                      | 89.7 ms: 1.21x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 663 us: 1.21x faster                                                       |
| django_template         | 28.9 ms                                                     | 24.0 ms: 1.20x faster                                                      |
| unpickle_pure_python    | 183 us                                                      | 152 us: 1.20x faster                                                       |
| dulwich_log             | 50.5 ms                                                     | 42.5 ms: 1.19x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 7.72 ms: 1.19x faster                                                      |
| xml_etree_process       | 44.5 ms                                                     | 37.6 ms: 1.18x faster                                                      |
| regex_compile           | 106 ms                                                      | 90.5 ms: 1.17x faster                                                      |
| dask                    | 313 ms                                                      | 268 ms: 1.17x faster                                                       |
| aiohttp                 | 995 us                                                      | 854 us: 1.17x faster                                                       |
| unpickle                | 9.09 us                                                     | 7.87 us: 1.16x faster                                                      |
| float                   | 61.7 ms                                                     | 53.5 ms: 1.15x faster                                                      |
| deepcopy_memo           | 28.8 us                                                     | 25.1 us: 1.15x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.69 us: 1.13x faster                                                      |
| pprint_pformat          | 1.22 sec                                                    | 1.08 sec: 1.13x faster                                                     |
| pprint_safe_repr        | 592 ms                                                      | 525 ms: 1.13x faster                                                       |
| regex_effbot            | 1.66 ms                                                     | 1.47 ms: 1.13x faster                                                      |
| regex_dna               | 136 ms                                                      | 121 ms: 1.13x faster                                                       |
| sympy_integrate         | 15.3 ms                                                     | 13.6 ms: 1.12x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 17.7 ms: 1.12x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 35.6 ms: 1.12x faster                                                      |
| pylint                  | 350 ms                                                      | 314 ms: 1.12x faster                                                       |
| spectral_norm           | 77.3 ms                                                     | 69.6 ms: 1.11x faster                                                      |
| regex_v8                | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                                      |
| sympy_sum               | 107 ms                                                      | 96.9 ms: 1.10x faster                                                      |
| mdp                     | 1.78 sec                                                    | 1.63 sec: 1.09x faster                                                     |
| asyncio_tcp             | 732 ms                                                      | 673 ms: 1.09x faster                                                       |
| logging_format          | 6.76 us                                                     | 6.25 us: 1.08x faster                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.37 ms: 1.08x faster                                                      |
| bench_thread_pool       | 958 us                                                      | 888 us: 1.08x faster                                                       |
| sympy_expand            | 314 ms                                                      | 293 ms: 1.07x faster                                                       |
| logging_simple          | 6.22 us                                                     | 5.80 us: 1.07x faster                                                      |
| sympy_str               | 194 ms                                                      | 183 ms: 1.06x faster                                                       |
| xml_etree_iterparse     | 65.0 ms                                                     | 61.1 ms: 1.06x faster                                                      |
| chameleon               | 5.79 ms                                                     | 5.45 ms: 1.06x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 71.4 ms: 1.06x faster                                                      |
| coroutines              | 16.0 ms                                                     | 15.2 ms: 1.05x faster                                                      |
| unpickle_list           | 2.71 us                                                     | 2.58 us: 1.05x faster                                                      |
| sqlglot_parse           | 1.22 ms                                                     | 1.15 ms: 1.05x faster                                                      |
| sqlglot_normalize       | 205 ms                                                      | 196 ms: 1.05x faster                                                       |
| nbody                   | 71.3 ms                                                     | 67.9 ms: 1.05x faster                                                      |
| xml_etree_generate      | 55.5 ms                                                     | 53.0 ms: 1.05x faster                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.60 ms: 1.05x faster                                                      |
| json_loads              | 14.0 us                                                     | 13.4 us: 1.04x faster                                                      |
| scimark_fft             | 187 ms                                                      | 180 ms: 1.04x faster                                                       |
| deepcopy_reduce         | 2.20 us                                                     | 2.12 us: 1.04x faster                                                      |
| xml_etree_parse         | 96.8 ms                                                     | 93.1 ms: 1.04x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.59 us: 1.04x faster                                                      |
| genshi_xml              | 41.0 ms                                                     | 39.8 ms: 1.03x faster                                                      |
| pickle_list             | 2.75 us                                                     | 2.67 us: 1.03x faster                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 60.6 ms: 1.02x faster                                                      |
| python_startup_no_site  | 15.5 ms                                                     | 15.2 ms: 1.02x faster                                                      |
| pidigits                | 149 ms                                                      | 147 ms: 1.02x faster                                                       |
| fannkuch                | 256 ms                                                      | 252 ms: 1.01x faster                                                       |
| deepcopy                | 255 us                                                      | 252 us: 1.01x faster                                                       |
| pickle_dict             | 17.2 us                                                     | 17.1 us: 1.01x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 75.5 ms: 1.01x faster                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.42 ms: 1.01x slower                                                      |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| nqueens                 | 66.6 ms                                                     | 67.6 ms: 1.01x slower                                                      |
| generators              | 32.4 ms                                                     | 33.9 ms: 1.05x slower                                                      |
| unpack_sequence         | 39.6 ns                                                     | 42.2 ns: 1.06x slower                                                      |
| comprehensions          | 16.5 us                                                     | 17.8 us: 1.08x slower                                                      |
| coverage                | 39.0 ms                                                     | 103 ms: 2.63x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.12x faster                                                               |

Benchmark hidden because not significant (2): telco, json
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown