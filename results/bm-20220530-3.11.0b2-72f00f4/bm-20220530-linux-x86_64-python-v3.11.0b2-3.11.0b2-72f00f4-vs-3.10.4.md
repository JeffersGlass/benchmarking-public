
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0b2
- machine: linux-x86_64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.33x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 256 ms: 1.36x faster                                       |
| chameleon      | 9.68 ms                                                | 6.62 ms: 1.46x faster                                      |
| docutils       | 3.30 sec                                               | 2.56 sec: 1.29x faster                                     |
| html5lib       | 88.9 ms                                                | 63.7 ms: 1.39x faster                                      |
| tornado_http   | 136 ms                                                 | 94.9 ms: 1.44x faster                                      |
| Geometric mean | (ref)                                                  | 1.39x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 526 ms: 1.39x faster                                       |
| async_tree_memoization  | 870 ms                                                 | 628 ms: 1.38x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 743 ms: 1.37x faster                                       |
| async_tree_io           | 1.77 sec                                               | 1.31 sec: 1.35x faster                                     |
| Geometric mean          | (ref)                                                  | 1.37x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.0 ms: 1.67x faster                                      |
| float          | 117 ms                                                 | 74.4 ms: 1.57x faster                                      |
| pidigits       | 191 ms                                                 | 199 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                  | 1.36x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 138 ms: 1.37x faster                                       |
| regex_v8       | 27.8 ms                                                | 22.0 ms: 1.26x faster                                      |
| regex_effbot   | 3.63 ms                                                | 3.11 ms: 1.17x faster                                      |
| regex_dna      | 227 ms                                                 | 196 ms: 1.15x faster                                       |
| Geometric mean | (ref)                                                  | 1.24x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                       |
| xml_etree_process    | 79.1 ms                                                | 53.4 ms: 1.48x faster                                      |
| unpickle_pure_python | 331 us                                                 | 227 us: 1.46x faster                                       |
| xml_etree_generate   | 99.4 ms                                                | 76.1 ms: 1.31x faster                                      |
| json_loads           | 31.2 us                                                | 25.0 us: 1.25x faster                                      |
| pickle_list          | 5.08 us                                                | 4.30 us: 1.18x faster                                      |
| pickle               | 10.7 us                                                | 9.44 us: 1.13x faster                                      |
| pickle_dict          | 29.6 us                                                | 26.4 us: 1.12x faster                                      |
| json_dumps           | 14.2 ms                                                | 12.8 ms: 1.11x faster                                      |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.09x faster                                       |
| unpickle             | 14.4 us                                                | 13.3 us: 1.08x faster                                      |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                       |
| unpickle_list        | 5.20 us                                                | 5.00 us: 1.04x faster                                      |
| Geometric mean       | (ref)                                                  | 1.21x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.49 ms: 1.72x faster                                      |
| python_startup_no_site | 5.93 ms                                                | 5.99 ms: 1.01x slower                                      |
| Geometric mean         | (ref)                                                  | 1.30x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.96 ms: 1.64x faster                                      |
| django_template | 48.2 ms                                                | 32.6 ms: 1.48x faster                                      |
| genshi_text     | 31.8 ms                                                | 21.5 ms: 1.48x faster                                      |
| genshi_xml      | 66.0 ms                                                | 52.4 ms: 1.26x faster                                      |
| Geometric mean  | (ref)                                                  | 1.46x faster                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-linux-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.84 ms: 2.06x faster                                      |
| scimark_sor             | 220 ms                                                 | 115 ms: 1.91x faster                                       |
| logging_silent          | 190 ns                                                 | 103 ns: 1.85x faster                                       |
| scimark_monte_carlo     | 118 ms                                                 | 66.0 ms: 1.79x faster                                      |
| richards                | 79.3 ms                                                | 44.5 ms: 1.78x faster                                      |
| raytrace                | 507 ms                                                 | 287 ms: 1.77x faster                                       |
| spectral_norm           | 170 ms                                                 | 97.3 ms: 1.75x faster                                      |
| pyflate                 | 716 ms                                                 | 413 ms: 1.74x faster                                       |
| go                      | 240 ms                                                 | 139 ms: 1.73x faster                                       |
| python_startup          | 14.6 ms                                                | 8.49 ms: 1.72x faster                                      |
| chaos                   | 115 ms                                                 | 67.3 ms: 1.71x faster                                      |
| crypto_pyaes            | 128 ms                                                 | 74.8 ms: 1.71x faster                                      |
| nbody                   | 154 ms                                                 | 92.0 ms: 1.67x faster                                      |
| hexiom                  | 10.4 ms                                                | 6.27 ms: 1.66x faster                                      |
| mako                    | 16.3 ms                                                | 9.96 ms: 1.64x faster                                      |
| deepcopy_memo           | 58.5 us                                                | 35.9 us: 1.63x faster                                      |
| scimark_lu              | 176 ms                                                 | 109 ms: 1.61x faster                                       |
| pickle_pure_python      | 484 us                                                 | 305 us: 1.59x faster                                       |
| float                   | 117 ms                                                 | 74.4 ms: 1.57x faster                                      |
| xml_etree_process       | 79.1 ms                                                | 53.4 ms: 1.48x faster                                      |
| django_template         | 48.2 ms                                                | 32.6 ms: 1.48x faster                                      |
| genshi_text             | 31.8 ms                                                | 21.5 ms: 1.48x faster                                      |
| chameleon               | 9.68 ms                                                | 6.62 ms: 1.46x faster                                      |
| unpickle_pure_python    | 331 us                                                 | 227 us: 1.46x faster                                       |
| pprint_safe_repr        | 1.02 sec                                               | 699 ms: 1.46x faster                                       |
| pprint_pformat          | 2.10 sec                                               | 1.45 sec: 1.45x faster                                     |
| logging_simple          | 8.30 us                                                | 5.74 us: 1.45x faster                                      |
| tornado_http            | 136 ms                                                 | 94.9 ms: 1.44x faster                                      |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.51 ms: 1.43x faster                                      |
| logging_format          | 9.09 us                                                | 6.34 us: 1.43x faster                                      |
| thrift                  | 1.07 ms                                                | 750 us: 1.43x faster                                       |
| scimark_fft             | 466 ms                                                 | 329 ms: 1.42x faster                                       |
| deepcopy                | 479 us                                                 | 340 us: 1.41x faster                                       |
| html5lib                | 88.9 ms                                                | 63.7 ms: 1.39x faster                                      |
| async_tree_none         | 728 ms                                                 | 526 ms: 1.39x faster                                       |
| async_tree_memoization  | 870 ms                                                 | 628 ms: 1.38x faster                                       |
| pycparser               | 1.58 sec                                               | 1.14 sec: 1.38x faster                                     |
| deepcopy_reduce         | 4.17 us                                                | 3.03 us: 1.38x faster                                      |
| regex_compile           | 188 ms                                                 | 138 ms: 1.37x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 743 ms: 1.37x faster                                       |
| coroutines              | 35.1 ms                                                | 25.7 ms: 1.36x faster                                      |
| aiohttp                 | 1.44 ms                                                | 1.06 ms: 1.36x faster                                      |
| 2to3                    | 348 ms                                                 | 256 ms: 1.36x faster                                       |
| gunicorn                | 1.53 ms                                                | 1.13 ms: 1.36x faster                                      |
| async_tree_io           | 1.77 sec                                               | 1.31 sec: 1.35x faster                                     |
| dulwich_log             | 84.3 ms                                                | 63.1 ms: 1.34x faster                                      |
| fannkuch                | 532 ms                                                 | 403 ms: 1.32x faster                                       |
| xml_etree_generate      | 99.4 ms                                                | 76.1 ms: 1.31x faster                                      |
| sqlalchemy_imperative   | 23.3 ms                                                | 17.9 ms: 1.30x faster                                      |
| unpack_sequence         | 60.0 ns                                                | 46.2 ns: 1.30x faster                                      |
| sqlglot_normalize       | 143 ms                                                 | 110 ms: 1.30x faster                                       |
| docutils                | 3.30 sec                                               | 2.56 sec: 1.29x faster                                     |
| sqlglot_optimize        | 69.2 ms                                                | 53.9 ms: 1.28x faster                                      |
| regex_v8                | 27.8 ms                                                | 22.0 ms: 1.26x faster                                      |
| genshi_xml              | 66.0 ms                                                | 52.4 ms: 1.26x faster                                      |
| sqlalchemy_declarative  | 172 ms                                                 | 137 ms: 1.26x faster                                       |
| sqlglot_transpile       | 2.57 ms                                                | 2.05 ms: 1.26x faster                                      |
| nqueens                 | 106 ms                                                 | 84.2 ms: 1.26x faster                                      |
| async_generators        | 444 ms                                                 | 354 ms: 1.25x faster                                       |
| sympy_integrate         | 25.8 ms                                                | 20.7 ms: 1.25x faster                                      |
| json_loads              | 31.2 us                                                | 25.0 us: 1.25x faster                                      |
| sqlglot_parse           | 2.17 ms                                                | 1.75 ms: 1.24x faster                                      |
| sympy_sum               | 196 ms                                                 | 161 ms: 1.22x faster                                       |
| bench_thread_pool       | 986 us                                                 | 811 us: 1.22x faster                                       |
| sympy_str               | 346 ms                                                 | 288 ms: 1.20x faster                                       |
| sqlite_synth            | 3.02 us                                                | 2.52 us: 1.20x faster                                      |
| dask                    | 441 ms                                                 | 368 ms: 1.20x faster                                       |
| json                    | 5.69 ms                                                | 4.75 ms: 1.20x faster                                      |
| pylint                  | 551 ms                                                 | 462 ms: 1.19x faster                                       |
| sympy_expand            | 566 ms                                                 | 475 ms: 1.19x faster                                       |
| pickle_list             | 5.08 us                                                | 4.30 us: 1.18x faster                                      |
| regex_effbot            | 3.63 ms                                                | 3.11 ms: 1.17x faster                                      |
| regex_dna               | 227 ms                                                 | 196 ms: 1.15x faster                                       |
| djangocms               | 38.4 us                                                | 33.5 us: 1.15x faster                                      |
| meteor_contest          | 120 ms                                                 | 104 ms: 1.15x faster                                       |
| pathlib                 | 20.5 ms                                                | 18.1 ms: 1.13x faster                                      |
| pickle                  | 10.7 us                                                | 9.44 us: 1.13x faster                                      |
| pickle_dict             | 29.6 us                                                | 26.4 us: 1.12x faster                                      |
| json_dumps              | 14.2 ms                                                | 12.8 ms: 1.11x faster                                      |
| telco                   | 7.27 ms                                                | 6.54 ms: 1.11x faster                                      |
| comprehensions          | 28.8 us                                                | 26.0 us: 1.11x faster                                      |
| xml_etree_iterparse     | 115 ms                                                 | 105 ms: 1.09x faster                                       |
| unpickle                | 14.4 us                                                | 13.3 us: 1.08x faster                                      |
| generators              | 80.1 ms                                                | 74.4 ms: 1.08x faster                                      |
| create_gc_cycles        | 1.62 ms                                                | 1.51 ms: 1.07x faster                                      |
| mdp                     | 2.85 sec                                               | 2.67 sec: 1.07x faster                                     |
| xml_etree_parse         | 168 ms                                                 | 159 ms: 1.06x faster                                       |
| unpickle_list           | 5.20 us                                                | 5.00 us: 1.04x faster                                      |
| asyncio_tcp             | 922 ms                                                 | 890 ms: 1.04x faster                                       |
| python_startup_no_site  | 5.93 ms                                                | 5.99 ms: 1.01x slower                                      |
| pidigits                | 191 ms                                                 | 199 ms: 1.04x slower                                       |
| gc_traversal            | 3.62 ms                                                | 4.21 ms: 1.16x slower                                      |
| Geometric mean          | (ref)                                                  | 1.33x faster                                               |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (8) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.09x