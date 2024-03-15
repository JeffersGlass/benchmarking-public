# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-amd64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 222 ms: 1.11x faster                                                      |
| chameleon      | 5.79 ms                                                     | 4.77 ms: 1.21x faster                                                     |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                    |
| tornado_http   | 108 ms                                                      | 84.6 ms: 1.28x faster                                                     |
| Geometric mean | (ref)                                                       | 1.20x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 263 ms: 1.65x faster                                                      |
| async_tree_memoization  | 526 ms                                                      | 338 ms: 1.56x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 725 ms: 1.53x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 451 ms: 1.41x faster                                                      |
| Geometric mean          | (ref)                                                       | 1.54x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 48.7 ms: 1.27x faster                                                     |
| nbody          | 71.3 ms                                                     | 60.2 ms: 1.18x faster                                                     |
| pidigits       | 149 ms                                                      | 151 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                       | 1.14x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 83.6 ms: 1.27x faster                                                     |
| regex_dna      | 136 ms                                                      | 120 ms: 1.13x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                     |
| regex_v8       | 15.4 ms                                                     | 14.8 ms: 1.05x faster                                                     |
| Geometric mean | (ref)                                                       | 1.12x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.43 ms: 1.69x faster                                                     |
| pickle_pure_python   | 270 us                                                      | 178 us: 1.52x faster                                                      |
| tomli_loads          | 1.67 sec                                                    | 1.17 sec: 1.42x faster                                                    |
| unpickle_pure_python | 183 us                                                      | 130 us: 1.41x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.4 ms: 1.22x faster                                                     |
| xml_etree_parse      | 96.8 ms                                                     | 92.2 ms: 1.05x faster                                                     |
| unpickle             | 9.09 us                                                     | 8.69 us: 1.05x faster                                                     |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.3 ms: 1.04x faster                                                     |
| xml_etree_generate   | 55.5 ms                                                     | 53.4 ms: 1.04x faster                                                     |
| json_loads           | 14.0 us                                                     | 13.8 us: 1.02x faster                                                     |
| pickle_dict          | 17.2 us                                                     | 17.7 us: 1.03x slower                                                     |
| unpickle_list        | 2.71 us                                                     | 2.83 us: 1.04x slower                                                     |
| pickle               | 6.85 us                                                     | 7.60 us: 1.11x slower                                                     |
| pickle_list          | 2.75 us                                                     | 3.12 us: 1.14x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 23.8 ms: 1.16x slower                                                     |
| python_startup_no_site | 15.5 ms                                                     | 21.7 ms: 1.40x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.27x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 5.63 ms: 1.60x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 69.9 us: 4.81x faster                                                     |
| deltablue                | 4.19 ms                                                     | 2.05 ms: 2.04x faster                                                     |
| logging_silent           | 94.6 ns                                                     | 54.7 ns: 1.73x faster                                                     |
| json_dumps               | 9.16 ms                                                     | 5.43 ms: 1.69x faster                                                     |
| async_tree_none          | 435 ms                                                      | 263 ms: 1.65x faster                                                      |
| richards_super           | 52.2 ms                                                     | 31.8 ms: 1.64x faster                                                     |
| comprehensions           | 16.5 us                                                     | 10.3 us: 1.61x faster                                                     |
| generators               | 32.4 ms                                                     | 20.2 ms: 1.60x faster                                                     |
| mako                     | 9.03 ms                                                     | 5.63 ms: 1.60x faster                                                     |
| asyncio_tcp              | 732 ms                                                      | 464 ms: 1.58x faster                                                      |
| chaos                    | 61.7 ms                                                     | 39.3 ms: 1.57x faster                                                     |
| sqlglot_parse            | 1.22 ms                                                     | 778 us: 1.56x faster                                                      |
| async_tree_memoization   | 526 ms                                                      | 338 ms: 1.56x faster                                                      |
| async_tree_io            | 1.11 sec                                                    | 725 ms: 1.53x faster                                                      |
| raytrace                 | 273 ms                                                      | 179 ms: 1.53x faster                                                      |
| pickle_pure_python       | 270 us                                                      | 178 us: 1.52x faster                                                      |
| spectral_norm            | 77.3 ms                                                     | 51.1 ms: 1.51x faster                                                     |
| richards                 | 42.4 ms                                                     | 28.5 ms: 1.49x faster                                                     |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.47x faster                                                     |
| crypto_pyaes             | 62.5 ms                                                     | 43.5 ms: 1.44x faster                                                     |
| go                       | 139 ms                                                      | 96.8 ms: 1.44x faster                                                     |
| pyflate                  | 409 ms                                                      | 287 ms: 1.43x faster                                                      |
| tomli_loads              | 1.67 sec                                                    | 1.17 sec: 1.42x faster                                                    |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 451 ms: 1.41x faster                                                      |
| unpickle_pure_python     | 183 us                                                      | 130 us: 1.41x faster                                                      |
| scimark_monte_carlo      | 57.3 ms                                                     | 41.5 ms: 1.38x faster                                                     |
| pycparser                | 930 ms                                                      | 696 ms: 1.34x faster                                                      |
| hexiom                   | 5.74 ms                                                     | 4.39 ms: 1.31x faster                                                     |
| deepcopy_memo            | 28.8 us                                                     | 22.1 us: 1.30x faster                                                     |
| tornado_http             | 108 ms                                                      | 84.6 ms: 1.28x faster                                                     |
| mypy2                    | 555 ms                                                      | 436 ms: 1.27x faster                                                      |
| regex_compile            | 106 ms                                                      | 83.6 ms: 1.27x faster                                                     |
| float                    | 61.7 ms                                                     | 48.7 ms: 1.27x faster                                                     |
| pprint_pformat           | 1.22 sec                                                    | 969 ms: 1.26x faster                                                      |
| scimark_sor              | 106 ms                                                      | 84.6 ms: 1.25x faster                                                     |
| pprint_safe_repr         | 592 ms                                                      | 475 ms: 1.25x faster                                                      |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.69 sec: 1.25x faster                                                    |
| sympy_sum                | 107 ms                                                      | 86.6 ms: 1.23x faster                                                     |
| dulwich_log              | 50.5 ms                                                     | 41.3 ms: 1.22x faster                                                     |
| xml_etree_process        | 44.5 ms                                                     | 36.4 ms: 1.22x faster                                                     |
| chameleon                | 5.79 ms                                                     | 4.77 ms: 1.21x faster                                                     |
| coroutines               | 16.0 ms                                                     | 13.2 ms: 1.21x faster                                                     |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                     |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                    |
| sympy_str                | 194 ms                                                      | 163 ms: 1.19x faster                                                      |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.29 ms: 1.19x faster                                                     |
| nbody                    | 71.3 ms                                                     | 60.2 ms: 1.18x faster                                                     |
| scimark_lu               | 85.8 ms                                                     | 73.0 ms: 1.18x faster                                                     |
| mdp                      | 1.78 sec                                                    | 1.52 sec: 1.17x faster                                                    |
| sympy_integrate          | 15.3 ms                                                     | 13.0 ms: 1.17x faster                                                     |
| sqlglot_normalize        | 205 ms                                                      | 177 ms: 1.16x faster                                                      |
| fannkuch                 | 256 ms                                                      | 221 ms: 1.16x faster                                                      |
| sqlglot_optimize         | 39.8 ms                                                     | 34.8 ms: 1.14x faster                                                     |
| deepcopy                 | 255 us                                                      | 224 us: 1.14x faster                                                      |
| regex_dna                | 136 ms                                                      | 120 ms: 1.13x faster                                                      |
| bench_thread_pool        | 958 us                                                      | 845 us: 1.13x faster                                                      |
| deepcopy_reduce          | 2.20 us                                                     | 1.95 us: 1.13x faster                                                     |
| sympy_expand             | 314 ms                                                      | 280 ms: 1.12x faster                                                      |
| scimark_fft              | 187 ms                                                      | 169 ms: 1.11x faster                                                      |
| 2to3                     | 246 ms                                                      | 222 ms: 1.11x faster                                                      |
| nqueens                  | 66.6 ms                                                     | 61.3 ms: 1.09x faster                                                     |
| logging_format           | 6.76 us                                                     | 6.24 us: 1.08x faster                                                     |
| create_gc_cycles         | 800 us                                                      | 738 us: 1.08x faster                                                      |
| logging_simple           | 6.22 us                                                     | 5.80 us: 1.07x faster                                                     |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                     |
| meteor_contest           | 75.9 ms                                                     | 72.2 ms: 1.05x faster                                                     |
| xml_etree_parse          | 96.8 ms                                                     | 92.2 ms: 1.05x faster                                                     |
| regex_v8                 | 15.4 ms                                                     | 14.8 ms: 1.05x faster                                                     |
| unpickle                 | 9.09 us                                                     | 8.69 us: 1.05x faster                                                     |
| xml_etree_iterparse      | 65.0 ms                                                     | 62.3 ms: 1.04x faster                                                     |
| xml_etree_generate       | 55.5 ms                                                     | 53.4 ms: 1.04x faster                                                     |
| json                     | 3.14 ms                                                     | 3.03 ms: 1.04x faster                                                     |
| json_loads               | 14.0 us                                                     | 13.8 us: 1.02x faster                                                     |
| pidigits                 | 149 ms                                                      | 151 ms: 1.01x slower                                                      |
| pickle_dict              | 17.2 us                                                     | 17.7 us: 1.03x slower                                                     |
| unpickle_list            | 2.71 us                                                     | 2.83 us: 1.04x slower                                                     |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                     |
| async_generators         | 222 ms                                                      | 240 ms: 1.08x slower                                                      |
| pickle                   | 6.85 us                                                     | 7.60 us: 1.11x slower                                                     |
| bench_mp_pool            | 62.0 ms                                                     | 69.8 ms: 1.13x slower                                                     |
| pickle_list              | 2.75 us                                                     | 3.12 us: 1.14x slower                                                     |
| unpack_sequence          | 39.6 ns                                                     | 45.2 ns: 1.14x slower                                                     |
| python_startup           | 20.6 ms                                                     | 23.8 ms: 1.16x slower                                                     |
| telco                    | 3.94 ms                                                     | 4.57 ms: 1.16x slower                                                     |
| coverage                 | 39.0 ms                                                     | 45.7 ms: 1.17x slower                                                     |
| python_startup_no_site   | 15.5 ms                                                     | 21.7 ms: 1.40x slower                                                     |
| Geometric mean           | (ref)                                                       | 1.23x faster                                                              |

Benchmark hidden because not significant (1): pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-594cca3-JIT/bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: unknown