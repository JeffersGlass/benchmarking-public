
# Results vs. 3.11.0

- fork: python
- ref: v3.11.0b3
- machine: linux-x86_64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 256 ms: 1.03x faster                                       |
| chameleon      | 6.70 ms                                                | 6.42 ms: 1.04x faster                                      |
| docutils       | 2.66 sec                                               | 2.56 sec: 1.04x faster                                     |
| html5lib       | 64.8 ms                                                | 62.8 ms: 1.03x faster                                      |
| tornado_http   | 98.1 ms                                                | 94.7 ms: 1.04x faster                                      |
| Geometric mean | (ref)                                                  | 1.04x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 735 ms: 1.02x faster                                       |
| async_tree_io           | 1.29 sec                                               | 1.30 sec: 1.01x slower                                     |
| Geometric mean          | (ref)                                                  | 1.00x faster                                               |

Benchmark hidden because not significant (2): async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| float          | 78.9 ms                                                | 73.9 ms: 1.07x faster                                      |
| nbody          | 96.0 ms                                                | 94.9 ms: 1.01x faster                                      |
| pidigits       | 194 ms                                                 | 194 ms: 1.00x faster                                       |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 2.92 ms: 1.20x faster                                      |
| regex_v8       | 22.9 ms                                                | 21.4 ms: 1.07x faster                                      |
| regex_dna      | 205 ms                                                 | 194 ms: 1.05x faster                                       |
| regex_compile  | 141 ms                                                 | 136 ms: 1.04x faster                                       |
| Geometric mean | (ref)                                                  | 1.09x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 26.0 us: 1.33x faster                                      |
| json_loads           | 29.2 us                                                | 24.9 us: 1.17x faster                                      |
| pickle               | 11.0 us                                                | 9.37 us: 1.17x faster                                      |
| pickle_list          | 4.59 us                                                | 4.27 us: 1.07x faster                                      |
| unpickle_pure_python | 242 us                                                 | 227 us: 1.06x faster                                       |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                       |
| xml_etree_process    | 56.9 ms                                                | 53.6 ms: 1.06x faster                                      |
| xml_etree_generate   | 81.1 ms                                                | 76.7 ms: 1.06x faster                                      |
| json_dumps           | 13.3 ms                                                | 12.7 ms: 1.05x faster                                      |
| unpickle_list        | 5.21 us                                                | 4.96 us: 1.05x faster                                      |
| unpickle             | 13.8 us                                                | 13.3 us: 1.04x faster                                      |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                       |
| Geometric mean       | (ref)                                                  | 1.09x faster                                               |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.51 ms: 1.01x faster                                      |
| python_startup_no_site | 6.01 ms                                                | 6.01 ms: 1.00x faster                                      |
| Geometric mean         | (ref)                                                  | 1.00x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.99 ms: 1.07x faster                                      |
| genshi_xml      | 53.4 ms                                                | 52.3 ms: 1.02x faster                                      |
| genshi_text     | 22.5 ms                                                | 22.0 ms: 1.02x faster                                      |
| django_template | 33.5 ms                                                | 33.0 ms: 1.02x faster                                      |
| Geometric mean  | (ref)                                                  | 1.03x faster                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-linux-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 26.0 us: 1.33x faster                                      |
| regex_effbot            | 3.51 ms                                                | 2.92 ms: 1.20x faster                                      |
| json_loads              | 29.2 us                                                | 24.9 us: 1.17x faster                                      |
| pickle                  | 11.0 us                                                | 9.37 us: 1.17x faster                                      |
| spectral_norm           | 108 ms                                                 | 97.5 ms: 1.11x faster                                      |
| json                    | 5.24 ms                                                | 4.74 ms: 1.10x faster                                      |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.57 ms: 1.10x faster                                      |
| richards                | 49.8 ms                                                | 45.3 ms: 1.10x faster                                      |
| logging_silent          | 111 ns                                                 | 101 ns: 1.10x faster                                       |
| deepcopy_memo           | 40.2 us                                                | 36.9 us: 1.09x faster                                      |
| scimark_lu              | 116 ms                                                 | 107 ms: 1.08x faster                                       |
| hexiom                  | 6.89 ms                                                | 6.36 ms: 1.08x faster                                      |
| deepcopy_reduce         | 3.22 us                                                | 2.98 us: 1.08x faster                                      |
| pprint_safe_repr        | 747 ms                                                 | 694 ms: 1.08x faster                                       |
| deepcopy                | 365 us                                                 | 340 us: 1.07x faster                                       |
| pickle_list             | 4.59 us                                                | 4.27 us: 1.07x faster                                      |
| pprint_pformat          | 1.55 sec                                               | 1.45 sec: 1.07x faster                                     |
| deltablue               | 3.92 ms                                                | 3.65 ms: 1.07x faster                                      |
| logging_format          | 6.81 us                                                | 6.35 us: 1.07x faster                                      |
| float                   | 78.9 ms                                                | 73.9 ms: 1.07x faster                                      |
| logging_simple          | 6.22 us                                                | 5.82 us: 1.07x faster                                      |
| regex_v8                | 22.9 ms                                                | 21.4 ms: 1.07x faster                                      |
| gunicorn                | 1.20 ms                                                | 1.12 ms: 1.07x faster                                      |
| go                      | 149 ms                                                 | 139 ms: 1.07x faster                                       |
| mako                    | 10.7 ms                                                | 9.99 ms: 1.07x faster                                      |
| unpickle_pure_python    | 242 us                                                 | 227 us: 1.06x faster                                       |
| pickle_pure_python      | 320 us                                                 | 301 us: 1.06x faster                                       |
| xml_etree_process       | 56.9 ms                                                | 53.6 ms: 1.06x faster                                      |
| scimark_monte_carlo     | 70.7 ms                                                | 66.6 ms: 1.06x faster                                      |
| scimark_sor             | 121 ms                                                 | 114 ms: 1.06x faster                                       |
| pyflate                 | 434 ms                                                 | 409 ms: 1.06x faster                                       |
| gc_traversal            | 4.01 ms                                                | 3.79 ms: 1.06x faster                                      |
| xml_etree_generate      | 81.1 ms                                                | 76.7 ms: 1.06x faster                                      |
| raytrace                | 309 ms                                                 | 292 ms: 1.06x faster                                       |
| json_dumps              | 13.3 ms                                                | 12.7 ms: 1.05x faster                                      |
| regex_dna               | 205 ms                                                 | 194 ms: 1.05x faster                                       |
| chaos                   | 71.9 ms                                                | 68.2 ms: 1.05x faster                                      |
| scimark_fft             | 345 ms                                                 | 328 ms: 1.05x faster                                       |
| unpickle_list           | 5.21 us                                                | 4.96 us: 1.05x faster                                      |
| aiohttp                 | 1.12 ms                                                | 1.06 ms: 1.05x faster                                      |
| async_generators        | 374 ms                                                 | 356 ms: 1.05x faster                                       |
| nqueens                 | 87.9 ms                                                | 83.8 ms: 1.05x faster                                      |
| chameleon               | 6.70 ms                                                | 6.42 ms: 1.04x faster                                      |
| sympy_str               | 297 ms                                                 | 285 ms: 1.04x faster                                       |
| sympy_sum               | 169 ms                                                 | 162 ms: 1.04x faster                                       |
| crypto_pyaes            | 76.7 ms                                                | 73.6 ms: 1.04x faster                                      |
| telco                   | 6.86 ms                                                | 6.59 ms: 1.04x faster                                      |
| meteor_contest          | 109 ms                                                 | 105 ms: 1.04x faster                                       |
| docutils                | 2.66 sec                                               | 2.56 sec: 1.04x faster                                     |
| coroutines              | 27.0 ms                                                | 26.0 ms: 1.04x faster                                      |
| unpickle                | 13.8 us                                                | 13.3 us: 1.04x faster                                      |
| regex_compile           | 141 ms                                                 | 136 ms: 1.04x faster                                       |
| xml_etree_parse         | 164 ms                                                 | 158 ms: 1.04x faster                                       |
| sympy_integrate         | 21.5 ms                                                | 20.7 ms: 1.04x faster                                      |
| flaskblogging           | 7.28 ms                                                | 7.04 ms: 1.04x faster                                      |
| tornado_http            | 98.1 ms                                                | 94.7 ms: 1.04x faster                                      |
| sympy_expand            | 484 ms                                                 | 469 ms: 1.03x faster                                       |
| fannkuch                | 405 ms                                                 | 393 ms: 1.03x faster                                       |
| sqlglot_normalize       | 113 ms                                                 | 109 ms: 1.03x faster                                       |
| html5lib                | 64.8 ms                                                | 62.8 ms: 1.03x faster                                      |
| mdp                     | 2.77 sec                                               | 2.69 sec: 1.03x faster                                     |
| 2to3                    | 264 ms                                                 | 256 ms: 1.03x faster                                       |
| thrift                  | 784 us                                                 | 763 us: 1.03x faster                                       |
| sqlalchemy_imperative   | 18.3 ms                                                | 17.8 ms: 1.03x faster                                      |
| sqlalchemy_declarative  | 140 ms                                                 | 137 ms: 1.03x faster                                       |
| dulwich_log             | 64.6 ms                                                | 63.0 ms: 1.03x faster                                      |
| sqlglot_optimize        | 55.3 ms                                                | 54.0 ms: 1.02x faster                                      |
| pylint                  | 476 ms                                                 | 465 ms: 1.02x faster                                       |
| bench_thread_pool       | 834 us                                                 | 816 us: 1.02x faster                                       |
| genshi_xml              | 53.4 ms                                                | 52.3 ms: 1.02x faster                                      |
| pathlib                 | 18.5 ms                                                | 18.1 ms: 1.02x faster                                      |
| genshi_text             | 22.5 ms                                                | 22.0 ms: 1.02x faster                                      |
| async_tree_cpu_io_mixed | 749 ms                                                 | 735 ms: 1.02x faster                                       |
| django_template         | 33.5 ms                                                | 33.0 ms: 1.02x faster                                      |
| sqlite_synth            | 2.57 us                                                | 2.53 us: 1.02x faster                                      |
| generators              | 74.9 ms                                                | 73.8 ms: 1.01x faster                                      |
| nbody                   | 96.0 ms                                                | 94.9 ms: 1.01x faster                                      |
| python_startup          | 8.56 ms                                                | 8.51 ms: 1.01x faster                                      |
| python_startup_no_site  | 6.01 ms                                                | 6.01 ms: 1.00x faster                                      |
| pidigits                | 194 ms                                                 | 194 ms: 1.00x faster                                       |
| async_tree_io           | 1.29 sec                                               | 1.30 sec: 1.01x slower                                     |
| asyncio_tcp             | 875 ms                                                 | 888 ms: 1.01x slower                                       |
| create_gc_cycles        | 1.43 ms                                                | 1.51 ms: 1.05x slower                                      |
| comprehensions          | 23.6 us                                                | 25.9 us: 1.10x slower                                      |
| unpack_sequence         | 43.5 ns                                                | 48.0 ns: 1.10x slower                                      |
| sqlglot_transpile       | 1.75 ms                                                | 2.04 ms: 1.16x slower                                      |
| sqlglot_parse           | 1.43 ms                                                | 1.75 ms: 1.22x slower                                      |
| Geometric mean          | (ref)                                                  | 1.04x faster                                               |

Benchmark hidden because not significant (7): djangocms, pycparser, async_tree_none, async_tree_memoization, xml_etree_iterparse, bench_mp_pool, dask
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 1.01x