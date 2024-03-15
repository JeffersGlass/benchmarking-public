
# Results vs. 3.11.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: linux-x86_64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 245 ms: 1.08x faster                                                  |
| chameleon      | 6.70 ms                                                | 6.30 ms: 1.06x faster                                                 |
| docutils       | 2.66 sec                                               | 2.50 sec: 1.07x faster                                                |
| html5lib       | 64.8 ms                                                | 58.9 ms: 1.10x faster                                                 |
| tornado_http   | 98.1 ms                                                | 93.1 ms: 1.05x faster                                                 |
| Geometric mean | (ref)                                                  | 1.07x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 730 ms: 1.03x faster                                                  |
| async_tree_memoization  | 639 ms                                                 | 653 ms: 1.02x slower                                                  |
| async_tree_io           | 1.29 sec                                               | 1.32 sec: 1.03x slower                                                |
| Geometric mean          | (ref)                                                  | 1.00x slower                                                          |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 78.9 ms                                                | 72.0 ms: 1.10x faster                                                 |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                  |
| nbody          | 96.0 ms                                                | 93.9 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 127 ms: 1.11x faster                                                  |
| regex_v8       | 22.9 ms                                                | 21.1 ms: 1.09x faster                                                 |
| regex_effbot   | 3.51 ms                                                | 3.47 ms: 1.01x faster                                                 |
| regex_dna      | 205 ms                                                 | 208 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.66 ms: 1.38x faster                                                 |
| json_loads           | 29.2 us                                                | 23.9 us: 1.22x faster                                                 |
| unpickle_pure_python | 242 us                                                 | 200 us: 1.21x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 283 us: 1.13x faster                                                  |
| pickle_list          | 4.59 us                                                | 4.06 us: 1.13x faster                                                 |
| pickle_dict          | 34.6 us                                                | 30.8 us: 1.12x faster                                                 |
| pickle               | 11.0 us                                                | 9.88 us: 1.11x faster                                                 |
| xml_etree_parse      | 164 ms                                                 | 149 ms: 1.10x faster                                                  |
| unpickle             | 13.8 us                                                | 12.9 us: 1.07x faster                                                 |
| xml_etree_process    | 56.9 ms                                                | 53.9 ms: 1.06x faster                                                 |
| xml_etree_generate   | 81.1 ms                                                | 77.2 ms: 1.05x faster                                                 |
| xml_etree_iterparse  | 108 ms                                                 | 103 ms: 1.05x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.98 us: 1.05x faster                                                 |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.58 ms: 1.00x slower                                                 |
| python_startup_no_site | 6.01 ms                                                | 6.12 ms: 1.02x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 47.0 ms: 1.14x faster                                                 |
| mako            | 10.7 ms                                                | 9.39 ms: 1.14x faster                                                 |
| genshi_text     | 22.5 ms                                                | 20.2 ms: 1.12x faster                                                 |
| django_template | 33.5 ms                                                | 32.8 ms: 1.02x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.10x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps              | 13.3 ms                                                | 9.66 ms: 1.38x faster                                                 |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.00 ms: 1.26x faster                                                 |
| json_loads              | 29.2 us                                                | 23.9 us: 1.22x faster                                                 |
| deltablue               | 3.92 ms                                                | 3.22 ms: 1.22x faster                                                 |
| unpickle_pure_python    | 242 us                                                 | 200 us: 1.21x faster                                                  |
| deepcopy_memo           | 40.2 us                                                | 33.6 us: 1.19x faster                                                 |
| richards                | 49.8 ms                                                | 41.8 ms: 1.19x faster                                                 |
| logging_silent          | 111 ns                                                 | 93.4 ns: 1.19x faster                                                 |
| scimark_sor             | 121 ms                                                 | 105 ms: 1.16x faster                                                  |
| hexiom                  | 6.89 ms                                                | 6.04 ms: 1.14x faster                                                 |
| spectral_norm           | 108 ms                                                 | 94.9 ms: 1.14x faster                                                 |
| genshi_xml              | 53.4 ms                                                | 47.0 ms: 1.14x faster                                                 |
| mako                    | 10.7 ms                                                | 9.39 ms: 1.14x faster                                                 |
| pickle_pure_python      | 320 us                                                 | 283 us: 1.13x faster                                                  |
| pickle_list             | 4.59 us                                                | 4.06 us: 1.13x faster                                                 |
| json                    | 5.24 ms                                                | 4.65 ms: 1.13x faster                                                 |
| pickle_dict             | 34.6 us                                                | 30.8 us: 1.12x faster                                                 |
| scimark_fft             | 345 ms                                                 | 309 ms: 1.12x faster                                                  |
| pprint_pformat          | 1.55 sec                                               | 1.39 sec: 1.12x faster                                                |
| genshi_text             | 22.5 ms                                                | 20.2 ms: 1.12x faster                                                 |
| mdp                     | 2.77 sec                                               | 2.48 sec: 1.12x faster                                                |
| aiohttp                 | 1.12 ms                                                | 999 us: 1.12x faster                                                  |
| raytrace                | 309 ms                                                 | 277 ms: 1.12x faster                                                  |
| deepcopy                | 365 us                                                 | 328 us: 1.11x faster                                                  |
| deepcopy_reduce         | 3.22 us                                                | 2.89 us: 1.11x faster                                                 |
| regex_compile           | 141 ms                                                 | 127 ms: 1.11x faster                                                  |
| pickle                  | 11.0 us                                                | 9.88 us: 1.11x faster                                                 |
| gunicorn                | 1.20 ms                                                | 1.08 ms: 1.11x faster                                                 |
| go                      | 149 ms                                                 | 135 ms: 1.10x faster                                                  |
| xml_etree_parse         | 164 ms                                                 | 149 ms: 1.10x faster                                                  |
| pycparser               | 1.19 sec                                               | 1.08 sec: 1.10x faster                                                |
| html5lib                | 64.8 ms                                                | 58.9 ms: 1.10x faster                                                 |
| fannkuch                | 405 ms                                                 | 369 ms: 1.10x faster                                                  |
| float                   | 78.9 ms                                                | 72.0 ms: 1.10x faster                                                 |
| logging_simple          | 6.22 us                                                | 5.70 us: 1.09x faster                                                 |
| coroutines              | 27.0 ms                                                | 24.7 ms: 1.09x faster                                                 |
| chaos                   | 71.9 ms                                                | 65.8 ms: 1.09x faster                                                 |
| pprint_safe_repr        | 747 ms                                                 | 685 ms: 1.09x faster                                                  |
| regex_v8                | 22.9 ms                                                | 21.1 ms: 1.09x faster                                                 |
| sqlglot_optimize        | 55.3 ms                                                | 51.0 ms: 1.08x faster                                                 |
| nqueens                 | 87.9 ms                                                | 81.1 ms: 1.08x faster                                                 |
| sqlglot_transpile       | 1.75 ms                                                | 1.62 ms: 1.08x faster                                                 |
| logging_format          | 6.81 us                                                | 6.30 us: 1.08x faster                                                 |
| pyflate                 | 434 ms                                                 | 402 ms: 1.08x faster                                                  |
| 2to3                    | 264 ms                                                 | 245 ms: 1.08x faster                                                  |
| sqlglot_parse           | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                 |
| scimark_lu              | 116 ms                                                 | 108 ms: 1.08x faster                                                  |
| telco                   | 6.86 ms                                                | 6.38 ms: 1.08x faster                                                 |
| unpickle                | 13.8 us                                                | 12.9 us: 1.07x faster                                                 |
| bench_thread_pool       | 834 us                                                 | 780 us: 1.07x faster                                                  |
| sqlglot_normalize       | 113 ms                                                 | 105 ms: 1.07x faster                                                  |
| meteor_contest          | 109 ms                                                 | 102 ms: 1.07x faster                                                  |
| docutils                | 2.66 sec                                               | 2.50 sec: 1.07x faster                                                |
| chameleon               | 6.70 ms                                                | 6.30 ms: 1.06x faster                                                 |
| sympy_expand            | 484 ms                                                 | 456 ms: 1.06x faster                                                  |
| gc_traversal            | 4.01 ms                                                | 3.77 ms: 1.06x faster                                                 |
| xml_etree_process       | 56.9 ms                                                | 53.9 ms: 1.06x faster                                                 |
| sympy_integrate         | 21.5 ms                                                | 20.4 ms: 1.05x faster                                                 |
| sympy_str               | 297 ms                                                 | 282 ms: 1.05x faster                                                  |
| tornado_http            | 98.1 ms                                                | 93.1 ms: 1.05x faster                                                 |
| async_generators        | 374 ms                                                 | 355 ms: 1.05x faster                                                  |
| xml_etree_generate      | 81.1 ms                                                | 77.2 ms: 1.05x faster                                                 |
| thrift                  | 784 us                                                 | 748 us: 1.05x faster                                                  |
| xml_etree_iterparse     | 108 ms                                                 | 103 ms: 1.05x faster                                                  |
| unpickle_list           | 5.21 us                                                | 4.98 us: 1.05x faster                                                 |
| dulwich_log             | 64.6 ms                                                | 61.8 ms: 1.05x faster                                                 |
| pathlib                 | 18.5 ms                                                | 17.7 ms: 1.04x faster                                                 |
| scimark_monte_carlo     | 70.7 ms                                                | 68.0 ms: 1.04x faster                                                 |
| djangocms               | 33.5 us                                                | 32.5 us: 1.03x faster                                                 |
| crypto_pyaes            | 76.7 ms                                                | 74.6 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed | 749 ms                                                 | 730 ms: 1.03x faster                                                  |
| pidigits                | 194 ms                                                 | 189 ms: 1.03x faster                                                  |
| sympy_sum               | 169 ms                                                 | 165 ms: 1.02x faster                                                  |
| nbody                   | 96.0 ms                                                | 93.9 ms: 1.02x faster                                                 |
| django_template         | 33.5 ms                                                | 32.8 ms: 1.02x faster                                                 |
| dask                    | 365 ms                                                 | 360 ms: 1.01x faster                                                  |
| regex_effbot            | 3.51 ms                                                | 3.47 ms: 1.01x faster                                                 |
| comprehensions          | 23.6 us                                                | 23.4 us: 1.01x faster                                                 |
| python_startup          | 8.56 ms                                                | 8.58 ms: 1.00x slower                                                 |
| asyncio_tcp             | 875 ms                                                 | 884 ms: 1.01x slower                                                  |
| sqlite_synth            | 2.57 us                                                | 2.60 us: 1.01x slower                                                 |
| regex_dna               | 205 ms                                                 | 208 ms: 1.01x slower                                                  |
| create_gc_cycles        | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                 |
| python_startup_no_site  | 6.01 ms                                                | 6.12 ms: 1.02x slower                                                 |
| async_tree_memoization  | 639 ms                                                 | 653 ms: 1.02x slower                                                  |
| async_tree_io           | 1.29 sec                                               | 1.32 sec: 1.03x slower                                                |
| generators              | 74.9 ms                                                | 77.4 ms: 1.03x slower                                                 |
| unpack_sequence         | 43.5 ns                                                | 45.7 ns: 1.05x slower                                                 |
| coverage                | 78.8 ms                                                | 101 ms: 1.28x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (2): async_tree_none, bench_mp_pool
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 1.01x