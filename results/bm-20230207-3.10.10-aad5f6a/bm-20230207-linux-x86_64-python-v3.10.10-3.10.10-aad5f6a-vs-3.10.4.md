
# Results vs. 3.10.4

- fork: python
- ref: v3.10.10
- machine: linux-x86_64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 335 ms: 1.04x faster                                     |
| chameleon      | 9.68 ms                                                | 9.13 ms: 1.06x faster                                    |
| docutils       | 3.30 sec                                               | 3.22 sec: 1.02x faster                                   |
| html5lib       | 88.9 ms                                                | 87.5 ms: 1.02x faster                                    |
| tornado_http   | 136 ms                                                 | 130 ms: 1.05x faster                                     |
| Geometric mean | (ref)                                                  | 1.04x faster                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| async_tree_cpu_io_mixed | 1.02 sec                                               | 997 ms: 1.02x faster                                     |
| async_tree_memoization  | 870 ms                                                 | 856 ms: 1.02x faster                                     |
| Geometric mean          | (ref)                                                  | 1.01x faster                                             |

Benchmark hidden because not significant (2): async_tree_none, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| nbody          | 154 ms                                                 | 137 ms: 1.12x faster                                     |
| float          | 117 ms                                                 | 109 ms: 1.07x faster                                     |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                     |
| Geometric mean | (ref)                                                  | 1.07x faster                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 24.1 ms: 1.15x faster                                    |
| regex_compile  | 188 ms                                                 | 177 ms: 1.07x faster                                     |
| regex_dna      | 227 ms                                                 | 216 ms: 1.05x faster                                     |
| Geometric mean | (ref)                                                  | 1.07x faster                                             |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.17 us: 1.22x faster                                    |
| unpickle_pure_python | 331 us                                                 | 297 us: 1.11x faster                                     |
| pickle_pure_python   | 484 us                                                 | 449 us: 1.08x faster                                     |
| xml_etree_generate   | 99.4 ms                                                | 93.0 ms: 1.07x faster                                    |
| json_loads           | 31.2 us                                                | 29.2 us: 1.07x faster                                    |
| xml_etree_process    | 79.1 ms                                                | 74.4 ms: 1.06x faster                                    |
| unpickle_list        | 5.20 us                                                | 4.94 us: 1.05x faster                                    |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                     |
| xml_etree_parse      | 168 ms                                                 | 161 ms: 1.04x faster                                     |
| pickle               | 10.7 us                                                | 10.2 us: 1.04x faster                                    |
| json_dumps           | 14.2 ms                                                | 13.6 ms: 1.04x faster                                    |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                    |
| pickle_dict          | 29.6 us                                                | 30.5 us: 1.03x slower                                    |
| Geometric mean       | (ref)                                                  | 1.06x faster                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.33 ms: 1.56x faster                                    |
| python_startup_no_site | 5.93 ms                                                | 5.79 ms: 1.02x faster                                    |
| Geometric mean         | (ref)                                                  | 1.27x faster                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| mako            | 16.3 ms                                                | 14.6 ms: 1.12x faster                                    |
| genshi_text     | 31.8 ms                                                | 30.1 ms: 1.06x faster                                    |
| genshi_xml      | 66.0 ms                                                | 62.6 ms: 1.06x faster                                    |
| django_template | 48.2 ms                                                | 46.6 ms: 1.03x faster                                    |
| Geometric mean  | (ref)                                                  | 1.07x faster                                             |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-linux-x86_64-python-v3.10.10-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------:|
| python_startup          | 14.6 ms                                                | 9.33 ms: 1.56x faster                                    |
| pickle_list             | 5.08 us                                                | 4.17 us: 1.22x faster                                    |
| scimark_sparse_mat_mult | 6.47 ms                                                | 5.39 ms: 1.20x faster                                    |
| spectral_norm           | 170 ms                                                 | 143 ms: 1.19x faster                                     |
| deepcopy_memo           | 58.5 us                                                | 49.9 us: 1.17x faster                                    |
| regex_v8                | 27.8 ms                                                | 24.1 ms: 1.15x faster                                    |
| coroutines              | 35.1 ms                                                | 30.6 ms: 1.14x faster                                    |
| scimark_fft             | 466 ms                                                 | 408 ms: 1.14x faster                                     |
| fannkuch                | 532 ms                                                 | 467 ms: 1.14x faster                                     |
| scimark_sor             | 220 ms                                                 | 193 ms: 1.14x faster                                     |
| scimark_monte_carlo     | 118 ms                                                 | 105 ms: 1.13x faster                                     |
| nbody                   | 154 ms                                                 | 137 ms: 1.12x faster                                     |
| deepcopy                | 479 us                                                 | 428 us: 1.12x faster                                     |
| dulwich_log             | 84.3 ms                                                | 75.4 ms: 1.12x faster                                    |
| mako                    | 16.3 ms                                                | 14.6 ms: 1.12x faster                                    |
| sqlalchemy_imperative   | 23.3 ms                                                | 20.9 ms: 1.11x faster                                    |
| aiohttp                 | 1.44 ms                                                | 1.29 ms: 1.11x faster                                    |
| crypto_pyaes            | 128 ms                                                 | 115 ms: 1.11x faster                                     |
| unpickle_pure_python    | 331 us                                                 | 297 us: 1.11x faster                                     |
| coverage                | 79.4 ms                                                | 71.5 ms: 1.11x faster                                    |
| hexiom                  | 10.4 ms                                                | 9.42 ms: 1.10x faster                                    |
| gunicorn                | 1.53 ms                                                | 1.39 ms: 1.10x faster                                    |
| scimark_lu              | 176 ms                                                 | 160 ms: 1.10x faster                                     |
| raytrace                | 507 ms                                                 | 463 ms: 1.10x faster                                     |
| deepcopy_reduce         | 4.17 us                                                | 3.81 us: 1.09x faster                                    |
| richards                | 79.3 ms                                                | 72.6 ms: 1.09x faster                                    |
| logging_silent          | 190 ns                                                 | 174 ns: 1.09x faster                                     |
| pyflate                 | 716 ms                                                 | 659 ms: 1.09x faster                                     |
| chaos                   | 115 ms                                                 | 106 ms: 1.09x faster                                     |
| telco                   | 7.27 ms                                                | 6.71 ms: 1.08x faster                                    |
| pickle_pure_python      | 484 us                                                 | 449 us: 1.08x faster                                     |
| float                   | 117 ms                                                 | 109 ms: 1.07x faster                                     |
| bench_thread_pool       | 986 us                                                 | 919 us: 1.07x faster                                     |
| sqlglot_parse           | 2.17 ms                                                | 2.03 ms: 1.07x faster                                    |
| xml_etree_generate      | 99.4 ms                                                | 93.0 ms: 1.07x faster                                    |
| regex_compile           | 188 ms                                                 | 177 ms: 1.07x faster                                     |
| deltablue               | 7.91 ms                                                | 7.41 ms: 1.07x faster                                    |
| json_loads              | 31.2 us                                                | 29.2 us: 1.07x faster                                    |
| sqlglot_transpile       | 2.57 ms                                                | 2.41 ms: 1.07x faster                                    |
| xml_etree_process       | 79.1 ms                                                | 74.4 ms: 1.06x faster                                    |
| chameleon               | 9.68 ms                                                | 9.13 ms: 1.06x faster                                    |
| go                      | 240 ms                                                 | 226 ms: 1.06x faster                                     |
| sympy_integrate         | 25.8 ms                                                | 24.4 ms: 1.06x faster                                    |
| meteor_contest          | 120 ms                                                 | 113 ms: 1.06x faster                                     |
| sqlglot_optimize        | 69.2 ms                                                | 65.4 ms: 1.06x faster                                    |
| genshi_text             | 31.8 ms                                                | 30.1 ms: 1.06x faster                                    |
| nqueens                 | 106 ms                                                 | 100 ms: 1.06x faster                                     |
| genshi_xml              | 66.0 ms                                                | 62.6 ms: 1.06x faster                                    |
| json                    | 5.69 ms                                                | 5.40 ms: 1.05x faster                                    |
| unpickle_list           | 5.20 us                                                | 4.94 us: 1.05x faster                                    |
| sqlglot_normalize       | 143 ms                                                 | 136 ms: 1.05x faster                                     |
| generators              | 80.1 ms                                                | 76.1 ms: 1.05x faster                                    |
| pylint                  | 551 ms                                                 | 524 ms: 1.05x faster                                     |
| sympy_str               | 346 ms                                                 | 329 ms: 1.05x faster                                     |
| tornado_http            | 136 ms                                                 | 130 ms: 1.05x faster                                     |
| djangocms               | 38.4 us                                                | 36.7 us: 1.05x faster                                    |
| regex_dna               | 227 ms                                                 | 216 ms: 1.05x faster                                     |
| xml_etree_iterparse     | 115 ms                                                 | 110 ms: 1.05x faster                                     |
| pprint_safe_repr        | 1.02 sec                                               | 975 ms: 1.04x faster                                     |
| xml_etree_parse         | 168 ms                                                 | 161 ms: 1.04x faster                                     |
| pickle                  | 10.7 us                                                | 10.2 us: 1.04x faster                                    |
| async_generators        | 444 ms                                                 | 426 ms: 1.04x faster                                     |
| pprint_pformat          | 2.10 sec                                               | 2.02 sec: 1.04x faster                                   |
| sympy_sum               | 196 ms                                                 | 189 ms: 1.04x faster                                     |
| json_dumps              | 14.2 ms                                                | 13.6 ms: 1.04x faster                                    |
| 2to3                    | 348 ms                                                 | 335 ms: 1.04x faster                                     |
| pathlib                 | 20.5 ms                                                | 19.7 ms: 1.04x faster                                    |
| sympy_expand            | 566 ms                                                 | 546 ms: 1.04x faster                                     |
| thrift                  | 1.07 ms                                                | 1.04 ms: 1.03x faster                                    |
| django_template         | 48.2 ms                                                | 46.6 ms: 1.03x faster                                    |
| sqlalchemy_declarative  | 172 ms                                                 | 167 ms: 1.03x faster                                     |
| pycparser               | 1.58 sec                                               | 1.54 sec: 1.02x faster                                   |
| gc_traversal            | 3.62 ms                                                | 3.54 ms: 1.02x faster                                    |
| python_startup_no_site  | 5.93 ms                                                | 5.79 ms: 1.02x faster                                    |
| docutils                | 3.30 sec                                               | 3.22 sec: 1.02x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 997 ms: 1.02x faster                                     |
| sqlite_synth            | 3.02 us                                                | 2.97 us: 1.02x faster                                    |
| async_tree_memoization  | 870 ms                                                 | 856 ms: 1.02x faster                                     |
| html5lib                | 88.9 ms                                                | 87.5 ms: 1.02x faster                                    |
| dask                    | 441 ms                                                 | 434 ms: 1.01x faster                                     |
| flaskblogging           | 8.58 ms                                                | 8.47 ms: 1.01x faster                                    |
| pidigits                | 191 ms                                                 | 189 ms: 1.01x faster                                     |
| mdp                     | 2.85 sec                                               | 2.82 sec: 1.01x faster                                   |
| asyncio_tcp             | 922 ms                                                 | 915 ms: 1.01x faster                                     |
| create_gc_cycles        | 1.62 ms                                                | 1.63 ms: 1.01x slower                                    |
| logging_format          | 9.09 us                                                | 9.20 us: 1.01x slower                                    |
| logging_simple          | 8.30 us                                                | 8.41 us: 1.01x slower                                    |
| unpickle                | 14.4 us                                                | 14.8 us: 1.03x slower                                    |
| pickle_dict             | 29.6 us                                                | 30.5 us: 1.03x slower                                    |
| unpack_sequence         | 60.0 ns                                                | 64.0 ns: 1.07x slower                                    |
| Geometric mean          | (ref)                                                  | 1.07x faster                                             |

Benchmark hidden because not significant (4): async_tree_none, regex_effbot, bench_mp_pool, async_tree_io
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, comprehensions, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: 1.02x