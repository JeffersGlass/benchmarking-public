# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_arena
- machine: darwin-arm64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 2.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 186 ms: 1.03x faster                                                 |
| chameleon      | 6.26 ms                                                | 4.82 ms: 1.30x faster                                                |
| docutils       | 1.73 sec                                               | 1.52 sec: 1.14x faster                                               |
| html5lib       | 42.4 ms                                                | 35.7 ms: 1.19x faster                                                |
| tornado_http   | 86.7 ms                                                | 69.4 ms: 1.25x faster                                                |
| Geometric mean | (ref)                                                  | 1.18x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 252 ms: 1.54x faster                                                 |
| async_tree_memoization  | 474 ms                                                 | 326 ms: 1.45x faster                                                 |
| async_tree_io           | 980 ms                                                 | 697 ms: 1.41x faster                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 520 ms: 1.25x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 70.7 ms: 1.32x faster                                                |
| float          | 69.0 ms                                                | 53.0 ms: 1.30x faster                                                |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.20x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                 |
| regex_compile  | 95.3 ms                                                | 87.8 ms: 1.08x faster                                                |
| regex_v8       | 17.1 ms                                                | 17.2 ms: 1.00x slower                                                |
| regex_effbot   | 2.46 ms                                                | 2.63 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 150 us: 1.29x faster                                                 |
| json_dumps           | 8.11 ms                                                | 6.53 ms: 1.24x faster                                                |
| tomli_loads          | 1.71 sec                                               | 1.38 sec: 1.24x faster                                               |
| xml_etree_process    | 46.5 ms                                                | 39.2 ms: 1.19x faster                                                |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| unpickle             | 8.80 us                                                | 9.10 us: 1.03x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 55.4 ms: 1.04x slower                                                |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 74.9 ms: 1.04x slower                                                |
| pickle               | 6.97 us                                                | 7.26 us: 1.04x slower                                                |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| pickle_list          | 2.74 us                                                | 2.96 us: 1.08x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.13 us: 1.16x slower                                                |
| Geometric mean       | (ref)                                                  | 1.06x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 18.0 ms: 1.66x slower                                                |
| python_startup_no_site | 7.91 ms                                                | 16.4 ms: 2.07x slower                                                |
| Geometric mean         | (ref)                                                  | 1.85x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 6.82 ms: 1.45x faster                                                |
| django_template | 26.4 ms                                                | 21.8 ms: 1.21x faster                                                |
| genshi_text     | 17.3 ms                                                | 15.9 ms: 1.09x faster                                                |
| genshi_xml      | 33.8 ms                                                | 37.8 ms: 1.12x slower                                                |
| Geometric mean  | (ref)                                                  | 1.14x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.5 us: 4.52x faster                                                |
| deltablue                | 4.91 ms                                                | 2.52 ms: 1.95x faster                                                |
| asyncio_tcp              | 659 ms                                                 | 396 ms: 1.66x faster                                                 |
| chaos                    | 65.8 ms                                                | 40.2 ms: 1.64x faster                                                |
| logging_silent           | 117 ns                                                 | 72.5 ns: 1.62x faster                                                |
| raytrace                 | 301 ms                                                 | 192 ms: 1.57x faster                                                 |
| pylint                   | 277 ms                                                 | 176 ms: 1.57x faster                                                 |
| async_tree_none          | 388 ms                                                 | 252 ms: 1.54x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 47.2 ms: 1.52x faster                                                |
| sqlglot_parse            | 1.24 ms                                                | 843 us: 1.47x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 326 ms: 1.45x faster                                                 |
| mako                     | 9.87 ms                                                | 6.82 ms: 1.45x faster                                                |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 46.1 ms: 1.42x faster                                                |
| richards_super           | 57.8 ms                                                | 40.8 ms: 1.42x faster                                                |
| async_tree_io            | 980 ms                                                 | 697 ms: 1.41x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.03 ms: 1.40x faster                                                |
| comprehensions           | 16.9 us                                                | 12.7 us: 1.34x faster                                                |
| deepcopy_memo            | 34.7 us                                                | 26.2 us: 1.32x faster                                                |
| go                       | 151 ms                                                 | 114 ms: 1.32x faster                                                 |
| richards                 | 48.7 ms                                                | 37.0 ms: 1.32x faster                                                |
| nbody                    | 93.0 ms                                                | 70.7 ms: 1.32x faster                                                |
| float                    | 69.0 ms                                                | 53.0 ms: 1.30x faster                                                |
| chameleon                | 6.26 ms                                                | 4.82 ms: 1.30x faster                                                |
| unpickle_pure_python     | 194 us                                                 | 150 us: 1.29x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.48 us: 1.28x faster                                                |
| logging_format           | 4.83 us                                                | 3.78 us: 1.28x faster                                                |
| pprint_safe_repr         | 641 ms                                                 | 507 ms: 1.26x faster                                                 |
| thrift                   | 572 us                                                 | 455 us: 1.26x faster                                                 |
| pprint_pformat           | 1.30 sec                                               | 1.04 sec: 1.25x faster                                               |
| tornado_http             | 86.7 ms                                                | 69.4 ms: 1.25x faster                                                |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 520 ms: 1.25x faster                                                 |
| pycparser                | 877 ms                                                 | 706 ms: 1.24x faster                                                 |
| json_dumps               | 8.11 ms                                                | 6.53 ms: 1.24x faster                                                |
| tomli_loads              | 1.71 sec                                               | 1.38 sec: 1.24x faster                                               |
| pyflate                  | 427 ms                                                 | 345 ms: 1.24x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                               |
| django_template          | 26.4 ms                                                | 21.8 ms: 1.21x faster                                                |
| spectral_norm            | 94.8 ms                                                | 78.4 ms: 1.21x faster                                                |
| create_gc_cycles         | 860 us                                                 | 711 us: 1.21x faster                                                 |
| scimark_lu               | 103 ms                                                 | 85.0 ms: 1.21x faster                                                |
| sympy_sum                | 92.2 ms                                                | 76.4 ms: 1.21x faster                                                |
| deepcopy                 | 272 us                                                 | 228 us: 1.19x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 39.2 ms: 1.19x faster                                                |
| html5lib                 | 42.4 ms                                                | 35.7 ms: 1.19x faster                                                |
| deepcopy_reduce          | 2.33 us                                                | 1.97 us: 1.18x faster                                                |
| hexiom                   | 6.19 ms                                                | 5.29 ms: 1.17x faster                                                |
| aiohttp                  | 1.22 ms                                                | 1.05 ms: 1.17x faster                                                |
| gunicorn                 | 1.30 ms                                                | 1.13 ms: 1.16x faster                                                |
| sympy_integrate          | 13.1 ms                                                | 11.4 ms: 1.15x faster                                                |
| sympy_str                | 165 ms                                                 | 144 ms: 1.15x faster                                                 |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                 |
| dulwich_log              | 35.3 ms                                                | 30.9 ms: 1.14x faster                                                |
| docutils                 | 1.73 sec                                               | 1.52 sec: 1.14x faster                                               |
| generators               | 32.3 ms                                                | 28.4 ms: 1.14x faster                                                |
| mypy2                    | 607 ms                                                 | 535 ms: 1.13x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.3 ms: 1.13x faster                                                |
| scimark_fft              | 224 ms                                                 | 200 ms: 1.12x faster                                                 |
| scimark_sor              | 128 ms                                                 | 114 ms: 1.12x faster                                                 |
| sympy_expand             | 269 ms                                                 | 245 ms: 1.10x faster                                                 |
| genshi_text              | 17.3 ms                                                | 15.9 ms: 1.09x faster                                                |
| regex_compile            | 95.3 ms                                                | 87.8 ms: 1.08x faster                                                |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.17 ms: 1.08x faster                                                |
| json                     | 3.08 ms                                                | 2.95 ms: 1.04x faster                                                |
| sqlglot_normalize        | 190 ms                                                 | 183 ms: 1.04x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 35.4 ms: 1.04x faster                                                |
| meteor_contest           | 77.7 ms                                                | 75.3 ms: 1.03x faster                                                |
| bench_thread_pool        | 527 us                                                 | 512 us: 1.03x faster                                                 |
| 2to3                     | 192 ms                                                 | 186 ms: 1.03x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| nqueens                  | 63.8 ms                                                | 63.4 ms: 1.01x faster                                                |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.00x faster                                               |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                 |
| pidigits                 | 282 ms                                                 | 281 ms: 1.00x faster                                                 |
| regex_v8                 | 17.1 ms                                                | 17.2 ms: 1.00x slower                                                |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                |
| fannkuch                 | 303 ms                                                 | 313 ms: 1.03x slower                                                 |
| unpickle                 | 8.80 us                                                | 9.10 us: 1.03x slower                                                |
| xml_etree_generate       | 53.5 ms                                                | 55.4 ms: 1.04x slower                                                |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                                |
| xml_etree_iterparse      | 72.1 ms                                                | 74.9 ms: 1.04x slower                                                |
| pickle                   | 6.97 us                                                | 7.26 us: 1.04x slower                                                |
| regex_effbot             | 2.46 ms                                                | 2.63 ms: 1.07x slower                                                |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                |
| pickle_list              | 2.74 us                                                | 2.96 us: 1.08x slower                                                |
| sqlite_synth             | 1.46 us                                                | 1.60 us: 1.10x slower                                                |
| genshi_xml               | 33.8 ms                                                | 37.8 ms: 1.12x slower                                                |
| coverage                 | 41.5 ms                                                | 47.5 ms: 1.15x slower                                                |
| unpickle_list            | 2.69 us                                                | 3.13 us: 1.16x slower                                                |
| telco                    | 3.49 ms                                                | 4.54 ms: 1.30x slower                                                |
| dask                     | 253 ms                                                 | 334 ms: 1.32x slower                                                 |
| async_generators         | 231 ms                                                 | 311 ms: 1.34x slower                                                 |
| bench_mp_pool            | 37.4 ms                                                | 53.0 ms: 1.42x slower                                                |
| python_startup           | 10.9 ms                                                | 18.0 ms: 1.66x slower                                                |
| python_startup_no_site   | 7.91 ms                                                | 16.4 ms: 2.07x slower                                                |
| unpack_sequence          | 39.0 ns                                                | 112 ns: 2.88x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.14x faster                                                         |

Benchmark hidden because not significant (1): pathlib
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 2.06x