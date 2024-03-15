# Results vs. base

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 212 ms                                                                                                                 | 225 ms: 1.07x slower                                                                                                               |
| chameleon      | 4.98 ms                                                                                                                | 5.07 ms: 1.02x slower                                                                                                              |
| docutils       | 1.57 sec                                                                                                               | 1.66 sec: 1.06x slower                                                                                                             |
| tornado_http   | 84.0 ms                                                                                                                | 86.2 ms: 1.03x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.04x slower                                                                                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| async_tree_io    | 738 ms                                                                                                                 | 729 ms: 1.01x faster                                                                                                               |
| async_tree_io_tg | 753 ms                                                                                                                 | 764 ms: 1.02x slower                                                                                                               |
| Geometric mean   | (ref)                                                                                                                  | 1.00x slower                                                                                                                       |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 148 ms                                                                                                                 | 147 ms: 1.00x faster                                                                                                               |
| float          | 54.3 ms                                                                                                                | 59.0 ms: 1.09x slower                                                                                                              |
| nbody          | 72.9 ms                                                                                                                | 81.4 ms: 1.12x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.06x slower                                                                                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| regex_dna      | 120 ms                                                                                                                 | 118 ms: 1.02x faster                                                                                                               |
| regex_effbot   | 1.58 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                              |
| regex_compile  | 79.8 ms                                                                                                                | 102 ms: 1.28x slower                                                                                                               |
| Geometric mean | (ref)                                                                                                                  | 1.07x slower                                                                                                                       |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| unpickle             | 8.58 us                                                                                                                | 8.32 us: 1.03x faster                                                                                                              |
| xml_etree_parse      | 94.1 ms                                                                                                                | 92.7 ms: 1.01x faster                                                                                                              |
| pickle               | 7.14 us                                                                                                                | 7.03 us: 1.01x faster                                                                                                              |
| json_loads           | 14.0 us                                                                                                                | 13.8 us: 1.01x faster                                                                                                              |
| json_dumps           | 5.65 ms                                                                                                                | 5.68 ms: 1.01x slower                                                                                                              |
| pickle_pure_python   | 185 us                                                                                                                 | 186 us: 1.01x slower                                                                                                               |
| pickle_dict          | 18.2 us                                                                                                                | 18.4 us: 1.01x slower                                                                                                              |
| unpickle_list        | 2.71 us                                                                                                                | 2.75 us: 1.01x slower                                                                                                              |
| xml_etree_generate   | 53.9 ms                                                                                                                | 56.8 ms: 1.05x slower                                                                                                              |
| xml_etree_process    | 36.7 ms                                                                                                                | 38.8 ms: 1.06x slower                                                                                                              |
| xml_etree_iterparse  | 64.1 ms                                                                                                                | 68.6 ms: 1.07x slower                                                                                                              |
| pickle_list          | 3.00 us                                                                                                                | 3.20 us: 1.07x slower                                                                                                              |
| tomli_loads          | 1.41 sec                                                                                                               | 1.58 sec: 1.12x slower                                                                                                             |
| unpickle_pure_python | 133 us                                                                                                                 | 168 us: 1.26x slower                                                                                                               |
| Geometric mean       | (ref)                                                                                                                  | 1.04x slower                                                                                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| python_startup_no_site | 17.6 ms                                                                                                                | 17.9 ms: 1.02x slower                                                                                                              |
| Geometric mean         | (ref)                                                                                                                  | 1.01x slower                                                                                                                       |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.49 ms                                                                                                                | 7.55 ms: 1.16x slower                                                                                                              |

All benchmarks:
===============

| Benchmark                | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|--------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| json                     | 3.28 ms                                                                                                                | 2.91 ms: 1.13x faster                                                                                                              |
| generators               | 21.5 ms                                                                                                                | 20.6 ms: 1.04x faster                                                                                                              |
| unpickle                 | 8.58 us                                                                                                                | 8.32 us: 1.03x faster                                                                                                              |
| coroutines               | 13.5 ms                                                                                                                | 13.2 ms: 1.03x faster                                                                                                              |
| regex_dna                | 120 ms                                                                                                                 | 118 ms: 1.02x faster                                                                                                               |
| xml_etree_parse          | 94.1 ms                                                                                                                | 92.7 ms: 1.01x faster                                                                                                              |
| pickle                   | 7.14 us                                                                                                                | 7.03 us: 1.01x faster                                                                                                              |
| async_tree_io            | 738 ms                                                                                                                 | 729 ms: 1.01x faster                                                                                                               |
| json_loads               | 14.0 us                                                                                                                | 13.8 us: 1.01x faster                                                                                                              |
| regex_effbot             | 1.58 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                              |
| pidigits                 | 148 ms                                                                                                                 | 147 ms: 1.00x faster                                                                                                               |
| sqlite_synth             | 1.59 us                                                                                                                | 1.60 us: 1.00x slower                                                                                                              |
| json_dumps               | 5.65 ms                                                                                                                | 5.68 ms: 1.01x slower                                                                                                              |
| coverage                 | 47.2 ms                                                                                                                | 47.5 ms: 1.01x slower                                                                                                              |
| pickle_pure_python       | 185 us                                                                                                                 | 186 us: 1.01x slower                                                                                                               |
| pathlib                  | 76.1 ms                                                                                                                | 76.8 ms: 1.01x slower                                                                                                              |
| pickle_dict              | 18.2 us                                                                                                                | 18.4 us: 1.01x slower                                                                                                              |
| deepcopy_reduce          | 1.99 us                                                                                                                | 2.01 us: 1.01x slower                                                                                                              |
| unpickle_list            | 2.71 us                                                                                                                | 2.75 us: 1.01x slower                                                                                                              |
| async_tree_io_tg         | 753 ms                                                                                                                 | 764 ms: 1.02x slower                                                                                                               |
| bench_mp_pool            | 64.0 ms                                                                                                                | 65.0 ms: 1.02x slower                                                                                                              |
| chameleon                | 4.98 ms                                                                                                                | 5.07 ms: 1.02x slower                                                                                                              |
| python_startup_no_site   | 17.6 ms                                                                                                                | 17.9 ms: 1.02x slower                                                                                                              |
| logging_silent           | 55.5 ns                                                                                                                | 56.9 ns: 1.02x slower                                                                                                              |
| tornado_http             | 84.0 ms                                                                                                                | 86.2 ms: 1.03x slower                                                                                                              |
| deepcopy                 | 227 us                                                                                                                 | 234 us: 1.03x slower                                                                                                               |
| create_gc_cycles         | 714 us                                                                                                                 | 738 us: 1.03x slower                                                                                                               |
| typing_runtime_protocols | 72.8 us                                                                                                                | 75.3 us: 1.03x slower                                                                                                              |
| bench_thread_pool        | 828 us                                                                                                                 | 863 us: 1.04x slower                                                                                                               |
| async_generators         | 226 ms                                                                                                                 | 237 ms: 1.05x slower                                                                                                               |
| xml_etree_generate       | 53.9 ms                                                                                                                | 56.8 ms: 1.05x slower                                                                                                              |
| logging_format           | 6.51 us                                                                                                                | 6.86 us: 1.05x slower                                                                                                              |
| logging_simple           | 6.06 us                                                                                                                | 6.42 us: 1.06x slower                                                                                                              |
| xml_etree_process        | 36.7 ms                                                                                                                | 38.8 ms: 1.06x slower                                                                                                              |
| sqlglot_transpile        | 1.00 ms                                                                                                                | 1.06 ms: 1.06x slower                                                                                                              |
| docutils                 | 1.57 sec                                                                                                               | 1.66 sec: 1.06x slower                                                                                                             |
| 2to3                     | 212 ms                                                                                                                 | 225 ms: 1.07x slower                                                                                                               |
| mdp                      | 1.37 sec                                                                                                               | 1.46 sec: 1.07x slower                                                                                                             |
| xml_etree_iterparse      | 64.1 ms                                                                                                                | 68.6 ms: 1.07x slower                                                                                                              |
| meteor_contest           | 71.9 ms                                                                                                                | 76.9 ms: 1.07x slower                                                                                                              |
| sqlglot_parse            | 781 us                                                                                                                 | 835 us: 1.07x slower                                                                                                               |
| pickle_list              | 3.00 us                                                                                                                | 3.20 us: 1.07x slower                                                                                                              |
| sqlglot_normalize        | 177 ms                                                                                                                 | 189 ms: 1.07x slower                                                                                                               |
| mypy2                    | 415 ms                                                                                                                 | 445 ms: 1.07x slower                                                                                                               |
| dulwich_log              | 40.4 ms                                                                                                                | 43.6 ms: 1.08x slower                                                                                                              |
| crypto_pyaes             | 44.3 ms                                                                                                                | 47.9 ms: 1.08x slower                                                                                                              |
| float                    | 54.3 ms                                                                                                                | 59.0 ms: 1.09x slower                                                                                                              |
| sympy_expand             | 275 ms                                                                                                                 | 300 ms: 1.09x slower                                                                                                               |
| sqlglot_optimize         | 33.4 ms                                                                                                                | 36.6 ms: 1.09x slower                                                                                                              |
| fannkuch                 | 249 ms                                                                                                                 | 273 ms: 1.10x slower                                                                                                               |
| deepcopy_memo            | 22.3 us                                                                                                                | 24.8 us: 1.11x slower                                                                                                              |
| tomli_loads              | 1.41 sec                                                                                                               | 1.58 sec: 1.12x slower                                                                                                             |
| nbody                    | 72.9 ms                                                                                                                | 81.4 ms: 1.12x slower                                                                                                              |
| sympy_str                | 160 ms                                                                                                                 | 179 ms: 1.12x slower                                                                                                               |
| sympy_sum                | 83.7 ms                                                                                                                | 94.0 ms: 1.12x slower                                                                                                              |
| sympy_integrate          | 12.5 ms                                                                                                                | 14.1 ms: 1.12x slower                                                                                                              |
| chaos                    | 40.4 ms                                                                                                                | 45.7 ms: 1.13x slower                                                                                                              |
| pprint_safe_repr         | 501 ms                                                                                                                 | 569 ms: 1.13x slower                                                                                                               |
| richards_super           | 31.3 ms                                                                                                                | 35.7 ms: 1.14x slower                                                                                                              |
| pprint_pformat           | 1.03 sec                                                                                                               | 1.17 sec: 1.14x slower                                                                                                             |
| richards                 | 27.7 ms                                                                                                                | 31.9 ms: 1.15x slower                                                                                                              |
| unpack_sequence          | 36.7 ns                                                                                                                | 42.4 ns: 1.16x slower                                                                                                              |
| deltablue                | 2.03 ms                                                                                                                | 2.35 ms: 1.16x slower                                                                                                              |
| mako                     | 6.49 ms                                                                                                                | 7.55 ms: 1.16x slower                                                                                                              |
| nqueens                  | 59.8 ms                                                                                                                | 71.4 ms: 1.19x slower                                                                                                              |
| pyflate                  | 291 ms                                                                                                                 | 352 ms: 1.21x slower                                                                                                               |
| raytrace                 | 166 ms                                                                                                                 | 202 ms: 1.21x slower                                                                                                               |
| scimark_sor              | 77.2 ms                                                                                                                | 94.1 ms: 1.22x slower                                                                                                              |
| go                       | 85.7 ms                                                                                                                | 104 ms: 1.22x slower                                                                                                               |
| scimark_fft              | 179 ms                                                                                                                 | 219 ms: 1.22x slower                                                                                                               |
| unpickle_pure_python     | 133 us                                                                                                                 | 168 us: 1.26x slower                                                                                                               |
| regex_compile            | 79.8 ms                                                                                                                | 102 ms: 1.28x slower                                                                                                               |
| spectral_norm            | 64.4 ms                                                                                                                | 83.5 ms: 1.30x slower                                                                                                              |
| scimark_sparse_mat_mult  | 2.45 ms                                                                                                                | 3.22 ms: 1.31x slower                                                                                                              |
| scimark_monte_carlo      | 41.0 ms                                                                                                                | 54.7 ms: 1.34x slower                                                                                                              |
| comprehensions           | 10.6 us                                                                                                                | 14.5 us: 1.37x slower                                                                                                              |
| hexiom                   | 3.89 ms                                                                                                                | 5.61 ms: 1.44x slower                                                                                                              |
| scimark_lu               | 52.9 ms                                                                                                                | 81.1 ms: 1.53x slower                                                                                                              |
| Geometric mean           | (ref)                                                                                                                  | 1.08x slower                                                                                                                       |

Benchmark hidden because not significant (13): pycparser, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, telco, python_startup, async_tree_none_tg, gc_traversal, asyncio_tcp_ssl, asyncio_tcp, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization, regex_v8


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: unknown