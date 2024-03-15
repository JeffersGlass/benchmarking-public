
# Results vs. 3.10.4

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: linux-x86_64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.06x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 335 ms: 1.04x faster                                                 |
| chameleon      | 9.68 ms                                                | 8.93 ms: 1.08x faster                                                |
| docutils       | 3.30 sec                                               | 3.21 sec: 1.03x faster                                               |
| html5lib       | 88.9 ms                                                | 85.4 ms: 1.04x faster                                                |
| tornado_http   | 136 ms                                                 | 131 ms: 1.04x faster                                                 |
| Geometric mean | (ref)                                                  | 1.05x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 1.02 sec                                               | 975 ms: 1.04x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.82 sec: 1.03x slower                                               |
| Geometric mean          | (ref)                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 137 ms: 1.12x faster                                                 |
| float          | 117 ms                                                 | 108 ms: 1.09x faster                                                 |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.07x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                |
| regex_compile  | 188 ms                                                 | 176 ms: 1.07x faster                                                 |
| regex_dna      | 227 ms                                                 | 213 ms: 1.06x faster                                                 |
| Geometric mean | (ref)                                                  | 1.06x faster                                                         |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.38 us: 1.16x faster                                                |
| unpickle_pure_python | 331 us                                                 | 298 us: 1.11x faster                                                 |
| unpickle_list        | 5.20 us                                                | 4.80 us: 1.08x faster                                                |
| json_loads           | 31.2 us                                                | 29.0 us: 1.08x faster                                                |
| pickle_pure_python   | 484 us                                                 | 452 us: 1.07x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 93.1 ms: 1.07x faster                                                |
| xml_etree_process    | 79.1 ms                                                | 74.1 ms: 1.07x faster                                                |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                 |
| json_dumps           | 14.2 ms                                                | 13.6 ms: 1.04x faster                                                |
| xml_etree_parse      | 168 ms                                                 | 163 ms: 1.03x faster                                                 |
| pickle               | 10.7 us                                                | 10.4 us: 1.03x faster                                                |
| unpickle             | 14.4 us                                                | 14.3 us: 1.00x faster                                                |
| pickle_dict          | 29.6 us                                                | 33.7 us: 1.14x slower                                                |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 14.2 ms: 1.03x faster                                                |
| python_startup_no_site | 5.93 ms                                                | 5.83 ms: 1.02x faster                                                |
| Geometric mean         | (ref)                                                  | 1.02x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 14.7 ms: 1.11x faster                                                |
| genshi_text     | 31.8 ms                                                | 30.1 ms: 1.06x faster                                                |
| genshi_xml      | 66.0 ms                                                | 62.6 ms: 1.05x faster                                                |
| django_template | 48.2 ms                                                | 45.8 ms: 1.05x faster                                                |
| Geometric mean  | (ref)                                                  | 1.07x faster                                                         |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-linux-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| spectral_norm           | 170 ms                                                 | 142 ms: 1.19x faster                                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 5.50 ms: 1.18x faster                                                |
| deepcopy_memo           | 58.5 us                                                | 49.8 us: 1.17x faster                                                |
| pickle_list             | 5.08 us                                                | 4.38 us: 1.16x faster                                                |
| scimark_sor             | 220 ms                                                 | 194 ms: 1.13x faster                                                 |
| coroutines              | 35.1 ms                                                | 31.0 ms: 1.13x faster                                                |
| fannkuch                | 532 ms                                                 | 471 ms: 1.13x faster                                                 |
| crypto_pyaes            | 128 ms                                                 | 114 ms: 1.12x faster                                                 |
| scimark_fft             | 466 ms                                                 | 416 ms: 1.12x faster                                                 |
| dulwich_log             | 84.3 ms                                                | 75.5 ms: 1.12x faster                                                |
| deepcopy                | 479 us                                                 | 429 us: 1.12x faster                                                 |
| nbody                   | 154 ms                                                 | 137 ms: 1.12x faster                                                 |
| aiohttp                 | 1.44 ms                                                | 1.29 ms: 1.11x faster                                                |
| sqlalchemy_imperative   | 23.3 ms                                                | 21.0 ms: 1.11x faster                                                |
| scimark_lu              | 176 ms                                                 | 159 ms: 1.11x faster                                                 |
| unpickle_pure_python    | 331 us                                                 | 298 us: 1.11x faster                                                 |
| mako                    | 16.3 ms                                                | 14.7 ms: 1.11x faster                                                |
| deepcopy_reduce         | 4.17 us                                                | 3.77 us: 1.11x faster                                                |
| chaos                   | 115 ms                                                 | 105 ms: 1.10x faster                                                 |
| hexiom                  | 10.4 ms                                                | 9.41 ms: 1.10x faster                                                |
| coverage                | 79.4 ms                                                | 72.1 ms: 1.10x faster                                                |
| gunicorn                | 1.53 ms                                                | 1.39 ms: 1.10x faster                                                |
| raytrace                | 507 ms                                                 | 462 ms: 1.10x faster                                                 |
| regex_v8                | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                |
| logging_silent          | 190 ns                                                 | 175 ns: 1.09x faster                                                 |
| float                   | 117 ms                                                 | 108 ms: 1.09x faster                                                 |
| pyflate                 | 716 ms                                                 | 660 ms: 1.09x faster                                                 |
| scimark_monte_carlo     | 118 ms                                                 | 109 ms: 1.08x faster                                                 |
| chameleon               | 9.68 ms                                                | 8.93 ms: 1.08x faster                                                |
| richards                | 79.3 ms                                                | 73.1 ms: 1.08x faster                                                |
| unpickle_list           | 5.20 us                                                | 4.80 us: 1.08x faster                                                |
| nqueens                 | 106 ms                                                 | 97.9 ms: 1.08x faster                                                |
| deltablue               | 7.91 ms                                                | 7.35 ms: 1.08x faster                                                |
| json_loads              | 31.2 us                                                | 29.0 us: 1.08x faster                                                |
| telco                   | 7.27 ms                                                | 6.78 ms: 1.07x faster                                                |
| pickle_pure_python      | 484 us                                                 | 452 us: 1.07x faster                                                 |
| regex_compile           | 188 ms                                                 | 176 ms: 1.07x faster                                                 |
| json                    | 5.69 ms                                                | 5.32 ms: 1.07x faster                                                |
| xml_etree_generate      | 99.4 ms                                                | 93.1 ms: 1.07x faster                                                |
| pprint_safe_repr        | 1.02 sec                                               | 953 ms: 1.07x faster                                                 |
| xml_etree_process       | 79.1 ms                                                | 74.1 ms: 1.07x faster                                                |
| pprint_pformat          | 2.10 sec                                               | 1.97 sec: 1.07x faster                                               |
| bench_thread_pool       | 986 us                                                 | 925 us: 1.07x faster                                                 |
| comprehensions          | 28.8 us                                                | 27.0 us: 1.06x faster                                                |
| regex_dna               | 227 ms                                                 | 213 ms: 1.06x faster                                                 |
| sympy_integrate         | 25.8 ms                                                | 24.3 ms: 1.06x faster                                                |
| generators              | 80.1 ms                                                | 75.5 ms: 1.06x faster                                                |
| sqlglot_parse           | 2.17 ms                                                | 2.04 ms: 1.06x faster                                                |
| genshi_text             | 31.8 ms                                                | 30.1 ms: 1.06x faster                                                |
| meteor_contest          | 120 ms                                                 | 113 ms: 1.06x faster                                                 |
| sqlglot_transpile       | 2.57 ms                                                | 2.44 ms: 1.06x faster                                                |
| go                      | 240 ms                                                 | 227 ms: 1.06x faster                                                 |
| sqlglot_optimize        | 69.2 ms                                                | 65.5 ms: 1.06x faster                                                |
| genshi_xml              | 66.0 ms                                                | 62.6 ms: 1.05x faster                                                |
| async_generators        | 444 ms                                                 | 421 ms: 1.05x faster                                                 |
| sqlglot_normalize       | 143 ms                                                 | 136 ms: 1.05x faster                                                 |
| django_template         | 48.2 ms                                                | 45.8 ms: 1.05x faster                                                |
| sympy_str               | 346 ms                                                 | 330 ms: 1.05x faster                                                 |
| dask                    | 441 ms                                                 | 421 ms: 1.05x faster                                                 |
| pylint                  | 551 ms                                                 | 526 ms: 1.05x faster                                                 |
| xml_etree_iterparse     | 115 ms                                                 | 110 ms: 1.05x faster                                                 |
| tornado_http            | 136 ms                                                 | 131 ms: 1.04x faster                                                 |
| sympy_sum               | 196 ms                                                 | 188 ms: 1.04x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 975 ms: 1.04x faster                                                 |
| html5lib                | 88.9 ms                                                | 85.4 ms: 1.04x faster                                                |
| json_dumps              | 14.2 ms                                                | 13.6 ms: 1.04x faster                                                |
| 2to3                    | 348 ms                                                 | 335 ms: 1.04x faster                                                 |
| sympy_expand            | 566 ms                                                 | 545 ms: 1.04x faster                                                 |
| pycparser               | 1.58 sec                                               | 1.52 sec: 1.03x faster                                               |
| xml_etree_parse         | 168 ms                                                 | 163 ms: 1.03x faster                                                 |
| djangocms               | 38.4 us                                                | 37.3 us: 1.03x faster                                                |
| asyncio_tcp             | 922 ms                                                 | 894 ms: 1.03x faster                                                 |
| pathlib                 | 20.5 ms                                                | 19.9 ms: 1.03x faster                                                |
| thrift                  | 1.07 ms                                                | 1.04 ms: 1.03x faster                                                |
| docutils                | 3.30 sec                                               | 3.21 sec: 1.03x faster                                               |
| pickle                  | 10.7 us                                                | 10.4 us: 1.03x faster                                                |
| sqlalchemy_declarative  | 172 ms                                                 | 168 ms: 1.03x faster                                                 |
| python_startup          | 14.6 ms                                                | 14.2 ms: 1.03x faster                                                |
| python_startup_no_site  | 5.93 ms                                                | 5.83 ms: 1.02x faster                                                |
| pidigits                | 191 ms                                                 | 188 ms: 1.01x faster                                                 |
| unpickle                | 14.4 us                                                | 14.3 us: 1.00x faster                                                |
| logging_format          | 9.09 us                                                | 9.16 us: 1.01x slower                                                |
| logging_simple          | 8.30 us                                                | 8.40 us: 1.01x slower                                                |
| gc_traversal            | 3.62 ms                                                | 3.71 ms: 1.02x slower                                                |
| create_gc_cycles        | 1.62 ms                                                | 1.66 ms: 1.03x slower                                                |
| async_tree_io           | 1.77 sec                                               | 1.82 sec: 1.03x slower                                               |
| unpack_sequence         | 60.0 ns                                                | 67.6 ns: 1.13x slower                                                |
| pickle_dict             | 29.6 us                                                | 33.7 us: 1.14x slower                                                |
| Geometric mean          | (ref)                                                  | 1.06x faster                                                         |

Benchmark hidden because not significant (7): flaskblogging, regex_effbot, bench_mp_pool, sqlite_synth, mdp, async_tree_memoization, async_tree_none
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.02x