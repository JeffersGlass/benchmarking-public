# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_nops
- machine: windows-amd64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 226 ms: 1.09x faster                                                     |
| chameleon      | 5.79 ms                                                     | 4.76 ms: 1.21x faster                                                    |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                   |
| html5lib       | 51.0 ms                                                     | 36.1 ms: 1.41x faster                                                    |
| tornado_http   | 108 ms                                                      | 84.8 ms: 1.28x faster                                                    |
| Geometric mean | (ref)                                                       | 1.24x faster                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 276 ms: 1.58x faster                                                     |
| async_tree_memoization  | 526 ms                                                      | 349 ms: 1.51x faster                                                     |
| async_tree_io           | 1.11 sec                                                    | 736 ms: 1.51x faster                                                     |
| async_tree_cpu_io_mixed | 638 ms                                                      | 460 ms: 1.39x faster                                                     |
| Geometric mean          | (ref)                                                       | 1.49x faster                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 49.5 ms: 1.25x faster                                                    |
| nbody          | 71.3 ms                                                     | 59.5 ms: 1.20x faster                                                    |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                                     |
| Geometric mean | (ref)                                                       | 1.14x faster                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 82.2 ms: 1.29x faster                                                    |
| regex_dna      | 136 ms                                                      | 121 ms: 1.12x faster                                                     |
| regex_v8       | 15.4 ms                                                     | 14.5 ms: 1.06x faster                                                    |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                    |
| Geometric mean | (ref)                                                       | 1.13x faster                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                    |
| pickle_pure_python   | 270 us                                                      | 176 us: 1.53x faster                                                     |
| unpickle_pure_python | 183 us                                                      | 130 us: 1.41x faster                                                     |
| tomli_loads          | 1.67 sec                                                    | 1.20 sec: 1.39x faster                                                   |
| xml_etree_process    | 44.5 ms                                                     | 36.3 ms: 1.23x faster                                                    |
| unpickle             | 9.09 us                                                     | 8.47 us: 1.07x faster                                                    |
| xml_etree_generate   | 55.5 ms                                                     | 53.3 ms: 1.04x faster                                                    |
| xml_etree_parse      | 96.8 ms                                                     | 93.6 ms: 1.03x faster                                                    |
| xml_etree_iterparse  | 65.0 ms                                                     | 64.1 ms: 1.01x faster                                                    |
| json_loads           | 14.0 us                                                     | 13.9 us: 1.01x faster                                                    |
| unpickle_list        | 2.71 us                                                     | 2.77 us: 1.02x slower                                                    |
| pickle_list          | 2.75 us                                                     | 2.84 us: 1.03x slower                                                    |
| pickle_dict          | 17.2 us                                                     | 17.7 us: 1.03x slower                                                    |
| pickle               | 6.85 us                                                     | 7.42 us: 1.08x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 24.1 ms: 1.17x slower                                                    |
| python_startup_no_site | 15.5 ms                                                     | 21.9 ms: 1.41x slower                                                    |
| Geometric mean         | (ref)                                                       | 1.28x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 5.78 ms: 1.56x faster                                                    |
| django_template | 28.9 ms                                                     | 21.6 ms: 1.34x faster                                                    |
| genshi_text     | 19.8 ms                                                     | 15.5 ms: 1.28x faster                                                    |
| genshi_xml      | 41.0 ms                                                     | 34.7 ms: 1.18x faster                                                    |
| Geometric mean  | (ref)                                                       | 1.33x faster                                                             |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 69.2 us: 4.86x faster                                                    |
| deltablue                | 4.19 ms                                                     | 2.04 ms: 2.05x faster                                                    |
| logging_silent           | 94.6 ns                                                     | 55.2 ns: 1.72x faster                                                    |
| pylint                   | 350 ms                                                      | 210 ms: 1.67x faster                                                     |
| richards_super           | 52.2 ms                                                     | 31.3 ms: 1.67x faster                                                    |
| json_dumps               | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                    |
| sqlglot_parse            | 1.22 ms                                                     | 767 us: 1.58x faster                                                     |
| comprehensions           | 16.5 us                                                     | 10.4 us: 1.58x faster                                                    |
| async_tree_none          | 435 ms                                                      | 276 ms: 1.58x faster                                                     |
| asyncio_tcp              | 732 ms                                                      | 465 ms: 1.58x faster                                                     |
| mako                     | 9.03 ms                                                     | 5.78 ms: 1.56x faster                                                    |
| generators               | 32.4 ms                                                     | 20.8 ms: 1.55x faster                                                    |
| chaos                    | 61.7 ms                                                     | 39.9 ms: 1.55x faster                                                    |
| raytrace                 | 273 ms                                                      | 178 ms: 1.53x faster                                                     |
| pickle_pure_python       | 270 us                                                      | 176 us: 1.53x faster                                                     |
| richards                 | 42.4 ms                                                     | 28.0 ms: 1.52x faster                                                    |
| async_tree_memoization   | 526 ms                                                      | 349 ms: 1.51x faster                                                     |
| async_tree_io            | 1.11 sec                                                    | 736 ms: 1.51x faster                                                     |
| sqlglot_transpile        | 1.48 ms                                                     | 988 us: 1.49x faster                                                     |
| spectral_norm            | 77.3 ms                                                     | 51.9 ms: 1.49x faster                                                    |
| crypto_pyaes             | 62.5 ms                                                     | 42.8 ms: 1.46x faster                                                    |
| go                       | 139 ms                                                      | 95.4 ms: 1.46x faster                                                    |
| pyflate                  | 409 ms                                                      | 284 ms: 1.44x faster                                                     |
| html5lib                 | 51.0 ms                                                     | 36.1 ms: 1.41x faster                                                    |
| unpickle_pure_python     | 183 us                                                      | 130 us: 1.41x faster                                                     |
| tomli_loads              | 1.67 sec                                                    | 1.20 sec: 1.39x faster                                                   |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 460 ms: 1.39x faster                                                     |
| django_template          | 28.9 ms                                                     | 21.6 ms: 1.34x faster                                                    |
| pycparser                | 930 ms                                                      | 697 ms: 1.33x faster                                                     |
| scimark_monte_carlo      | 57.3 ms                                                     | 43.0 ms: 1.33x faster                                                    |
| scimark_sor              | 106 ms                                                      | 81.7 ms: 1.30x faster                                                    |
| hexiom                   | 5.74 ms                                                     | 4.43 ms: 1.30x faster                                                    |
| regex_compile            | 106 ms                                                      | 82.2 ms: 1.29x faster                                                    |
| deepcopy_memo            | 28.8 us                                                     | 22.3 us: 1.29x faster                                                    |
| tornado_http             | 108 ms                                                      | 84.8 ms: 1.28x faster                                                    |
| mypy2                    | 555 ms                                                      | 435 ms: 1.28x faster                                                     |
| genshi_text              | 19.8 ms                                                     | 15.5 ms: 1.28x faster                                                    |
| float                    | 61.7 ms                                                     | 49.5 ms: 1.25x faster                                                    |
| sympy_sum                | 107 ms                                                      | 86.2 ms: 1.24x faster                                                    |
| pprint_pformat           | 1.22 sec                                                    | 988 ms: 1.23x faster                                                     |
| xml_etree_process        | 44.5 ms                                                     | 36.3 ms: 1.23x faster                                                    |
| dulwich_log              | 50.5 ms                                                     | 41.2 ms: 1.22x faster                                                    |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.22x faster                                                    |
| chameleon                | 5.79 ms                                                     | 4.76 ms: 1.21x faster                                                    |
| docutils                 | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                   |
| pprint_safe_repr         | 592 ms                                                      | 491 ms: 1.21x faster                                                     |
| coroutines               | 16.0 ms                                                     | 13.3 ms: 1.20x faster                                                    |
| nbody                    | 71.3 ms                                                     | 59.5 ms: 1.20x faster                                                    |
| sympy_str                | 194 ms                                                      | 163 ms: 1.20x faster                                                     |
| genshi_xml               | 41.0 ms                                                     | 34.7 ms: 1.18x faster                                                    |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.31 ms: 1.18x faster                                                    |
| scimark_lu               | 85.8 ms                                                     | 72.8 ms: 1.18x faster                                                    |
| sqlglot_normalize        | 205 ms                                                      | 175 ms: 1.17x faster                                                     |
| sympy_integrate          | 15.3 ms                                                     | 13.1 ms: 1.17x faster                                                    |
| fannkuch                 | 256 ms                                                      | 221 ms: 1.16x faster                                                     |
| sqlglot_optimize         | 39.8 ms                                                     | 34.4 ms: 1.16x faster                                                    |
| mdp                      | 1.78 sec                                                    | 1.54 sec: 1.16x faster                                                   |
| deepcopy                 | 255 us                                                      | 222 us: 1.15x faster                                                     |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.84 sec: 1.15x faster                                                   |
| bench_thread_pool        | 958 us                                                      | 838 us: 1.14x faster                                                     |
| deepcopy_reduce          | 2.20 us                                                     | 1.93 us: 1.14x faster                                                    |
| sympy_expand             | 314 ms                                                      | 278 ms: 1.13x faster                                                     |
| regex_dna                | 136 ms                                                      | 121 ms: 1.12x faster                                                     |
| aiohttp                  | 995 us                                                      | 904 us: 1.10x faster                                                     |
| 2to3                     | 246 ms                                                      | 226 ms: 1.09x faster                                                     |
| scimark_fft              | 187 ms                                                      | 173 ms: 1.08x faster                                                     |
| logging_format           | 6.76 us                                                     | 6.29 us: 1.07x faster                                                    |
| unpickle                 | 9.09 us                                                     | 8.47 us: 1.07x faster                                                    |
| create_gc_cycles         | 800 us                                                      | 749 us: 1.07x faster                                                     |
| nqueens                  | 66.6 ms                                                     | 62.7 ms: 1.06x faster                                                    |
| regex_v8                 | 15.4 ms                                                     | 14.5 ms: 1.06x faster                                                    |
| logging_simple           | 6.22 us                                                     | 5.86 us: 1.06x faster                                                    |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                    |
| xml_etree_generate       | 55.5 ms                                                     | 53.3 ms: 1.04x faster                                                    |
| meteor_contest           | 75.9 ms                                                     | 72.9 ms: 1.04x faster                                                    |
| xml_etree_parse          | 96.8 ms                                                     | 93.6 ms: 1.03x faster                                                    |
| xml_etree_iterparse      | 65.0 ms                                                     | 64.1 ms: 1.01x faster                                                    |
| json_loads               | 14.0 us                                                     | 13.9 us: 1.01x faster                                                    |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                                     |
| unpickle_list            | 2.71 us                                                     | 2.77 us: 1.02x slower                                                    |
| pickle_list              | 2.75 us                                                     | 2.84 us: 1.03x slower                                                    |
| pickle_dict              | 17.2 us                                                     | 17.7 us: 1.03x slower                                                    |
| gc_traversal             | 1.41 ms                                                     | 1.50 ms: 1.06x slower                                                    |
| async_generators         | 222 ms                                                      | 240 ms: 1.08x slower                                                     |
| pickle                   | 6.85 us                                                     | 7.42 us: 1.08x slower                                                    |
| unpack_sequence          | 39.6 ns                                                     | 43.8 ns: 1.10x slower                                                    |
| bench_mp_pool            | 62.0 ms                                                     | 70.3 ms: 1.13x slower                                                    |
| dask                     | 313 ms                                                      | 362 ms: 1.16x slower                                                     |
| python_startup           | 20.6 ms                                                     | 24.1 ms: 1.17x slower                                                    |
| telco                    | 3.94 ms                                                     | 4.74 ms: 1.20x slower                                                    |
| coverage                 | 39.0 ms                                                     | 47.6 ms: 1.22x slower                                                    |
| python_startup_no_site   | 15.5 ms                                                     | 21.9 ms: 1.41x slower                                                    |
| thrift                   | 617 us                                                      | 8.88 ms: 14.38x slower                                                   |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                             |

Benchmark hidden because not significant (2): pathlib, json
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown