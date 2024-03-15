
# Results vs. 3.10.4

- fork: python
- ref: v3.12.2
- machine: windows-amd64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 214 ms: 1.15x faster                                        |
| chameleon      | 5.79 ms                                                     | 5.14 ms: 1.13x faster                                       |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                      |
| tornado_http   | 108 ms                                                      | 85.8 ms: 1.26x faster                                       |
| Geometric mean | (ref)                                                       | 1.18x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 338 ms: 1.56x faster                                        |
| async_tree_io           | 1.11 sec                                                    | 716 ms: 1.55x faster                                        |
| async_tree_none         | 435 ms                                                      | 289 ms: 1.50x faster                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 478 ms: 1.33x faster                                        |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.1 ms: 1.10x faster                                       |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                        |
| nbody          | 71.3 ms                                                     | 74.3 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 86.2 ms: 1.23x faster                                       |
| regex_dna      | 136 ms                                                      | 121 ms: 1.12x faster                                        |
| regex_v8       | 15.4 ms                                                     | 14.0 ms: 1.10x faster                                       |
| regex_effbot   | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.69 ms: 1.61x faster                                       |
| pickle_pure_python   | 270 us                                                      | 200 us: 1.35x faster                                        |
| unpickle_pure_python | 183 us                                                      | 139 us: 1.32x faster                                        |
| tomli_loads          | 1.67 sec                                                    | 1.41 sec: 1.19x faster                                      |
| xml_etree_process    | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                       |
| unpickle             | 9.09 us                                                     | 8.03 us: 1.13x faster                                       |
| xml_etree_parse      | 96.8 ms                                                     | 89.8 ms: 1.08x faster                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.2 ms: 1.03x faster                                       |
| unpickle_list        | 2.71 us                                                     | 2.65 us: 1.03x faster                                       |
| xml_etree_generate   | 55.5 ms                                                     | 56.3 ms: 1.01x slower                                       |
| pickle_list          | 2.75 us                                                     | 2.85 us: 1.04x slower                                       |
| pickle               | 6.85 us                                                     | 7.29 us: 1.06x slower                                       |
| pickle_dict          | 17.2 us                                                     | 18.9 us: 1.10x slower                                       |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.0 ms: 1.09x faster                                       |
| python_startup_no_site | 15.5 ms                                                     | 15.8 ms: 1.02x slower                                       |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 6.93 ms: 1.30x faster                                       |
| django_template | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                       |
| Geometric mean  | (ref)                                                       | 1.26x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 78.9 us: 4.26x faster                                       |
| deltablue                | 4.19 ms                                                     | 2.15 ms: 1.94x faster                                       |
| richards_super           | 52.2 ms                                                     | 31.0 ms: 1.69x faster                                       |
| json_dumps               | 9.16 ms                                                     | 5.69 ms: 1.61x faster                                       |
| asyncio_tcp              | 732 ms                                                      | 466 ms: 1.57x faster                                        |
| async_tree_memoization   | 526 ms                                                      | 338 ms: 1.56x faster                                        |
| richards                 | 42.4 ms                                                     | 27.4 ms: 1.55x faster                                       |
| async_tree_io            | 1.11 sec                                                    | 716 ms: 1.55x faster                                        |
| go                       | 139 ms                                                      | 90.0 ms: 1.54x faster                                       |
| logging_silent           | 94.6 ns                                                     | 62.6 ns: 1.51x faster                                       |
| async_tree_none          | 435 ms                                                      | 289 ms: 1.50x faster                                        |
| sqlglot_parse            | 1.22 ms                                                     | 830 us: 1.46x faster                                        |
| generators               | 32.4 ms                                                     | 22.3 ms: 1.45x faster                                       |
| scimark_lu               | 85.8 ms                                                     | 60.0 ms: 1.43x faster                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.05 ms: 1.41x faster                                       |
| raytrace                 | 273 ms                                                      | 197 ms: 1.39x faster                                        |
| chaos                    | 61.7 ms                                                     | 44.5 ms: 1.39x faster                                       |
| hexiom                   | 5.74 ms                                                     | 4.18 ms: 1.37x faster                                       |
| pyflate                  | 409 ms                                                      | 299 ms: 1.37x faster                                        |
| pickle_pure_python       | 270 us                                                      | 200 us: 1.35x faster                                        |
| pycparser                | 930 ms                                                      | 690 ms: 1.35x faster                                        |
| mypy2                    | 555 ms                                                      | 412 ms: 1.35x faster                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 478 ms: 1.33x faster                                        |
| crypto_pyaes             | 62.5 ms                                                     | 46.9 ms: 1.33x faster                                       |
| unpickle_pure_python     | 183 us                                                      | 139 us: 1.32x faster                                        |
| mako                     | 9.03 ms                                                     | 6.93 ms: 1.30x faster                                       |
| mdp                      | 1.78 sec                                                    | 1.39 sec: 1.28x faster                                      |
| scimark_sor              | 106 ms                                                      | 83.9 ms: 1.27x faster                                       |
| tornado_http             | 108 ms                                                      | 85.8 ms: 1.26x faster                                       |
| sqlalchemy_imperative    | 11.4 ms                                                     | 9.02 ms: 1.26x faster                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 46.1 ms: 1.24x faster                                       |
| dask                     | 313 ms                                                      | 254 ms: 1.23x faster                                        |
| regex_compile            | 106 ms                                                      | 86.2 ms: 1.23x faster                                       |
| sqlalchemy_declarative   | 103 ms                                                      | 84.7 ms: 1.22x faster                                       |
| dulwich_log              | 50.5 ms                                                     | 41.4 ms: 1.22x faster                                       |
| django_template          | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                       |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                      |
| sympy_sum                | 107 ms                                                      | 89.1 ms: 1.20x faster                                       |
| sympy_integrate          | 15.3 ms                                                     | 12.8 ms: 1.19x faster                                       |
| tomli_loads              | 1.67 sec                                                    | 1.41 sec: 1.19x faster                                      |
| comprehensions           | 16.5 us                                                     | 14.0 us: 1.17x faster                                       |
| aiohttp                  | 995 us                                                      | 851 us: 1.17x faster                                        |
| xml_etree_process        | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                       |
| deepcopy_memo            | 28.8 us                                                     | 24.7 us: 1.16x faster                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 34.3 ms: 1.16x faster                                       |
| 2to3                     | 246 ms                                                      | 214 ms: 1.15x faster                                        |
| spectral_norm            | 77.3 ms                                                     | 67.2 ms: 1.15x faster                                       |
| bench_thread_pool        | 958 us                                                      | 836 us: 1.15x faster                                        |
| sympy_str                | 194 ms                                                      | 171 ms: 1.14x faster                                        |
| coroutines               | 16.0 ms                                                     | 14.1 ms: 1.14x faster                                       |
| sympy_expand             | 314 ms                                                      | 277 ms: 1.14x faster                                        |
| unpickle                 | 9.09 us                                                     | 8.03 us: 1.13x faster                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.08 sec: 1.13x faster                                      |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.88 sec: 1.13x faster                                      |
| chameleon                | 5.79 ms                                                     | 5.14 ms: 1.13x faster                                       |
| regex_dna                | 136 ms                                                      | 121 ms: 1.12x faster                                        |
| sqlglot_normalize        | 205 ms                                                      | 185 ms: 1.11x faster                                        |
| create_gc_cycles         | 800 us                                                      | 721 us: 1.11x faster                                        |
| pprint_safe_repr         | 592 ms                                                      | 534 ms: 1.11x faster                                        |
| regex_v8                 | 15.4 ms                                                     | 14.0 ms: 1.10x faster                                       |
| float                    | 61.7 ms                                                     | 56.1 ms: 1.10x faster                                       |
| python_startup           | 20.6 ms                                                     | 19.0 ms: 1.09x faster                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.51 ms: 1.08x faster                                       |
| deepcopy                 | 255 us                                                      | 236 us: 1.08x faster                                        |
| xml_etree_parse          | 96.8 ms                                                     | 89.8 ms: 1.08x faster                                       |
| sqlite_synth             | 1.91 us                                                     | 1.78 us: 1.07x faster                                       |
| json                     | 3.14 ms                                                     | 2.95 ms: 1.06x faster                                       |
| fannkuch                 | 256 ms                                                      | 242 ms: 1.06x faster                                        |
| meteor_contest           | 75.9 ms                                                     | 72.4 ms: 1.05x faster                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.11 us: 1.05x faster                                       |
| nqueens                  | 66.6 ms                                                     | 63.8 ms: 1.04x faster                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.2 ms: 1.03x faster                                       |
| regex_effbot             | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                       |
| unpickle_list            | 2.71 us                                                     | 2.65 us: 1.03x faster                                       |
| scimark_fft              | 187 ms                                                      | 184 ms: 1.02x faster                                        |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                        |
| logging_format           | 6.76 us                                                     | 6.82 us: 1.01x slower                                       |
| xml_etree_generate       | 55.5 ms                                                     | 56.3 ms: 1.01x slower                                       |
| python_startup_no_site   | 15.5 ms                                                     | 15.8 ms: 1.02x slower                                       |
| coverage                 | 39.0 ms                                                     | 40.0 ms: 1.03x slower                                       |
| logging_simple           | 6.22 us                                                     | 6.41 us: 1.03x slower                                       |
| telco                    | 3.94 ms                                                     | 4.08 ms: 1.04x slower                                       |
| pickle_list              | 2.75 us                                                     | 2.85 us: 1.04x slower                                       |
| nbody                    | 71.3 ms                                                     | 74.3 ms: 1.04x slower                                       |
| async_generators         | 222 ms                                                      | 231 ms: 1.04x slower                                        |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.06x slower                                       |
| bench_mp_pool            | 62.0 ms                                                     | 65.5 ms: 1.06x slower                                       |
| pickle                   | 6.85 us                                                     | 7.29 us: 1.06x slower                                       |
| pickle_dict              | 17.2 us                                                     | 18.9 us: 1.10x slower                                       |
| unpack_sequence          | 39.6 ns                                                     | 46.3 ns: 1.17x slower                                       |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                |

Benchmark hidden because not significant (1): pathlib
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20240206-3.12.2-6abddd9/bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown