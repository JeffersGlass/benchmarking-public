# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_arena
- machine: linux-x86_64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.64%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 276 ms: 1.01x slower                                                 |
| chameleon      | 7.41 ms                                                | 6.86 ms: 1.08x faster                                                |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                               |
| tornado_http   | 103 ms                                                 | 96.9 ms: 1.06x faster                                                |
| Geometric mean | (ref)                                                  | 1.04x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 435 ms: 1.08x faster                                                 |
| async_tree_memoization  | 578 ms                                                 | 561 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed | 726 ms                                                 | 707 ms: 1.03x faster                                                 |
| async_tree_none_tg      | 450 ms                                                 | 446 ms: 1.01x faster                                                 |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                               |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 77.9 ms: 1.09x faster                                                |
| nbody          | 97.0 ms                                                | 92.0 ms: 1.05x faster                                                |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.05x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.05x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                |
| regex_v8       | 23.1 ms                                                | 24.2 ms: 1.05x slower                                                |
| regex_dna      | 212 ms                                                 | 224 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.01 sec: 1.16x faster                                               |
| pickle_pure_python   | 324 us                                                 | 297 us: 1.09x faster                                                 |
| unpickle_list        | 5.29 us                                                | 4.90 us: 1.08x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 58.2 ms: 1.06x faster                                                |
| xml_etree_generate   | 89.2 ms                                                | 84.9 ms: 1.05x faster                                                |
| json_loads           | 28.5 us                                                | 27.5 us: 1.04x faster                                                |
| pickle_list          | 5.08 us                                                | 4.90 us: 1.04x faster                                                |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                                |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                 |
| pickle_dict          | 35.5 us                                                | 34.7 us: 1.02x faster                                                |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                 |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                |
| unpickle_pure_python | 230 us                                                 | 236 us: 1.03x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                         |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.1 ms: 1.27x slower                                                |
| python_startup_no_site | 6.94 ms                                                | 10.7 ms: 1.55x slower                                                |
| Geometric mean         | (ref)                                                  | 1.40x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                |
| django_template | 34.6 ms                                                | 34.3 ms: 1.01x faster                                                |
| Geometric mean  | (ref)                                                  | 1.05x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.44x faster                                                 |
| comprehensions           | 21.8 us                                                | 17.1 us: 1.27x faster                                                |
| tomli_loads              | 2.33 sec                                               | 2.01 sec: 1.16x faster                                               |
| logging_format           | 7.23 us                                                | 6.24 us: 1.16x faster                                                |
| scimark_fft              | 382 ms                                                 | 333 ms: 1.15x faster                                                 |
| logging_simple           | 6.46 us                                                | 5.65 us: 1.14x faster                                                |
| crypto_pyaes             | 81.9 ms                                                | 73.7 ms: 1.11x faster                                                |
| deepcopy_reduce          | 3.35 us                                                | 3.02 us: 1.11x faster                                                |
| deltablue                | 3.72 ms                                                | 3.39 ms: 1.10x faster                                                |
| pickle_pure_python       | 324 us                                                 | 297 us: 1.09x faster                                                 |
| mako                     | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                |
| float                    | 84.7 ms                                                | 77.9 ms: 1.09x faster                                                |
| raytrace                 | 312 ms                                                 | 288 ms: 1.08x faster                                                 |
| sympy_sum                | 169 ms                                                 | 156 ms: 1.08x faster                                                 |
| async_tree_none          | 472 ms                                                 | 435 ms: 1.08x faster                                                 |
| gc_traversal             | 3.79 ms                                                | 3.51 ms: 1.08x faster                                                |
| chameleon                | 7.41 ms                                                | 6.86 ms: 1.08x faster                                                |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.68 ms: 1.08x faster                                                |
| unpickle_list            | 5.29 us                                                | 4.90 us: 1.08x faster                                                |
| sympy_str                | 300 ms                                                 | 280 ms: 1.07x faster                                                 |
| deepcopy                 | 371 us                                                 | 347 us: 1.07x faster                                                 |
| logging_silent           | 104 ns                                                 | 97.9 ns: 1.07x faster                                                |
| chaos                    | 67.0 ms                                                | 62.9 ms: 1.06x faster                                                |
| generators               | 31.2 ms                                                | 29.3 ms: 1.06x faster                                                |
| xml_etree_process        | 61.7 ms                                                | 58.2 ms: 1.06x faster                                                |
| sqlglot_parse            | 1.36 ms                                                | 1.28 ms: 1.06x faster                                                |
| fannkuch                 | 417 ms                                                 | 393 ms: 1.06x faster                                                 |
| tornado_http             | 103 ms                                                 | 96.9 ms: 1.06x faster                                                |
| scimark_monte_carlo      | 75.1 ms                                                | 71.0 ms: 1.06x faster                                                |
| deepcopy_memo            | 40.7 us                                                | 38.6 us: 1.06x faster                                                |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.06x faster                                                 |
| nbody                    | 97.0 ms                                                | 92.0 ms: 1.05x faster                                                |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                |
| xml_etree_generate       | 89.2 ms                                                | 84.9 ms: 1.05x faster                                                |
| regex_compile            | 148 ms                                                 | 142 ms: 1.05x faster                                                 |
| pprint_safe_repr         | 776 ms                                                 | 746 ms: 1.04x faster                                                 |
| json_loads               | 28.5 us                                                | 27.5 us: 1.04x faster                                                |
| pickle_list              | 5.08 us                                                | 4.90 us: 1.04x faster                                                |
| json                     | 5.26 ms                                                | 5.07 ms: 1.04x faster                                                |
| sqlglot_transpile        | 1.68 ms                                                | 1.63 ms: 1.04x faster                                                |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                                 |
| async_tree_memoization   | 578 ms                                                 | 561 ms: 1.03x faster                                                 |
| sympy_integrate          | 21.4 ms                                                | 20.8 ms: 1.03x faster                                                |
| spectral_norm            | 115 ms                                                 | 112 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 707 ms: 1.03x faster                                                 |
| docutils                 | 2.77 sec                                               | 2.70 sec: 1.03x faster                                               |
| pickle                   | 11.6 us                                                | 11.3 us: 1.02x faster                                                |
| xml_etree_parse          | 159 ms                                                 | 156 ms: 1.02x faster                                                 |
| pyflate                  | 482 ms                                                 | 471 ms: 1.02x faster                                                 |
| pickle_dict              | 35.5 us                                                | 34.7 us: 1.02x faster                                                |
| pycparser                | 1.18 sec                                               | 1.16 sec: 1.02x faster                                               |
| coroutines               | 23.2 ms                                                | 22.8 ms: 1.02x faster                                                |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                 |
| django_template          | 34.6 ms                                                | 34.3 ms: 1.01x faster                                                |
| async_tree_none_tg       | 450 ms                                                 | 446 ms: 1.01x faster                                                 |
| sympy_expand             | 478 ms                                                 | 475 ms: 1.01x faster                                                 |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                 |
| asyncio_tcp              | 491 ms                                                 | 489 ms: 1.00x faster                                                 |
| bench_thread_pool        | 842 us                                                 | 844 us: 1.00x slower                                                 |
| json_dumps               | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                |
| 2to3                     | 274 ms                                                 | 276 ms: 1.01x slower                                                 |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                               |
| richards_super           | 51.5 ms                                                | 52.2 ms: 1.01x slower                                                |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.01x slower                                                |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                               |
| sqlglot_optimize         | 54.8 ms                                                | 55.7 ms: 1.02x slower                                                |
| aiohttp                  | 1.15 ms                                                | 1.17 ms: 1.02x slower                                                |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| gunicorn                 | 1.24 ms                                                | 1.27 ms: 1.02x slower                                                |
| unpickle_pure_python     | 230 us                                                 | 236 us: 1.03x slower                                                 |
| regex_effbot             | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                |
| regex_v8                 | 23.1 ms                                                | 24.2 ms: 1.05x slower                                                |
| regex_dna                | 212 ms                                                 | 224 ms: 1.05x slower                                                 |
| nqueens                  | 83.3 ms                                                | 89.0 ms: 1.07x slower                                                |
| hexiom                   | 6.41 ms                                                | 6.98 ms: 1.09x slower                                                |
| scimark_lu               | 118 ms                                                 | 129 ms: 1.09x slower                                                 |
| go                       | 139 ms                                                 | 155 ms: 1.11x slower                                                 |
| telco                    | 7.10 ms                                                | 8.26 ms: 1.16x slower                                                |
| bench_mp_pool            | 24.0 ms                                                | 28.1 ms: 1.17x slower                                                |
| python_startup           | 9.55 ms                                                | 12.1 ms: 1.27x slower                                                |
| coverage                 | 72.7 ms                                                | 95.9 ms: 1.32x slower                                                |
| dask                     | 372 ms                                                 | 530 ms: 1.43x slower                                                 |
| python_startup_no_site   | 6.94 ms                                                | 10.7 ms: 1.55x slower                                                |
| unpack_sequence          | 54.0 ns                                                | 92.1 ns: 1.71x slower                                                |
| Geometric mean           | (ref)                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (12): unpickle, sqlite_synth, async_generators, richards, scimark_sor, async_tree_cpu_io_mixed_tg, pprint_pformat, dulwich_log, asyncio_websockets, async_tree_memoization_tg, mdp, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-linux-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.64% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.17x