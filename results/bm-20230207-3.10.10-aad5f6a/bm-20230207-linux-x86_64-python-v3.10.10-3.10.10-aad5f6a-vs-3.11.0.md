
# Results vs. 3.11.0

- fork: python
- ref: v3.10.10
- machine: linux-x86_64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.20x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 335 ms: 1.27x slower                                     |
| chameleon      | 6.70 ms                                                | 9.13 ms: 1.36x slower                                    |
| docutils       | 2.66 sec                                               | 3.22 sec: 1.21x slower                                   |
| html5lib       | 64.8 ms                                                | 87.5 ms: 1.35x slower                                    |
| tornado_http   | 98.1 ms                                                | 130 ms: 1.33x slower                                     |
| Geometric mean | (ref)                                                  | 1.30x slower                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 997 ms: 1.33x slower                                     |
| async_tree_memoization  | 639 ms                                                 | 856 ms: 1.34x slower                                     |
| async_tree_none         | 528 ms                                                 | 721 ms: 1.37x slower                                     |
| async_tree_io           | 1.29 sec                                               | 1.78 sec: 1.39x slower                                   |
| Geometric mean          | (ref)                                                  | 1.36x slower                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                     |
| float          | 78.9 ms                                                | 109 ms: 1.38x slower                                     |
| nbody          | 96.0 ms                                                | 137 ms: 1.43x slower                                     |
| Geometric mean | (ref)                                                  | 1.24x slower                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.62 ms: 1.03x slower                                    |
| regex_v8       | 22.9 ms                                                | 24.1 ms: 1.06x slower                                    |
| regex_dna      | 205 ms                                                 | 216 ms: 1.06x slower                                     |
| regex_compile  | 141 ms                                                 | 177 ms: 1.25x slower                                     |
| Geometric mean | (ref)                                                  | 1.10x slower                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 30.5 us: 1.13x faster                                    |
| pickle_list          | 4.59 us                                                | 4.17 us: 1.10x faster                                    |
| pickle               | 11.0 us                                                | 10.2 us: 1.08x faster                                    |
| unpickle_list        | 5.21 us                                                | 4.94 us: 1.06x faster                                    |
| xml_etree_parse      | 164 ms                                                 | 161 ms: 1.02x faster                                     |
| json_loads           | 29.2 us                                                | 29.2 us: 1.00x slower                                    |
| json_dumps           | 13.3 ms                                                | 13.6 ms: 1.02x slower                                    |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                     |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                    |
| xml_etree_generate   | 81.1 ms                                                | 93.0 ms: 1.15x slower                                    |
| unpickle_pure_python | 242 us                                                 | 297 us: 1.23x slower                                     |
| xml_etree_process    | 56.9 ms                                                | 74.4 ms: 1.31x slower                                    |
| pickle_pure_python   | 320 us                                                 | 449 us: 1.40x slower                                     |
| Geometric mean       | (ref)                                                  | 1.06x slower                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 5.79 ms: 1.04x faster                                    |
| python_startup         | 8.56 ms                                                | 9.33 ms: 1.09x slower                                    |
| Geometric mean         | (ref)                                                  | 1.02x slower                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 62.6 ms: 1.17x slower                                    |
| genshi_text     | 22.5 ms                                                | 30.1 ms: 1.34x slower                                    |
| mako            | 10.7 ms                                                | 14.6 ms: 1.37x slower                                    |
| django_template | 33.5 ms                                                | 46.6 ms: 1.39x slower                                    |
| Geometric mean  | (ref)                                                  | 1.31x slower                                             |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| pickle_dict             | 34.6 us                                                | 30.5 us: 1.13x faster                                    |
| gc_traversal            | 4.01 ms                                                | 3.54 ms: 1.13x faster                                    |
| coverage                | 78.8 ms                                                | 71.5 ms: 1.10x faster                                    |
| pickle_list             | 4.59 us                                                | 4.17 us: 1.10x faster                                    |
| pickle                  | 11.0 us                                                | 10.2 us: 1.08x faster                                    |
| unpickle_list           | 5.21 us                                                | 4.94 us: 1.06x faster                                    |
| python_startup_no_site  | 6.01 ms                                                | 5.79 ms: 1.04x faster                                    |
| pidigits                | 194 ms                                                 | 189 ms: 1.03x faster                                     |
| telco                   | 6.86 ms                                                | 6.71 ms: 1.02x faster                                    |
| xml_etree_parse         | 164 ms                                                 | 161 ms: 1.02x faster                                     |
| json_loads              | 29.2 us                                                | 29.2 us: 1.00x slower                                    |
| mdp                     | 2.77 sec                                               | 2.82 sec: 1.02x slower                                   |
| generators              | 74.9 ms                                                | 76.1 ms: 1.02x slower                                    |
| json_dumps              | 13.3 ms                                                | 13.6 ms: 1.02x slower                                    |
| xml_etree_iterparse     | 108 ms                                                 | 110 ms: 1.02x slower                                     |
| json                    | 5.24 ms                                                | 5.40 ms: 1.03x slower                                    |
| regex_effbot            | 3.51 ms                                                | 3.62 ms: 1.03x slower                                    |
| meteor_contest          | 109 ms                                                 | 113 ms: 1.04x slower                                     |
| asyncio_tcp             | 875 ms                                                 | 915 ms: 1.04x slower                                     |
| regex_v8                | 22.9 ms                                                | 24.1 ms: 1.06x slower                                    |
| regex_dna               | 205 ms                                                 | 216 ms: 1.06x slower                                     |
| pathlib                 | 18.5 ms                                                | 19.7 ms: 1.07x slower                                    |
| unpickle                | 13.8 us                                                | 14.8 us: 1.07x slower                                    |
| scimark_sparse_mat_mult | 5.03 ms                                                | 5.39 ms: 1.07x slower                                    |
| python_startup          | 8.56 ms                                                | 9.33 ms: 1.09x slower                                    |
| djangocms               | 33.5 us                                                | 36.7 us: 1.09x slower                                    |
| bench_thread_pool       | 834 us                                                 | 919 us: 1.10x slower                                     |
| pylint                  | 476 ms                                                 | 524 ms: 1.10x slower                                     |
| sympy_str               | 297 ms                                                 | 329 ms: 1.11x slower                                     |
| sympy_sum               | 169 ms                                                 | 189 ms: 1.12x slower                                     |
| sympy_expand            | 484 ms                                                 | 546 ms: 1.13x slower                                     |
| coroutines              | 27.0 ms                                                | 30.6 ms: 1.13x slower                                    |
| sympy_integrate         | 21.5 ms                                                | 24.4 ms: 1.13x slower                                    |
| async_generators        | 374 ms                                                 | 426 ms: 1.14x slower                                     |
| create_gc_cycles        | 1.43 ms                                                | 1.63 ms: 1.14x slower                                    |
| nqueens                 | 87.9 ms                                                | 100 ms: 1.14x slower                                     |
| sqlalchemy_imperative   | 18.3 ms                                                | 20.9 ms: 1.14x slower                                    |
| xml_etree_generate      | 81.1 ms                                                | 93.0 ms: 1.15x slower                                    |
| fannkuch                | 405 ms                                                 | 467 ms: 1.15x slower                                     |
| sqlite_synth            | 2.57 us                                                | 2.97 us: 1.15x slower                                    |
| aiohttp                 | 1.12 ms                                                | 1.29 ms: 1.16x slower                                    |
| gunicorn                | 1.20 ms                                                | 1.39 ms: 1.16x slower                                    |
| flaskblogging           | 7.28 ms                                                | 8.47 ms: 1.16x slower                                    |
| dulwich_log             | 64.6 ms                                                | 75.4 ms: 1.17x slower                                    |
| genshi_xml              | 53.4 ms                                                | 62.6 ms: 1.17x slower                                    |
| deepcopy                | 365 us                                                 | 428 us: 1.17x slower                                     |
| scimark_fft             | 345 ms                                                 | 408 ms: 1.18x slower                                     |
| sqlglot_optimize        | 55.3 ms                                                | 65.4 ms: 1.18x slower                                    |
| deepcopy_reduce         | 3.22 us                                                | 3.81 us: 1.18x slower                                    |
| dask                    | 365 ms                                                 | 434 ms: 1.19x slower                                     |
| sqlalchemy_declarative  | 140 ms                                                 | 167 ms: 1.19x slower                                     |
| sqlglot_normalize       | 113 ms                                                 | 136 ms: 1.20x slower                                     |
| docutils                | 2.66 sec                                               | 3.22 sec: 1.21x slower                                   |
| unpickle_pure_python    | 242 us                                                 | 297 us: 1.23x slower                                     |
| deepcopy_memo           | 40.2 us                                                | 49.9 us: 1.24x slower                                    |
| regex_compile           | 141 ms                                                 | 177 ms: 1.25x slower                                     |
| 2to3                    | 264 ms                                                 | 335 ms: 1.27x slower                                     |
| pycparser               | 1.19 sec                                               | 1.54 sec: 1.30x slower                                   |
| pprint_pformat          | 1.55 sec                                               | 2.02 sec: 1.30x slower                                   |
| pprint_safe_repr        | 747 ms                                                 | 975 ms: 1.30x slower                                     |
| xml_etree_process       | 56.9 ms                                                | 74.4 ms: 1.31x slower                                    |
| thrift                  | 784 us                                                 | 1.04 ms: 1.32x slower                                    |
| spectral_norm           | 108 ms                                                 | 143 ms: 1.32x slower                                     |
| tornado_http            | 98.1 ms                                                | 130 ms: 1.33x slower                                     |
| async_tree_cpu_io_mixed | 749 ms                                                 | 997 ms: 1.33x slower                                     |
| genshi_text             | 22.5 ms                                                | 30.1 ms: 1.34x slower                                    |
| async_tree_memoization  | 639 ms                                                 | 856 ms: 1.34x slower                                     |
| html5lib                | 64.8 ms                                                | 87.5 ms: 1.35x slower                                    |
| logging_format          | 6.81 us                                                | 9.20 us: 1.35x slower                                    |
| logging_simple          | 6.22 us                                                | 8.41 us: 1.35x slower                                    |
| chameleon               | 6.70 ms                                                | 9.13 ms: 1.36x slower                                    |
| async_tree_none         | 528 ms                                                 | 721 ms: 1.37x slower                                     |
| hexiom                  | 6.89 ms                                                | 9.42 ms: 1.37x slower                                    |
| mako                    | 10.7 ms                                                | 14.6 ms: 1.37x slower                                    |
| scimark_lu              | 116 ms                                                 | 160 ms: 1.38x slower                                     |
| sqlglot_transpile       | 1.75 ms                                                | 2.41 ms: 1.38x slower                                    |
| float                   | 78.9 ms                                                | 109 ms: 1.38x slower                                     |
| async_tree_io           | 1.29 sec                                               | 1.78 sec: 1.39x slower                                   |
| django_template         | 33.5 ms                                                | 46.6 ms: 1.39x slower                                    |
| pickle_pure_python      | 320 us                                                 | 449 us: 1.40x slower                                     |
| sqlglot_parse           | 1.43 ms                                                | 2.03 ms: 1.41x slower                                    |
| nbody                   | 96.0 ms                                                | 137 ms: 1.43x slower                                     |
| richards                | 49.8 ms                                                | 72.6 ms: 1.46x slower                                    |
| unpack_sequence         | 43.5 ns                                                | 64.0 ns: 1.47x slower                                    |
| chaos                   | 71.9 ms                                                | 106 ms: 1.48x slower                                     |
| scimark_monte_carlo     | 70.7 ms                                                | 105 ms: 1.49x slower                                     |
| crypto_pyaes            | 76.7 ms                                                | 115 ms: 1.50x slower                                     |
| raytrace                | 309 ms                                                 | 463 ms: 1.50x slower                                     |
| pyflate                 | 434 ms                                                 | 659 ms: 1.52x slower                                     |
| go                      | 149 ms                                                 | 226 ms: 1.52x slower                                     |
| logging_silent          | 111 ns                                                 | 174 ns: 1.57x slower                                     |
| scimark_sor             | 121 ms                                                 | 193 ms: 1.59x slower                                     |
| deltablue               | 3.92 ms                                                | 7.41 ms: 1.89x slower                                    |
| Geometric mean          | (ref)                                                  | 1.20x slower                                             |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.17x
- 95% likely to have a slowdown of 1.16x
- 99% likely to have a slowdown of 1.15x


# Memory

- memory change: 0.95x