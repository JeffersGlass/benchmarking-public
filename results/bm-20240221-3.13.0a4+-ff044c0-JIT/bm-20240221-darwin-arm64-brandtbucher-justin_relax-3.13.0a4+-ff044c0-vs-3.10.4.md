
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: 2.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 185 ms: 1.04x faster                                                 |
| chameleon      | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.15x faster                                               |
| tornado_http   | 86.7 ms                                                | 69.7 ms: 1.24x faster                                                |
| Geometric mean | (ref)                                                  | 1.17x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 252 ms: 1.54x faster                                                 |
| async_tree_memoization  | 474 ms                                                 | 328 ms: 1.44x faster                                                 |
| async_tree_io           | 980 ms                                                 | 701 ms: 1.40x faster                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 521 ms: 1.25x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.40x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 69.9 ms: 1.33x faster                                                |
| float          | 69.0 ms                                                | 53.2 ms: 1.30x faster                                                |
| Geometric mean | (ref)                                                  | 1.20x faster                                                         |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                 |
| regex_compile  | 95.3 ms                                                | 84.7 ms: 1.12x faster                                                |
| regex_v8       | 17.1 ms                                                | 17.1 ms: 1.00x faster                                                |
| regex_effbot   | 2.46 ms                                                | 2.56 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                  | 1.06x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.43x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 149 us: 1.30x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.37 sec: 1.25x faster                                               |
| json_dumps           | 8.11 ms                                                | 6.50 ms: 1.25x faster                                                |
| xml_etree_process    | 46.5 ms                                                | 38.9 ms: 1.19x faster                                                |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| unpickle             | 8.80 us                                                | 9.09 us: 1.03x slower                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 74.7 ms: 1.04x slower                                                |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                                |
| pickle               | 6.97 us                                                | 7.24 us: 1.04x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 55.6 ms: 1.04x slower                                                |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| pickle_list          | 2.74 us                                                | 2.98 us: 1.09x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.04 us: 1.13x slower                                                |
| Geometric mean       | (ref)                                                  | 1.06x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 18.0 ms: 1.65x slower                                                |
| python_startup_no_site | 7.91 ms                                                | 16.5 ms: 2.08x slower                                                |
| Geometric mean         | (ref)                                                  | 1.85x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 6.85 ms: 1.44x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.7 us: 4.51x faster                                                |
| deltablue                | 4.91 ms                                                | 2.55 ms: 1.93x faster                                                |
| logging_silent           | 117 ns                                                 | 70.7 ns: 1.66x faster                                                |
| chaos                    | 65.8 ms                                                | 40.2 ms: 1.64x faster                                                |
| asyncio_tcp              | 659 ms                                                 | 413 ms: 1.60x faster                                                 |
| raytrace                 | 301 ms                                                 | 191 ms: 1.58x faster                                                 |
| async_tree_none          | 388 ms                                                 | 252 ms: 1.54x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 827 us: 1.50x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 47.8 ms: 1.50x faster                                                |
| async_tree_memoization   | 474 ms                                                 | 328 ms: 1.44x faster                                                 |
| mako                     | 9.87 ms                                                | 6.85 ms: 1.44x faster                                                |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.43x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.01 ms: 1.42x faster                                                |
| scimark_monte_carlo      | 65.6 ms                                                | 46.1 ms: 1.42x faster                                                |
| async_tree_io            | 980 ms                                                 | 701 ms: 1.40x faster                                                 |
| comprehensions           | 16.9 us                                                | 12.6 us: 1.34x faster                                                |
| richards_super           | 57.8 ms                                                | 43.3 ms: 1.34x faster                                                |
| nbody                    | 93.0 ms                                                | 69.9 ms: 1.33x faster                                                |
| deepcopy_memo            | 34.7 us                                                | 26.3 us: 1.32x faster                                                |
| go                       | 151 ms                                                 | 115 ms: 1.31x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 149 us: 1.30x faster                                                 |
| float                    | 69.0 ms                                                | 53.2 ms: 1.30x faster                                                |
| spectral_norm            | 94.8 ms                                                | 74.0 ms: 1.28x faster                                                |
| chameleon                | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                |
| logging_format           | 4.83 us                                                | 3.78 us: 1.28x faster                                                |
| logging_simple           | 4.45 us                                                | 3.49 us: 1.28x faster                                                |
| pyflate                  | 427 ms                                                 | 339 ms: 1.26x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 512 ms: 1.25x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.37 sec: 1.25x faster                                               |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 521 ms: 1.25x faster                                                 |
| json_dumps               | 8.11 ms                                                | 6.50 ms: 1.25x faster                                                |
| tornado_http             | 86.7 ms                                                | 69.7 ms: 1.24x faster                                                |
| pprint_pformat           | 1.30 sec                                               | 1.05 sec: 1.24x faster                                               |
| richards                 | 48.7 ms                                                | 39.4 ms: 1.24x faster                                                |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                               |
| sympy_sum                | 92.2 ms                                                | 76.6 ms: 1.20x faster                                                |
| deepcopy                 | 272 us                                                 | 226 us: 1.20x faster                                                 |
| pycparser                | 877 ms                                                 | 732 ms: 1.20x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 38.9 ms: 1.19x faster                                                |
| create_gc_cycles         | 860 us                                                 | 723 us: 1.19x faster                                                 |
| scimark_lu               | 103 ms                                                 | 86.7 ms: 1.19x faster                                                |
| hexiom                   | 6.19 ms                                                | 5.27 ms: 1.18x faster                                                |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                                |
| dulwich_log              | 35.3 ms                                                | 30.6 ms: 1.15x faster                                                |
| sympy_str                | 165 ms                                                 | 144 ms: 1.15x faster                                                 |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.15x faster                                                |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.15x faster                                               |
| generators               | 32.3 ms                                                | 28.6 ms: 1.13x faster                                                |
| regex_compile            | 95.3 ms                                                | 84.7 ms: 1.12x faster                                                |
| scimark_fft              | 224 ms                                                 | 200 ms: 1.12x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.5 ms: 1.12x faster                                                |
| scimark_sor              | 128 ms                                                 | 116 ms: 1.10x faster                                                 |
| sympy_expand             | 269 ms                                                 | 246 ms: 1.09x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.13 ms: 1.09x faster                                                |
| meteor_contest           | 77.7 ms                                                | 74.0 ms: 1.05x faster                                                |
| json                     | 3.08 ms                                                | 2.95 ms: 1.05x faster                                                |
| 2to3                     | 192 ms                                                 | 185 ms: 1.04x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 35.5 ms: 1.04x faster                                                |
| sqlglot_normalize        | 190 ms                                                 | 184 ms: 1.03x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 517 us: 1.02x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| regex_v8                 | 17.1 ms                                                | 17.1 ms: 1.00x faster                                                |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                 |
| mdp                      | 1.63 sec                                               | 1.63 sec: 1.00x slower                                               |
| nqueens                  | 63.8 ms                                                | 64.5 ms: 1.01x slower                                                |
| gc_traversal             | 2.36 ms                                                | 2.43 ms: 1.03x slower                                                |
| fannkuch                 | 303 ms                                                 | 311 ms: 1.03x slower                                                 |
| unpickle                 | 8.80 us                                                | 9.09 us: 1.03x slower                                                |
| xml_etree_iterparse      | 72.1 ms                                                | 74.7 ms: 1.04x slower                                                |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                                |
| pickle                   | 6.97 us                                                | 7.24 us: 1.04x slower                                                |
| xml_etree_generate       | 53.5 ms                                                | 55.6 ms: 1.04x slower                                                |
| regex_effbot             | 2.46 ms                                                | 2.56 ms: 1.04x slower                                                |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| sqlite_synth             | 1.46 us                                                | 1.59 us: 1.09x slower                                                |
| pickle_list              | 2.74 us                                                | 2.98 us: 1.09x slower                                                |
| unpickle_list            | 2.69 us                                                | 3.04 us: 1.13x slower                                                |
| coverage                 | 41.5 ms                                                | 47.9 ms: 1.16x slower                                                |
| telco                    | 3.49 ms                                                | 4.55 ms: 1.31x slower                                                |
| async_generators         | 231 ms                                                 | 310 ms: 1.34x slower                                                 |
| bench_mp_pool            | 37.4 ms                                                | 53.3 ms: 1.42x slower                                                |
| python_startup           | 10.9 ms                                                | 18.0 ms: 1.65x slower                                                |
| python_startup_no_site   | 7.91 ms                                                | 16.5 ms: 2.08x slower                                                |
| unpack_sequence          | 39.0 ns                                                | 115 ns: 2.94x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.14x faster                                                         |

Benchmark hidden because not significant (3): mypy2, pathlib, pidigits
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240221-3.13.0a4+-ff044c0-JIT/bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: 2.08x