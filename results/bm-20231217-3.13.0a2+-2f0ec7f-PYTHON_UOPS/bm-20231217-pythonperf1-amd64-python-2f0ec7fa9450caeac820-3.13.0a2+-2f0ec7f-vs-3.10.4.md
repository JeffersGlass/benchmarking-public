
# Results vs. 3.10.4

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: windows-amd64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 217 ms: 1.13x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.01 ms: 1.15x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                      |
| tornado_http   | 108 ms                                                      | 87.5 ms: 1.24x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 269 ms: 1.62x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 340 ms: 1.55x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 455 ms: 1.40x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 58.1 ms: 1.06x faster                                                       |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                                        |
| nbody          | 71.3 ms                                                     | 82.6 ms: 1.16x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.8 ms: 1.25x faster                                                       |
| regex_dna      | 136 ms                                                      | 117 ms: 1.17x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.58 ms: 1.64x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 180 us: 1.50x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 135 us: 1.36x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.3 ms: 1.19x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.48 sec: 1.13x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.28 us: 1.10x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.56 us: 1.06x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.3 us: 1.05x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 94.0 ms: 1.03x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 54.9 ms: 1.01x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 66.5 ms: 1.02x slower                                                       |
| pickle               | 6.85 us                                                     | 7.30 us: 1.07x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.36 us: 1.22x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.4 ms: 1.01x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 18.2 ms: 1.18x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.67 ms: 1.18x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 75.4 us: 4.46x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.3 ns: 1.71x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.0 ms: 1.69x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.58 ms: 1.64x faster                                                       |
| async_tree_none          | 435 ms                                                      | 269 ms: 1.62x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 464 ms: 1.58x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 773 us: 1.57x faster                                                        |
| raytrace                 | 273 ms                                                      | 175 ms: 1.56x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 340 ms: 1.55x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 55.9 ms: 1.54x faster                                                       |
| richards                 | 42.4 ms                                                     | 27.9 ms: 1.52x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| deltablue                | 4.19 ms                                                     | 2.77 ms: 1.51x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 180 us: 1.50x faster                                                        |
| go                       | 139 ms                                                      | 93.0 ms: 1.49x faster                                                       |
| generators               | 32.4 ms                                                     | 22.0 ms: 1.47x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.00 ms: 1.47x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 455 ms: 1.40x faster                                                        |
| chaos                    | 61.7 ms                                                     | 45.2 ms: 1.37x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 135 us: 1.36x faster                                                        |
| pycparser                | 930 ms                                                      | 693 ms: 1.34x faster                                                        |
| mypy2                    | 555 ms                                                      | 420 ms: 1.32x faster                                                        |
| scimark_sor              | 106 ms                                                      | 81.1 ms: 1.31x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.65 sec: 1.28x faster                                                      |
| crypto_pyaes             | 62.5 ms                                                     | 48.9 ms: 1.28x faster                                                       |
| pyflate                  | 409 ms                                                      | 323 ms: 1.27x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 22.9 us: 1.26x faster                                                       |
| regex_compile            | 106 ms                                                      | 84.8 ms: 1.25x faster                                                       |
| comprehensions           | 16.5 us                                                     | 13.3 us: 1.24x faster                                                       |
| coroutines               | 16.0 ms                                                     | 12.9 ms: 1.24x faster                                                       |
| tornado_http             | 108 ms                                                      | 87.5 ms: 1.24x faster                                                       |
| sympy_sum                | 107 ms                                                      | 87.0 ms: 1.23x faster                                                       |
| dask                     | 313 ms                                                      | 255 ms: 1.23x faster                                                        |
| docutils                 | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                      |
| sqlite_synth             | 1.91 us                                                     | 1.57 us: 1.22x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.3 ms: 1.19x faster                                                       |
| mako                     | 9.03 ms                                                     | 7.67 ms: 1.18x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 42.9 ms: 1.18x faster                                                       |
| regex_dna                | 136 ms                                                      | 117 ms: 1.17x faster                                                        |
| sympy_str                | 194 ms                                                      | 167 ms: 1.16x faster                                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.2 ms: 1.16x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.53 sec: 1.16x faster                                                      |
| scimark_monte_carlo      | 57.3 ms                                                     | 49.5 ms: 1.16x faster                                                       |
| chameleon                | 5.79 ms                                                     | 5.01 ms: 1.15x faster                                                       |
| sympy_expand             | 314 ms                                                      | 277 ms: 1.14x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 5.07 ms: 1.13x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.48 sec: 1.13x faster                                                      |
| 2to3                     | 246 ms                                                      | 217 ms: 1.13x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 35.4 ms: 1.13x faster                                                       |
| deepcopy                 | 255 us                                                      | 227 us: 1.12x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.09 sec: 1.12x faster                                                      |
| bench_thread_pool        | 958 us                                                      | 855 us: 1.12x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 531 ms: 1.11x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 185 ms: 1.11x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.99 us: 1.11x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 728 us: 1.10x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.28 us: 1.10x faster                                                       |
| float                    | 61.7 ms                                                     | 58.1 ms: 1.06x faster                                                       |
| unpickle_list            | 2.71 us                                                     | 2.56 us: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.3 us: 1.05x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| json                     | 3.14 ms                                                     | 2.99 ms: 1.05x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 94.0 ms: 1.03x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 65.9 ms: 1.01x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.68 us: 1.01x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 54.9 ms: 1.01x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.4 ms: 1.01x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 76.3 ms: 1.00x slower                                                       |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                                        |
| unpack_sequence          | 39.6 ns                                                     | 40.3 ns: 1.02x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 66.5 ms: 1.02x slower                                                       |
| async_generators         | 222 ms                                                      | 229 ms: 1.04x slower                                                        |
| pathlib                  | 75.7 ms                                                     | 79.1 ms: 1.05x slower                                                       |
| fannkuch                 | 256 ms                                                      | 268 ms: 1.05x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.30 us: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 66.7 ms: 1.08x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| spectral_norm            | 77.3 ms                                                     | 85.0 ms: 1.10x slower                                                       |
| scimark_fft              | 187 ms                                                      | 210 ms: 1.12x slower                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.12 ms: 1.15x slower                                                       |
| coverage                 | 39.0 ms                                                     | 44.7 ms: 1.15x slower                                                       |
| nbody                    | 71.3 ms                                                     | 82.6 ms: 1.16x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.2 ms: 1.18x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.72 ms: 1.20x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.36 us: 1.22x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.18x faster                                                                |

Benchmark hidden because not significant (1): logging_simple
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown