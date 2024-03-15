
# Results vs. 3.11.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: linux-x86_64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 246 ms: 1.07x faster                                                  |
| chameleon      | 6.70 ms                                                | 6.45 ms: 1.04x faster                                                 |
| docutils       | 2.66 sec                                               | 2.57 sec: 1.04x faster                                                |
| html5lib       | 64.8 ms                                                | 59.7 ms: 1.09x faster                                                 |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 528 ms                                                 | 536 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed | 749 ms                                                 | 769 ms: 1.03x slower                                                  |
| async_tree_io           | 1.29 sec                                               | 1.34 sec: 1.04x slower                                                |
| async_tree_memoization  | 639 ms                                                 | 665 ms: 1.04x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 78.9 ms                                                | 73.2 ms: 1.08x faster                                                 |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                  |
| nbody          | 96.0 ms                                                | 94.0 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.10x faster                                                  |
| regex_v8       | 22.9 ms                                                | 22.3 ms: 1.02x faster                                                 |
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                 |
| regex_dna      | 205 ms                                                 | 217 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.52 ms: 1.40x faster                                                 |
| json_loads           | 29.2 us                                                | 23.8 us: 1.22x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 200 us: 1.21x faster                                                  |
| pickle_list          | 4.59 us                                                | 3.95 us: 1.16x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 282 us: 1.13x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 148 ms: 1.11x faster                                                  |
| pickle_dict          | 34.6 us                                                | 31.5 us: 1.10x faster                                                 |
| pickle               | 11.0 us                                                | 10.1 us: 1.08x faster                                                 |
| xml_etree_process    | 56.9 ms                                                | 53.7 ms: 1.06x faster                                                 |
| xml_etree_generate   | 81.1 ms                                                | 76.9 ms: 1.05x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.97 us: 1.05x faster                                                 |
| unpickle             | 13.8 us                                                | 13.3 us: 1.04x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.52 ms: 1.00x faster                                                 |
| python_startup_no_site | 6.01 ms                                                | 6.07 ms: 1.01x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.43 ms: 1.13x faster                                                 |
| genshi_xml      | 53.4 ms                                                | 48.0 ms: 1.11x faster                                                 |
| genshi_text     | 22.5 ms                                                | 20.9 ms: 1.08x faster                                                 |
| django_template | 33.5 ms                                                | 33.0 ms: 1.02x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.08x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps              | 13.3 ms                                                | 9.52 ms: 1.40x faster                                                 |
| json_loads              | 29.2 us                                                | 23.8 us: 1.22x faster                                                 |
| logging_silent          | 111 ns                                                 | 90.9 ns: 1.22x faster                                                 |
| deltablue               | 3.92 ms                                                | 3.22 ms: 1.22x faster                                                 |
| unpickle_pure_python    | 242 us                                                 | 200 us: 1.21x faster                                                  |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.20 ms: 1.20x faster                                                 |
| richards                | 49.8 ms                                                | 42.0 ms: 1.19x faster                                                 |
| deepcopy_memo           | 40.2 us                                                | 34.2 us: 1.17x faster                                                 |
| pickle_list             | 4.59 us                                                | 3.95 us: 1.16x faster                                                 |
| scimark_sor             | 121 ms                                                 | 105 ms: 1.16x faster                                                  |
| pickle_pure_python      | 320 us                                                 | 282 us: 1.13x faster                                                  |
| hexiom                  | 6.89 ms                                                | 6.08 ms: 1.13x faster                                                 |
| mako                    | 10.7 ms                                                | 9.43 ms: 1.13x faster                                                 |
| spectral_norm           | 108 ms                                                 | 96.0 ms: 1.13x faster                                                 |
| json                    | 5.24 ms                                                | 4.67 ms: 1.12x faster                                                 |
| genshi_xml              | 53.4 ms                                                | 48.0 ms: 1.11x faster                                                 |
| mdp                     | 2.77 sec                                               | 2.50 sec: 1.11x faster                                                |
| xml_etree_parse         | 164 ms                                                 | 148 ms: 1.11x faster                                                  |
| scimark_fft             | 345 ms                                                 | 314 ms: 1.10x faster                                                  |
| pprint_pformat          | 1.55 sec                                               | 1.41 sec: 1.10x faster                                                |
| raytrace                | 309 ms                                                 | 281 ms: 1.10x faster                                                  |
| deepcopy                | 365 us                                                 | 332 us: 1.10x faster                                                  |
| nqueens                 | 87.9 ms                                                | 80.1 ms: 1.10x faster                                                 |
| pickle_dict             | 34.6 us                                                | 31.5 us: 1.10x faster                                                 |
| go                      | 149 ms                                                 | 136 ms: 1.10x faster                                                  |
| regex_compile           | 141 ms                                                 | 129 ms: 1.10x faster                                                  |
| scimark_lu              | 116 ms                                                 | 106 ms: 1.09x faster                                                  |
| sqlglot_optimize        | 55.3 ms                                                | 50.6 ms: 1.09x faster                                                 |
| pprint_safe_repr        | 747 ms                                                 | 686 ms: 1.09x faster                                                  |
| html5lib                | 64.8 ms                                                | 59.7 ms: 1.09x faster                                                 |
| pickle                  | 11.0 us                                                | 10.1 us: 1.08x faster                                                 |
| pycparser               | 1.19 sec                                               | 1.09 sec: 1.08x faster                                                |
| deepcopy_reduce         | 3.22 us                                                | 2.97 us: 1.08x faster                                                 |
| coroutines              | 27.0 ms                                                | 25.0 ms: 1.08x faster                                                 |
| scimark_monte_carlo     | 70.7 ms                                                | 65.4 ms: 1.08x faster                                                 |
| genshi_text             | 22.5 ms                                                | 20.9 ms: 1.08x faster                                                 |
| float                   | 78.9 ms                                                | 73.2 ms: 1.08x faster                                                 |
| sqlglot_normalize       | 113 ms                                                 | 105 ms: 1.08x faster                                                  |
| 2to3                    | 264 ms                                                 | 246 ms: 1.07x faster                                                  |
| chaos                   | 71.9 ms                                                | 66.9 ms: 1.07x faster                                                 |
| bench_thread_pool       | 834 us                                                 | 778 us: 1.07x faster                                                  |
| sqlglot_transpile       | 1.75 ms                                                | 1.63 ms: 1.07x faster                                                 |
| fannkuch                | 405 ms                                                 | 379 ms: 1.07x faster                                                  |
| pyflate                 | 434 ms                                                 | 405 ms: 1.07x faster                                                  |
| sqlglot_parse           | 1.43 ms                                                | 1.34 ms: 1.07x faster                                                 |
| telco                   | 6.86 ms                                                | 6.46 ms: 1.06x faster                                                 |
| logging_format          | 6.81 us                                                | 6.41 us: 1.06x faster                                                 |
| xml_etree_process       | 56.9 ms                                                | 53.7 ms: 1.06x faster                                                 |
| sympy_expand            | 484 ms                                                 | 458 ms: 1.06x faster                                                  |
| logging_simple          | 6.22 us                                                | 5.88 us: 1.06x faster                                                 |
| xml_etree_generate      | 81.1 ms                                                | 76.9 ms: 1.05x faster                                                 |
| async_generators        | 374 ms                                                 | 354 ms: 1.05x faster                                                  |
| gc_traversal            | 4.01 ms                                                | 3.81 ms: 1.05x faster                                                 |
| sympy_integrate         | 21.5 ms                                                | 20.4 ms: 1.05x faster                                                 |
| sympy_str               | 297 ms                                                 | 283 ms: 1.05x faster                                                  |
| unpickle_list           | 5.21 us                                                | 4.97 us: 1.05x faster                                                 |
| meteor_contest          | 109 ms                                                 | 104 ms: 1.05x faster                                                  |
| thrift                  | 784 us                                                 | 751 us: 1.04x faster                                                  |
| chameleon               | 6.70 ms                                                | 6.45 ms: 1.04x faster                                                 |
| unpickle                | 13.8 us                                                | 13.3 us: 1.04x faster                                                 |
| xml_etree_iterparse     | 108 ms                                                 | 104 ms: 1.04x faster                                                  |
| docutils                | 2.66 sec                                               | 2.57 sec: 1.04x faster                                                |
| dulwich_log             | 64.6 ms                                                | 62.5 ms: 1.03x faster                                                 |
| sympy_sum               | 169 ms                                                 | 164 ms: 1.03x faster                                                  |
| djangocms               | 33.5 us                                                | 32.6 us: 1.03x faster                                                 |
| pidigits                | 194 ms                                                 | 189 ms: 1.03x faster                                                  |
| regex_v8                | 22.9 ms                                                | 22.3 ms: 1.02x faster                                                 |
| nbody                   | 96.0 ms                                                | 94.0 ms: 1.02x faster                                                 |
| crypto_pyaes            | 76.7 ms                                                | 75.3 ms: 1.02x faster                                                 |
| django_template         | 33.5 ms                                                | 33.0 ms: 1.02x faster                                                 |
| pathlib                 | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                 |
| dask                    | 365 ms                                                 | 360 ms: 1.01x faster                                                  |
| python_startup          | 8.56 ms                                                | 8.52 ms: 1.00x faster                                                 |
| create_gc_cycles        | 1.43 ms                                                | 1.44 ms: 1.00x slower                                                 |
| python_startup_no_site  | 6.01 ms                                                | 6.07 ms: 1.01x slower                                                 |
| async_tree_none         | 528 ms                                                 | 536 ms: 1.02x slower                                                  |
| asyncio_tcp             | 875 ms                                                 | 890 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed | 749 ms                                                 | 769 ms: 1.03x slower                                                  |
| regex_effbot            | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                 |
| async_tree_io           | 1.29 sec                                               | 1.34 sec: 1.04x slower                                                |
| async_tree_memoization  | 639 ms                                                 | 665 ms: 1.04x slower                                                  |
| generators              | 74.9 ms                                                | 79.1 ms: 1.06x slower                                                 |
| regex_dna               | 205 ms                                                 | 217 ms: 1.06x slower                                                  |
| coverage                | 78.8 ms                                                | 102 ms: 1.30x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (4): unpack_sequence, comprehensions, bench_mp_pool, sqlite_synth
Ignored benchmarks (17) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.01x