
# Results vs. 3.10.4

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: linux-x86_64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.38x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.33x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 253 ms: 1.38x faster                                                  |
| chameleon      | 9.68 ms                                                | 6.46 ms: 1.50x faster                                                 |
| docutils       | 3.30 sec                                               | 2.48 sec: 1.33x faster                                                |
| html5lib       | 88.9 ms                                                | 59.8 ms: 1.49x faster                                                 |
| Geometric mean | (ref)                                                  | 1.42x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 870 ms                                                 | 616 ms: 1.41x faster                                                  |
| async_tree_none         | 728 ms                                                 | 521 ms: 1.40x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                                |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 747 ms: 1.36x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.1 ms: 1.65x faster                                                 |
| float          | 117 ms                                                 | 72.2 ms: 1.62x faster                                                 |
| pidigits       | 191 ms                                                 | 192 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.38x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 132 ms: 1.43x faster                                                  |
| regex_v8       | 27.8 ms                                                | 21.1 ms: 1.32x faster                                                 |
| regex_dna      | 227 ms                                                 | 209 ms: 1.09x faster                                                  |
| regex_effbot   | 3.63 ms                                                | 3.49 ms: 1.04x faster                                                 |
| Geometric mean | (ref)                                                  | 1.21x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 285 us: 1.70x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 200 us: 1.65x faster                                                  |
| json_dumps           | 14.2 ms                                                | 9.54 ms: 1.49x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 53.9 ms: 1.47x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 77.5 ms: 1.28x faster                                                 |
| json_loads           | 31.2 us                                                | 24.3 us: 1.28x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.02 us: 1.26x faster                                                 |
| xml_etree_parse      | 168 ms                                                 | 149 ms: 1.13x faster                                                  |
| unpickle             | 14.4 us                                                | 13.0 us: 1.11x faster                                                 |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                  |
| pickle               | 10.7 us                                                | 10.0 us: 1.06x faster                                                 |
| unpickle_list        | 5.20 us                                                | 4.96 us: 1.05x faster                                                 |
| pickle_dict          | 29.6 us                                                | 30.0 us: 1.01x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.25x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.54 ms: 1.71x faster                                                 |
| python_startup_no_site | 5.93 ms                                                | 6.09 ms: 1.03x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.29x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.74 ms: 1.68x faster                                                 |
| genshi_text     | 31.8 ms                                                | 20.8 ms: 1.53x faster                                                 |
| django_template | 48.2 ms                                                | 32.6 ms: 1.48x faster                                                 |
| genshi_xml      | 66.0 ms                                                | 46.5 ms: 1.42x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.52x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.25 ms: 2.43x faster                                                 |
| logging_silent          | 190 ns                                                 | 93.5 ns: 2.03x faster                                                 |
| scimark_sor             | 220 ms                                                 | 108 ms: 2.03x faster                                                  |
| richards                | 79.3 ms                                                | 42.3 ms: 1.87x faster                                                 |
| asyncio_tcp             | 922 ms                                                 | 504 ms: 1.83x faster                                                  |
| pyflate                 | 716 ms                                                 | 397 ms: 1.81x faster                                                  |
| scimark_monte_carlo     | 118 ms                                                 | 65.7 ms: 1.80x faster                                                 |
| spectral_norm           | 170 ms                                                 | 95.0 ms: 1.79x faster                                                 |
| raytrace                | 507 ms                                                 | 284 ms: 1.79x faster                                                  |
| go                      | 240 ms                                                 | 135 ms: 1.78x faster                                                  |
| hexiom                  | 10.4 ms                                                | 5.98 ms: 1.74x faster                                                 |
| python_startup          | 14.6 ms                                                | 8.54 ms: 1.71x faster                                                 |
| chaos                   | 115 ms                                                 | 67.7 ms: 1.70x faster                                                 |
| pickle_pure_python      | 484 us                                                 | 285 us: 1.70x faster                                                  |
| crypto_pyaes            | 128 ms                                                 | 75.7 ms: 1.69x faster                                                 |
| deepcopy_memo           | 58.5 us                                                | 34.7 us: 1.69x faster                                                 |
| mako                    | 16.3 ms                                                | 9.74 ms: 1.68x faster                                                 |
| unpickle_pure_python    | 331 us                                                 | 200 us: 1.65x faster                                                  |
| nbody                   | 154 ms                                                 | 93.1 ms: 1.65x faster                                                 |
| scimark_lu              | 176 ms                                                 | 107 ms: 1.64x faster                                                  |
| float                   | 117 ms                                                 | 72.2 ms: 1.62x faster                                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.13 ms: 1.57x faster                                                 |
| sqlglot_parse           | 2.17 ms                                                | 1.41 ms: 1.54x faster                                                 |
| genshi_text             | 31.8 ms                                                | 20.8 ms: 1.53x faster                                                 |
| pprint_pformat          | 2.10 sec                                               | 1.38 sec: 1.52x faster                                                |
| sqlglot_transpile       | 2.57 ms                                                | 1.69 ms: 1.52x faster                                                 |
| chameleon               | 9.68 ms                                                | 6.46 ms: 1.50x faster                                                 |
| pprint_safe_repr        | 1.02 sec                                               | 680 ms: 1.50x faster                                                  |
| html5lib                | 88.9 ms                                                | 59.8 ms: 1.49x faster                                                 |
| json_dumps              | 14.2 ms                                                | 9.54 ms: 1.49x faster                                                 |
| scimark_fft             | 466 ms                                                 | 314 ms: 1.48x faster                                                  |
| django_template         | 48.2 ms                                                | 32.6 ms: 1.48x faster                                                 |
| xml_etree_process       | 79.1 ms                                                | 53.9 ms: 1.47x faster                                                 |
| fannkuch                | 532 ms                                                 | 362 ms: 1.47x faster                                                  |
| pycparser               | 1.58 sec                                               | 1.08 sec: 1.46x faster                                                |
| unpack_sequence         | 60.0 ns                                                | 41.4 ns: 1.45x faster                                                 |
| logging_simple          | 8.30 us                                                | 5.77 us: 1.44x faster                                                 |
| logging_format          | 9.09 us                                                | 6.35 us: 1.43x faster                                                 |
| regex_compile           | 188 ms                                                 | 132 ms: 1.43x faster                                                  |
| thrift                  | 1.07 ms                                                | 752 us: 1.42x faster                                                  |
| genshi_xml              | 66.0 ms                                                | 46.5 ms: 1.42x faster                                                 |
| deepcopy                | 479 us                                                 | 339 us: 1.41x faster                                                  |
| async_tree_memoization  | 870 ms                                                 | 616 ms: 1.41x faster                                                  |
| async_tree_none         | 728 ms                                                 | 521 ms: 1.40x faster                                                  |
| deepcopy_reduce         | 4.17 us                                                | 2.99 us: 1.39x faster                                                 |
| 2to3                    | 348 ms                                                 | 253 ms: 1.38x faster                                                  |
| coroutines              | 35.1 ms                                                | 25.4 ms: 1.38x faster                                                 |
| sqlglot_normalize       | 143 ms                                                 | 104 ms: 1.37x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                                |
| sqlglot_optimize        | 69.2 ms                                                | 50.7 ms: 1.36x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 747 ms: 1.36x faster                                                  |
| dulwich_log             | 84.3 ms                                                | 62.1 ms: 1.36x faster                                                 |
| nqueens                 | 106 ms                                                 | 78.0 ms: 1.36x faster                                                 |
| docutils                | 3.30 sec                                               | 2.48 sec: 1.33x faster                                                |
| regex_v8                | 27.8 ms                                                | 21.1 ms: 1.32x faster                                                 |
| xml_etree_generate      | 99.4 ms                                                | 77.5 ms: 1.28x faster                                                 |
| json_loads              | 31.2 us                                                | 24.3 us: 1.28x faster                                                 |
| sympy_integrate         | 25.8 ms                                                | 20.3 ms: 1.27x faster                                                 |
| pickle_list             | 5.08 us                                                | 4.02 us: 1.26x faster                                                 |
| bench_thread_pool       | 986 us                                                 | 782 us: 1.26x faster                                                  |
| async_generators        | 444 ms                                                 | 354 ms: 1.25x faster                                                  |
| sympy_expand            | 566 ms                                                 | 455 ms: 1.24x faster                                                  |
| djangocms               | 38.4 us                                                | 30.9 us: 1.24x faster                                                 |
| dask                    | 441 ms                                                 | 355 ms: 1.24x faster                                                  |
| sympy_str               | 346 ms                                                 | 282 ms: 1.23x faster                                                  |
| comprehensions          | 28.8 us                                                | 23.7 us: 1.21x faster                                                 |
| sympy_sum               | 196 ms                                                 | 163 ms: 1.21x faster                                                  |
| json                    | 5.69 ms                                                | 4.74 ms: 1.20x faster                                                 |
| sqlite_synth            | 3.02 us                                                | 2.57 us: 1.18x faster                                                 |
| telco                   | 7.27 ms                                                | 6.26 ms: 1.16x faster                                                 |
| meteor_contest          | 120 ms                                                 | 104 ms: 1.15x faster                                                  |
| pathlib                 | 20.5 ms                                                | 18.0 ms: 1.13x faster                                                 |
| xml_etree_parse         | 168 ms                                                 | 149 ms: 1.13x faster                                                  |
| create_gc_cycles        | 1.62 ms                                                | 1.45 ms: 1.12x faster                                                 |
| unpickle                | 14.4 us                                                | 13.0 us: 1.11x faster                                                 |
| regex_dna               | 227 ms                                                 | 209 ms: 1.09x faster                                                  |
| xml_etree_iterparse     | 115 ms                                                 | 106 ms: 1.09x faster                                                  |
| mdp                     | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                |
| pickle                  | 10.7 us                                                | 10.0 us: 1.06x faster                                                 |
| unpickle_list           | 5.20 us                                                | 4.96 us: 1.05x faster                                                 |
| regex_effbot            | 3.63 ms                                                | 3.49 ms: 1.04x faster                                                 |
| gc_traversal            | 3.62 ms                                                | 3.57 ms: 1.02x faster                                                 |
| generators              | 80.1 ms                                                | 79.1 ms: 1.01x faster                                                 |
| pidigits                | 191 ms                                                 | 192 ms: 1.01x slower                                                  |
| pickle_dict             | 29.6 us                                                | 30.0 us: 1.01x slower                                                 |
| python_startup_no_site  | 5.93 ms                                                | 6.09 ms: 1.03x slower                                                 |
| coverage                | 79.4 ms                                                | 99.0 ms: 1.25x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                          |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.36x
- 95% likely to have a speedup of 1.36x
- 99% likely to have a speedup of 1.33x


# Memory

- memory change: 1.08x