
# Results vs. 3.11.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: linux-x86_64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 253 ms: 1.05x faster                                                  |
| chameleon      | 6.70 ms                                                | 6.46 ms: 1.04x faster                                                 |
| docutils       | 2.66 sec                                               | 2.48 sec: 1.07x faster                                                |
| html5lib       | 64.8 ms                                                | 59.8 ms: 1.08x faster                                                 |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization | 639 ms                                                 | 616 ms: 1.04x faster                                                  |
| async_tree_none        | 528 ms                                                 | 521 ms: 1.01x faster                                                  |
| async_tree_io          | 1.29 sec                                               | 1.30 sec: 1.01x slower                                                |
| Geometric mean         | (ref)                                                  | 1.01x faster                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 78.9 ms                                                | 72.2 ms: 1.09x faster                                                 |
| nbody          | 96.0 ms                                                | 93.1 ms: 1.03x faster                                                 |
| pidigits       | 194 ms                                                 | 192 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 21.1 ms: 1.09x faster                                                 |
| regex_compile  | 141 ms                                                 | 132 ms: 1.07x faster                                                  |
| regex_effbot   | 3.51 ms                                                | 3.49 ms: 1.00x faster                                                 |
| regex_dna      | 205 ms                                                 | 209 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.54 ms: 1.40x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 200 us: 1.21x faster                                                  |
| json_loads           | 29.2 us                                                | 24.3 us: 1.20x faster                                                 |
| pickle_dict          | 34.6 us                                                | 30.0 us: 1.15x faster                                                 |
| pickle_list          | 4.59 us                                                | 4.02 us: 1.14x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 285 us: 1.12x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 149 ms: 1.10x faster                                                  |
| pickle               | 11.0 us                                                | 10.0 us: 1.10x faster                                                 |
| unpickle             | 13.8 us                                                | 13.0 us: 1.07x faster                                                 |
| xml_etree_process    | 56.9 ms                                                | 53.9 ms: 1.06x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.96 us: 1.05x faster                                                 |
| xml_etree_generate   | 81.1 ms                                                | 77.5 ms: 1.05x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.54 ms: 1.00x faster                                                 |
| python_startup_no_site | 6.01 ms                                                | 6.09 ms: 1.01x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 46.5 ms: 1.15x faster                                                 |
| mako            | 10.7 ms                                                | 9.74 ms: 1.09x faster                                                 |
| genshi_text     | 22.5 ms                                                | 20.8 ms: 1.08x faster                                                 |
| django_template | 33.5 ms                                                | 32.6 ms: 1.03x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.09x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-linux-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| asyncio_tcp             | 875 ms                                                 | 504 ms: 1.74x faster                                                  |
| json_dumps              | 13.3 ms                                                | 9.54 ms: 1.40x faster                                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.13 ms: 1.22x faster                                                 |
| unpickle_pure_python    | 242 us                                                 | 200 us: 1.21x faster                                                  |
| deltablue               | 3.92 ms                                                | 3.25 ms: 1.21x faster                                                 |
| json_loads              | 29.2 us                                                | 24.3 us: 1.20x faster                                                 |
| logging_silent          | 111 ns                                                 | 93.5 ns: 1.19x faster                                                 |
| richards                | 49.8 ms                                                | 42.3 ms: 1.18x faster                                                 |
| deepcopy_memo           | 40.2 us                                                | 34.7 us: 1.16x faster                                                 |
| pickle_dict             | 34.6 us                                                | 30.0 us: 1.15x faster                                                 |
| hexiom                  | 6.89 ms                                                | 5.98 ms: 1.15x faster                                                 |
| genshi_xml              | 53.4 ms                                                | 46.5 ms: 1.15x faster                                                 |
| pickle_list             | 4.59 us                                                | 4.02 us: 1.14x faster                                                 |
| spectral_norm           | 108 ms                                                 | 95.0 ms: 1.14x faster                                                 |
| nqueens                 | 87.9 ms                                                | 78.0 ms: 1.13x faster                                                 |
| pprint_pformat          | 1.55 sec                                               | 1.38 sec: 1.12x faster                                                |
| gc_traversal            | 4.01 ms                                                | 3.57 ms: 1.12x faster                                                 |
| pickle_pure_python      | 320 us                                                 | 285 us: 1.12x faster                                                  |
| scimark_sor             | 121 ms                                                 | 108 ms: 1.12x faster                                                  |
| fannkuch                | 405 ms                                                 | 362 ms: 1.12x faster                                                  |
| json                    | 5.24 ms                                                | 4.74 ms: 1.11x faster                                                 |
| scimark_fft             | 345 ms                                                 | 314 ms: 1.10x faster                                                  |
| xml_etree_parse         | 164 ms                                                 | 149 ms: 1.10x faster                                                  |
| go                      | 149 ms                                                 | 135 ms: 1.10x faster                                                  |
| pprint_safe_repr        | 747 ms                                                 | 680 ms: 1.10x faster                                                  |
| pickle                  | 11.0 us                                                | 10.0 us: 1.10x faster                                                 |
| pycparser               | 1.19 sec                                               | 1.08 sec: 1.10x faster                                                |
| telco                   | 6.86 ms                                                | 6.26 ms: 1.10x faster                                                 |
| mako                    | 10.7 ms                                                | 9.74 ms: 1.09x faster                                                 |
| pyflate                 | 434 ms                                                 | 397 ms: 1.09x faster                                                  |
| float                   | 78.9 ms                                                | 72.2 ms: 1.09x faster                                                 |
| sqlglot_optimize        | 55.3 ms                                                | 50.7 ms: 1.09x faster                                                 |
| raytrace                | 309 ms                                                 | 284 ms: 1.09x faster                                                  |
| regex_v8                | 22.9 ms                                                | 21.1 ms: 1.09x faster                                                 |
| sqlglot_normalize       | 113 ms                                                 | 104 ms: 1.08x faster                                                  |
| scimark_lu              | 116 ms                                                 | 107 ms: 1.08x faster                                                  |
| genshi_text             | 22.5 ms                                                | 20.8 ms: 1.08x faster                                                 |
| html5lib                | 64.8 ms                                                | 59.8 ms: 1.08x faster                                                 |
| djangocms               | 33.5 us                                                | 30.9 us: 1.08x faster                                                 |
| logging_simple          | 6.22 us                                                | 5.77 us: 1.08x faster                                                 |
| deepcopy                | 365 us                                                 | 339 us: 1.08x faster                                                  |
| scimark_monte_carlo     | 70.7 ms                                                | 65.7 ms: 1.08x faster                                                 |
| deepcopy_reduce         | 3.22 us                                                | 2.99 us: 1.08x faster                                                 |
| docutils                | 2.66 sec                                               | 2.48 sec: 1.07x faster                                                |
| regex_compile           | 141 ms                                                 | 132 ms: 1.07x faster                                                  |
| logging_format          | 6.81 us                                                | 6.35 us: 1.07x faster                                                 |
| unpickle                | 13.8 us                                                | 13.0 us: 1.07x faster                                                 |
| bench_thread_pool       | 834 us                                                 | 782 us: 1.07x faster                                                  |
| sympy_expand            | 484 ms                                                 | 455 ms: 1.07x faster                                                  |
| coroutines              | 27.0 ms                                                | 25.4 ms: 1.06x faster                                                 |
| chaos                   | 71.9 ms                                                | 67.7 ms: 1.06x faster                                                 |
| sympy_integrate         | 21.5 ms                                                | 20.3 ms: 1.06x faster                                                 |
| xml_etree_process       | 56.9 ms                                                | 53.9 ms: 1.06x faster                                                 |
| async_generators        | 374 ms                                                 | 354 ms: 1.05x faster                                                  |
| sympy_str               | 297 ms                                                 | 282 ms: 1.05x faster                                                  |
| unpickle_list           | 5.21 us                                                | 4.96 us: 1.05x faster                                                 |
| unpack_sequence         | 43.5 ns                                                | 41.4 ns: 1.05x faster                                                 |
| xml_etree_generate      | 81.1 ms                                                | 77.5 ms: 1.05x faster                                                 |
| 2to3                    | 264 ms                                                 | 253 ms: 1.05x faster                                                  |
| meteor_contest          | 109 ms                                                 | 104 ms: 1.05x faster                                                  |
| mdp                     | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                |
| thrift                  | 784 us                                                 | 752 us: 1.04x faster                                                  |
| dulwich_log             | 64.6 ms                                                | 62.1 ms: 1.04x faster                                                 |
| sympy_sum               | 169 ms                                                 | 163 ms: 1.04x faster                                                  |
| async_tree_memoization  | 639 ms                                                 | 616 ms: 1.04x faster                                                  |
| chameleon               | 6.70 ms                                                | 6.46 ms: 1.04x faster                                                 |
| sqlglot_transpile       | 1.75 ms                                                | 1.69 ms: 1.03x faster                                                 |
| nbody                   | 96.0 ms                                                | 93.1 ms: 1.03x faster                                                 |
| django_template         | 33.5 ms                                                | 32.6 ms: 1.03x faster                                                 |
| dask                    | 365 ms                                                 | 355 ms: 1.03x faster                                                  |
| pathlib                 | 18.5 ms                                                | 18.0 ms: 1.03x faster                                                 |
| sqlglot_parse           | 1.43 ms                                                | 1.41 ms: 1.02x faster                                                 |
| xml_etree_iterparse     | 108 ms                                                 | 106 ms: 1.02x faster                                                  |
| async_tree_none         | 528 ms                                                 | 521 ms: 1.01x faster                                                  |
| crypto_pyaes            | 76.7 ms                                                | 75.7 ms: 1.01x faster                                                 |
| pidigits                | 194 ms                                                 | 192 ms: 1.01x faster                                                  |
| regex_effbot            | 3.51 ms                                                | 3.49 ms: 1.00x faster                                                 |
| python_startup          | 8.56 ms                                                | 8.54 ms: 1.00x faster                                                 |
| comprehensions          | 23.6 us                                                | 23.7 us: 1.01x slower                                                 |
| async_tree_io           | 1.29 sec                                               | 1.30 sec: 1.01x slower                                                |
| python_startup_no_site  | 6.01 ms                                                | 6.09 ms: 1.01x slower                                                 |
| create_gc_cycles        | 1.43 ms                                                | 1.45 ms: 1.01x slower                                                 |
| regex_dna               | 205 ms                                                 | 209 ms: 1.02x slower                                                  |
| generators              | 74.9 ms                                                | 79.1 ms: 1.06x slower                                                 |
| coverage                | 78.8 ms                                                | 99.0 ms: 1.26x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.08x faster                                                          |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, sqlite_synth, bench_mp_pool
Ignored benchmarks (17) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.01x