
# Results vs. 3.10.4

- fork: python
- ref: 68a7b78cd5185cbd9456
- machine: windows-amd64
- commit hash: 68a7b78
- commit date: 2024-01-18
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 218 ms: 1.13x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.90 ms: 1.18x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.58 sec: 1.22x faster                                                      |
| tornado_http   | 108 ms                                                      | 88.2 ms: 1.23x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 728 ms: 1.52x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 455 ms: 1.40x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.6 ms: 1.09x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 83.1 ms: 1.17x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.8 ms: 1.25x faster                                                       |
| regex_dna      | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.59 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 176 us: 1.53x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 133 us: 1.38x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.7 ms: 1.18x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.40 us: 1.08x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 92.6 ms: 1.05x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.4 us: 1.04x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.75 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| pickle               | 6.85 us                                                     | 7.30 us: 1.07x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.8 us: 1.09x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.28 us: 1.19x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.2 ms: 1.17x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.66 ms: 1.18x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 74.0 us: 4.54x faster                                                       |
| richards_super           | 52.2 ms                                                     | 30.3 ms: 1.72x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.2 ns: 1.71x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                                       |
| async_tree_none          | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 54.4 ms: 1.58x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 771 us: 1.58x faster                                                        |
| raytrace                 | 273 ms                                                      | 174 ms: 1.57x faster                                                        |
| richards                 | 42.4 ms                                                     | 27.1 ms: 1.57x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.69 ms: 1.56x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 474 ms: 1.54x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| go                       | 139 ms                                                      | 90.4 ms: 1.54x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 176 us: 1.53x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 728 ms: 1.52x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 994 us: 1.48x faster                                                        |
| generators               | 32.4 ms                                                     | 21.9 ms: 1.48x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 455 ms: 1.40x faster                                                        |
| chaos                    | 61.7 ms                                                     | 44.1 ms: 1.40x faster                                                       |
| scimark_sor              | 106 ms                                                      | 76.3 ms: 1.39x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 133 us: 1.38x faster                                                        |
| mypy2                    | 555 ms                                                      | 421 ms: 1.32x faster                                                        |
| pycparser                | 930 ms                                                      | 706 ms: 1.32x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.62 sec: 1.30x faster                                                      |
| deepcopy_memo            | 28.8 us                                                     | 22.4 us: 1.29x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 48.7 ms: 1.29x faster                                                       |
| comprehensions           | 16.5 us                                                     | 12.9 us: 1.28x faster                                                       |
| pyflate                  | 409 ms                                                      | 324 ms: 1.26x faster                                                        |
| regex_compile            | 106 ms                                                      | 84.8 ms: 1.25x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.44 sec: 1.24x faster                                                      |
| tornado_http             | 108 ms                                                      | 88.2 ms: 1.23x faster                                                       |
| sympy_sum                | 107 ms                                                      | 87.9 ms: 1.22x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.58 sec: 1.22x faster                                                      |
| dask                     | 313 ms                                                      | 258 ms: 1.21x faster                                                        |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 47.8 ms: 1.20x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.4 ms: 1.19x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 42.6 ms: 1.18x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.90 ms: 1.18x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.7 ms: 1.18x faster                                                       |
| mako                     | 9.03 ms                                                     | 7.66 ms: 1.18x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.0 ms: 1.18x faster                                                       |
| sympy_str                | 194 ms                                                      | 166 ms: 1.17x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                      |
| hexiom                   | 5.74 ms                                                     | 4.92 ms: 1.17x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 34.6 ms: 1.15x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 517 ms: 1.15x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.07 sec: 1.14x faster                                                      |
| deepcopy                 | 255 us                                                      | 224 us: 1.14x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 181 ms: 1.13x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 845 us: 1.13x faster                                                        |
| regex_dna                | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| sympy_expand             | 314 ms                                                      | 278 ms: 1.13x faster                                                        |
| 2to3                     | 246 ms                                                      | 218 ms: 1.13x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 2.00 us: 1.10x faster                                                       |
| float                    | 61.7 ms                                                     | 56.6 ms: 1.09x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 735 us: 1.09x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.40 us: 1.08x faster                                                       |
| json                     | 3.14 ms                                                     | 2.91 ms: 1.08x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 92.6 ms: 1.05x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.59 ms: 1.05x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.4 us: 1.04x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 64.5 ms: 1.03x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 39.1 ns: 1.01x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.69 us: 1.01x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 76.7 ms: 1.01x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.75 us: 1.01x slower                                                       |
| logging_simple           | 6.22 us                                                     | 6.32 us: 1.02x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 79.1 ms: 1.04x slower                                                       |
| async_generators         | 222 ms                                                      | 232 ms: 1.05x slower                                                        |
| gc_traversal             | 1.41 ms                                                     | 1.48 ms: 1.05x slower                                                       |
| fannkuch                 | 256 ms                                                      | 272 ms: 1.06x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.30 us: 1.07x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 67.2 ms: 1.08x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.8 us: 1.09x slower                                                       |
| spectral_norm            | 77.3 ms                                                     | 85.2 ms: 1.10x slower                                                       |
| scimark_fft              | 187 ms                                                      | 215 ms: 1.15x slower                                                        |
| nbody                    | 71.3 ms                                                     | 83.1 ms: 1.17x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.2 ms: 1.17x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.65 ms: 1.18x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.28 us: 1.19x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.1 ms: 1.21x slower                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.29 ms: 1.21x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                                |

Benchmark hidden because not significant (2): python_startup, xml_etree_generate
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240118-3.13.0a3+-68a7b78-PYTHON_UOPS/bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown