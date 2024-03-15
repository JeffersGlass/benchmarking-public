
# Results vs. 3.10.4

- fork: python
- ref: 5a7e1e0a92622c605ab2
- machine: windows-amd64
- commit hash: 5a7e1e0
- commit date: 2022-07-11
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 206 ms: 1.19x faster                                                       |
| chameleon      | 5.79 ms                                                     | 5.14 ms: 1.13x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.58 sec: 1.22x faster                                                     |
| html5lib       | 51.0 ms                                                     | 38.9 ms: 1.31x faster                                                      |
| tornado_http   | 108 ms                                                      | 91.9 ms: 1.18x faster                                                      |
| Geometric mean | (ref)                                                       | 1.20x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 753 ms: 1.47x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 375 ms: 1.40x faster                                                       |
| async_tree_none         | 435 ms                                                      | 317 ms: 1.37x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 508 ms: 1.26x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.37x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.9 ms: 1.15x faster                                                      |
| nbody          | 71.3 ms                                                     | 68.7 ms: 1.04x faster                                                      |
| pidigits       | 149 ms                                                      | 146 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 114 ms: 1.19x faster                                                       |
| regex_compile  | 106 ms                                                      | 90.8 ms: 1.17x faster                                                      |
| regex_v8       | 15.4 ms                                                     | 13.4 ms: 1.15x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.70 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                       | 1.12x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 204 us: 1.32x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 152 us: 1.21x faster                                                       |
| json_dumps           | 9.16 ms                                                     | 7.78 ms: 1.18x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 37.8 ms: 1.18x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.32 us: 1.09x faster                                                      |
| pickle               | 6.85 us                                                     | 6.48 us: 1.06x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 53.4 ms: 1.04x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.65 us: 1.04x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.7 ms: 1.04x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 95.1 ms: 1.02x faster                                                      |
| unpickle_list        | 2.71 us                                                     | 2.80 us: 1.03x slower                                                      |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.08x faster                                                               |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                      |
| python_startup_no_site | 15.5 ms                                                     | 15.4 ms: 1.01x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.23 ms: 1.25x faster                                                      |
| django_template | 28.9 ms                                                     | 25.0 ms: 1.16x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 17.6 ms: 1.13x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 38.6 ms: 1.06x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.15x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.66 ms: 1.57x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 753 ms: 1.47x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 375 ms: 1.40x faster                                                       |
| go                      | 139 ms                                                      | 99.5 ms: 1.40x faster                                                      |
| async_tree_none         | 435 ms                                                      | 317 ms: 1.37x faster                                                       |
| scimark_lu              | 85.8 ms                                                     | 62.7 ms: 1.37x faster                                                      |
| scimark_sor             | 106 ms                                                      | 78.5 ms: 1.35x faster                                                      |
| raytrace                | 273 ms                                                      | 204 ms: 1.34x faster                                                       |
| pyflate                 | 409 ms                                                      | 306 ms: 1.34x faster                                                       |
| richards                | 42.4 ms                                                     | 31.7 ms: 1.34x faster                                                      |
| pickle_pure_python      | 270 us                                                      | 204 us: 1.32x faster                                                       |
| pycparser               | 930 ms                                                      | 706 ms: 1.32x faster                                                       |
| html5lib                | 51.0 ms                                                     | 38.9 ms: 1.31x faster                                                      |
| logging_silent          | 94.6 ns                                                     | 72.4 ns: 1.31x faster                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.13 ms: 1.31x faster                                                      |
| sqlglot_parse           | 1.22 ms                                                     | 936 us: 1.30x faster                                                       |
| scimark_monte_carlo     | 57.3 ms                                                     | 44.3 ms: 1.29x faster                                                      |
| chaos                   | 61.7 ms                                                     | 48.7 ms: 1.27x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 508 ms: 1.26x faster                                                       |
| mako                    | 9.03 ms                                                     | 7.23 ms: 1.25x faster                                                      |
| async_generators        | 222 ms                                                      | 178 ms: 1.25x faster                                                       |
| hexiom                  | 5.74 ms                                                     | 4.61 ms: 1.25x faster                                                      |
| crypto_pyaes            | 62.5 ms                                                     | 50.6 ms: 1.24x faster                                                      |
| sqlalchemy_declarative  | 103 ms                                                      | 84.7 ms: 1.22x faster                                                      |
| docutils                | 1.92 sec                                                    | 1.58 sec: 1.22x faster                                                     |
| unpickle_pure_python    | 183 us                                                      | 152 us: 1.21x faster                                                       |
| create_gc_cycles        | 800 us                                                      | 664 us: 1.20x faster                                                       |
| 2to3                    | 246 ms                                                      | 206 ms: 1.19x faster                                                       |
| thrift                  | 617 us                                                      | 518 us: 1.19x faster                                                       |
| regex_dna               | 136 ms                                                      | 114 ms: 1.19x faster                                                       |
| tornado_http            | 108 ms                                                      | 91.9 ms: 1.18x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 7.78 ms: 1.18x faster                                                      |
| xml_etree_process       | 44.5 ms                                                     | 37.8 ms: 1.18x faster                                                      |
| regex_compile           | 106 ms                                                      | 90.8 ms: 1.17x faster                                                      |
| dask                    | 313 ms                                                      | 270 ms: 1.16x faster                                                       |
| aiohttp                 | 995 us                                                      | 860 us: 1.16x faster                                                       |
| django_template         | 28.9 ms                                                     | 25.0 ms: 1.16x faster                                                      |
| regex_v8                | 15.4 ms                                                     | 13.4 ms: 1.15x faster                                                      |
| pprint_safe_repr        | 592 ms                                                      | 515 ms: 1.15x faster                                                       |
| float                   | 61.7 ms                                                     | 53.9 ms: 1.15x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 34.8 ms: 1.14x faster                                                      |
| pprint_pformat          | 1.22 sec                                                    | 1.07 sec: 1.14x faster                                                     |
| dulwich_log             | 50.5 ms                                                     | 44.2 ms: 1.14x faster                                                      |
| deepcopy_memo           | 28.8 us                                                     | 25.3 us: 1.14x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.70 us: 1.13x faster                                                      |
| chameleon               | 5.79 ms                                                     | 5.14 ms: 1.13x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 17.6 ms: 1.13x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                                      |
| sympy_sum               | 107 ms                                                      | 95.8 ms: 1.12x faster                                                      |
| bench_thread_pool       | 958 us                                                      | 858 us: 1.12x faster                                                       |
| sympy_integrate         | 15.3 ms                                                     | 13.7 ms: 1.12x faster                                                      |
| pylint                  | 350 ms                                                      | 318 ms: 1.10x faster                                                       |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.4 ms: 1.10x faster                                                      |
| unpickle                | 9.09 us                                                     | 8.32 us: 1.09x faster                                                      |
| asyncio_tcp             | 732 ms                                                      | 675 ms: 1.08x faster                                                       |
| coroutines              | 16.0 ms                                                     | 14.8 ms: 1.08x faster                                                      |
| sympy_expand            | 314 ms                                                      | 291 ms: 1.08x faster                                                       |
| sqlglot_normalize       | 205 ms                                                      | 192 ms: 1.07x faster                                                       |
| sympy_str               | 194 ms                                                      | 182 ms: 1.07x faster                                                       |
| mdp                     | 1.78 sec                                                    | 1.67 sec: 1.07x faster                                                     |
| genshi_xml              | 41.0 ms                                                     | 38.6 ms: 1.06x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.48 us: 1.06x faster                                                      |
| spectral_norm           | 77.3 ms                                                     | 73.7 ms: 1.05x faster                                                      |
| comprehensions          | 16.5 us                                                     | 15.7 us: 1.05x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 72.4 ms: 1.05x faster                                                      |
| deepcopy                | 255 us                                                      | 246 us: 1.04x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 53.4 ms: 1.04x faster                                                      |
| nbody                   | 71.3 ms                                                     | 68.7 ms: 1.04x faster                                                      |
| pickle_list             | 2.75 us                                                     | 2.65 us: 1.04x faster                                                      |
| xml_etree_iterparse     | 65.0 ms                                                     | 62.7 ms: 1.04x faster                                                      |
| deepcopy_reduce         | 2.20 us                                                     | 2.14 us: 1.03x faster                                                      |
| pidigits                | 149 ms                                                      | 146 ms: 1.02x faster                                                       |
| fannkuch                | 256 ms                                                      | 251 ms: 1.02x faster                                                       |
| xml_etree_parse         | 96.8 ms                                                     | 95.1 ms: 1.02x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 74.8 ms: 1.02x faster                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.68 ms: 1.02x faster                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 61.4 ms: 1.01x faster                                                      |
| python_startup_no_site  | 15.5 ms                                                     | 15.4 ms: 1.01x faster                                                      |
| scimark_fft             | 187 ms                                                      | 186 ms: 1.01x faster                                                       |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| nqueens                 | 66.6 ms                                                     | 67.6 ms: 1.01x slower                                                      |
| telco                   | 3.94 ms                                                     | 4.02 ms: 1.02x slower                                                      |
| regex_effbot            | 1.66 ms                                                     | 1.70 ms: 1.03x slower                                                      |
| unpickle_list           | 2.71 us                                                     | 2.80 us: 1.03x slower                                                      |
| generators              | 32.4 ms                                                     | 33.9 ms: 1.05x slower                                                      |
| logging_format          | 6.76 us                                                     | 7.19 us: 1.06x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 18.4 us: 1.07x slower                                                      |
| logging_simple          | 6.22 us                                                     | 6.68 us: 1.07x slower                                                      |
| unpack_sequence         | 39.6 ns                                                     | 45.4 ns: 1.14x slower                                                      |
| coverage                | 39.0 ms                                                     | 54.1 ms: 1.39x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.13x faster                                                               |

Benchmark hidden because not significant (3): gc_traversal, json_loads, json
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown