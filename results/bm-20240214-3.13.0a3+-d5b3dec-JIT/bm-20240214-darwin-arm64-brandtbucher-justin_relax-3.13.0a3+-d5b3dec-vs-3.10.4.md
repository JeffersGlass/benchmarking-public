
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: d5b3dec
- commit date: 2024-02-14
- overall geometric mean: 1.18x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 174 ms: 1.10x faster                                                 |
| chameleon      | 6.26 ms                                                | 4.79 ms: 1.31x faster                                                |
| docutils       | 1.73 sec                                               | 1.47 sec: 1.18x faster                                               |
| tornado_http   | 86.7 ms                                                | 70.1 ms: 1.24x faster                                                |
| Geometric mean | (ref)                                                  | 1.20x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 251 ms: 1.55x faster                                                 |
| async_tree_memoization  | 474 ms                                                 | 326 ms: 1.45x faster                                                 |
| async_tree_io           | 980 ms                                                 | 694 ms: 1.41x faster                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 518 ms: 1.25x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 55.6 ms: 1.24x faster                                                |
| nbody          | 93.0 ms                                                | 76.5 ms: 1.22x faster                                                |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.15x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 75.6 ms: 1.26x faster                                                |
| regex_dna      | 174 ms                                                 | 151 ms: 1.15x faster                                                 |
| regex_v8       | 17.1 ms                                                | 17.1 ms: 1.01x faster                                                |
| regex_effbot   | 2.46 ms                                                | 2.55 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                  | 1.09x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 195 us: 1.44x faster                                                 |
| json_dumps           | 8.11 ms                                                | 6.46 ms: 1.25x faster                                                |
| unpickle_pure_python | 194 us                                                 | 158 us: 1.23x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.40 sec: 1.22x faster                                               |
| xml_etree_process    | 46.5 ms                                                | 38.8 ms: 1.20x faster                                                |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| json_loads           | 16.4 us                                                | 17.0 us: 1.04x slower                                                |
| pickle               | 6.97 us                                                | 7.24 us: 1.04x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 55.7 ms: 1.04x slower                                                |
| unpickle             | 8.80 us                                                | 9.15 us: 1.04x slower                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 75.6 ms: 1.05x slower                                                |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| pickle_list          | 2.74 us                                                | 2.93 us: 1.07x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.10 us: 1.15x slower                                                |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.6 ms: 1.25x slower                                                |
| python_startup_no_site | 7.91 ms                                                | 12.1 ms: 1.53x slower                                                |
| Geometric mean         | (ref)                                                  | 1.38x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.80 ms: 1.27x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 70.4 us: 4.59x faster                                                |
| deltablue                | 4.91 ms                                                | 2.46 ms: 2.00x faster                                                |
| raytrace                 | 301 ms                                                 | 177 ms: 1.70x faster                                                 |
| logging_silent           | 117 ns                                                 | 70.6 ns: 1.66x faster                                                |
| richards_super           | 57.8 ms                                                | 35.7 ms: 1.62x faster                                                |
| asyncio_tcp              | 659 ms                                                 | 411 ms: 1.60x faster                                                 |
| chaos                    | 65.8 ms                                                | 41.3 ms: 1.59x faster                                                |
| sqlglot_parse            | 1.24 ms                                                | 792 us: 1.57x faster                                                 |
| async_tree_none          | 388 ms                                                 | 251 ms: 1.55x faster                                                 |
| richards                 | 48.7 ms                                                | 31.9 ms: 1.53x faster                                                |
| sqlglot_transpile        | 1.44 ms                                                | 978 us: 1.48x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 48.9 ms: 1.47x faster                                                |
| async_tree_memoization   | 474 ms                                                 | 326 ms: 1.45x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 195 us: 1.44x faster                                                 |
| async_tree_io            | 980 ms                                                 | 694 ms: 1.41x faster                                                 |
| go                       | 151 ms                                                 | 110 ms: 1.37x faster                                                 |
| scimark_lu               | 103 ms                                                 | 75.0 ms: 1.37x faster                                                |
| unpack_sequence          | 39.0 ns                                                | 28.5 ns: 1.37x faster                                                |
| deepcopy_memo            | 34.7 us                                                | 25.8 us: 1.34x faster                                                |
| comprehensions           | 16.9 us                                                | 12.6 us: 1.34x faster                                                |
| scimark_monte_carlo      | 65.6 ms                                                | 48.9 ms: 1.34x faster                                                |
| pyflate                  | 427 ms                                                 | 327 ms: 1.31x faster                                                 |
| chameleon                | 6.26 ms                                                | 4.79 ms: 1.31x faster                                                |
| logging_simple           | 4.45 us                                                | 3.47 us: 1.28x faster                                                |
| logging_format           | 4.83 us                                                | 3.77 us: 1.28x faster                                                |
| mako                     | 9.87 ms                                                | 7.80 ms: 1.27x faster                                                |
| pycparser                | 877 ms                                                 | 693 ms: 1.26x faster                                                 |
| regex_compile            | 95.3 ms                                                | 75.6 ms: 1.26x faster                                                |
| json_dumps               | 8.11 ms                                                | 6.46 ms: 1.25x faster                                                |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 518 ms: 1.25x faster                                                 |
| float                    | 69.0 ms                                                | 55.6 ms: 1.24x faster                                                |
| tornado_http             | 86.7 ms                                                | 70.1 ms: 1.24x faster                                                |
| pprint_pformat           | 1.30 sec                                               | 1.05 sec: 1.24x faster                                               |
| pprint_safe_repr         | 641 ms                                                 | 519 ms: 1.24x faster                                                 |
| hexiom                   | 6.19 ms                                                | 5.04 ms: 1.23x faster                                                |
| unpickle_pure_python     | 194 us                                                 | 158 us: 1.23x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.23x faster                                               |
| sympy_sum                | 92.2 ms                                                | 75.6 ms: 1.22x faster                                                |
| create_gc_cycles         | 860 us                                                 | 706 us: 1.22x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.40 sec: 1.22x faster                                               |
| nbody                    | 93.0 ms                                                | 76.5 ms: 1.22x faster                                                |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.22x faster                                                 |
| deepcopy                 | 272 us                                                 | 225 us: 1.21x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 38.8 ms: 1.20x faster                                                |
| dulwich_log              | 35.3 ms                                                | 29.8 ms: 1.19x faster                                                |
| spectral_norm            | 94.8 ms                                                | 80.5 ms: 1.18x faster                                                |
| docutils                 | 1.73 sec                                               | 1.47 sec: 1.18x faster                                               |
| deepcopy_reduce          | 2.33 us                                                | 1.99 us: 1.17x faster                                                |
| sympy_str                | 165 ms                                                 | 142 ms: 1.17x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.3 ms: 1.17x faster                                                |
| mypy2                    | 607 ms                                                 | 524 ms: 1.16x faster                                                 |
| regex_dna                | 174 ms                                                 | 151 ms: 1.15x faster                                                 |
| generators               | 32.3 ms                                                | 28.3 ms: 1.14x faster                                                |
| dask                     | 253 ms                                                 | 225 ms: 1.12x faster                                                 |
| fannkuch                 | 303 ms                                                 | 270 ms: 1.12x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.5 ms: 1.12x faster                                                |
| sympy_expand             | 269 ms                                                 | 241 ms: 1.12x faster                                                 |
| 2to3                     | 192 ms                                                 | 174 ms: 1.10x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 34.5 ms: 1.07x faster                                                |
| bench_thread_pool        | 527 us                                                 | 505 us: 1.04x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 74.7 ms: 1.04x faster                                                |
| sqlglot_normalize        | 190 ms                                                 | 183 ms: 1.04x faster                                                 |
| json                     | 3.08 ms                                                | 2.98 ms: 1.04x faster                                                |
| scimark_fft              | 224 ms                                                 | 218 ms: 1.03x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.33 ms: 1.03x faster                                                |
| nqueens                  | 63.8 ms                                                | 62.2 ms: 1.03x faster                                                |
| pathlib                  | 24.5 ms                                                | 24.0 ms: 1.02x faster                                                |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.01x faster                                               |
| regex_v8                 | 17.1 ms                                                | 17.1 ms: 1.01x faster                                                |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                 |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x faster                                                 |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                                |
| json_loads               | 16.4 us                                                | 17.0 us: 1.04x slower                                                |
| regex_effbot             | 2.46 ms                                                | 2.55 ms: 1.04x slower                                                |
| pickle                   | 6.97 us                                                | 7.24 us: 1.04x slower                                                |
| xml_etree_generate       | 53.5 ms                                                | 55.7 ms: 1.04x slower                                                |
| unpickle                 | 8.80 us                                                | 9.15 us: 1.04x slower                                                |
| xml_etree_iterparse      | 72.1 ms                                                | 75.6 ms: 1.05x slower                                                |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| pickle_list              | 2.74 us                                                | 2.93 us: 1.07x slower                                                |
| sqlite_synth             | 1.46 us                                                | 1.60 us: 1.09x slower                                                |
| coverage                 | 41.5 ms                                                | 47.5 ms: 1.14x slower                                                |
| unpickle_list            | 2.69 us                                                | 3.10 us: 1.15x slower                                                |
| python_startup           | 10.9 ms                                                | 13.6 ms: 1.25x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 47.2 ms: 1.26x slower                                                |
| telco                    | 3.49 ms                                                | 4.49 ms: 1.29x slower                                                |
| async_generators         | 231 ms                                                 | 304 ms: 1.31x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 12.1 ms: 1.53x slower                                                |
| Geometric mean           | (ref)                                                  | 1.18x faster                                                         |
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-d5b3dec-JIT/bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.26x