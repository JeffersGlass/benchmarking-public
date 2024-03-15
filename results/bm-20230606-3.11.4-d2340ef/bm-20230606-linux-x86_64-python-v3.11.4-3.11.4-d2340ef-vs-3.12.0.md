
# Results vs. 3.12.0

- fork: python
- ref: v3.11.4
- machine: linux-x86_64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 258 ms: 1.06x faster                                   |
| chameleon      | 7.41 ms                                                | 6.58 ms: 1.13x faster                                  |
| docutils       | 2.77 sec                                               | 2.57 sec: 1.08x faster                                 |
| tornado_http   | 103 ms                                                 | 96.6 ms: 1.06x faster                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 738 ms: 1.02x slower                                   |
| async_tree_memoization  | 578 ms                                                 | 638 ms: 1.10x slower                                   |
| async_tree_none         | 472 ms                                                 | 523 ms: 1.11x slower                                   |
| async_tree_io           | 1.16 sec                                               | 1.29 sec: 1.12x slower                                 |
| Geometric mean          | (ref)                                                  | 1.09x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 77.1 ms: 1.10x faster                                  |
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| nbody          | 97.0 ms                                                | 99.4 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 136 ms: 1.09x faster                                   |
| regex_dna      | 212 ms                                                 | 200 ms: 1.06x faster                                   |
| regex_effbot   | 3.61 ms                                                | 3.45 ms: 1.05x faster                                  |
| regex_v8       | 23.1 ms                                                | 22.2 ms: 1.04x faster                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.01 us: 1.27x faster                                  |
| unpickle             | 15.9 us                                                | 13.1 us: 1.21x faster                                  |
| pickle               | 11.6 us                                                | 9.76 us: 1.19x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 76.5 ms: 1.16x faster                                  |
| pickle_dict          | 35.5 us                                                | 30.7 us: 1.16x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 53.9 ms: 1.14x faster                                  |
| json_loads           | 28.5 us                                                | 26.2 us: 1.09x faster                                  |
| pickle_pure_python   | 324 us                                                 | 302 us: 1.07x faster                                   |
| tomli_loads          | 2.33 sec                                               | 2.19 sec: 1.06x faster                                 |
| unpickle_list        | 5.29 us                                                | 5.02 us: 1.05x faster                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.02x faster                                   |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.01x faster                                   |
| json_dumps           | 10.4 ms                                                | 12.6 ms: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.08x faster                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.01 ms: 1.16x faster                                  |
| python_startup         | 9.55 ms                                                | 8.53 ms: 1.12x faster                                  |
| Geometric mean         | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.80 ms: 1.21x faster                                  |
| django_template | 34.6 ms                                                | 33.0 ms: 1.05x faster                                  |
| Geometric mean  | (ref)                                                  | 1.13x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators         | 463 ms                                                 | 361 ms: 1.28x faster                                   |
| pickle_list              | 5.08 us                                                | 4.01 us: 1.27x faster                                  |
| unpack_sequence          | 54.0 ns                                                | 43.6 ns: 1.24x faster                                  |
| mako                     | 11.9 ms                                                | 9.80 ms: 1.21x faster                                  |
| unpickle                 | 15.9 us                                                | 13.1 us: 1.21x faster                                  |
| pickle                   | 11.6 us                                                | 9.76 us: 1.19x faster                                  |
| spectral_norm            | 115 ms                                                 | 97.1 ms: 1.18x faster                                  |
| scimark_fft              | 382 ms                                                 | 326 ms: 1.17x faster                                   |
| xml_etree_generate       | 89.2 ms                                                | 76.5 ms: 1.16x faster                                  |
| pickle_dict              | 35.5 us                                                | 30.7 us: 1.16x faster                                  |
| python_startup_no_site   | 6.94 ms                                                | 6.01 ms: 1.16x faster                                  |
| pyflate                  | 482 ms                                                 | 421 ms: 1.15x faster                                   |
| xml_etree_process        | 61.7 ms                                                | 53.9 ms: 1.14x faster                                  |
| deepcopy_reduce          | 3.35 us                                                | 2.94 us: 1.14x faster                                  |
| sqlite_synth             | 2.83 us                                                | 2.51 us: 1.13x faster                                  |
| chameleon                | 7.41 ms                                                | 6.58 ms: 1.13x faster                                  |
| python_startup           | 9.55 ms                                                | 8.53 ms: 1.12x faster                                  |
| deepcopy_memo            | 40.7 us                                                | 36.5 us: 1.12x faster                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 67.7 ms: 1.11x faster                                  |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.58 ms: 1.11x faster                                  |
| logging_format           | 7.23 us                                                | 6.58 us: 1.10x faster                                  |
| float                    | 84.7 ms                                                | 77.1 ms: 1.10x faster                                  |
| scimark_sor              | 129 ms                                                 | 118 ms: 1.10x faster                                   |
| pprint_safe_repr         | 776 ms                                                 | 707 ms: 1.10x faster                                   |
| crypto_pyaes             | 81.9 ms                                                | 74.6 ms: 1.10x faster                                  |
| regex_compile            | 148 ms                                                 | 136 ms: 1.09x faster                                   |
| json_loads               | 28.5 us                                                | 26.2 us: 1.09x faster                                  |
| deepcopy                 | 371 us                                                 | 341 us: 1.09x faster                                   |
| json                     | 5.26 ms                                                | 4.85 ms: 1.08x faster                                  |
| pprint_pformat           | 1.57 sec                                               | 1.45 sec: 1.08x faster                                 |
| scimark_lu               | 118 ms                                                 | 109 ms: 1.08x faster                                   |
| docutils                 | 2.77 sec                                               | 2.57 sec: 1.08x faster                                 |
| pathlib                  | 19.3 ms                                                | 18.0 ms: 1.08x faster                                  |
| pickle_pure_python       | 324 us                                                 | 302 us: 1.07x faster                                   |
| telco                    | 7.10 ms                                                | 6.62 ms: 1.07x faster                                  |
| tomli_loads              | 2.33 sec                                               | 2.19 sec: 1.06x faster                                 |
| 2to3                     | 274 ms                                                 | 258 ms: 1.06x faster                                   |
| tornado_http             | 103 ms                                                 | 96.6 ms: 1.06x faster                                  |
| meteor_contest           | 112 ms                                                 | 106 ms: 1.06x faster                                   |
| logging_simple           | 6.46 us                                                | 6.09 us: 1.06x faster                                  |
| raytrace                 | 312 ms                                                 | 294 ms: 1.06x faster                                   |
| regex_dna                | 212 ms                                                 | 200 ms: 1.06x faster                                   |
| gunicorn                 | 1.24 ms                                                | 1.17 ms: 1.06x faster                                  |
| sqlalchemy_declarative   | 147 ms                                                 | 139 ms: 1.06x faster                                   |
| fannkuch                 | 417 ms                                                 | 394 ms: 1.06x faster                                   |
| unpickle_list            | 5.29 us                                                | 5.02 us: 1.05x faster                                  |
| aiohttp                  | 1.15 ms                                                | 1.09 ms: 1.05x faster                                  |
| regex_effbot             | 3.61 ms                                                | 3.45 ms: 1.05x faster                                  |
| django_template          | 34.6 ms                                                | 33.0 ms: 1.05x faster                                  |
| dulwich_log              | 68.5 ms                                                | 65.5 ms: 1.05x faster                                  |
| sqlalchemy_imperative    | 18.7 ms                                                | 17.9 ms: 1.05x faster                                  |
| regex_v8                 | 23.1 ms                                                | 22.2 ms: 1.04x faster                                  |
| sqlglot_optimize         | 54.8 ms                                                | 53.0 ms: 1.03x faster                                  |
| sympy_str                | 300 ms                                                 | 290 ms: 1.03x faster                                   |
| dask                     | 372 ms                                                 | 360 ms: 1.03x faster                                   |
| bench_thread_pool        | 842 us                                                 | 816 us: 1.03x faster                                   |
| sympy_integrate          | 21.4 ms                                                | 20.9 ms: 1.03x faster                                  |
| xml_etree_iterparse      | 107 ms                                                 | 104 ms: 1.02x faster                                   |
| sympy_sum                | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                   |
| sympy_expand             | 478 ms                                                 | 470 ms: 1.02x faster                                   |
| logging_silent           | 104 ns                                                 | 103 ns: 1.02x faster                                   |
| mdp                      | 2.63 sec                                               | 2.60 sec: 1.01x faster                                 |
| sqlglot_transpile        | 1.68 ms                                                | 1.67 ms: 1.01x faster                                  |
| unpickle_pure_python     | 230 us                                                 | 229 us: 1.01x faster                                   |
| go                       | 139 ms                                                 | 140 ms: 1.00x slower                                   |
| create_gc_cycles         | 1.48 ms                                                | 1.49 ms: 1.01x slower                                  |
| sqlglot_parse            | 1.36 ms                                                | 1.37 ms: 1.01x slower                                  |
| pidigits                 | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| hexiom                   | 6.41 ms                                                | 6.50 ms: 1.01x slower                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 738 ms: 1.02x slower                                   |
| nbody                    | 97.0 ms                                                | 99.4 ms: 1.02x slower                                  |
| comprehensions           | 21.8 us                                                | 22.6 us: 1.04x slower                                  |
| chaos                    | 67.0 ms                                                | 70.2 ms: 1.05x slower                                  |
| richards                 | 45.8 ms                                                | 48.5 ms: 1.06x slower                                  |
| gc_traversal             | 3.79 ms                                                | 4.04 ms: 1.07x slower                                  |
| async_tree_memoization   | 578 ms                                                 | 638 ms: 1.10x slower                                   |
| async_tree_none          | 472 ms                                                 | 523 ms: 1.11x slower                                   |
| coroutines               | 23.2 ms                                                | 25.9 ms: 1.12x slower                                  |
| async_tree_io            | 1.16 sec                                               | 1.29 sec: 1.12x slower                                 |
| richards_super           | 51.5 ms                                                | 60.0 ms: 1.16x slower                                  |
| json_dumps               | 10.4 ms                                                | 12.6 ms: 1.21x slower                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 3.15 sec: 1.76x slower                                 |
| asyncio_tcp              | 491 ms                                                 | 922 ms: 1.88x slower                                   |
| generators               | 31.2 ms                                                | 73.7 ms: 2.36x slower                                  |
| typing_runtime_protocols | 158 us                                                 | 495 us: 3.13x slower                                   |
| Geometric mean           | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (5): nqueens, deltablue, bench_mp_pool, pycparser, xml_etree_parse
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
Ignored benchmarks (7) of results/bm-20230606-3.11.4-d2340ef/bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.96x