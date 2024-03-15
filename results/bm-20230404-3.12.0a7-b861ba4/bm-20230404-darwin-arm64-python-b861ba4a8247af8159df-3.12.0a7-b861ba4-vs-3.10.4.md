
# Results vs. 3.10.4

- fork: python
- ref: b861ba4a8247af8159df
- machine: darwin-arm64
- commit hash: b861ba4
- commit date: 2023-04-04
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 170 ms: 1.13x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.73 ms: 1.32x faster                                                 |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                |
| html5lib       | 42.4 ms                                                | 35.6 ms: 1.19x faster                                                 |
| tornado_http   | 86.7 ms                                                | 70.9 ms: 1.22x faster                                                 |
| Geometric mean | (ref)                                                  | 1.20x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 325 ms: 1.46x faster                                                  |
| async_tree_none         | 388 ms                                                 | 288 ms: 1.35x faster                                                  |
| async_tree_io           | 980 ms                                                 | 740 ms: 1.32x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 537 ms: 1.21x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.33x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 64.0 ms: 1.45x faster                                                 |
| float          | 69.0 ms                                                | 54.3 ms: 1.27x faster                                                 |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.23x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 78.7 ms: 1.21x faster                                                 |
| regex_dna      | 174 ms                                                 | 148 ms: 1.18x faster                                                  |
| regex_v8       | 17.1 ms                                                | 15.2 ms: 1.13x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.46 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 206 us: 1.36x faster                                                  |
| json_dumps           | 8.11 ms                                                | 6.01 ms: 1.35x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 158 us: 1.23x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 39.0 ms: 1.19x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.43 sec: 1.19x faster                                                |
| xml_etree_parse      | 108 ms                                                 | 98.6 ms: 1.09x faster                                                 |
| xml_etree_generate   | 53.5 ms                                                | 49.6 ms: 1.08x faster                                                 |
| unpickle             | 8.80 us                                                | 8.39 us: 1.05x faster                                                 |
| json_loads           | 16.4 us                                                | 15.8 us: 1.04x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.70 us: 1.00x slower                                                 |
| pickle_list          | 2.74 us                                                | 2.76 us: 1.01x slower                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 73.5 ms: 1.02x slower                                                 |
| pickle_dict          | 17.0 us                                                | 17.3 us: 1.02x slower                                                 |
| pickle               | 6.97 us                                                | 7.16 us: 1.03x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.10x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.8 ms: 1.09x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.57 ms: 1.21x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.17 ms: 1.38x faster                                                 |
| django_template | 26.4 ms                                                | 22.2 ms: 1.19x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 31.5 ms: 1.07x faster                                                 |
| genshi_text     | 17.3 ms                                                | 16.2 ms: 1.07x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.17x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.77 ms: 1.77x faster                                                 |
| asyncio_tcp              | 659 ms                                                 | 434 ms: 1.52x faster                                                  |
| logging_silent           | 117 ns                                                 | 77.7 ns: 1.51x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 325 ms: 1.46x faster                                                  |
| nbody                    | 93.0 ms                                                | 64.0 ms: 1.45x faster                                                 |
| scimark_sor              | 128 ms                                                 | 90.7 ms: 1.41x faster                                                 |
| richards                 | 48.7 ms                                                | 35.3 ms: 1.38x faster                                                 |
| mako                     | 9.87 ms                                                | 7.17 ms: 1.38x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 52.4 ms: 1.37x faster                                                 |
| chaos                    | 65.8 ms                                                | 48.1 ms: 1.37x faster                                                 |
| richards_super           | 57.8 ms                                                | 42.3 ms: 1.37x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 206 us: 1.36x faster                                                  |
| raytrace                 | 301 ms                                                 | 223 ms: 1.35x faster                                                  |
| json_dumps               | 8.11 ms                                                | 6.01 ms: 1.35x faster                                                 |
| async_tree_none          | 388 ms                                                 | 288 ms: 1.35x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.60 ms: 1.35x faster                                                 |
| async_tree_io            | 980 ms                                                 | 740 ms: 1.32x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.73 ms: 1.32x faster                                                 |
| pycparser                | 877 ms                                                 | 676 ms: 1.30x faster                                                  |
| go                       | 151 ms                                                 | 117 ms: 1.29x faster                                                  |
| pyflate                  | 427 ms                                                 | 332 ms: 1.29x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 51.1 ms: 1.28x faster                                                 |
| float                    | 69.0 ms                                                | 54.3 ms: 1.27x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 505 ms: 1.27x faster                                                  |
| scimark_fft              | 224 ms                                                 | 177 ms: 1.27x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.03 sec: 1.26x faster                                                |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.72 ms: 1.26x faster                                                 |
| thrift                   | 572 us                                                 | 459 us: 1.25x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 27.9 us: 1.24x faster                                                 |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.13 ms: 1.24x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 158 us: 1.23x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 698 us: 1.23x faster                                                  |
| tornado_http             | 86.7 ms                                                | 70.9 ms: 1.22x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.22x faster                                                |
| scimark_lu               | 103 ms                                                 | 84.7 ms: 1.21x faster                                                 |
| regex_compile            | 95.3 ms                                                | 78.7 ms: 1.21x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 537 ms: 1.21x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 29.3 ms: 1.20x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 39.0 ms: 1.19x faster                                                 |
| django_template          | 26.4 ms                                                | 22.2 ms: 1.19x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.43 sec: 1.19x faster                                                |
| html5lib                 | 42.4 ms                                                | 35.6 ms: 1.19x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 80.5 ms: 1.18x faster                                                 |
| regex_dna                | 174 ms                                                 | 148 ms: 1.18x faster                                                  |
| sqlalchemy_declarative   | 73.3 ms                                                | 62.6 ms: 1.17x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.24 ms: 1.17x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 1.07 ms: 1.17x faster                                                 |
| fannkuch                 | 303 ms                                                 | 260 ms: 1.17x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 33.6 ns: 1.16x faster                                                 |
| deepcopy                 | 272 us                                                 | 236 us: 1.15x faster                                                  |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                |
| logging_format           | 4.83 us                                                | 4.21 us: 1.15x faster                                                 |
| deepcopy_reduce          | 2.33 us                                                | 2.04 us: 1.14x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.93 us: 1.13x faster                                                 |
| dask                     | 253 ms                                                 | 224 ms: 1.13x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 15.2 ms: 1.13x faster                                                 |
| 2to3                     | 192 ms                                                 | 170 ms: 1.13x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.8 ms: 1.12x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 33.0 ms: 1.11x faster                                                 |
| json                     | 3.08 ms                                                | 2.80 ms: 1.10x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 98.6 ms: 1.09x faster                                                 |
| sympy_expand             | 269 ms                                                 | 246 ms: 1.09x faster                                                  |
| sqlite_synth             | 1.46 us                                                | 1.34 us: 1.09x faster                                                 |
| sympy_str                | 165 ms                                                 | 152 ms: 1.09x faster                                                  |
| xml_etree_generate       | 53.5 ms                                                | 49.6 ms: 1.08x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 72.3 ms: 1.08x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 31.5 ms: 1.07x faster                                                 |
| genshi_text              | 17.3 ms                                                | 16.2 ms: 1.07x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 85.9 ms: 1.07x faster                                                 |
| telco                    | 3.49 ms                                                | 3.27 ms: 1.07x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 498 us: 1.06x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 181 ms: 1.05x faster                                                  |
| unpickle                 | 8.80 us                                                | 8.39 us: 1.05x faster                                                 |
| json_loads               | 16.4 us                                                | 15.8 us: 1.04x faster                                                 |
| nqueens                  | 63.8 ms                                                | 61.1 ms: 1.04x faster                                                 |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.01x faster                                                |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x faster                                                  |
| regex_effbot             | 2.46 ms                                                | 2.46 ms: 1.00x faster                                                 |
| comprehensions           | 16.9 us                                                | 17.0 us: 1.00x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.70 us: 1.00x slower                                                 |
| pickle_list              | 2.74 us                                                | 2.76 us: 1.01x slower                                                 |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 73.5 ms: 1.02x slower                                                 |
| pickle_dict              | 17.0 us                                                | 17.3 us: 1.02x slower                                                 |
| pickle                   | 6.97 us                                                | 7.16 us: 1.03x slower                                                 |
| coroutines               | 20.7 ms                                                | 21.4 ms: 1.03x slower                                                 |
| python_startup           | 10.9 ms                                                | 11.8 ms: 1.09x slower                                                 |
| generators               | 32.3 ms                                                | 35.4 ms: 1.09x slower                                                 |
| async_generators         | 231 ms                                                 | 260 ms: 1.12x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 9.57 ms: 1.21x slower                                                 |
| typing_runtime_protocols | 323 us                                                 | 392 us: 1.21x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 45.4 ms: 1.22x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.16x faster                                                          |

Benchmark hidden because not significant (2): asyncio_websockets, pathlib
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint
Ignored benchmarks (4) of results/bm-20230404-3.12.0a7-b861ba4/bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.09x