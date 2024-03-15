
# Results vs. 3.10.4

- fork: python
- ref: f3909b8bc83675b7ab09
- machine: windows-amd64
- commit hash: f3909b8
- commit date: 2023-04-04
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 206 ms: 1.19x faster                                                     |
| chameleon      | 5.79 ms                                                     | 5.27 ms: 1.10x faster                                                    |
| docutils       | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                                   |
| html5lib       | 51.0 ms                                                     | 39.8 ms: 1.28x faster                                                    |
| tornado_http   | 108 ms                                                      | 90.1 ms: 1.20x faster                                                    |
| Geometric mean | (ref)                                                       | 1.20x faster                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 739 ms: 1.50x faster                                                     |
| async_tree_memoization  | 526 ms                                                      | 368 ms: 1.43x faster                                                     |
| async_tree_none         | 435 ms                                                      | 314 ms: 1.38x faster                                                     |
| async_tree_cpu_io_mixed | 638 ms                                                      | 500 ms: 1.28x faster                                                     |
| Geometric mean          | (ref)                                                       | 1.40x faster                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 52.6 ms: 1.17x faster                                                    |
| nbody          | 71.3 ms                                                     | 69.8 ms: 1.02x faster                                                    |
| pidigits       | 149 ms                                                      | 147 ms: 1.01x faster                                                     |
| Geometric mean | (ref)                                                       | 1.07x faster                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 89.7 ms: 1.18x faster                                                    |
| regex_dna      | 136 ms                                                      | 120 ms: 1.13x faster                                                     |
| regex_v8       | 15.4 ms                                                     | 14.3 ms: 1.08x faster                                                    |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                    |
| Geometric mean | (ref)                                                       | 1.11x faster                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 198 us: 1.36x faster                                                     |
| xml_etree_process    | 44.5 ms                                                     | 36.3 ms: 1.22x faster                                                    |
| unpickle_pure_python | 183 us                                                      | 150 us: 1.22x faster                                                     |
| json_dumps           | 9.16 ms                                                     | 7.60 ms: 1.20x faster                                                    |
| unpickle             | 9.09 us                                                     | 7.97 us: 1.14x faster                                                    |
| json_loads           | 14.0 us                                                     | 13.0 us: 1.08x faster                                                    |
| xml_etree_generate   | 55.5 ms                                                     | 51.8 ms: 1.07x faster                                                    |
| xml_etree_parse      | 96.8 ms                                                     | 91.3 ms: 1.06x faster                                                    |
| xml_etree_iterparse  | 65.0 ms                                                     | 61.4 ms: 1.06x faster                                                    |
| pickle               | 6.85 us                                                     | 6.73 us: 1.02x faster                                                    |
| unpickle_list        | 2.71 us                                                     | 2.68 us: 1.01x faster                                                    |
| pickle_list          | 2.75 us                                                     | 2.78 us: 1.01x slower                                                    |
| pickle_dict          | 17.2 us                                                     | 18.6 us: 1.08x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                    |
| Geometric mean | (ref)                                                       | 1.06x faster                                                             |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.22 ms: 1.25x faster                                                    |
| django_template | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                                    |
| genshi_text     | 19.8 ms                                                     | 17.3 ms: 1.14x faster                                                    |
| genshi_xml      | 41.0 ms                                                     | 37.6 ms: 1.09x faster                                                    |
| Geometric mean  | (ref)                                                       | 1.17x faster                                                             |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.65 ms: 1.58x faster                                                    |
| async_tree_io           | 1.11 sec                                                    | 739 ms: 1.50x faster                                                     |
| async_tree_memoization  | 526 ms                                                      | 368 ms: 1.43x faster                                                     |
| scimark_sor             | 106 ms                                                      | 75.2 ms: 1.41x faster                                                    |
| go                      | 139 ms                                                      | 99.2 ms: 1.40x faster                                                    |
| richards                | 42.4 ms                                                     | 30.4 ms: 1.40x faster                                                    |
| async_tree_none         | 435 ms                                                      | 314 ms: 1.38x faster                                                     |
| pickle_pure_python      | 270 us                                                      | 198 us: 1.36x faster                                                     |
| pyflate                 | 409 ms                                                      | 301 ms: 1.36x faster                                                     |
| scimark_lu              | 85.8 ms                                                     | 63.3 ms: 1.35x faster                                                    |
| logging_silent          | 94.6 ns                                                     | 70.1 ns: 1.35x faster                                                    |
| raytrace                | 273 ms                                                      | 203 ms: 1.35x faster                                                     |
| pycparser               | 930 ms                                                      | 703 ms: 1.32x faster                                                     |
| sqlglot_parse           | 1.22 ms                                                     | 931 us: 1.31x faster                                                     |
| sqlglot_transpile       | 1.48 ms                                                     | 1.13 ms: 1.30x faster                                                    |
| crypto_pyaes            | 62.5 ms                                                     | 48.2 ms: 1.30x faster                                                    |
| html5lib                | 51.0 ms                                                     | 39.8 ms: 1.28x faster                                                    |
| thrift                  | 617 us                                                      | 482 us: 1.28x faster                                                     |
| async_tree_cpu_io_mixed | 638 ms                                                      | 500 ms: 1.28x faster                                                     |
| sqlalchemy_declarative  | 103 ms                                                      | 81.1 ms: 1.28x faster                                                    |
| scimark_monte_carlo     | 57.3 ms                                                     | 45.1 ms: 1.27x faster                                                    |
| async_generators        | 222 ms                                                      | 176 ms: 1.26x faster                                                     |
| chaos                   | 61.7 ms                                                     | 48.9 ms: 1.26x faster                                                    |
| hexiom                  | 5.74 ms                                                     | 4.56 ms: 1.26x faster                                                    |
| mako                    | 9.03 ms                                                     | 7.22 ms: 1.25x faster                                                    |
| xml_etree_process       | 44.5 ms                                                     | 36.3 ms: 1.22x faster                                                    |
| unpickle_pure_python    | 183 us                                                      | 150 us: 1.22x faster                                                     |
| docutils                | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                                   |
| django_template         | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                                    |
| json_dumps              | 9.16 ms                                                     | 7.60 ms: 1.20x faster                                                    |
| create_gc_cycles        | 800 us                                                      | 664 us: 1.20x faster                                                     |
| tornado_http            | 108 ms                                                      | 90.1 ms: 1.20x faster                                                    |
| dask                    | 313 ms                                                      | 261 ms: 1.20x faster                                                     |
| 2to3                    | 246 ms                                                      | 206 ms: 1.19x faster                                                     |
| dulwich_log             | 50.5 ms                                                     | 42.5 ms: 1.19x faster                                                    |
| regex_compile           | 106 ms                                                      | 89.7 ms: 1.18x faster                                                    |
| float                   | 61.7 ms                                                     | 52.6 ms: 1.17x faster                                                    |
| aiohttp                 | 995 us                                                      | 857 us: 1.16x faster                                                     |
| deepcopy_memo           | 28.8 us                                                     | 24.8 us: 1.16x faster                                                    |
| pprint_pformat          | 1.22 sec                                                    | 1.06 sec: 1.15x faster                                                   |
| sqlglot_optimize        | 39.8 ms                                                     | 34.7 ms: 1.15x faster                                                    |
| spectral_norm           | 77.3 ms                                                     | 67.6 ms: 1.14x faster                                                    |
| genshi_text             | 19.8 ms                                                     | 17.3 ms: 1.14x faster                                                    |
| unpickle                | 9.09 us                                                     | 7.97 us: 1.14x faster                                                    |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.0 ms: 1.14x faster                                                    |
| regex_dna               | 136 ms                                                      | 120 ms: 1.13x faster                                                     |
| bench_thread_pool       | 958 us                                                      | 848 us: 1.13x faster                                                     |
| sqlite_synth            | 1.91 us                                                     | 1.69 us: 1.13x faster                                                    |
| pprint_safe_repr        | 592 ms                                                      | 526 ms: 1.13x faster                                                     |
| sympy_integrate         | 15.3 ms                                                     | 13.6 ms: 1.12x faster                                                    |
| python_startup          | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                    |
| chameleon               | 5.79 ms                                                     | 5.27 ms: 1.10x faster                                                    |
| genshi_xml              | 41.0 ms                                                     | 37.6 ms: 1.09x faster                                                    |
| pylint                  | 350 ms                                                      | 321 ms: 1.09x faster                                                     |
| sympy_sum               | 107 ms                                                      | 98.4 ms: 1.09x faster                                                    |
| sympy_expand            | 314 ms                                                      | 290 ms: 1.09x faster                                                     |
| regex_v8                | 15.4 ms                                                     | 14.3 ms: 1.08x faster                                                    |
| deepcopy_reduce         | 2.20 us                                                     | 2.04 us: 1.08x faster                                                    |
| json_loads              | 14.0 us                                                     | 13.0 us: 1.08x faster                                                    |
| sqlglot_normalize       | 205 ms                                                      | 191 ms: 1.07x faster                                                     |
| comprehensions          | 16.5 us                                                     | 15.4 us: 1.07x faster                                                    |
| xml_etree_generate      | 55.5 ms                                                     | 51.8 ms: 1.07x faster                                                    |
| sympy_str               | 194 ms                                                      | 182 ms: 1.07x faster                                                     |
| xml_etree_parse         | 96.8 ms                                                     | 91.3 ms: 1.06x faster                                                    |
| xml_etree_iterparse     | 65.0 ms                                                     | 61.4 ms: 1.06x faster                                                    |
| coroutines              | 16.0 ms                                                     | 15.1 ms: 1.06x faster                                                    |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.58 ms: 1.06x faster                                                    |
| regex_effbot            | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                    |
| deepcopy                | 255 us                                                      | 243 us: 1.05x faster                                                     |
| pathlib                 | 75.7 ms                                                     | 73.2 ms: 1.03x faster                                                    |
| nbody                   | 71.3 ms                                                     | 69.8 ms: 1.02x faster                                                    |
| mdp                     | 1.78 sec                                                    | 1.74 sec: 1.02x faster                                                   |
| pickle                  | 6.85 us                                                     | 6.73 us: 1.02x faster                                                    |
| meteor_contest          | 75.9 ms                                                     | 74.7 ms: 1.02x faster                                                    |
| nqueens                 | 66.6 ms                                                     | 65.6 ms: 1.02x faster                                                    |
| scimark_fft             | 187 ms                                                      | 185 ms: 1.02x faster                                                     |
| pidigits                | 149 ms                                                      | 147 ms: 1.01x faster                                                     |
| unpickle_list           | 2.71 us                                                     | 2.68 us: 1.01x faster                                                    |
| pickle_list             | 2.75 us                                                     | 2.78 us: 1.01x slower                                                    |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                   |
| gc_traversal            | 1.41 ms                                                     | 1.43 ms: 1.01x slower                                                    |
| telco                   | 3.94 ms                                                     | 4.02 ms: 1.02x slower                                                    |
| logging_format          | 6.76 us                                                     | 6.99 us: 1.03x slower                                                    |
| generators              | 32.4 ms                                                     | 34.0 ms: 1.05x slower                                                    |
| logging_simple          | 6.22 us                                                     | 6.67 us: 1.07x slower                                                    |
| pickle_dict             | 17.2 us                                                     | 18.6 us: 1.08x slower                                                    |
| unpack_sequence         | 39.6 ns                                                     | 46.0 ns: 1.16x slower                                                    |
| coverage                | 39.0 ms                                                     | 53.2 ms: 1.36x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.14x faster                                                             |

Benchmark hidden because not significant (5): asyncio_tcp, python_startup_no_site, bench_mp_pool, fannkuch, json
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown