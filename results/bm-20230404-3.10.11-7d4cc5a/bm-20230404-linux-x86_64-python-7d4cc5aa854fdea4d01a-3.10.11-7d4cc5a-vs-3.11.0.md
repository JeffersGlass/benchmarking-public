
# Results vs. 3.11.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: linux-x86_64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.21x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 335 ms: 1.27x slower                                                 |
| chameleon      | 6.70 ms                                                | 8.93 ms: 1.33x slower                                                |
| docutils       | 2.66 sec                                               | 3.21 sec: 1.20x slower                                               |
| html5lib       | 64.8 ms                                                | 85.4 ms: 1.32x slower                                                |
| tornado_http   | 98.1 ms                                                | 131 ms: 1.33x slower                                                 |
| Geometric mean | (ref)                                                  | 1.29x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 975 ms: 1.30x slower                                                 |
| async_tree_memoization  | 639 ms                                                 | 873 ms: 1.37x slower                                                 |
| async_tree_none         | 528 ms                                                 | 732 ms: 1.39x slower                                                 |
| async_tree_io           | 1.29 sec                                               | 1.82 sec: 1.41x slower                                               |
| Geometric mean          | (ref)                                                  | 1.37x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                 |
| float          | 78.9 ms                                                | 108 ms: 1.37x slower                                                 |
| nbody          | 96.0 ms                                                | 137 ms: 1.43x slower                                                 |
| Geometric mean | (ref)                                                  | 1.24x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                |
| regex_dna      | 205 ms                                                 | 213 ms: 1.04x slower                                                 |
| regex_v8       | 22.9 ms                                                | 25.5 ms: 1.11x slower                                                |
| regex_compile  | 141 ms                                                 | 176 ms: 1.25x slower                                                 |
| Geometric mean | (ref)                                                  | 1.11x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_list        | 5.21 us                                                | 4.80 us: 1.09x faster                                                |
| pickle               | 11.0 us                                                | 10.4 us: 1.06x faster                                                |
| pickle_list          | 4.59 us                                                | 4.38 us: 1.05x faster                                                |
| pickle_dict          | 34.6 us                                                | 33.7 us: 1.03x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 163 ms: 1.01x faster                                                 |
| json_loads           | 29.2 us                                                | 29.0 us: 1.01x faster                                                |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                 |
| json_dumps           | 13.3 ms                                                | 13.6 ms: 1.02x slower                                                |
| unpickle             | 13.8 us                                                | 14.3 us: 1.03x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 93.1 ms: 1.15x slower                                                |
| unpickle_pure_python | 242 us                                                 | 298 us: 1.23x slower                                                 |
| xml_etree_process    | 56.9 ms                                                | 74.1 ms: 1.30x slower                                                |
| pickle_pure_python   | 320 us                                                 | 452 us: 1.41x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.06x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 5.83 ms: 1.03x faster                                                |
| python_startup         | 8.56 ms                                                | 14.2 ms: 1.66x slower                                                |
| Geometric mean         | (ref)                                                  | 1.27x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 62.6 ms: 1.17x slower                                                |
| genshi_text     | 22.5 ms                                                | 30.1 ms: 1.33x slower                                                |
| django_template | 33.5 ms                                                | 45.8 ms: 1.36x slower                                                |
| mako            | 10.7 ms                                                | 14.7 ms: 1.38x slower                                                |
| Geometric mean  | (ref)                                                  | 1.31x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| coverage                | 78.8 ms                                                | 72.1 ms: 1.09x faster                                                |
| unpickle_list           | 5.21 us                                                | 4.80 us: 1.09x faster                                                |
| gc_traversal            | 4.01 ms                                                | 3.71 ms: 1.08x faster                                                |
| pickle                  | 11.0 us                                                | 10.4 us: 1.06x faster                                                |
| pickle_list             | 4.59 us                                                | 4.38 us: 1.05x faster                                                |
| python_startup_no_site  | 6.01 ms                                                | 5.83 ms: 1.03x faster                                                |
| pidigits                | 194 ms                                                 | 188 ms: 1.03x faster                                                 |
| pickle_dict             | 34.6 us                                                | 33.7 us: 1.03x faster                                                |
| telco                   | 6.86 ms                                                | 6.78 ms: 1.01x faster                                                |
| xml_etree_parse         | 164 ms                                                 | 163 ms: 1.01x faster                                                 |
| json_loads              | 29.2 us                                                | 29.0 us: 1.01x faster                                                |
| generators              | 74.9 ms                                                | 75.5 ms: 1.01x slower                                                |
| json                    | 5.24 ms                                                | 5.32 ms: 1.01x slower                                                |
| xml_etree_iterparse     | 108 ms                                                 | 110 ms: 1.02x slower                                                 |
| asyncio_tcp             | 875 ms                                                 | 894 ms: 1.02x slower                                                 |
| json_dumps              | 13.3 ms                                                | 13.6 ms: 1.02x slower                                                |
| mdp                     | 2.77 sec                                               | 2.85 sec: 1.03x slower                                               |
| unpickle                | 13.8 us                                                | 14.3 us: 1.03x slower                                                |
| regex_effbot            | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                |
| meteor_contest          | 109 ms                                                 | 113 ms: 1.04x slower                                                 |
| regex_dna               | 205 ms                                                 | 213 ms: 1.04x slower                                                 |
| pathlib                 | 18.5 ms                                                | 19.9 ms: 1.07x slower                                                |
| scimark_sparse_mat_mult | 5.03 ms                                                | 5.50 ms: 1.09x slower                                                |
| pylint                  | 476 ms                                                 | 526 ms: 1.11x slower                                                 |
| sympy_str               | 297 ms                                                 | 330 ms: 1.11x slower                                                 |
| bench_thread_pool       | 834 us                                                 | 925 us: 1.11x slower                                                 |
| djangocms               | 33.5 us                                                | 37.3 us: 1.11x slower                                                |
| regex_v8                | 22.9 ms                                                | 25.5 ms: 1.11x slower                                                |
| nqueens                 | 87.9 ms                                                | 97.9 ms: 1.11x slower                                                |
| sympy_sum               | 169 ms                                                 | 188 ms: 1.12x slower                                                 |
| sympy_expand            | 484 ms                                                 | 545 ms: 1.12x slower                                                 |
| async_generators        | 374 ms                                                 | 421 ms: 1.13x slower                                                 |
| sympy_integrate         | 21.5 ms                                                | 24.3 ms: 1.13x slower                                                |
| comprehensions          | 23.6 us                                                | 27.0 us: 1.14x slower                                                |
| sqlalchemy_imperative   | 18.3 ms                                                | 21.0 ms: 1.15x slower                                                |
| coroutines              | 27.0 ms                                                | 31.0 ms: 1.15x slower                                                |
| xml_etree_generate      | 81.1 ms                                                | 93.1 ms: 1.15x slower                                                |
| dask                    | 365 ms                                                 | 421 ms: 1.15x slower                                                 |
| aiohttp                 | 1.12 ms                                                | 1.29 ms: 1.16x slower                                                |
| create_gc_cycles        | 1.43 ms                                                | 1.66 ms: 1.16x slower                                                |
| gunicorn                | 1.20 ms                                                | 1.39 ms: 1.16x slower                                                |
| fannkuch                | 405 ms                                                 | 471 ms: 1.16x slower                                                 |
| dulwich_log             | 64.6 ms                                                | 75.5 ms: 1.17x slower                                                |
| genshi_xml              | 53.4 ms                                                | 62.6 ms: 1.17x slower                                                |
| flaskblogging           | 7.28 ms                                                | 8.53 ms: 1.17x slower                                                |
| deepcopy_reduce         | 3.22 us                                                | 3.77 us: 1.17x slower                                                |
| deepcopy                | 365 us                                                 | 429 us: 1.17x slower                                                 |
| sqlite_synth            | 2.57 us                                                | 3.02 us: 1.18x slower                                                |
| sqlglot_optimize        | 55.3 ms                                                | 65.5 ms: 1.18x slower                                                |
| sqlalchemy_declarative  | 140 ms                                                 | 168 ms: 1.19x slower                                                 |
| docutils                | 2.66 sec                                               | 3.21 sec: 1.20x slower                                               |
| sqlglot_normalize       | 113 ms                                                 | 136 ms: 1.20x slower                                                 |
| scimark_fft             | 345 ms                                                 | 416 ms: 1.20x slower                                                 |
| unpickle_pure_python    | 242 us                                                 | 298 us: 1.23x slower                                                 |
| deepcopy_memo           | 40.2 us                                                | 49.8 us: 1.24x slower                                                |
| regex_compile           | 141 ms                                                 | 176 ms: 1.25x slower                                                 |
| pprint_pformat          | 1.55 sec                                               | 1.97 sec: 1.27x slower                                               |
| 2to3                    | 264 ms                                                 | 335 ms: 1.27x slower                                                 |
| pprint_safe_repr        | 747 ms                                                 | 953 ms: 1.28x slower                                                 |
| pycparser               | 1.19 sec                                               | 1.52 sec: 1.28x slower                                               |
| async_tree_cpu_io_mixed | 749 ms                                                 | 975 ms: 1.30x slower                                                 |
| xml_etree_process       | 56.9 ms                                                | 74.1 ms: 1.30x slower                                                |
| spectral_norm           | 108 ms                                                 | 142 ms: 1.32x slower                                                 |
| html5lib                | 64.8 ms                                                | 85.4 ms: 1.32x slower                                                |
| thrift                  | 784 us                                                 | 1.04 ms: 1.33x slower                                                |
| tornado_http            | 98.1 ms                                                | 131 ms: 1.33x slower                                                 |
| chameleon               | 6.70 ms                                                | 8.93 ms: 1.33x slower                                                |
| genshi_text             | 22.5 ms                                                | 30.1 ms: 1.33x slower                                                |
| logging_format          | 6.81 us                                                | 9.16 us: 1.35x slower                                                |
| logging_simple          | 6.22 us                                                | 8.40 us: 1.35x slower                                                |
| scimark_lu              | 116 ms                                                 | 159 ms: 1.36x slower                                                 |
| django_template         | 33.5 ms                                                | 45.8 ms: 1.36x slower                                                |
| float                   | 78.9 ms                                                | 108 ms: 1.37x slower                                                 |
| async_tree_memoization  | 639 ms                                                 | 873 ms: 1.37x slower                                                 |
| hexiom                  | 6.89 ms                                                | 9.41 ms: 1.37x slower                                                |
| mako                    | 10.7 ms                                                | 14.7 ms: 1.38x slower                                                |
| async_tree_none         | 528 ms                                                 | 732 ms: 1.39x slower                                                 |
| sqlglot_transpile       | 1.75 ms                                                | 2.44 ms: 1.39x slower                                                |
| async_tree_io           | 1.29 sec                                               | 1.82 sec: 1.41x slower                                               |
| pickle_pure_python      | 320 us                                                 | 452 us: 1.41x slower                                                 |
| sqlglot_parse           | 1.43 ms                                                | 2.04 ms: 1.43x slower                                                |
| nbody                   | 96.0 ms                                                | 137 ms: 1.43x slower                                                 |
| chaos                   | 71.9 ms                                                | 105 ms: 1.45x slower                                                 |
| richards                | 49.8 ms                                                | 73.1 ms: 1.47x slower                                                |
| crypto_pyaes            | 76.7 ms                                                | 114 ms: 1.49x slower                                                 |
| raytrace                | 309 ms                                                 | 462 ms: 1.50x slower                                                 |
| pyflate                 | 434 ms                                                 | 660 ms: 1.52x slower                                                 |
| go                      | 149 ms                                                 | 227 ms: 1.53x slower                                                 |
| scimark_monte_carlo     | 70.7 ms                                                | 109 ms: 1.54x slower                                                 |
| unpack_sequence         | 43.5 ns                                                | 67.6 ns: 1.56x slower                                                |
| logging_silent          | 111 ns                                                 | 175 ns: 1.57x slower                                                 |
| scimark_sor             | 121 ms                                                 | 194 ms: 1.60x slower                                                 |
| python_startup          | 8.56 ms                                                | 14.2 ms: 1.66x slower                                                |
| deltablue               | 3.92 ms                                                | 7.35 ms: 1.87x slower                                                |
| Geometric mean          | (ref)                                                  | 1.21x slower                                                         |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.17x
- 95% likely to have a slowdown of 1.16x
- 99% likely to have a slowdown of 1.15x


# Memory

- memory change: 0.95x