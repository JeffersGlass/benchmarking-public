
# Results vs. 3.11.0

- fork: python
- ref: v3.11.1
- machine: linux-x86_64
- commit hash: a7a450f
- commit date: 2022-12-06
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 258 ms: 1.02x faster                                   |
| chameleon      | 6.70 ms                                                | 6.63 ms: 1.01x faster                                  |
| docutils       | 2.66 sec                                               | 2.57 sec: 1.04x faster                                 |
| html5lib       | 64.8 ms                                                | 63.4 ms: 1.02x faster                                  |
| tornado_http   | 98.1 ms                                                | 99.8 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 639 ms                                                 | 627 ms: 1.02x faster                                   |
| async_tree_cpu_io_mixed | 749 ms                                                 | 742 ms: 1.01x faster                                   |
| async_tree_none         | 528 ms                                                 | 523 ms: 1.01x faster                                   |
| async_tree_io           | 1.29 sec                                               | 1.31 sec: 1.02x slower                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 78.9 ms                                                | 76.0 ms: 1.04x faster                                  |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| nbody          | 96.0 ms                                                | 95.4 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.31 ms: 1.06x faster                                  |
| regex_compile  | 141 ms                                                 | 137 ms: 1.03x faster                                   |
| regex_v8       | 22.9 ms                                                | 22.3 ms: 1.03x faster                                  |
| regex_dna      | 205 ms                                                 | 200 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads           | 29.2 us                                                | 24.0 us: 1.22x faster                                  |
| pickle               | 11.0 us                                                | 9.72 us: 1.13x faster                                  |
| pickle_dict          | 34.6 us                                                | 31.1 us: 1.11x faster                                  |
| pickle_list          | 4.59 us                                                | 4.17 us: 1.10x faster                                  |
| xml_etree_process    | 56.9 ms                                                | 53.7 ms: 1.06x faster                                  |
| xml_etree_generate   | 81.1 ms                                                | 76.6 ms: 1.06x faster                                  |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.06x faster                                   |
| json_dumps           | 13.3 ms                                                | 12.6 ms: 1.06x faster                                  |
| unpickle_list        | 5.21 us                                                | 4.95 us: 1.05x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 103 ms: 1.05x faster                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                   |
| unpickle             | 13.8 us                                                | 13.4 us: 1.04x faster                                  |
| pickle_pure_python   | 320 us                                                 | 310 us: 1.03x faster                                   |
| Geometric mean       | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.49 ms: 1.01x faster                                  |
| python_startup_no_site | 6.01 ms                                                | 5.98 ms: 1.01x faster                                  |
| Geometric mean         | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.92 ms: 1.07x faster                                  |
| genshi_xml      | 53.4 ms                                                | 52.5 ms: 1.02x faster                                  |
| genshi_text     | 22.5 ms                                                | 22.1 ms: 1.02x faster                                  |
| django_template | 33.5 ms                                                | 33.2 ms: 1.01x faster                                  |
| Geometric mean  | (ref)                                                  | 1.03x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-v3.11.1-3.11.1-a7a450f |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads              | 29.2 us                                                | 24.0 us: 1.22x faster                                  |
| json                    | 5.24 ms                                                | 4.63 ms: 1.13x faster                                  |
| pickle                  | 11.0 us                                                | 9.72 us: 1.13x faster                                  |
| pickle_dict             | 34.6 us                                                | 31.1 us: 1.11x faster                                  |
| pickle_list             | 4.59 us                                                | 4.17 us: 1.10x faster                                  |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.59 ms: 1.10x faster                                  |
| logging_silent          | 111 ns                                                 | 102 ns: 1.09x faster                                   |
| scimark_lu              | 116 ms                                                 | 107 ms: 1.08x faster                                   |
| pprint_pformat          | 1.55 sec                                               | 1.44 sec: 1.08x faster                                 |
| deepcopy_memo           | 40.2 us                                                | 37.2 us: 1.08x faster                                  |
| mako                    | 10.7 ms                                                | 9.92 ms: 1.07x faster                                  |
| deltablue               | 3.92 ms                                                | 3.67 ms: 1.07x faster                                  |
| coroutines              | 27.0 ms                                                | 25.3 ms: 1.07x faster                                  |
| pprint_safe_repr        | 747 ms                                                 | 700 ms: 1.07x faster                                   |
| hexiom                  | 6.89 ms                                                | 6.46 ms: 1.07x faster                                  |
| spectral_norm           | 108 ms                                                 | 101 ms: 1.07x faster                                   |
| gunicorn                | 1.20 ms                                                | 1.13 ms: 1.07x faster                                  |
| go                      | 149 ms                                                 | 140 ms: 1.06x faster                                   |
| aiohttp                 | 1.12 ms                                                | 1.05 ms: 1.06x faster                                  |
| richards                | 49.8 ms                                                | 46.9 ms: 1.06x faster                                  |
| regex_effbot            | 3.51 ms                                                | 3.31 ms: 1.06x faster                                  |
| xml_etree_process       | 56.9 ms                                                | 53.7 ms: 1.06x faster                                  |
| xml_etree_generate      | 81.1 ms                                                | 76.6 ms: 1.06x faster                                  |
| unpickle_pure_python    | 242 us                                                 | 229 us: 1.06x faster                                   |
| json_dumps              | 13.3 ms                                                | 12.6 ms: 1.06x faster                                  |
| crypto_pyaes            | 76.7 ms                                                | 72.6 ms: 1.06x faster                                  |
| fannkuch                | 405 ms                                                 | 384 ms: 1.06x faster                                   |
| scimark_fft             | 345 ms                                                 | 327 ms: 1.05x faster                                   |
| unpickle_list           | 5.21 us                                                | 4.95 us: 1.05x faster                                  |
| mdp                     | 2.77 sec                                               | 2.64 sec: 1.05x faster                                 |
| raytrace                | 309 ms                                                 | 294 ms: 1.05x faster                                   |
| scimark_sor             | 121 ms                                                 | 116 ms: 1.05x faster                                   |
| deepcopy                | 365 us                                                 | 349 us: 1.05x faster                                   |
| xml_etree_iterparse     | 108 ms                                                 | 103 ms: 1.05x faster                                   |
| logging_simple          | 6.22 us                                                | 5.95 us: 1.05x faster                                  |
| pyflate                 | 434 ms                                                 | 415 ms: 1.04x faster                                   |
| async_generators        | 374 ms                                                 | 358 ms: 1.04x faster                                   |
| sqlglot_transpile       | 1.75 ms                                                | 1.68 ms: 1.04x faster                                  |
| sqlite_synth            | 2.57 us                                                | 2.47 us: 1.04x faster                                  |
| logging_format          | 6.81 us                                                | 6.54 us: 1.04x faster                                  |
| xml_etree_parse         | 164 ms                                                 | 158 ms: 1.04x faster                                   |
| deepcopy_reduce         | 3.22 us                                                | 3.09 us: 1.04x faster                                  |
| sqlglot_normalize       | 113 ms                                                 | 108 ms: 1.04x faster                                   |
| sqlglot_parse           | 1.43 ms                                                | 1.38 ms: 1.04x faster                                  |
| float                   | 78.9 ms                                                | 76.0 ms: 1.04x faster                                  |
| sqlglot_optimize        | 55.3 ms                                                | 53.3 ms: 1.04x faster                                  |
| docutils                | 2.66 sec                                               | 2.57 sec: 1.04x faster                                 |
| unpickle                | 13.8 us                                                | 13.4 us: 1.04x faster                                  |
| nqueens                 | 87.9 ms                                                | 85.0 ms: 1.03x faster                                  |
| scimark_monte_carlo     | 70.7 ms                                                | 68.4 ms: 1.03x faster                                  |
| pickle_pure_python      | 320 us                                                 | 310 us: 1.03x faster                                   |
| chaos                   | 71.9 ms                                                | 69.6 ms: 1.03x faster                                  |
| pylint                  | 476 ms                                                 | 461 ms: 1.03x faster                                   |
| regex_compile           | 141 ms                                                 | 137 ms: 1.03x faster                                   |
| flaskblogging           | 7.28 ms                                                | 7.07 ms: 1.03x faster                                  |
| telco                   | 6.86 ms                                                | 6.66 ms: 1.03x faster                                  |
| meteor_contest          | 109 ms                                                 | 106 ms: 1.03x faster                                   |
| sympy_str               | 297 ms                                                 | 289 ms: 1.03x faster                                   |
| bench_thread_pool       | 834 us                                                 | 813 us: 1.03x faster                                   |
| regex_v8                | 22.9 ms                                                | 22.3 ms: 1.03x faster                                  |
| sympy_expand            | 484 ms                                                 | 472 ms: 1.03x faster                                   |
| thrift                  | 784 us                                                 | 765 us: 1.02x faster                                   |
| pathlib                 | 18.5 ms                                                | 18.1 ms: 1.02x faster                                  |
| pidigits                | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| 2to3                    | 264 ms                                                 | 258 ms: 1.02x faster                                   |
| sympy_integrate         | 21.5 ms                                                | 21.0 ms: 1.02x faster                                  |
| regex_dna               | 205 ms                                                 | 200 ms: 1.02x faster                                   |
| html5lib                | 64.8 ms                                                | 63.4 ms: 1.02x faster                                  |
| generators              | 74.9 ms                                                | 73.3 ms: 1.02x faster                                  |
| genshi_xml              | 53.4 ms                                                | 52.5 ms: 1.02x faster                                  |
| sqlalchemy_imperative   | 18.3 ms                                                | 18.0 ms: 1.02x faster                                  |
| async_tree_memoization  | 639 ms                                                 | 627 ms: 1.02x faster                                   |
| pycparser               | 1.19 sec                                               | 1.16 sec: 1.02x faster                                 |
| dulwich_log             | 64.6 ms                                                | 63.5 ms: 1.02x faster                                  |
| sympy_sum               | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| genshi_text             | 22.5 ms                                                | 22.1 ms: 1.02x faster                                  |
| chameleon               | 6.70 ms                                                | 6.63 ms: 1.01x faster                                  |
| async_tree_cpu_io_mixed | 749 ms                                                 | 742 ms: 1.01x faster                                   |
| django_template         | 33.5 ms                                                | 33.2 ms: 1.01x faster                                  |
| async_tree_none         | 528 ms                                                 | 523 ms: 1.01x faster                                   |
| python_startup          | 8.56 ms                                                | 8.49 ms: 1.01x faster                                  |
| nbody                   | 96.0 ms                                                | 95.4 ms: 1.01x faster                                  |
| python_startup_no_site  | 6.01 ms                                                | 5.98 ms: 1.01x faster                                  |
| asyncio_tcp             | 875 ms                                                 | 889 ms: 1.02x slower                                   |
| async_tree_io           | 1.29 sec                                               | 1.31 sec: 1.02x slower                                 |
| tornado_http            | 98.1 ms                                                | 99.8 ms: 1.02x slower                                  |
| unpack_sequence         | 43.5 ns                                                | 44.6 ns: 1.03x slower                                  |
| create_gc_cycles        | 1.43 ms                                                | 1.48 ms: 1.03x slower                                  |
| gc_traversal            | 4.01 ms                                                | 4.26 ms: 1.06x slower                                  |
| coverage                | 78.8 ms                                                | 104 ms: 1.32x slower                                   |
| Geometric mean          | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (4): djangocms, bench_mp_pool, dask, sqlalchemy_declarative
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x