
# Results vs. 3.11.0

- fork: python
- ref: v3.11.0b2
- machine: linux-x86_64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 256 ms: 1.03x faster                                       |
| chameleon      | 6.70 ms                                                | 6.62 ms: 1.01x faster                                      |
| docutils       | 2.66 sec                                               | 2.56 sec: 1.04x faster                                     |
| html5lib       | 64.8 ms                                                | 63.7 ms: 1.02x faster                                      |
| tornado_http   | 98.1 ms                                                | 94.9 ms: 1.03x faster                                      |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_memoization  | 639 ms                                                 | 628 ms: 1.02x faster                                       |
| async_tree_cpu_io_mixed | 749 ms                                                 | 743 ms: 1.01x faster                                       |
| async_tree_io           | 1.29 sec                                               | 1.31 sec: 1.02x slower                                     |
| Geometric mean          | (ref)                                                  | 1.00x faster                                               |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| float          | 78.9 ms                                                | 74.4 ms: 1.06x faster                                      |
| nbody          | 96.0 ms                                                | 92.0 ms: 1.04x faster                                      |
| pidigits       | 194 ms                                                 | 199 ms: 1.03x slower                                       |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.11 ms: 1.13x faster                                      |
| regex_dna      | 205 ms                                                 | 196 ms: 1.04x faster                                       |
| regex_v8       | 22.9 ms                                                | 22.0 ms: 1.04x faster                                      |
| regex_compile  | 141 ms                                                 | 138 ms: 1.03x faster                                       |
| Geometric mean | (ref)                                                  | 1.06x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 26.4 us: 1.31x faster                                      |
| json_loads           | 29.2 us                                                | 25.0 us: 1.17x faster                                      |
| pickle               | 11.0 us                                                | 9.44 us: 1.16x faster                                      |
| unpickle_pure_python | 242 us                                                 | 227 us: 1.07x faster                                       |
| pickle_list          | 4.59 us                                                | 4.30 us: 1.07x faster                                      |
| xml_etree_process    | 56.9 ms                                                | 53.4 ms: 1.07x faster                                      |
| xml_etree_generate   | 81.1 ms                                                | 76.1 ms: 1.07x faster                                      |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                       |
| json_dumps           | 13.3 ms                                                | 12.8 ms: 1.05x faster                                      |
| unpickle_list        | 5.21 us                                                | 5.00 us: 1.04x faster                                      |
| unpickle             | 13.8 us                                                | 13.3 us: 1.04x faster                                      |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                       |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.02x faster                                       |
| Geometric mean       | (ref)                                                  | 1.09x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.49 ms: 1.01x faster                                      |
| python_startup_no_site | 6.01 ms                                                | 5.99 ms: 1.00x faster                                      |
| Geometric mean         | (ref)                                                  | 1.01x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.96 ms: 1.07x faster                                      |
| genshi_text     | 22.5 ms                                                | 21.5 ms: 1.05x faster                                      |
| django_template | 33.5 ms                                                | 32.6 ms: 1.03x faster                                      |
| genshi_xml      | 53.4 ms                                                | 52.4 ms: 1.02x faster                                      |
| Geometric mean  | (ref)                                                  | 1.04x faster                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 26.4 us: 1.31x faster                                      |
| json_loads              | 29.2 us                                                | 25.0 us: 1.17x faster                                      |
| pickle                  | 11.0 us                                                | 9.44 us: 1.16x faster                                      |
| regex_effbot            | 3.51 ms                                                | 3.11 ms: 1.13x faster                                      |
| deepcopy_memo           | 40.2 us                                                | 35.9 us: 1.12x faster                                      |
| richards                | 49.8 ms                                                | 44.5 ms: 1.12x faster                                      |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.51 ms: 1.11x faster                                      |
| spectral_norm           | 108 ms                                                 | 97.3 ms: 1.11x faster                                      |
| json                    | 5.24 ms                                                | 4.75 ms: 1.10x faster                                      |
| hexiom                  | 6.89 ms                                                | 6.27 ms: 1.10x faster                                      |
| logging_simple          | 6.22 us                                                | 5.74 us: 1.08x faster                                      |
| logging_silent          | 111 ns                                                 | 103 ns: 1.08x faster                                       |
| raytrace                | 309 ms                                                 | 287 ms: 1.08x faster                                       |
| deepcopy                | 365 us                                                 | 340 us: 1.08x faster                                       |
| pprint_pformat          | 1.55 sec                                               | 1.45 sec: 1.07x faster                                     |
| logging_format          | 6.81 us                                                | 6.34 us: 1.07x faster                                      |
| scimark_monte_carlo     | 70.7 ms                                                | 66.0 ms: 1.07x faster                                      |
| go                      | 149 ms                                                 | 139 ms: 1.07x faster                                       |
| mako                    | 10.7 ms                                                | 9.96 ms: 1.07x faster                                      |
| pprint_safe_repr        | 747 ms                                                 | 699 ms: 1.07x faster                                       |
| chaos                   | 71.9 ms                                                | 67.3 ms: 1.07x faster                                      |
| unpickle_pure_python    | 242 us                                                 | 227 us: 1.07x faster                                       |
| scimark_lu              | 116 ms                                                 | 109 ms: 1.07x faster                                       |
| pickle_list             | 4.59 us                                                | 4.30 us: 1.07x faster                                      |
| xml_etree_process       | 56.9 ms                                                | 53.4 ms: 1.07x faster                                      |
| xml_etree_generate      | 81.1 ms                                                | 76.1 ms: 1.07x faster                                      |
| gunicorn                | 1.20 ms                                                | 1.13 ms: 1.06x faster                                      |
| deepcopy_reduce         | 3.22 us                                                | 3.03 us: 1.06x faster                                      |
| float                   | 78.9 ms                                                | 74.4 ms: 1.06x faster                                      |
| scimark_sor             | 121 ms                                                 | 115 ms: 1.06x faster                                       |
| async_generators        | 374 ms                                                 | 354 ms: 1.06x faster                                       |
| aiohttp                 | 1.12 ms                                                | 1.06 ms: 1.06x faster                                      |
| coroutines              | 27.0 ms                                                | 25.7 ms: 1.05x faster                                      |
| pyflate                 | 434 ms                                                 | 413 ms: 1.05x faster                                       |
| scimark_fft             | 345 ms                                                 | 329 ms: 1.05x faster                                       |
| pickle_pure_python      | 320 us                                                 | 305 us: 1.05x faster                                       |
| telco                   | 6.86 ms                                                | 6.54 ms: 1.05x faster                                      |
| sympy_sum               | 169 ms                                                 | 161 ms: 1.05x faster                                       |
| thrift                  | 784 us                                                 | 750 us: 1.05x faster                                       |
| genshi_text             | 22.5 ms                                                | 21.5 ms: 1.05x faster                                      |
| json_dumps              | 13.3 ms                                                | 12.8 ms: 1.05x faster                                      |
| nqueens                 | 87.9 ms                                                | 84.2 ms: 1.04x faster                                      |
| meteor_contest          | 109 ms                                                 | 104 ms: 1.04x faster                                       |
| nbody                   | 96.0 ms                                                | 92.0 ms: 1.04x faster                                      |
| unpickle_list           | 5.21 us                                                | 5.00 us: 1.04x faster                                      |
| regex_dna               | 205 ms                                                 | 196 ms: 1.04x faster                                       |
| docutils                | 2.66 sec                                               | 2.56 sec: 1.04x faster                                     |
| regex_v8                | 22.9 ms                                                | 22.0 ms: 1.04x faster                                      |
| unpickle                | 13.8 us                                                | 13.3 us: 1.04x faster                                      |
| pycparser               | 1.19 sec                                               | 1.14 sec: 1.04x faster                                     |
| sympy_integrate         | 21.5 ms                                                | 20.7 ms: 1.04x faster                                      |
| mdp                     | 2.77 sec                                               | 2.67 sec: 1.04x faster                                     |
| xml_etree_parse         | 164 ms                                                 | 159 ms: 1.03x faster                                       |
| tornado_http            | 98.1 ms                                                | 94.9 ms: 1.03x faster                                      |
| sympy_str               | 297 ms                                                 | 288 ms: 1.03x faster                                       |
| 2to3                    | 264 ms                                                 | 256 ms: 1.03x faster                                       |
| pylint                  | 476 ms                                                 | 462 ms: 1.03x faster                                       |
| django_template         | 33.5 ms                                                | 32.6 ms: 1.03x faster                                      |
| bench_thread_pool       | 834 us                                                 | 811 us: 1.03x faster                                       |
| sqlalchemy_declarative  | 140 ms                                                 | 137 ms: 1.03x faster                                       |
| regex_compile           | 141 ms                                                 | 138 ms: 1.03x faster                                       |
| sqlglot_optimize        | 55.3 ms                                                | 53.9 ms: 1.03x faster                                      |
| crypto_pyaes            | 76.7 ms                                                | 74.8 ms: 1.03x faster                                      |
| pathlib                 | 18.5 ms                                                | 18.1 ms: 1.02x faster                                      |
| sqlalchemy_imperative   | 18.3 ms                                                | 17.9 ms: 1.02x faster                                      |
| xml_etree_iterparse     | 108 ms                                                 | 105 ms: 1.02x faster                                       |
| sqlglot_normalize       | 113 ms                                                 | 110 ms: 1.02x faster                                       |
| dulwich_log             | 64.6 ms                                                | 63.1 ms: 1.02x faster                                      |
| deltablue               | 3.92 ms                                                | 3.84 ms: 1.02x faster                                      |
| sympy_expand            | 484 ms                                                 | 475 ms: 1.02x faster                                       |
| sqlite_synth            | 2.57 us                                                | 2.52 us: 1.02x faster                                      |
| genshi_xml              | 53.4 ms                                                | 52.4 ms: 1.02x faster                                      |
| html5lib                | 64.8 ms                                                | 63.7 ms: 1.02x faster                                      |
| async_tree_memoization  | 639 ms                                                 | 628 ms: 1.02x faster                                       |
| chameleon               | 6.70 ms                                                | 6.62 ms: 1.01x faster                                      |
| async_tree_cpu_io_mixed | 749 ms                                                 | 743 ms: 1.01x faster                                       |
| python_startup          | 8.56 ms                                                | 8.49 ms: 1.01x faster                                      |
| generators              | 74.9 ms                                                | 74.4 ms: 1.01x faster                                      |
| fannkuch                | 405 ms                                                 | 403 ms: 1.00x faster                                       |
| python_startup_no_site  | 6.01 ms                                                | 5.99 ms: 1.00x faster                                      |
| async_tree_io           | 1.29 sec                                               | 1.31 sec: 1.02x slower                                     |
| asyncio_tcp             | 875 ms                                                 | 890 ms: 1.02x slower                                       |
| pidigits                | 194 ms                                                 | 199 ms: 1.03x slower                                       |
| gc_traversal            | 4.01 ms                                                | 4.21 ms: 1.05x slower                                      |
| create_gc_cycles        | 1.43 ms                                                | 1.51 ms: 1.05x slower                                      |
| unpack_sequence         | 43.5 ns                                                | 46.2 ns: 1.06x slower                                      |
| comprehensions          | 23.6 us                                                | 26.0 us: 1.10x slower                                      |
| sqlglot_transpile       | 1.75 ms                                                | 2.05 ms: 1.17x slower                                      |
| sqlglot_parse           | 1.43 ms                                                | 1.75 ms: 1.22x slower                                      |
| Geometric mean          | (ref)                                                  | 1.04x faster                                               |

Benchmark hidden because not significant (4): async_tree_none, bench_mp_pool, djangocms, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.01x