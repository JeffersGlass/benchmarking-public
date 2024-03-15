
# Results vs. 3.10.4

- fork: python
- ref: v3.11.2
- machine: linux-x86_64
- commit hash: 878ead1
- commit date: 2023-02-07
- overall geometric mean: 1.33x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 257 ms: 1.35x faster                                   |
| chameleon      | 9.68 ms                                                | 6.49 ms: 1.49x faster                                  |
| docutils       | 3.30 sec                                               | 2.55 sec: 1.29x faster                                 |
| html5lib       | 88.9 ms                                                | 64.0 ms: 1.39x faster                                  |
| tornado_http   | 136 ms                                                 | 96.1 ms: 1.42x faster                                  |
| Geometric mean | (ref)                                                  | 1.39x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 524 ms: 1.39x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 628 ms: 1.39x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 740 ms: 1.37x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| Geometric mean          | (ref)                                                  | 1.38x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.0 ms: 1.65x faster                                  |
| float          | 117 ms                                                 | 76.6 ms: 1.53x faster                                  |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| Geometric mean | (ref)                                                  | 1.36x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 138 ms: 1.37x faster                                   |
| regex_v8       | 27.8 ms                                                | 21.3 ms: 1.30x faster                                  |
| regex_dna      | 227 ms                                                 | 192 ms: 1.18x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.39 ms: 1.07x faster                                  |
| Geometric mean | (ref)                                                  | 1.22x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 53.8 ms: 1.47x faster                                  |
| unpickle_pure_python | 331 us                                                 | 228 us: 1.45x faster                                   |
| xml_etree_generate   | 99.4 ms                                                | 76.5 ms: 1.30x faster                                  |
| pickle_list          | 5.08 us                                                | 4.16 us: 1.22x faster                                  |
| json_loads           | 31.2 us                                                | 26.2 us: 1.19x faster                                  |
| json_dumps           | 14.2 ms                                                | 12.5 ms: 1.14x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                   |
| unpickle             | 14.4 us                                                | 13.2 us: 1.09x faster                                  |
| pickle               | 10.7 us                                                | 10.00 us: 1.07x faster                                 |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                   |
| unpickle_list        | 5.20 us                                                | 4.94 us: 1.05x faster                                  |
| pickle_dict          | 29.6 us                                                | 31.4 us: 1.06x slower                                  |
| Geometric mean       | (ref)                                                  | 1.19x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.47 ms: 1.72x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 5.97 ms: 1.01x slower                                  |
| Geometric mean         | (ref)                                                  | 1.31x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.83 ms: 1.66x faster                                  |
| django_template | 48.2 ms                                                | 32.7 ms: 1.47x faster                                  |
| genshi_text     | 31.8 ms                                                | 21.7 ms: 1.47x faster                                  |
| genshi_xml      | 66.0 ms                                                | 51.5 ms: 1.28x faster                                  |
| Geometric mean  | (ref)                                                  | 1.46x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.11.2-3.11.2-878ead1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.68 ms: 2.15x faster                                  |
| scimark_sor             | 220 ms                                                 | 115 ms: 1.91x faster                                   |
| logging_silent          | 190 ns                                                 | 99.8 ns: 1.90x faster                                  |
| scimark_monte_carlo     | 118 ms                                                 | 67.7 ms: 1.74x faster                                  |
| raytrace                | 507 ms                                                 | 291 ms: 1.74x faster                                   |
| richards                | 79.3 ms                                                | 45.6 ms: 1.74x faster                                  |
| crypto_pyaes            | 128 ms                                                 | 73.8 ms: 1.73x faster                                  |
| spectral_norm           | 170 ms                                                 | 98.4 ms: 1.73x faster                                  |
| python_startup          | 14.6 ms                                                | 8.47 ms: 1.72x faster                                  |
| pyflate                 | 716 ms                                                 | 417 ms: 1.72x faster                                   |
| go                      | 240 ms                                                 | 141 ms: 1.70x faster                                   |
| chaos                   | 115 ms                                                 | 68.2 ms: 1.69x faster                                  |
| mako                    | 16.3 ms                                                | 9.83 ms: 1.66x faster                                  |
| nbody                   | 154 ms                                                 | 93.0 ms: 1.65x faster                                  |
| scimark_lu              | 176 ms                                                 | 107 ms: 1.65x faster                                   |
| hexiom                  | 10.4 ms                                                | 6.36 ms: 1.63x faster                                  |
| deepcopy_memo           | 58.5 us                                                | 36.8 us: 1.59x faster                                  |
| pickle_pure_python      | 484 us                                                 | 305 us: 1.59x faster                                   |
| sqlglot_parse           | 2.17 ms                                                | 1.38 ms: 1.58x faster                                  |
| sqlglot_transpile       | 2.57 ms                                                | 1.67 ms: 1.54x faster                                  |
| float                   | 117 ms                                                 | 76.6 ms: 1.53x faster                                  |
| chameleon               | 9.68 ms                                                | 6.49 ms: 1.49x faster                                  |
| django_template         | 48.2 ms                                                | 32.7 ms: 1.47x faster                                  |
| xml_etree_process       | 79.1 ms                                                | 53.8 ms: 1.47x faster                                  |
| genshi_text             | 31.8 ms                                                | 21.7 ms: 1.47x faster                                  |
| pprint_safe_repr        | 1.02 sec                                               | 697 ms: 1.46x faster                                   |
| pprint_pformat          | 2.10 sec                                               | 1.45 sec: 1.45x faster                                 |
| unpickle_pure_python    | 331 us                                                 | 228 us: 1.45x faster                                   |
| pycparser               | 1.58 sec                                               | 1.11 sec: 1.42x faster                                 |
| scimark_fft             | 466 ms                                                 | 327 ms: 1.42x faster                                   |
| tornado_http            | 136 ms                                                 | 96.1 ms: 1.42x faster                                  |
| logging_format          | 9.09 us                                                | 6.49 us: 1.40x faster                                  |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.63 ms: 1.40x faster                                  |
| thrift                  | 1.07 ms                                                | 770 us: 1.39x faster                                   |
| logging_simple          | 8.30 us                                                | 5.97 us: 1.39x faster                                  |
| async_tree_none         | 728 ms                                                 | 524 ms: 1.39x faster                                   |
| html5lib                | 88.9 ms                                                | 64.0 ms: 1.39x faster                                  |
| async_tree_memoization  | 870 ms                                                 | 628 ms: 1.39x faster                                   |
| deepcopy                | 479 us                                                 | 348 us: 1.38x faster                                   |
| aiohttp                 | 1.44 ms                                                | 1.05 ms: 1.37x faster                                  |
| deepcopy_reduce         | 4.17 us                                                | 3.04 us: 1.37x faster                                  |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 740 ms: 1.37x faster                                   |
| coroutines              | 35.1 ms                                                | 25.6 ms: 1.37x faster                                  |
| regex_compile           | 188 ms                                                 | 138 ms: 1.37x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| fannkuch                | 532 ms                                                 | 392 ms: 1.36x faster                                   |
| gunicorn                | 1.53 ms                                                | 1.13 ms: 1.36x faster                                  |
| 2to3                    | 348 ms                                                 | 257 ms: 1.35x faster                                   |
| dulwich_log             | 84.3 ms                                                | 63.7 ms: 1.32x faster                                  |
| sqlglot_normalize       | 143 ms                                                 | 109 ms: 1.32x faster                                   |
| regex_v8                | 27.8 ms                                                | 21.3 ms: 1.30x faster                                  |
| xml_etree_generate      | 99.4 ms                                                | 76.5 ms: 1.30x faster                                  |
| sqlglot_optimize        | 69.2 ms                                                | 53.3 ms: 1.30x faster                                  |
| docutils                | 3.30 sec                                               | 2.55 sec: 1.29x faster                                 |
| sqlalchemy_imperative   | 23.3 ms                                                | 18.2 ms: 1.28x faster                                  |
| genshi_xml              | 66.0 ms                                                | 51.5 ms: 1.28x faster                                  |
| nqueens                 | 106 ms                                                 | 83.1 ms: 1.27x faster                                  |
| async_generators        | 444 ms                                                 | 357 ms: 1.24x faster                                   |
| sympy_integrate         | 25.8 ms                                                | 20.8 ms: 1.24x faster                                  |
| unpack_sequence         | 60.0 ns                                                | 48.8 ns: 1.23x faster                                  |
| sqlite_synth            | 3.02 us                                                | 2.46 us: 1.23x faster                                  |
| flaskblogging           | 8.58 ms                                                | 7.02 ms: 1.22x faster                                  |
| pickle_list             | 5.08 us                                                | 4.16 us: 1.22x faster                                  |
| sqlalchemy_declarative  | 172 ms                                                 | 141 ms: 1.22x faster                                   |
| bench_thread_pool       | 986 us                                                 | 812 us: 1.21x faster                                   |
| dask                    | 441 ms                                                 | 365 ms: 1.21x faster                                   |
| sympy_expand            | 566 ms                                                 | 468 ms: 1.21x faster                                   |
| sympy_str               | 346 ms                                                 | 288 ms: 1.20x faster                                   |
| json_loads              | 31.2 us                                                | 26.2 us: 1.19x faster                                  |
| djangocms               | 38.4 us                                                | 32.3 us: 1.19x faster                                  |
| sympy_sum               | 196 ms                                                 | 166 ms: 1.19x faster                                   |
| regex_dna               | 227 ms                                                 | 192 ms: 1.18x faster                                   |
| pylint                  | 551 ms                                                 | 475 ms: 1.16x faster                                   |
| json                    | 5.69 ms                                                | 4.92 ms: 1.16x faster                                  |
| pathlib                 | 20.5 ms                                                | 17.8 ms: 1.15x faster                                  |
| meteor_contest          | 120 ms                                                 | 105 ms: 1.14x faster                                   |
| json_dumps              | 14.2 ms                                                | 12.5 ms: 1.14x faster                                  |
| xml_etree_iterparse     | 115 ms                                                 | 104 ms: 1.11x faster                                   |
| telco                   | 7.27 ms                                                | 6.59 ms: 1.10x faster                                  |
| create_gc_cycles        | 1.62 ms                                                | 1.49 ms: 1.09x faster                                  |
| unpickle                | 14.4 us                                                | 13.2 us: 1.09x faster                                  |
| generators              | 80.1 ms                                                | 74.1 ms: 1.08x faster                                  |
| regex_effbot            | 3.63 ms                                                | 3.39 ms: 1.07x faster                                  |
| pickle                  | 10.7 us                                                | 10.00 us: 1.07x faster                                 |
| xml_etree_parse         | 168 ms                                                 | 159 ms: 1.06x faster                                   |
| unpickle_list           | 5.20 us                                                | 4.94 us: 1.05x faster                                  |
| asyncio_tcp             | 922 ms                                                 | 884 ms: 1.04x faster                                   |
| mdp                     | 2.85 sec                                               | 2.77 sec: 1.03x faster                                 |
| pidigits                | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| python_startup_no_site  | 5.93 ms                                                | 5.97 ms: 1.01x slower                                  |
| pickle_dict             | 29.6 us                                                | 31.4 us: 1.06x slower                                  |
| gc_traversal            | 3.62 ms                                                | 4.15 ms: 1.15x slower                                  |
| coverage                | 79.4 ms                                                | 103 ms: 1.30x slower                                   |
| Geometric mean          | (ref)                                                  | 1.33x faster                                           |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.09x