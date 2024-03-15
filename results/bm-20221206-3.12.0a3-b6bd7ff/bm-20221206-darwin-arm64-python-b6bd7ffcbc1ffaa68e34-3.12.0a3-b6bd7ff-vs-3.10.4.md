
# Results vs. 3.10.4

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: darwin-arm64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.15x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 166 ms: 1.16x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.68 ms: 1.34x faster                                                 |
| docutils       | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                |
| html5lib       | 42.4 ms                                                | 34.7 ms: 1.22x faster                                                 |
| Geometric mean | (ref)                                                  | 1.22x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 333 ms: 1.42x faster                                                  |
| async_tree_none         | 388 ms                                                 | 295 ms: 1.31x faster                                                  |
| async_tree_io           | 980 ms                                                 | 758 ms: 1.29x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 539 ms: 1.21x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.31x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 68.4 ms: 1.36x faster                                                 |
| float          | 69.0 ms                                                | 57.6 ms: 1.20x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.18x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 78.1 ms: 1.22x faster                                                 |
| regex_dna      | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| regex_v8       | 17.1 ms                                                | 15.1 ms: 1.13x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.45 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.13x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 213 us: 1.32x faster                                                  |
| json_dumps           | 8.11 ms                                                | 6.15 ms: 1.32x faster                                                 |
| xml_etree_process    | 46.5 ms                                                | 36.4 ms: 1.28x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 160 us: 1.21x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.51 sec: 1.13x faster                                                |
| xml_etree_generate   | 53.5 ms                                                | 47.5 ms: 1.13x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 96.5 ms: 1.12x faster                                                 |
| json_loads           | 16.4 us                                                | 15.8 us: 1.04x faster                                                 |
| unpickle             | 8.80 us                                                | 8.45 us: 1.04x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.67 us: 1.03x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 70.3 ms: 1.03x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| pickle               | 6.97 us                                                | 7.13 us: 1.02x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                          |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.48 ms: 1.20x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.12x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.45 ms: 1.32x faster                                                 |
| django_template | 26.4 ms                                                | 21.9 ms: 1.21x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 30.7 ms: 1.10x faster                                                 |
| genshi_text     | 17.3 ms                                                | 15.9 ms: 1.09x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.18x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.83 ms: 1.73x faster                                                 |
| logging_silent           | 117 ns                                                 | 79.3 ns: 1.48x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 333 ms: 1.42x faster                                                  |
| richards                 | 48.7 ms                                                | 34.7 ms: 1.40x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 51.5 ms: 1.40x faster                                                 |
| richards_super           | 57.8 ms                                                | 41.5 ms: 1.39x faster                                                 |
| raytrace                 | 301 ms                                                 | 218 ms: 1.38x faster                                                  |
| nbody                    | 93.0 ms                                                | 68.4 ms: 1.36x faster                                                 |
| chameleon                | 6.26 ms                                                | 4.68 ms: 1.34x faster                                                 |
| mako                     | 9.87 ms                                                | 7.45 ms: 1.32x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 213 us: 1.32x faster                                                  |
| json_dumps               | 8.11 ms                                                | 6.15 ms: 1.32x faster                                                 |
| async_tree_none          | 388 ms                                                 | 295 ms: 1.31x faster                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.65 ms: 1.29x faster                                                 |
| async_tree_io            | 980 ms                                                 | 758 ms: 1.29x faster                                                  |
| thrift                   | 572 us                                                 | 445 us: 1.29x faster                                                  |
| chaos                    | 65.8 ms                                                | 51.4 ms: 1.28x faster                                                 |
| go                       | 151 ms                                                 | 118 ms: 1.28x faster                                                  |
| pycparser                | 877 ms                                                 | 686 ms: 1.28x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 36.4 ms: 1.28x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 507 ms: 1.26x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.03 sec: 1.26x faster                                                |
| create_gc_cycles         | 860 us                                                 | 682 us: 1.26x faster                                                  |
| scimark_lu               | 103 ms                                                 | 81.7 ms: 1.26x faster                                                 |
| pyflate                  | 427 ms                                                 | 340 ms: 1.26x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.97 ms: 1.25x faster                                                 |
| scimark_sor              | 128 ms                                                 | 105 ms: 1.23x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 53.6 ms: 1.22x faster                                                 |
| html5lib                 | 42.4 ms                                                | 34.7 ms: 1.22x faster                                                 |
| regex_compile            | 95.3 ms                                                | 78.1 ms: 1.22x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 1.02 ms: 1.22x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 160 us: 1.21x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 28.7 us: 1.21x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.19 ms: 1.21x faster                                                 |
| unpack_sequence          | 39.0 ns                                                | 32.3 ns: 1.21x faster                                                 |
| django_template          | 26.4 ms                                                | 21.9 ms: 1.21x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 539 ms: 1.21x faster                                                  |
| scimark_fft              | 224 ms                                                 | 186 ms: 1.21x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 29.4 ms: 1.20x faster                                                 |
| float                    | 69.0 ms                                                | 57.6 ms: 1.20x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 79.6 ms: 1.19x faster                                                 |
| regex_dna                | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| logging_format           | 4.83 us                                                | 4.10 us: 1.18x faster                                                 |
| docutils                 | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                |
| logging_simple           | 4.45 us                                                | 3.81 us: 1.17x faster                                                 |
| 2to3                     | 192 ms                                                 | 166 ms: 1.16x faster                                                  |
| fannkuch                 | 303 ms                                                 | 267 ms: 1.13x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 15.1 ms: 1.13x faster                                                 |
| deepcopy                 | 272 us                                                 | 240 us: 1.13x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.51 sec: 1.13x faster                                                |
| telco                    | 3.49 ms                                                | 3.09 ms: 1.13x faster                                                 |
| xml_etree_generate       | 53.5 ms                                                | 47.5 ms: 1.13x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 96.5 ms: 1.12x faster                                                 |
| deepcopy_reduce          | 2.33 us                                                | 2.09 us: 1.12x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 33.1 ms: 1.11x faster                                                 |
| async_generators         | 231 ms                                                 | 208 ms: 1.11x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.9 ms: 1.11x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 30.7 ms: 1.10x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.46 sec: 1.10x faster                                                |
| sympy_expand             | 269 ms                                                 | 246 ms: 1.09x faster                                                  |
| genshi_text              | 17.3 ms                                                | 15.9 ms: 1.09x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 485 us: 1.09x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 85.0 ms: 1.08x faster                                                 |
| sympy_str                | 165 ms                                                 | 153 ms: 1.08x faster                                                  |
| json                     | 3.08 ms                                                | 2.85 ms: 1.08x faster                                                 |
| nqueens                  | 63.8 ms                                                | 60.0 ms: 1.06x faster                                                 |
| sqlglot_normalize        | 190 ms                                                 | 180 ms: 1.06x faster                                                  |
| pathlib                  | 24.5 ms                                                | 23.3 ms: 1.05x faster                                                 |
| json_loads               | 16.4 us                                                | 15.8 us: 1.04x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.45 us: 1.04x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.67 us: 1.03x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 70.3 ms: 1.03x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 75.9 ms: 1.02x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.43 us: 1.02x faster                                                 |
| coroutines               | 20.7 ms                                                | 20.5 ms: 1.01x faster                                                 |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| regex_effbot             | 2.46 ms                                                | 2.45 ms: 1.00x faster                                                 |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                  |
| gc_traversal             | 2.36 ms                                                | 2.38 ms: 1.01x slower                                                 |
| typing_runtime_protocols | 323 us                                                 | 329 us: 1.02x slower                                                  |
| comprehensions           | 16.9 us                                                | 17.3 us: 1.02x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| pickle                   | 6.97 us                                                | 7.13 us: 1.02x slower                                                 |
| python_startup           | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.77 sec: 1.09x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 42.6 ms: 1.14x slower                                                 |
| generators               | 32.3 ms                                                | 37.2 ms: 1.15x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.48 ms: 1.20x slower                                                 |
| dask                     | 253 ms                                                 | 331 ms: 1.31x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.15x faster                                                          |

Benchmark hidden because not significant (2): pickle_dict, asyncio_tcp
Ignored benchmarks (9) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
Ignored benchmarks (4) of results/bm-20221206-3.12.0a3-b6bd7ff/bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.06x