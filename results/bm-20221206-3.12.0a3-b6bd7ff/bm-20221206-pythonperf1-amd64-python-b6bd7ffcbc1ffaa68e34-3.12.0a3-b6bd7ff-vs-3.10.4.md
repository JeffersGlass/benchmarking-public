
# Results vs. 3.10.4

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: windows-amd64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.22x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 196 ms: 1.26x faster                                                       |
| chameleon      | 5.79 ms                                                     | 4.53 ms: 1.28x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                     |
| html5lib       | 51.0 ms                                                     | 35.0 ms: 1.46x faster                                                      |
| Geometric mean | (ref)                                                       | 1.30x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 780 ms: 1.42x faster                                                       |
| async_tree_none         | 435 ms                                                      | 317 ms: 1.37x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 388 ms: 1.35x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 501 ms: 1.27x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.35x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.1 ms: 1.23x faster                                                      |
| nbody          | 71.3 ms                                                     | 62.3 ms: 1.14x faster                                                      |
| pidigits       | 149 ms                                                      | 151 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 82.5 ms: 1.29x faster                                                      |
| regex_dna      | 136 ms                                                      | 120 ms: 1.14x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.0 ms: 1.10x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.54 ms: 1.07x faster                                                      |
| Geometric mean | (ref)                                                       | 1.15x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.17 ms: 1.77x faster                                                      |
| unpickle_pure_python | 183 us                                                      | 121 us: 1.51x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 179 us: 1.51x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 35.0 ms: 1.27x faster                                                      |
| unpickle             | 9.09 us                                                     | 7.99 us: 1.14x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 49.7 ms: 1.12x faster                                                      |
| json_loads           | 14.0 us                                                     | 12.9 us: 1.09x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 90.5 ms: 1.07x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.3 ms: 1.04x faster                                                      |
| unpickle_list        | 2.71 us                                                     | 2.61 us: 1.04x faster                                                      |
| pickle               | 6.85 us                                                     | 6.90 us: 1.01x slower                                                      |
| pickle_list          | 2.75 us                                                     | 2.85 us: 1.03x slower                                                      |
| pickle_dict          | 17.2 us                                                     | 19.4 us: 1.13x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.16x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.5 ms: 1.11x faster                                                      |
| python_startup_no_site | 15.5 ms                                                     | 15.7 ms: 1.01x slower                                                      |
| Geometric mean         | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 6.19 ms: 1.46x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 13.8 ms: 1.43x faster                                                      |
| django_template | 28.9 ms                                                     | 21.4 ms: 1.35x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 32.3 ms: 1.27x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.38x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.07 ms: 2.02x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 5.17 ms: 1.77x faster                                                      |
| richards                | 42.4 ms                                                     | 24.5 ms: 1.73x faster                                                      |
| logging_silent          | 94.6 ns                                                     | 57.2 ns: 1.66x faster                                                      |
| scimark_sor             | 106 ms                                                      | 64.6 ms: 1.64x faster                                                      |
| go                      | 139 ms                                                      | 84.8 ms: 1.64x faster                                                      |
| scimark_lu              | 85.8 ms                                                     | 54.8 ms: 1.56x faster                                                      |
| pyflate                 | 409 ms                                                      | 264 ms: 1.55x faster                                                       |
| raytrace                | 273 ms                                                      | 179 ms: 1.53x faster                                                       |
| unpickle_pure_python    | 183 us                                                      | 121 us: 1.51x faster                                                       |
| pickle_pure_python      | 270 us                                                      | 179 us: 1.51x faster                                                       |
| scimark_monte_carlo     | 57.3 ms                                                     | 38.1 ms: 1.50x faster                                                      |
| unpack_sequence         | 39.6 ns                                                     | 26.4 ns: 1.50x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 3.89 ms: 1.48x faster                                                      |
| html5lib                | 51.0 ms                                                     | 35.0 ms: 1.46x faster                                                      |
| mako                    | 9.03 ms                                                     | 6.19 ms: 1.46x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 13.8 ms: 1.43x faster                                                      |
| chaos                   | 61.7 ms                                                     | 43.2 ms: 1.43x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 780 ms: 1.42x faster                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 860 us: 1.41x faster                                                       |
| sqlglot_transpile       | 1.48 ms                                                     | 1.06 ms: 1.39x faster                                                      |
| crypto_pyaes            | 62.5 ms                                                     | 45.1 ms: 1.39x faster                                                      |
| async_tree_none         | 435 ms                                                      | 317 ms: 1.37x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 21.2 us: 1.36x faster                                                      |
| async_tree_memoization  | 526 ms                                                      | 388 ms: 1.35x faster                                                       |
| django_template         | 28.9 ms                                                     | 21.4 ms: 1.35x faster                                                      |
| pycparser               | 930 ms                                                      | 691 ms: 1.35x faster                                                       |
| thrift                  | 617 us                                                      | 469 us: 1.32x faster                                                       |
| pprint_safe_repr        | 592 ms                                                      | 458 ms: 1.29x faster                                                       |
| pprint_pformat          | 1.22 sec                                                    | 947 ms: 1.29x faster                                                       |
| regex_compile           | 106 ms                                                      | 82.5 ms: 1.29x faster                                                      |
| chameleon               | 5.79 ms                                                     | 4.53 ms: 1.28x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 501 ms: 1.27x faster                                                       |
| genshi_xml              | 41.0 ms                                                     | 32.3 ms: 1.27x faster                                                      |
| xml_etree_process       | 44.5 ms                                                     | 35.0 ms: 1.27x faster                                                      |
| spectral_norm           | 77.3 ms                                                     | 61.4 ms: 1.26x faster                                                      |
| 2to3                    | 246 ms                                                      | 196 ms: 1.26x faster                                                       |
| sqlglot_optimize        | 39.8 ms                                                     | 32.0 ms: 1.24x faster                                                      |
| async_generators        | 222 ms                                                      | 179 ms: 1.24x faster                                                       |
| float                   | 61.7 ms                                                     | 50.1 ms: 1.23x faster                                                      |
| docutils                | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                     |
| dulwich_log             | 50.5 ms                                                     | 41.2 ms: 1.23x faster                                                      |
| dask                    | 313 ms                                                      | 258 ms: 1.21x faster                                                       |
| sqlglot_normalize       | 205 ms                                                      | 172 ms: 1.19x faster                                                       |
| deepcopy                | 255 us                                                      | 214 us: 1.19x faster                                                       |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.30 ms: 1.19x faster                                                      |
| deepcopy_reduce         | 2.20 us                                                     | 1.88 us: 1.17x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 682 us: 1.17x faster                                                       |
| fannkuch                | 256 ms                                                      | 222 ms: 1.15x faster                                                       |
| nqueens                 | 66.6 ms                                                     | 57.9 ms: 1.15x faster                                                      |
| sympy_integrate         | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                      |
| json                    | 3.14 ms                                                     | 2.74 ms: 1.15x faster                                                      |
| bench_thread_pool       | 958 us                                                      | 837 us: 1.14x faster                                                       |
| nbody                   | 71.3 ms                                                     | 62.3 ms: 1.14x faster                                                      |
| unpickle                | 9.09 us                                                     | 7.99 us: 1.14x faster                                                      |
| regex_dna               | 136 ms                                                      | 120 ms: 1.14x faster                                                       |
| sympy_str               | 194 ms                                                      | 173 ms: 1.12x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 49.7 ms: 1.12x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.5 ms: 1.11x faster                                                      |
| mdp                     | 1.78 sec                                                    | 1.61 sec: 1.11x faster                                                     |
| sqlite_synth            | 1.91 us                                                     | 1.73 us: 1.10x faster                                                      |
| regex_v8                | 15.4 ms                                                     | 14.0 ms: 1.10x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 68.8 ms: 1.10x faster                                                      |
| sympy_expand            | 314 ms                                                      | 286 ms: 1.10x faster                                                       |
| json_loads              | 14.0 us                                                     | 12.9 us: 1.09x faster                                                      |
| telco                   | 3.94 ms                                                     | 3.64 ms: 1.08x faster                                                      |
| sympy_sum               | 107 ms                                                      | 99.0 ms: 1.08x faster                                                      |
| regex_effbot            | 1.66 ms                                                     | 1.54 ms: 1.07x faster                                                      |
| xml_etree_parse         | 96.8 ms                                                     | 90.5 ms: 1.07x faster                                                      |
| comprehensions          | 16.5 us                                                     | 15.5 us: 1.07x faster                                                      |
| scimark_fft             | 187 ms                                                      | 177 ms: 1.06x faster                                                       |
| coroutines              | 16.0 ms                                                     | 15.1 ms: 1.06x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 72.1 ms: 1.05x faster                                                      |
| xml_etree_iterparse     | 65.0 ms                                                     | 62.3 ms: 1.04x faster                                                      |
| unpickle_list           | 2.71 us                                                     | 2.61 us: 1.04x faster                                                      |
| logging_format          | 6.76 us                                                     | 6.64 us: 1.02x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.90 us: 1.01x slower                                                      |
| pidigits                | 149 ms                                                      | 151 ms: 1.01x slower                                                       |
| bench_mp_pool           | 62.0 ms                                                     | 62.8 ms: 1.01x slower                                                      |
| python_startup_no_site  | 15.5 ms                                                     | 15.7 ms: 1.01x slower                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.44 ms: 1.02x slower                                                      |
| pickle_list             | 2.75 us                                                     | 2.85 us: 1.03x slower                                                      |
| generators              | 32.4 ms                                                     | 33.9 ms: 1.05x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 19.4 us: 1.13x slower                                                      |
| coverage                | 39.0 ms                                                     | 51.6 ms: 1.32x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.22x faster                                                               |

Benchmark hidden because not significant (2): logging_simple, asyncio_tcp
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown