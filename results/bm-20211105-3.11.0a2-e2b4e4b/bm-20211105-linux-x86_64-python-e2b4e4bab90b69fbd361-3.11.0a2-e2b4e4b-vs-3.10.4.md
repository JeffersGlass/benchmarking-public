
# Results vs. 3.10.4

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: linux-x86_64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 274 ms: 1.27x faster                                                  |
| chameleon      | 9.68 ms                                                | 7.46 ms: 1.30x faster                                                 |
| docutils       | 3.30 sec                                               | 2.79 sec: 1.18x faster                                                |
| html5lib       | 88.9 ms                                                | 71.5 ms: 1.24x faster                                                 |
| tornado_http   | 136 ms                                                 | 111 ms: 1.23x faster                                                  |
| Geometric mean | (ref)                                                  | 1.24x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 518 ms: 1.41x faster                                                  |
| async_tree_memoization  | 870 ms                                                 | 676 ms: 1.29x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.41 sec: 1.26x faster                                                |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 818 ms: 1.24x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.30x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 117 ms                                                 | 83.3 ms: 1.41x faster                                                 |
| nbody          | 154 ms                                                 | 112 ms: 1.37x faster                                                  |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.25x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 145 ms: 1.30x faster                                                  |
| regex_v8       | 27.8 ms                                                | 23.7 ms: 1.17x faster                                                 |
| regex_effbot   | 3.63 ms                                                | 3.26 ms: 1.11x faster                                                 |
| regex_dna      | 227 ms                                                 | 219 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.15x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 364 us: 1.33x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.6 ms: 1.33x faster                                                 |
| unpickle_pure_python | 331 us                                                 | 271 us: 1.22x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 81.6 ms: 1.22x faster                                                 |
| json_loads           | 31.2 us                                                | 25.9 us: 1.20x faster                                                 |
| json_dumps           | 14.2 ms                                                | 12.4 ms: 1.14x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.68 us: 1.08x faster                                                 |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                  |
| pickle               | 10.7 us                                                | 10.1 us: 1.06x faster                                                 |
| unpickle             | 14.4 us                                                | 13.7 us: 1.05x faster                                                 |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                  |
| pickle_dict          | 29.6 us                                                | 28.6 us: 1.03x faster                                                 |
| unpickle_list        | 5.20 us                                                | 5.13 us: 1.01x faster                                                 |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 5.93 ms                                                | 5.77 ms: 1.03x faster                                                 |
| python_startup         | 14.6 ms                                                | 14.6 ms: 1.00x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.02x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                 |
| genshi_text     | 31.8 ms                                                | 24.6 ms: 1.29x faster                                                 |
| django_template | 48.2 ms                                                | 37.9 ms: 1.27x faster                                                 |
| genshi_xml      | 66.0 ms                                                | 56.1 ms: 1.18x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.27x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 4.86 ms: 1.63x faster                                                 |
| logging_silent          | 190 ns                                                 | 117 ns: 1.63x faster                                                  |
| spectral_norm           | 170 ms                                                 | 106 ms: 1.61x faster                                                  |
| raytrace                | 507 ms                                                 | 326 ms: 1.55x faster                                                  |
| scimark_monte_carlo     | 118 ms                                                 | 78.4 ms: 1.51x faster                                                 |
| chaos                   | 115 ms                                                 | 77.1 ms: 1.50x faster                                                 |
| deepcopy_memo           | 58.5 us                                                | 40.4 us: 1.45x faster                                                 |
| go                      | 240 ms                                                 | 167 ms: 1.43x faster                                                  |
| richards                | 79.3 ms                                                | 55.7 ms: 1.42x faster                                                 |
| crypto_pyaes            | 128 ms                                                 | 90.2 ms: 1.42x faster                                                 |
| scimark_sor             | 220 ms                                                 | 156 ms: 1.41x faster                                                  |
| float                   | 117 ms                                                 | 83.3 ms: 1.41x faster                                                 |
| async_tree_none         | 728 ms                                                 | 518 ms: 1.41x faster                                                  |
| hexiom                  | 10.4 ms                                                | 7.42 ms: 1.40x faster                                                 |
| generators              | 80.1 ms                                                | 57.4 ms: 1.40x faster                                                 |
| unpack_sequence         | 60.0 ns                                                | 43.6 ns: 1.38x faster                                                 |
| nbody                   | 154 ms                                                 | 112 ms: 1.37x faster                                                  |
| logging_simple          | 8.30 us                                                | 6.07 us: 1.37x faster                                                 |
| logging_format          | 9.09 us                                                | 6.71 us: 1.36x faster                                                 |
| mako                    | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                 |
| pprint_safe_repr        | 1.02 sec                                               | 763 ms: 1.33x faster                                                  |
| pprint_pformat          | 2.10 sec                                               | 1.58 sec: 1.33x faster                                                |
| pickle_pure_python      | 484 us                                                 | 364 us: 1.33x faster                                                  |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.86 ms: 1.33x faster                                                 |
| gunicorn                | 1.53 ms                                                | 1.15 ms: 1.33x faster                                                 |
| xml_etree_process       | 79.1 ms                                                | 59.6 ms: 1.33x faster                                                 |
| pyflate                 | 716 ms                                                 | 541 ms: 1.33x faster                                                  |
| scimark_fft             | 466 ms                                                 | 355 ms: 1.31x faster                                                  |
| thrift                  | 1.07 ms                                                | 821 us: 1.31x faster                                                  |
| regex_compile           | 188 ms                                                 | 145 ms: 1.30x faster                                                  |
| chameleon               | 9.68 ms                                                | 7.46 ms: 1.30x faster                                                 |
| genshi_text             | 31.8 ms                                                | 24.6 ms: 1.29x faster                                                 |
| scimark_lu              | 176 ms                                                 | 136 ms: 1.29x faster                                                  |
| async_tree_memoization  | 870 ms                                                 | 676 ms: 1.29x faster                                                  |
| deepcopy_reduce         | 4.17 us                                                | 3.27 us: 1.27x faster                                                 |
| 2to3                    | 348 ms                                                 | 274 ms: 1.27x faster                                                  |
| django_template         | 48.2 ms                                                | 37.9 ms: 1.27x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.41 sec: 1.26x faster                                                |
| deepcopy                | 479 us                                                 | 382 us: 1.25x faster                                                  |
| pycparser               | 1.58 sec                                               | 1.26 sec: 1.25x faster                                                |
| fannkuch                | 532 ms                                                 | 427 ms: 1.24x faster                                                  |
| sqlalchemy_imperative   | 23.3 ms                                                | 18.8 ms: 1.24x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 818 ms: 1.24x faster                                                  |
| html5lib                | 88.9 ms                                                | 71.5 ms: 1.24x faster                                                 |
| dulwich_log             | 84.3 ms                                                | 68.3 ms: 1.24x faster                                                 |
| tornado_http            | 136 ms                                                 | 111 ms: 1.23x faster                                                  |
| async_generators        | 444 ms                                                 | 361 ms: 1.23x faster                                                  |
| coroutines              | 35.1 ms                                                | 28.8 ms: 1.22x faster                                                 |
| unpickle_pure_python    | 331 us                                                 | 271 us: 1.22x faster                                                  |
| xml_etree_generate      | 99.4 ms                                                | 81.6 ms: 1.22x faster                                                 |
| json_loads              | 31.2 us                                                | 25.9 us: 1.20x faster                                                 |
| sqlglot_normalize       | 143 ms                                                 | 119 ms: 1.20x faster                                                  |
| sqlalchemy_declarative  | 172 ms                                                 | 145 ms: 1.19x faster                                                  |
| sqlglot_optimize        | 69.2 ms                                                | 58.4 ms: 1.19x faster                                                 |
| docutils                | 3.30 sec                                               | 2.79 sec: 1.18x faster                                                |
| genshi_xml              | 66.0 ms                                                | 56.1 ms: 1.18x faster                                                 |
| pylint                  | 551 ms                                                 | 469 ms: 1.18x faster                                                  |
| regex_v8                | 27.8 ms                                                | 23.7 ms: 1.17x faster                                                 |
| sympy_integrate         | 25.8 ms                                                | 22.2 ms: 1.16x faster                                                 |
| json                    | 5.69 ms                                                | 4.91 ms: 1.16x faster                                                 |
| nqueens                 | 106 ms                                                 | 91.4 ms: 1.16x faster                                                 |
| sympy_sum               | 196 ms                                                 | 170 ms: 1.15x faster                                                  |
| flaskblogging           | 8.58 ms                                                | 7.46 ms: 1.15x faster                                                 |
| json_dumps              | 14.2 ms                                                | 12.4 ms: 1.14x faster                                                 |
| sympy_str               | 346 ms                                                 | 306 ms: 1.13x faster                                                  |
| meteor_contest          | 120 ms                                                 | 106 ms: 1.12x faster                                                  |
| sympy_expand            | 566 ms                                                 | 505 ms: 1.12x faster                                                  |
| telco                   | 7.27 ms                                                | 6.50 ms: 1.12x faster                                                 |
| regex_effbot            | 3.63 ms                                                | 3.26 ms: 1.11x faster                                                 |
| bench_thread_pool       | 986 us                                                 | 892 us: 1.11x faster                                                  |
| sqlite_synth            | 3.02 us                                                | 2.76 us: 1.10x faster                                                 |
| sqlglot_transpile       | 2.57 ms                                                | 2.37 ms: 1.09x faster                                                 |
| pickle_list             | 5.08 us                                                | 4.68 us: 1.08x faster                                                 |
| pathlib                 | 20.5 ms                                                | 19.1 ms: 1.07x faster                                                 |
| xml_etree_parse         | 168 ms                                                 | 158 ms: 1.06x faster                                                  |
| pickle                  | 10.7 us                                                | 10.1 us: 1.06x faster                                                 |
| sqlglot_parse           | 2.17 ms                                                | 2.06 ms: 1.05x faster                                                 |
| mdp                     | 2.85 sec                                               | 2.71 sec: 1.05x faster                                                |
| unpickle                | 14.4 us                                                | 13.7 us: 1.05x faster                                                 |
| coverage                | 79.4 ms                                                | 75.8 ms: 1.05x faster                                                 |
| xml_etree_iterparse     | 115 ms                                                 | 110 ms: 1.05x faster                                                  |
| regex_dna               | 227 ms                                                 | 219 ms: 1.04x faster                                                  |
| pickle_dict             | 29.6 us                                                | 28.6 us: 1.03x faster                                                 |
| python_startup_no_site  | 5.93 ms                                                | 5.77 ms: 1.03x faster                                                 |
| pidigits                | 191 ms                                                 | 188 ms: 1.02x faster                                                  |
| unpickle_list           | 5.20 us                                                | 5.13 us: 1.01x faster                                                 |
| python_startup          | 14.6 ms                                                | 14.6 ms: 1.00x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.23x faster                                                          |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.07x