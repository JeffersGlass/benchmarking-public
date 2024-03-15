
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: a379acd
- commit date: 2024-02-15
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| chameleon      | 6.26 ms                                                | 4.79 ms: 1.31x faster                                                |
| docutils       | 1.73 sec                                               | 1.46 sec: 1.18x faster                                               |
| tornado_http   | 86.7 ms                                                | 69.9 ms: 1.24x faster                                                |
| Geometric mean | (ref)                                                  | 1.18x faster                                                         |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 249 ms: 1.56x faster                                                 |
| async_tree_memoization  | 474 ms                                                 | 325 ms: 1.46x faster                                                 |
| async_tree_io           | 980 ms                                                 | 692 ms: 1.42x faster                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 516 ms: 1.26x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.42x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 71.3 ms: 1.30x faster                                                |
| float          | 69.0 ms                                                | 53.1 ms: 1.30x faster                                                |
| Geometric mean | (ref)                                                  | 1.19x faster                                                         |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.7 ms: 1.29x faster                                                |
| regex_dna      | 174 ms                                                 | 151 ms: 1.15x faster                                                 |
| regex_v8       | 17.1 ms                                                | 17.0 ms: 1.01x faster                                                |
| regex_effbot   | 2.46 ms                                                | 2.55 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                  | 1.10x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 195 us: 1.44x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.34 sec: 1.27x faster                                               |
| json_dumps           | 8.11 ms                                                | 6.44 ms: 1.26x faster                                                |
| unpickle_pure_python | 194 us                                                 | 157 us: 1.24x faster                                                 |
| xml_etree_process    | 46.5 ms                                                | 38.3 ms: 1.21x faster                                                |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 73.6 ms: 1.02x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 54.9 ms: 1.03x slower                                                |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                                |
| pickle               | 6.97 us                                                | 7.25 us: 1.04x slower                                                |
| unpickle             | 8.80 us                                                | 9.15 us: 1.04x slower                                                |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| pickle_list          | 2.74 us                                                | 2.95 us: 1.08x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| Geometric mean       | (ref)                                                  | 1.06x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.5 ms: 1.24x slower                                                |
| python_startup_no_site | 7.91 ms                                                | 12.2 ms: 1.54x slower                                                |
| Geometric mean         | (ref)                                                  | 1.38x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 6.98 ms: 1.41x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 70.0 us: 4.61x faster                                                |
| deltablue                | 4.91 ms                                                | 2.43 ms: 2.02x faster                                                |
| raytrace                 | 301 ms                                                 | 174 ms: 1.73x faster                                                 |
| asyncio_tcp              | 659 ms                                                 | 394 ms: 1.67x faster                                                 |
| logging_silent           | 117 ns                                                 | 70.3 ns: 1.67x faster                                                |
| chaos                    | 65.8 ms                                                | 40.0 ms: 1.64x faster                                                |
| richards_super           | 57.8 ms                                                | 35.4 ms: 1.63x faster                                                |
| sqlglot_parse            | 1.24 ms                                                | 785 us: 1.58x faster                                                 |
| async_tree_none          | 388 ms                                                 | 249 ms: 1.56x faster                                                 |
| richards                 | 48.7 ms                                                | 31.7 ms: 1.54x faster                                                |
| crypto_pyaes             | 71.8 ms                                                | 47.5 ms: 1.51x faster                                                |
| sqlglot_transpile        | 1.44 ms                                                | 970 us: 1.49x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 325 ms: 1.46x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 195 us: 1.44x faster                                                 |
| async_tree_io            | 980 ms                                                 | 692 ms: 1.42x faster                                                 |
| mako                     | 9.87 ms                                                | 6.98 ms: 1.41x faster                                                |
| comprehensions           | 16.9 us                                                | 12.0 us: 1.41x faster                                                |
| go                       | 151 ms                                                 | 108 ms: 1.40x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 47.3 ms: 1.39x faster                                                |
| scimark_lu               | 103 ms                                                 | 74.5 ms: 1.38x faster                                                |
| unpack_sequence          | 39.0 ns                                                | 28.4 ns: 1.37x faster                                                |
| pyflate                  | 427 ms                                                 | 316 ms: 1.35x faster                                                 |
| deepcopy_memo            | 34.7 us                                                | 25.7 us: 1.35x faster                                                |
| chameleon                | 6.26 ms                                                | 4.79 ms: 1.31x faster                                                |
| nbody                    | 93.0 ms                                                | 71.3 ms: 1.30x faster                                                |
| float                    | 69.0 ms                                                | 53.1 ms: 1.30x faster                                                |
| logging_simple           | 4.45 us                                                | 3.43 us: 1.30x faster                                                |
| hexiom                   | 6.19 ms                                                | 4.79 ms: 1.29x faster                                                |
| regex_compile            | 95.3 ms                                                | 73.7 ms: 1.29x faster                                                |
| logging_format           | 4.83 us                                                | 3.75 us: 1.29x faster                                                |
| pycparser                | 877 ms                                                 | 688 ms: 1.27x faster                                                 |
| pprint_pformat           | 1.30 sec                                               | 1.02 sec: 1.27x faster                                               |
| tomli_loads              | 1.71 sec                                               | 1.34 sec: 1.27x faster                                               |
| pprint_safe_repr         | 641 ms                                                 | 507 ms: 1.26x faster                                                 |
| json_dumps               | 8.11 ms                                                | 6.44 ms: 1.26x faster                                                |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 516 ms: 1.26x faster                                                 |
| tornado_http             | 86.7 ms                                                | 69.9 ms: 1.24x faster                                                |
| unpickle_pure_python     | 194 us                                                 | 157 us: 1.24x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 77.1 ms: 1.23x faster                                                |
| sympy_sum                | 92.2 ms                                                | 75.0 ms: 1.23x faster                                                |
| create_gc_cycles         | 860 us                                                 | 703 us: 1.22x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.22x faster                                               |
| scimark_sor              | 128 ms                                                 | 105 ms: 1.22x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 38.3 ms: 1.21x faster                                                |
| deepcopy                 | 272 us                                                 | 225 us: 1.21x faster                                                 |
| dulwich_log              | 35.3 ms                                                | 29.6 ms: 1.19x faster                                                |
| docutils                 | 1.73 sec                                               | 1.46 sec: 1.18x faster                                               |
| sympy_integrate          | 13.1 ms                                                | 11.2 ms: 1.18x faster                                                |
| sympy_str                | 165 ms                                                 | 141 ms: 1.17x faster                                                 |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                                |
| regex_dna                | 174 ms                                                 | 151 ms: 1.15x faster                                                 |
| fannkuch                 | 303 ms                                                 | 263 ms: 1.15x faster                                                 |
| generators               | 32.3 ms                                                | 28.2 ms: 1.15x faster                                                |
| dask                     | 253 ms                                                 | 226 ms: 1.12x faster                                                 |
| sympy_expand             | 269 ms                                                 | 240 ms: 1.12x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.9 ms: 1.10x faster                                                |
| scimark_fft              | 224 ms                                                 | 205 ms: 1.10x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.17 ms: 1.08x faster                                                |
| sqlglot_optimize         | 36.8 ms                                                | 34.2 ms: 1.08x faster                                                |
| meteor_contest           | 77.7 ms                                                | 73.6 ms: 1.06x faster                                                |
| json                     | 3.08 ms                                                | 2.94 ms: 1.05x faster                                                |
| sqlglot_normalize        | 190 ms                                                 | 181 ms: 1.05x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 504 us: 1.05x faster                                                 |
| nqueens                  | 63.8 ms                                                | 61.1 ms: 1.04x faster                                                |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| mdp                      | 1.63 sec                                               | 1.61 sec: 1.01x faster                                               |
| regex_v8                 | 17.1 ms                                                | 17.0 ms: 1.01x faster                                                |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                                |
| xml_etree_iterparse      | 72.1 ms                                                | 73.6 ms: 1.02x slower                                                |
| xml_etree_generate       | 53.5 ms                                                | 54.9 ms: 1.03x slower                                                |
| regex_effbot             | 2.46 ms                                                | 2.55 ms: 1.04x slower                                                |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                                |
| pickle                   | 6.97 us                                                | 7.25 us: 1.04x slower                                                |
| unpickle                 | 8.80 us                                                | 9.15 us: 1.04x slower                                                |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| pickle_list              | 2.74 us                                                | 2.95 us: 1.08x slower                                                |
| sqlite_synth             | 1.46 us                                                | 1.59 us: 1.09x slower                                                |
| unpickle_list            | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| coverage                 | 41.5 ms                                                | 47.9 ms: 1.15x slower                                                |
| python_startup           | 10.9 ms                                                | 13.5 ms: 1.24x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 47.0 ms: 1.26x slower                                                |
| telco                    | 3.49 ms                                                | 4.43 ms: 1.27x slower                                                |
| async_generators         | 231 ms                                                 | 304 ms: 1.31x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 12.2 ms: 1.54x slower                                                |
| Geometric mean           | (ref)                                                  | 1.19x faster                                                         |

Benchmark hidden because not significant (5): mypy2, pathlib, asyncio_websockets, pidigits, 2to3
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-a379acd-JIT/bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.26x