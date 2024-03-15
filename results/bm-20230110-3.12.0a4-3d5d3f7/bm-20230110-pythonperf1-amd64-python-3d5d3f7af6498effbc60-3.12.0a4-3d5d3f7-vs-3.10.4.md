
# Results vs. 3.10.4

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: windows-amd64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.27x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 193 ms: 1.27x faster                                                       |
| chameleon      | 5.79 ms                                                     | 4.39 ms: 1.32x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.48 sec: 1.30x faster                                                     |
| html5lib       | 51.0 ms                                                     | 33.7 ms: 1.51x faster                                                      |
| Geometric mean | (ref)                                                       | 1.35x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 342 ms: 1.54x faster                                                       |
| async_tree_io           | 1.11 sec                                                    | 742 ms: 1.49x faster                                                       |
| async_tree_none         | 435 ms                                                      | 295 ms: 1.47x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 465 ms: 1.37x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.47x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 47.2 ms: 1.31x faster                                                      |
| nbody          | 71.3 ms                                                     | 59.5 ms: 1.20x faster                                                      |
| pidigits       | 149 ms                                                      | 145 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.17x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 78.8 ms: 1.34x faster                                                      |
| regex_dna      | 136 ms                                                      | 120 ms: 1.13x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 13.6 ms: 1.13x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                      |
| Geometric mean | (ref)                                                       | 1.16x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.10 ms: 1.80x faster                                                      |
| pickle_pure_python   | 270 us                                                      | 169 us: 1.59x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 119 us: 1.54x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 33.8 ms: 1.31x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 48.3 ms: 1.15x faster                                                      |
| json_loads           | 14.0 us                                                     | 12.4 us: 1.13x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 86.5 ms: 1.12x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 60.1 ms: 1.08x faster                                                      |
| unpickle_list        | 2.71 us                                                     | 2.59 us: 1.05x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.70 us: 1.05x faster                                                      |
| pickle               | 6.85 us                                                     | 6.55 us: 1.04x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.81 us: 1.02x slower                                                      |
| pickle_dict          | 17.2 us                                                     | 18.2 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.19x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.1 ms: 1.14x faster                                                      |
| python_startup_no_site | 15.5 ms                                                     | 15.2 ms: 1.02x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.08x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 6.05 ms: 1.49x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 13.3 ms: 1.49x faster                                                      |
| django_template | 28.9 ms                                                     | 20.7 ms: 1.40x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 30.5 ms: 1.35x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.43x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 1.94 ms: 2.15x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 5.10 ms: 1.80x faster                                                      |
| richards                | 42.4 ms                                                     | 24.0 ms: 1.77x faster                                                      |
| logging_silent          | 94.6 ns                                                     | 54.2 ns: 1.75x faster                                                      |
| go                      | 139 ms                                                      | 80.4 ms: 1.73x faster                                                      |
| scimark_sor             | 106 ms                                                      | 63.7 ms: 1.67x faster                                                      |
| raytrace                | 273 ms                                                      | 171 ms: 1.60x faster                                                       |
| pickle_pure_python      | 270 us                                                      | 169 us: 1.59x faster                                                       |
| asyncio_tcp             | 732 ms                                                      | 466 ms: 1.57x faster                                                       |
| pyflate                 | 409 ms                                                      | 263 ms: 1.55x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 342 ms: 1.54x faster                                                       |
| unpickle_pure_python    | 183 us                                                      | 119 us: 1.54x faster                                                       |
| scimark_lu              | 85.8 ms                                                     | 56.0 ms: 1.53x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 3.77 ms: 1.52x faster                                                      |
| unpack_sequence         | 39.6 ns                                                     | 26.2 ns: 1.51x faster                                                      |
| html5lib                | 51.0 ms                                                     | 33.7 ms: 1.51x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 38.0 ms: 1.51x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 742 ms: 1.49x faster                                                       |
| mako                    | 9.03 ms                                                     | 6.05 ms: 1.49x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 13.3 ms: 1.49x faster                                                      |
| pycparser               | 930 ms                                                      | 628 ms: 1.48x faster                                                       |
| async_tree_none         | 435 ms                                                      | 295 ms: 1.47x faster                                                       |
| chaos                   | 61.7 ms                                                     | 42.1 ms: 1.47x faster                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.02 ms: 1.44x faster                                                      |
| sqlglot_parse           | 1.22 ms                                                     | 848 us: 1.43x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 20.4 us: 1.41x faster                                                      |
| django_template         | 28.9 ms                                                     | 20.7 ms: 1.40x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 465 ms: 1.37x faster                                                       |
| crypto_pyaes            | 62.5 ms                                                     | 45.9 ms: 1.36x faster                                                      |
| genshi_xml              | 41.0 ms                                                     | 30.5 ms: 1.35x faster                                                      |
| regex_compile           | 106 ms                                                      | 78.8 ms: 1.34x faster                                                      |
| thrift                  | 617 us                                                      | 463 us: 1.33x faster                                                       |
| pprint_pformat          | 1.22 sec                                                    | 918 ms: 1.33x faster                                                       |
| pprint_safe_repr        | 592 ms                                                      | 448 ms: 1.32x faster                                                       |
| chameleon               | 5.79 ms                                                     | 4.39 ms: 1.32x faster                                                      |
| xml_etree_process       | 44.5 ms                                                     | 33.8 ms: 1.31x faster                                                      |
| async_generators        | 222 ms                                                      | 169 ms: 1.31x faster                                                       |
| float                   | 61.7 ms                                                     | 47.2 ms: 1.31x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 30.6 ms: 1.30x faster                                                      |
| docutils                | 1.92 sec                                                    | 1.48 sec: 1.30x faster                                                     |
| deepcopy                | 255 us                                                      | 199 us: 1.28x faster                                                       |
| dask                    | 313 ms                                                      | 246 ms: 1.27x faster                                                       |
| 2to3                    | 246 ms                                                      | 193 ms: 1.27x faster                                                       |
| dulwich_log             | 50.5 ms                                                     | 40.1 ms: 1.26x faster                                                      |
| deepcopy_reduce         | 2.20 us                                                     | 1.78 us: 1.24x faster                                                      |
| spectral_norm           | 77.3 ms                                                     | 62.8 ms: 1.23x faster                                                      |
| sqlglot_normalize       | 205 ms                                                      | 168 ms: 1.22x faster                                                       |
| sympy_integrate         | 15.3 ms                                                     | 12.6 ms: 1.21x faster                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.25 ms: 1.21x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 661 us: 1.21x faster                                                       |
| json                    | 3.14 ms                                                     | 2.61 ms: 1.20x faster                                                      |
| bench_thread_pool       | 958 us                                                      | 798 us: 1.20x faster                                                       |
| nbody                   | 71.3 ms                                                     | 59.5 ms: 1.20x faster                                                      |
| fannkuch                | 256 ms                                                      | 217 ms: 1.18x faster                                                       |
| mdp                     | 1.78 sec                                                    | 1.51 sec: 1.18x faster                                                     |
| sympy_expand            | 314 ms                                                      | 269 ms: 1.17x faster                                                       |
| nqueens                 | 66.6 ms                                                     | 57.3 ms: 1.16x faster                                                      |
| sympy_sum               | 107 ms                                                      | 92.0 ms: 1.16x faster                                                      |
| sympy_str               | 194 ms                                                      | 168 ms: 1.16x faster                                                       |
| coroutines              | 16.0 ms                                                     | 13.9 ms: 1.15x faster                                                      |
| xml_etree_generate      | 55.5 ms                                                     | 48.3 ms: 1.15x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.1 ms: 1.14x faster                                                      |
| regex_dna               | 136 ms                                                      | 120 ms: 1.13x faster                                                       |
| regex_v8                | 15.4 ms                                                     | 13.6 ms: 1.13x faster                                                      |
| json_loads              | 14.0 us                                                     | 12.4 us: 1.13x faster                                                      |
| scimark_fft             | 187 ms                                                      | 167 ms: 1.13x faster                                                       |
| xml_etree_parse         | 96.8 ms                                                     | 86.5 ms: 1.12x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 67.9 ms: 1.12x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.72 us: 1.11x faster                                                      |
| comprehensions          | 16.5 us                                                     | 15.0 us: 1.10x faster                                                      |
| telco                   | 3.94 ms                                                     | 3.59 ms: 1.10x faster                                                      |
| xml_etree_iterparse     | 65.0 ms                                                     | 60.1 ms: 1.08x faster                                                      |
| logging_format          | 6.76 us                                                     | 6.29 us: 1.07x faster                                                      |
| logging_simple          | 6.22 us                                                     | 5.84 us: 1.07x faster                                                      |
| unpickle_list           | 2.71 us                                                     | 2.59 us: 1.05x faster                                                      |
| unpickle                | 9.09 us                                                     | 8.70 us: 1.05x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.55 us: 1.04x faster                                                      |
| regex_effbot            | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 73.2 ms: 1.03x faster                                                      |
| pidigits                | 149 ms                                                      | 145 ms: 1.03x faster                                                       |
| python_startup_no_site  | 15.5 ms                                                     | 15.2 ms: 1.02x faster                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 61.1 ms: 1.01x faster                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.43 ms: 1.02x slower                                                      |
| pickle_list             | 2.75 us                                                     | 2.81 us: 1.02x slower                                                      |
| generators              | 32.4 ms                                                     | 33.1 ms: 1.02x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 18.2 us: 1.06x slower                                                      |
| coverage                | 39.0 ms                                                     | 52.5 ms: 1.35x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.27x faster                                                               |
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: unknown