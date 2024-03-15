
# Results vs. 3.11.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: linux-x86_64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 249 ms: 1.06x faster                                                  |
| chameleon      | 6.70 ms                                                | 6.51 ms: 1.03x faster                                                 |
| docutils       | 2.66 sec                                               | 2.52 sec: 1.06x faster                                                |
| html5lib       | 64.8 ms                                                | 59.9 ms: 1.08x faster                                                 |
| tornado_http   | 98.1 ms                                                | 93.7 ms: 1.05x faster                                                 |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 730 ms: 1.03x faster                                                  |
| async_tree_memoization  | 639 ms                                                 | 656 ms: 1.03x slower                                                  |
| async_tree_io           | 1.29 sec                                               | 1.33 sec: 1.03x slower                                                |
| Geometric mean          | (ref)                                                  | 1.01x slower                                                          |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 78.9 ms                                                | 71.4 ms: 1.11x faster                                                 |
| nbody          | 96.0 ms                                                | 96.6 ms: 1.01x slower                                                 |
| pidigits       | 194 ms                                                 | 198 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 127 ms: 1.11x faster                                                  |
| regex_v8       | 22.9 ms                                                | 21.4 ms: 1.07x faster                                                 |
| regex_effbot   | 3.51 ms                                                | 3.37 ms: 1.04x faster                                                 |
| regex_dna      | 205 ms                                                 | 201 ms: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.36 ms: 1.42x faster                                                 |
| json_loads           | 29.2 us                                                | 23.5 us: 1.24x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 202 us: 1.20x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 145 ms: 1.13x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 285 us: 1.12x faster                                                  |
| pickle_dict          | 34.6 us                                                | 31.1 us: 1.11x faster                                                 |
| pickle_list          | 4.59 us                                                | 4.19 us: 1.09x faster                                                 |
| pickle               | 11.0 us                                                | 10.1 us: 1.08x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 101 ms: 1.07x faster                                                  |
| xml_etree_generate   | 81.1 ms                                                | 76.0 ms: 1.07x faster                                                 |
| xml_etree_process    | 56.9 ms                                                | 53.4 ms: 1.07x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.91 us: 1.06x faster                                                 |
| unpickle             | 13.8 us                                                | 13.2 us: 1.05x faster                                                 |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.42 ms: 1.02x faster                                                 |
| python_startup_no_site | 6.01 ms                                                | 5.93 ms: 1.01x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.02x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.64 ms: 1.11x faster                                                 |
| genshi_xml      | 53.4 ms                                                | 50.0 ms: 1.07x faster                                                 |
| genshi_text     | 22.5 ms                                                | 21.5 ms: 1.05x faster                                                 |
| django_template | 33.5 ms                                                | 33.0 ms: 1.02x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.06x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps              | 13.3 ms                                                | 9.36 ms: 1.42x faster                                                 |
| json_loads              | 29.2 us                                                | 23.5 us: 1.24x faster                                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.13 ms: 1.22x faster                                                 |
| logging_silent          | 111 ns                                                 | 91.6 ns: 1.21x faster                                                 |
| unpickle_pure_python    | 242 us                                                 | 202 us: 1.20x faster                                                  |
| deltablue               | 3.92 ms                                                | 3.30 ms: 1.19x faster                                                 |
| richards                | 49.8 ms                                                | 42.4 ms: 1.17x faster                                                 |
| deepcopy_memo           | 40.2 us                                                | 34.4 us: 1.17x faster                                                 |
| json                    | 5.24 ms                                                | 4.55 ms: 1.15x faster                                                 |
| scimark_sor             | 121 ms                                                 | 106 ms: 1.15x faster                                                  |
| spectral_norm           | 108 ms                                                 | 95.2 ms: 1.14x faster                                                 |
| pprint_pformat          | 1.55 sec                                               | 1.38 sec: 1.13x faster                                                |
| gc_traversal            | 4.01 ms                                                | 3.55 ms: 1.13x faster                                                 |
| hexiom                  | 6.89 ms                                                | 6.11 ms: 1.13x faster                                                 |
| xml_etree_parse         | 164 ms                                                 | 145 ms: 1.13x faster                                                  |
| pprint_safe_repr        | 747 ms                                                 | 665 ms: 1.12x faster                                                  |
| pickle_pure_python      | 320 us                                                 | 285 us: 1.12x faster                                                  |
| gunicorn                | 1.20 ms                                                | 1.07 ms: 1.12x faster                                                 |
| mdp                     | 2.77 sec                                               | 2.48 sec: 1.12x faster                                                |
| pickle_dict             | 34.6 us                                                | 31.1 us: 1.11x faster                                                 |
| aiohttp                 | 1.12 ms                                                | 1.00 ms: 1.11x faster                                                 |
| regex_compile           | 141 ms                                                 | 127 ms: 1.11x faster                                                  |
| scimark_fft             | 345 ms                                                 | 312 ms: 1.11x faster                                                  |
| deepcopy_reduce         | 3.22 us                                                | 2.91 us: 1.11x faster                                                 |
| comprehensions          | 23.6 us                                                | 21.3 us: 1.11x faster                                                 |
| float                   | 78.9 ms                                                | 71.4 ms: 1.11x faster                                                 |
| mako                    | 10.7 ms                                                | 9.64 ms: 1.11x faster                                                 |
| go                      | 149 ms                                                 | 135 ms: 1.10x faster                                                  |
| deepcopy                | 365 us                                                 | 333 us: 1.10x faster                                                  |
| coroutines              | 27.0 ms                                                | 24.7 ms: 1.10x faster                                                 |
| fannkuch                | 405 ms                                                 | 370 ms: 1.10x faster                                                  |
| pickle_list             | 4.59 us                                                | 4.19 us: 1.09x faster                                                 |
| raytrace                | 309 ms                                                 | 282 ms: 1.09x faster                                                  |
| nqueens                 | 87.9 ms                                                | 80.7 ms: 1.09x faster                                                 |
| pickle                  | 11.0 us                                                | 10.1 us: 1.08x faster                                                 |
| html5lib                | 64.8 ms                                                | 59.9 ms: 1.08x faster                                                 |
| sqlglot_normalize       | 113 ms                                                 | 104 ms: 1.08x faster                                                  |
| sqlglot_optimize        | 55.3 ms                                                | 51.2 ms: 1.08x faster                                                 |
| xml_etree_iterparse     | 108 ms                                                 | 101 ms: 1.07x faster                                                  |
| logging_simple          | 6.22 us                                                | 5.80 us: 1.07x faster                                                 |
| scimark_lu              | 116 ms                                                 | 108 ms: 1.07x faster                                                  |
| sqlglot_transpile       | 1.75 ms                                                | 1.63 ms: 1.07x faster                                                 |
| async_generators        | 374 ms                                                 | 349 ms: 1.07x faster                                                  |
| chaos                   | 71.9 ms                                                | 67.1 ms: 1.07x faster                                                 |
| regex_v8                | 22.9 ms                                                | 21.4 ms: 1.07x faster                                                 |
| genshi_xml              | 53.4 ms                                                | 50.0 ms: 1.07x faster                                                 |
| bench_thread_pool       | 834 us                                                 | 780 us: 1.07x faster                                                  |
| sqlglot_parse           | 1.43 ms                                                | 1.34 ms: 1.07x faster                                                 |
| xml_etree_generate      | 81.1 ms                                                | 76.0 ms: 1.07x faster                                                 |
| logging_format          | 6.81 us                                                | 6.38 us: 1.07x faster                                                 |
| xml_etree_process       | 56.9 ms                                                | 53.4 ms: 1.07x faster                                                 |
| pyflate                 | 434 ms                                                 | 407 ms: 1.07x faster                                                  |
| sympy_expand            | 484 ms                                                 | 455 ms: 1.07x faster                                                  |
| unpickle_list           | 5.21 us                                                | 4.91 us: 1.06x faster                                                 |
| scimark_monte_carlo     | 70.7 ms                                                | 66.6 ms: 1.06x faster                                                 |
| pycparser               | 1.19 sec                                               | 1.12 sec: 1.06x faster                                                |
| 2to3                    | 264 ms                                                 | 249 ms: 1.06x faster                                                  |
| docutils                | 2.66 sec                                               | 2.52 sec: 1.06x faster                                                |
| sympy_str               | 297 ms                                                 | 283 ms: 1.05x faster                                                  |
| thrift                  | 784 us                                                 | 746 us: 1.05x faster                                                  |
| sympy_integrate         | 21.5 ms                                                | 20.4 ms: 1.05x faster                                                 |
| genshi_text             | 22.5 ms                                                | 21.5 ms: 1.05x faster                                                 |
| unpickle                | 13.8 us                                                | 13.2 us: 1.05x faster                                                 |
| meteor_contest          | 109 ms                                                 | 104 ms: 1.05x faster                                                  |
| tornado_http            | 98.1 ms                                                | 93.7 ms: 1.05x faster                                                 |
| telco                   | 6.86 ms                                                | 6.55 ms: 1.05x faster                                                 |
| regex_effbot            | 3.51 ms                                                | 3.37 ms: 1.04x faster                                                 |
| pylint                  | 476 ms                                                 | 458 ms: 1.04x faster                                                  |
| dulwich_log             | 64.6 ms                                                | 62.4 ms: 1.04x faster                                                 |
| pathlib                 | 18.5 ms                                                | 17.9 ms: 1.03x faster                                                 |
| djangocms               | 33.5 us                                                | 32.5 us: 1.03x faster                                                 |
| sympy_sum               | 169 ms                                                 | 164 ms: 1.03x faster                                                  |
| chameleon               | 6.70 ms                                                | 6.51 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed | 749 ms                                                 | 730 ms: 1.03x faster                                                  |
| crypto_pyaes            | 76.7 ms                                                | 74.8 ms: 1.03x faster                                                 |
| python_startup          | 8.56 ms                                                | 8.42 ms: 1.02x faster                                                 |
| regex_dna               | 205 ms                                                 | 201 ms: 1.02x faster                                                  |
| django_template         | 33.5 ms                                                | 33.0 ms: 1.02x faster                                                 |
| dask                    | 365 ms                                                 | 360 ms: 1.01x faster                                                  |
| python_startup_no_site  | 6.01 ms                                                | 5.93 ms: 1.01x faster                                                 |
| generators              | 74.9 ms                                                | 74.1 ms: 1.01x faster                                                 |
| nbody                   | 96.0 ms                                                | 96.6 ms: 1.01x slower                                                 |
| unpack_sequence         | 43.5 ns                                                | 44.1 ns: 1.01x slower                                                 |
| create_gc_cycles        | 1.43 ms                                                | 1.46 ms: 1.01x slower                                                 |
| asyncio_tcp             | 875 ms                                                 | 890 ms: 1.02x slower                                                  |
| pidigits                | 194 ms                                                 | 198 ms: 1.02x slower                                                  |
| sqlite_synth            | 2.57 us                                                | 2.62 us: 1.02x slower                                                 |
| async_tree_memoization  | 639 ms                                                 | 656 ms: 1.03x slower                                                  |
| async_tree_io           | 1.29 sec                                               | 1.33 sec: 1.03x slower                                                |
| coverage                | 78.8 ms                                                | 102 ms: 1.29x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (2): bench_mp_pool, async_tree_none
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.01x