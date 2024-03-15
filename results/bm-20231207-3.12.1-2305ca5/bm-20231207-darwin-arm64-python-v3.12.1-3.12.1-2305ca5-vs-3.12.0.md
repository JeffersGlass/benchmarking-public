
# Results vs. 3.12.0

- fork: python
- ref: v3.12.1
- machine: darwin-arm64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.01x faster
- HPT reliability: 99.92%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 167 ms: 1.01x faster                                   |
| chameleon      | 4.70 ms                                                | 4.50 ms: 1.04x faster                                  |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.01x faster                                 |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_io          | 668 ms                                                 | 655 ms: 1.02x faster                                   |
| async_tree_none_tg     | 258 ms                                                 | 252 ms: 1.02x faster                                   |
| async_tree_none        | 266 ms                                                 | 260 ms: 1.02x faster                                   |
| async_tree_memoization | 312 ms                                                 | 306 ms: 1.02x faster                                   |
| async_tree_io_tg       | 669 ms                                                 | 660 ms: 1.01x faster                                   |
| Geometric mean         | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                   |
| float          | 55.8 ms                                                | 56.5 ms: 1.01x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                           |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 73.7 ms: 1.06x faster                                  |
| regex_dna      | 154 ms                                                 | 152 ms: 1.01x faster                                   |
| regex_effbot   | 2.64 ms                                                | 2.69 ms: 1.02x slower                                  |
| regex_v8       | 16.0 ms                                                | 16.3 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 188 us: 1.06x faster                                   |
| unpickle_pure_python | 151 us                                                 | 142 us: 1.06x faster                                   |
| xml_etree_process    | 39.7 ms                                                | 38.7 ms: 1.03x faster                                  |
| pickle_list          | 2.89 us                                                | 2.85 us: 1.01x faster                                  |
| xml_etree_generate   | 55.8 ms                                                | 55.8 ms: 1.00x faster                                  |
| pickle               | 7.23 us                                                | 7.27 us: 1.01x slower                                  |
| unpickle             | 9.12 us                                                | 9.24 us: 1.01x slower                                  |
| json_dumps           | 6.22 ms                                                | 6.31 ms: 1.01x slower                                  |
| unpickle_list        | 3.02 us                                                | 3.25 us: 1.08x slower                                  |
| Geometric mean       | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (5): pickle_dict, xml_etree_iterparse, json_loads, tomli_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.9 ms: 1.13x slower                                  |
| python_startup_no_site | 9.37 ms                                                | 11.0 ms: 1.17x slower                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 22.3 ms                                                | 21.2 ms: 1.05x faster                                  |
| mako            | 7.71 ms                                                | 7.59 ms: 1.02x faster                                  |
| Geometric mean  | (ref)                                                  | 1.04x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-darwin-arm64-python-v3.12.1-3.12.1-2305ca5 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 72.5 us: 1.28x faster                                  |
| generators               | 31.1 ms                                                | 25.9 ms: 1.20x faster                                  |
| deltablue                | 2.71 ms                                                | 2.40 ms: 1.13x faster                                  |
| logging_silent           | 76.4 ns                                                | 67.7 ns: 1.13x faster                                  |
| deepcopy_memo            | 27.7 us                                                | 24.9 us: 1.11x faster                                  |
| unpack_sequence          | 31.5 ns                                                | 29.0 ns: 1.09x faster                                  |
| go                       | 102 ms                                                 | 94.3 ms: 1.08x faster                                  |
| hexiom                   | 4.54 ms                                                | 4.23 ms: 1.08x faster                                  |
| asyncio_tcp              | 449 ms                                                 | 418 ms: 1.07x faster                                   |
| richards_super           | 36.0 ms                                                | 33.8 ms: 1.07x faster                                  |
| pickle_pure_python       | 200 us                                                 | 188 us: 1.06x faster                                   |
| scimark_lu               | 76.0 ms                                                | 71.5 ms: 1.06x faster                                  |
| richards                 | 32.1 ms                                                | 30.2 ms: 1.06x faster                                  |
| regex_compile            | 77.9 ms                                                | 73.7 ms: 1.06x faster                                  |
| unpickle_pure_python     | 151 us                                                 | 142 us: 1.06x faster                                   |
| django_template          | 22.3 ms                                                | 21.2 ms: 1.05x faster                                  |
| deepcopy                 | 235 us                                                 | 224 us: 1.05x faster                                   |
| chameleon                | 4.70 ms                                                | 4.50 ms: 1.04x faster                                  |
| scimark_monte_carlo      | 45.0 ms                                                | 43.2 ms: 1.04x faster                                  |
| json                     | 3.09 ms                                                | 2.97 ms: 1.04x faster                                  |
| nqueens                  | 62.4 ms                                                | 60.4 ms: 1.03x faster                                  |
| logging_simple           | 3.69 us                                                | 3.57 us: 1.03x faster                                  |
| logging_format           | 3.98 us                                                | 3.86 us: 1.03x faster                                  |
| sqlglot_parse            | 848 us                                                 | 823 us: 1.03x faster                                   |
| deepcopy_reduce          | 2.07 us                                                | 2.01 us: 1.03x faster                                  |
| raytrace                 | 212 ms                                                 | 206 ms: 1.03x faster                                   |
| sqlglot_transpile        | 1.02 ms                                                | 995 us: 1.03x faster                                   |
| scimark_sor              | 87.4 ms                                                | 85.1 ms: 1.03x faster                                  |
| xml_etree_process        | 39.7 ms                                                | 38.7 ms: 1.03x faster                                  |
| sympy_integrate          | 11.4 ms                                                | 11.1 ms: 1.02x faster                                  |
| dulwich_log              | 29.8 ms                                                | 29.1 ms: 1.02x faster                                  |
| pyflate                  | 316 ms                                                 | 309 ms: 1.02x faster                                   |
| async_tree_io            | 668 ms                                                 | 655 ms: 1.02x faster                                   |
| async_tree_none_tg       | 258 ms                                                 | 252 ms: 1.02x faster                                   |
| async_tree_none          | 266 ms                                                 | 260 ms: 1.02x faster                                   |
| async_tree_memoization   | 312 ms                                                 | 306 ms: 1.02x faster                                   |
| spectral_norm            | 76.4 ms                                                | 75.0 ms: 1.02x faster                                  |
| chaos                    | 42.5 ms                                                | 41.8 ms: 1.02x faster                                  |
| mako                     | 7.71 ms                                                | 7.59 ms: 1.02x faster                                  |
| bench_thread_pool        | 504 us                                                 | 497 us: 1.01x faster                                   |
| 2to3                     | 169 ms                                                 | 167 ms: 1.01x faster                                   |
| docutils                 | 1.50 sec                                               | 1.48 sec: 1.01x faster                                 |
| async_tree_io_tg         | 669 ms                                                 | 660 ms: 1.01x faster                                   |
| pickle_list              | 2.89 us                                                | 2.85 us: 1.01x faster                                  |
| create_gc_cycles         | 701 us                                                 | 693 us: 1.01x faster                                   |
| regex_dna                | 154 ms                                                 | 152 ms: 1.01x faster                                   |
| pprint_pformat           | 1.01 sec                                               | 999 ms: 1.01x faster                                   |
| pycparser                | 677 ms                                                 | 670 ms: 1.01x faster                                   |
| pprint_safe_repr         | 497 ms                                                 | 492 ms: 1.01x faster                                   |
| coroutines               | 19.2 ms                                                | 19.1 ms: 1.01x faster                                  |
| sqlglot_normalize        | 186 ms                                                 | 184 ms: 1.01x faster                                   |
| crypto_pyaes             | 51.9 ms                                                | 51.5 ms: 1.01x faster                                  |
| async_generators         | 304 ms                                                 | 303 ms: 1.00x faster                                   |
| xml_etree_generate       | 55.8 ms                                                | 55.8 ms: 1.00x faster                                  |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                   |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.15 ms: 1.00x slower                                  |
| sympy_str                | 148 ms                                                 | 148 ms: 1.01x slower                                   |
| pickle                   | 7.23 us                                                | 7.27 us: 1.01x slower                                  |
| comprehensions           | 14.5 us                                                | 14.7 us: 1.01x slower                                  |
| pathlib                  | 24.2 ms                                                | 24.5 ms: 1.01x slower                                  |
| meteor_contest           | 71.7 ms                                                | 72.5 ms: 1.01x slower                                  |
| float                    | 55.8 ms                                                | 56.5 ms: 1.01x slower                                  |
| unpickle                 | 9.12 us                                                | 9.24 us: 1.01x slower                                  |
| json_dumps               | 6.22 ms                                                | 6.31 ms: 1.01x slower                                  |
| regex_effbot             | 2.64 ms                                                | 2.69 ms: 1.02x slower                                  |
| bench_mp_pool            | 44.9 ms                                                | 45.8 ms: 1.02x slower                                  |
| coverage                 | 38.9 ms                                                | 39.6 ms: 1.02x slower                                  |
| sympy_expand             | 241 ms                                                 | 247 ms: 1.02x slower                                   |
| regex_v8                 | 16.0 ms                                                | 16.3 ms: 1.02x slower                                  |
| sqlite_synth             | 1.57 us                                                | 1.61 us: 1.02x slower                                  |
| scimark_fft              | 195 ms                                                 | 200 ms: 1.03x slower                                   |
| mdp                      | 1.58 sec                                               | 1.62 sec: 1.03x slower                                 |
| sqlalchemy_imperative    | 6.68 ms                                                | 6.93 ms: 1.04x slower                                  |
| sqlalchemy_declarative   | 62.3 ms                                                | 64.7 ms: 1.04x slower                                  |
| telco                    | 3.68 ms                                                | 3.82 ms: 1.04x slower                                  |
| fannkuch                 | 248 ms                                                 | 265 ms: 1.06x slower                                   |
| aiohttp                  | 1.08 ms                                                | 1.15 ms: 1.07x slower                                  |
| unpickle_list            | 3.02 us                                                | 3.25 us: 1.08x slower                                  |
| gunicorn                 | 1.15 ms                                                | 1.26 ms: 1.10x slower                                  |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.39 sec: 1.12x slower                                 |
| python_startup           | 11.4 ms                                                | 12.9 ms: 1.13x slower                                  |
| python_startup_no_site   | 9.37 ms                                                | 11.0 ms: 1.17x slower                                  |
| mypy2                    | 380 ms                                                 | 469 ms: 1.23x slower                                   |
| Geometric mean           | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (15): tornado_http, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, pickle_dict, xml_etree_iterparse, gc_traversal, sqlglot_optimize, asyncio_websockets, json_loads, dask, sympy_sum, tomli_loads, nbody, xml_etree_parse


# HPT report

- Reliability score: 99.92% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x