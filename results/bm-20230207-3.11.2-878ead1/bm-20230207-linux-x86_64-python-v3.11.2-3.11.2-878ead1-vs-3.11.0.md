
# Results vs. 3.11.0

- fork: python
- ref: v3.11.2
- machine: linux-x86_64
- commit hash: 878ead1
- commit date: 2023-02-07
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 257 ms: 1.03x faster                                   |
| chameleon      | 6.70 ms                                                | 6.49 ms: 1.03x faster                                  |
| docutils       | 2.66 sec                                               | 2.55 sec: 1.05x faster                                 |
| tornado_http   | 98.1 ms                                                | 96.1 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 639 ms                                                 | 628 ms: 1.02x faster                                   |
| async_tree_cpu_io_mixed | 749 ms                                                 | 740 ms: 1.01x faster                                   |
| async_tree_none         | 528 ms                                                 | 524 ms: 1.01x faster                                   |
| async_tree_io           | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 93.0 ms: 1.03x faster                                  |
| float          | 78.9 ms                                                | 76.6 ms: 1.03x faster                                  |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 21.3 ms: 1.07x faster                                  |
| regex_dna      | 205 ms                                                 | 192 ms: 1.06x faster                                   |
| regex_effbot   | 3.51 ms                                                | 3.39 ms: 1.04x faster                                  |
| regex_compile  | 141 ms                                                 | 138 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads           | 29.2 us                                                | 26.2 us: 1.12x faster                                  |
| pickle_list          | 4.59 us                                                | 4.16 us: 1.10x faster                                  |
| pickle_dict          | 34.6 us                                                | 31.4 us: 1.10x faster                                  |
| pickle               | 11.0 us                                                | 10.00 us: 1.10x faster                                 |
| json_dumps           | 13.3 ms                                                | 12.5 ms: 1.07x faster                                  |
| unpickle_pure_python | 242 us                                                 | 228 us: 1.06x faster                                   |
| xml_etree_generate   | 81.1 ms                                                | 76.5 ms: 1.06x faster                                  |
| xml_etree_process    | 56.9 ms                                                | 53.8 ms: 1.06x faster                                  |
| unpickle_list        | 5.21 us                                                | 4.94 us: 1.06x faster                                  |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                   |
| unpickle             | 13.8 us                                                | 13.2 us: 1.05x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                   |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| Geometric mean       | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.47 ms: 1.01x faster                                  |
| python_startup_no_site | 6.01 ms                                                | 5.97 ms: 1.01x faster                                  |
| Geometric mean         | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.83 ms: 1.08x faster                                  |
| genshi_text     | 22.5 ms                                                | 21.7 ms: 1.04x faster                                  |
| genshi_xml      | 53.4 ms                                                | 51.5 ms: 1.04x faster                                  |
| django_template | 33.5 ms                                                | 32.7 ms: 1.03x faster                                  |
| Geometric mean  | (ref)                                                  | 1.05x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads              | 29.2 us                                                | 26.2 us: 1.12x faster                                  |
| logging_silent          | 111 ns                                                 | 99.8 ns: 1.11x faster                                  |
| pickle_list             | 4.59 us                                                | 4.16 us: 1.10x faster                                  |
| pickle_dict             | 34.6 us                                                | 31.4 us: 1.10x faster                                  |
| pickle                  | 11.0 us                                                | 10.00 us: 1.10x faster                                 |
| spectral_norm           | 108 ms                                                 | 98.4 ms: 1.10x faster                                  |
| deepcopy_memo           | 40.2 us                                                | 36.8 us: 1.09x faster                                  |
| richards                | 49.8 ms                                                | 45.6 ms: 1.09x faster                                  |
| scimark_lu              | 116 ms                                                 | 107 ms: 1.09x faster                                   |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.63 ms: 1.09x faster                                  |
| mako                    | 10.7 ms                                                | 9.83 ms: 1.08x faster                                  |
| hexiom                  | 6.89 ms                                                | 6.36 ms: 1.08x faster                                  |
| pprint_pformat          | 1.55 sec                                               | 1.45 sec: 1.07x faster                                 |
| pprint_safe_repr        | 747 ms                                                 | 697 ms: 1.07x faster                                   |
| regex_v8                | 22.9 ms                                                | 21.3 ms: 1.07x faster                                  |
| json_dumps              | 13.3 ms                                                | 12.5 ms: 1.07x faster                                  |
| pycparser               | 1.19 sec                                               | 1.11 sec: 1.07x faster                                 |
| deltablue               | 3.92 ms                                                | 3.68 ms: 1.07x faster                                  |
| json                    | 5.24 ms                                                | 4.92 ms: 1.07x faster                                  |
| aiohttp                 | 1.12 ms                                                | 1.05 ms: 1.06x faster                                  |
| regex_dna               | 205 ms                                                 | 192 ms: 1.06x faster                                   |
| gunicorn                | 1.20 ms                                                | 1.13 ms: 1.06x faster                                  |
| raytrace                | 309 ms                                                 | 291 ms: 1.06x faster                                   |
| unpickle_pure_python    | 242 us                                                 | 228 us: 1.06x faster                                   |
| xml_etree_generate      | 81.1 ms                                                | 76.5 ms: 1.06x faster                                  |
| deepcopy_reduce         | 3.22 us                                                | 3.04 us: 1.06x faster                                  |
| scimark_sor             | 121 ms                                                 | 115 ms: 1.06x faster                                   |
| nqueens                 | 87.9 ms                                                | 83.1 ms: 1.06x faster                                  |
| xml_etree_process       | 56.9 ms                                                | 53.8 ms: 1.06x faster                                  |
| unpickle_list           | 5.21 us                                                | 4.94 us: 1.06x faster                                  |
| scimark_fft             | 345 ms                                                 | 327 ms: 1.06x faster                                   |
| coroutines              | 27.0 ms                                                | 25.6 ms: 1.06x faster                                  |
| chaos                   | 71.9 ms                                                | 68.2 ms: 1.05x faster                                  |
| go                      | 149 ms                                                 | 141 ms: 1.05x faster                                   |
| deepcopy                | 365 us                                                 | 348 us: 1.05x faster                                   |
| sqlglot_transpile       | 1.75 ms                                                | 1.67 ms: 1.05x faster                                  |
| logging_format          | 6.81 us                                                | 6.49 us: 1.05x faster                                  |
| pickle_pure_python      | 320 us                                                 | 305 us: 1.05x faster                                   |
| async_generators        | 374 ms                                                 | 357 ms: 1.05x faster                                   |
| docutils                | 2.66 sec                                               | 2.55 sec: 1.05x faster                                 |
| unpickle                | 13.8 us                                                | 13.2 us: 1.05x faster                                  |
| scimark_monte_carlo     | 70.7 ms                                                | 67.7 ms: 1.04x faster                                  |
| sqlite_synth            | 2.57 us                                                | 2.46 us: 1.04x faster                                  |
| meteor_contest          | 109 ms                                                 | 105 ms: 1.04x faster                                   |
| logging_simple          | 6.22 us                                                | 5.97 us: 1.04x faster                                  |
| telco                   | 6.86 ms                                                | 6.59 ms: 1.04x faster                                  |
| pyflate                 | 434 ms                                                 | 417 ms: 1.04x faster                                   |
| sqlglot_parse           | 1.43 ms                                                | 1.38 ms: 1.04x faster                                  |
| pathlib                 | 18.5 ms                                                | 17.8 ms: 1.04x faster                                  |
| xml_etree_iterparse     | 108 ms                                                 | 104 ms: 1.04x faster                                   |
| crypto_pyaes            | 76.7 ms                                                | 73.8 ms: 1.04x faster                                  |
| genshi_text             | 22.5 ms                                                | 21.7 ms: 1.04x faster                                  |
| sqlglot_optimize        | 55.3 ms                                                | 53.3 ms: 1.04x faster                                  |
| flaskblogging           | 7.28 ms                                                | 7.02 ms: 1.04x faster                                  |
| sqlglot_normalize       | 113 ms                                                 | 109 ms: 1.04x faster                                   |
| genshi_xml              | 53.4 ms                                                | 51.5 ms: 1.04x faster                                  |
| djangocms               | 33.5 us                                                | 32.3 us: 1.04x faster                                  |
| regex_effbot            | 3.51 ms                                                | 3.39 ms: 1.04x faster                                  |
| sympy_expand            | 484 ms                                                 | 468 ms: 1.03x faster                                   |
| fannkuch                | 405 ms                                                 | 392 ms: 1.03x faster                                   |
| chameleon               | 6.70 ms                                                | 6.49 ms: 1.03x faster                                  |
| sympy_str               | 297 ms                                                 | 288 ms: 1.03x faster                                   |
| nbody                   | 96.0 ms                                                | 93.0 ms: 1.03x faster                                  |
| float                   | 78.9 ms                                                | 76.6 ms: 1.03x faster                                  |
| xml_etree_parse         | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| sympy_integrate         | 21.5 ms                                                | 20.8 ms: 1.03x faster                                  |
| bench_thread_pool       | 834 us                                                 | 812 us: 1.03x faster                                   |
| 2to3                    | 264 ms                                                 | 257 ms: 1.03x faster                                   |
| django_template         | 33.5 ms                                                | 32.7 ms: 1.03x faster                                  |
| regex_compile           | 141 ms                                                 | 138 ms: 1.02x faster                                   |
| pidigits                | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| tornado_http            | 98.1 ms                                                | 96.1 ms: 1.02x faster                                  |
| sympy_sum               | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| thrift                  | 784 us                                                 | 770 us: 1.02x faster                                   |
| async_tree_memoization  | 639 ms                                                 | 628 ms: 1.02x faster                                   |
| dulwich_log             | 64.6 ms                                                | 63.7 ms: 1.01x faster                                  |
| async_tree_cpu_io_mixed | 749 ms                                                 | 740 ms: 1.01x faster                                   |
| python_startup          | 8.56 ms                                                | 8.47 ms: 1.01x faster                                  |
| generators              | 74.9 ms                                                | 74.1 ms: 1.01x faster                                  |
| sqlalchemy_imperative   | 18.3 ms                                                | 18.2 ms: 1.01x faster                                  |
| async_tree_none         | 528 ms                                                 | 524 ms: 1.01x faster                                   |
| python_startup_no_site  | 6.01 ms                                                | 5.97 ms: 1.01x faster                                  |
| mdp                     | 2.77 sec                                               | 2.77 sec: 1.00x faster                                 |
| async_tree_io           | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| asyncio_tcp             | 875 ms                                                 | 884 ms: 1.01x slower                                   |
| gc_traversal            | 4.01 ms                                                | 4.15 ms: 1.04x slower                                  |
| create_gc_cycles        | 1.43 ms                                                | 1.49 ms: 1.04x slower                                  |
| unpack_sequence         | 43.5 ns                                                | 48.8 ns: 1.12x slower                                  |
| coverage                | 78.8 ms                                                | 103 ms: 1.31x slower                                   |
| Geometric mean          | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (5): html5lib, pylint, dask, bench_mp_pool, sqlalchemy_declarative
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x