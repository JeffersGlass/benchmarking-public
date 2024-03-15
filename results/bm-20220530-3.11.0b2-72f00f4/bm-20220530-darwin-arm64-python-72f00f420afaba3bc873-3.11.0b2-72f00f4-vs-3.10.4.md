
# Results vs. 3.10.4

- fork: python
- ref: 72f00f420afaba3bc873
- machine: darwin-arm64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 153 ms: 1.25x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.32 ms: 1.45x faster                                                 |
| docutils       | 1.73 sec                                               | 1.42 sec: 1.22x faster                                                |
| html5lib       | 42.4 ms                                                | 32.7 ms: 1.30x faster                                                 |
| tornado_http   | 86.7 ms                                                | 68.8 ms: 1.26x faster                                                 |
| Geometric mean | (ref)                                                  | 1.29x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_io           | 980 ms                                                 | 688 ms: 1.42x faster                                                  |
| async_tree_none         | 388 ms                                                 | 278 ms: 1.40x faster                                                  |
| async_tree_memoization  | 474 ms                                                 | 363 ms: 1.31x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 514 ms: 1.26x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.35x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 65.5 ms: 1.42x faster                                                 |
| float          | 69.0 ms                                                | 54.4 ms: 1.27x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.22x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.8 ms: 1.29x faster                                                 |
| regex_dna      | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| regex_v8       | 17.1 ms                                                | 15.2 ms: 1.12x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.22 ms: 1.11x faster                                                 |
| Geometric mean | (ref)                                                  | 1.17x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 194 us: 1.45x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 33.9 ms: 1.37x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.30 sec: 1.31x faster                                                |
| unpickle_pure_python | 194 us                                                 | 151 us: 1.29x faster                                                  |
| xml_etree_generate   | 53.5 ms                                                | 46.7 ms: 1.14x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 97.2 ms: 1.11x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 66.9 ms: 1.08x faster                                                 |
| json_dumps           | 8.11 ms                                                | 7.58 ms: 1.07x faster                                                 |
| json_loads           | 16.4 us                                                | 15.4 us: 1.07x faster                                                 |
| unpickle             | 8.80 us                                                | 8.23 us: 1.07x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.59 us: 1.06x faster                                                 |
| pickle_dict          | 17.0 us                                                | 16.1 us: 1.06x faster                                                 |
| pickle               | 6.97 us                                                | 7.03 us: 1.01x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.80 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.31 ms: 1.18x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.11x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 19.8 ms: 1.33x faster                                                 |
| mako            | 9.87 ms                                                | 8.11 ms: 1.22x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.6 ms: 1.18x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 28.8 ms: 1.17x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.22x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.72 ms: 1.80x faster                                                 |
| logging_silent           | 117 ns                                                 | 66.3 ns: 1.77x faster                                                 |
| scimark_sor              | 128 ms                                                 | 76.1 ms: 1.68x faster                                                 |
| richards                 | 48.7 ms                                                | 31.3 ms: 1.56x faster                                                 |
| richards_super           | 57.8 ms                                                | 37.8 ms: 1.53x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 47.4 ms: 1.52x faster                                                 |
| raytrace                 | 301 ms                                                 | 200 ms: 1.51x faster                                                  |
| scimark_lu               | 103 ms                                                 | 68.2 ms: 1.51x faster                                                 |
| pyflate                  | 427 ms                                                 | 285 ms: 1.50x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 44.3 ms: 1.48x faster                                                 |
| go                       | 151 ms                                                 | 103 ms: 1.46x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.32 ms: 1.45x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 194 us: 1.45x faster                                                  |
| async_tree_io            | 980 ms                                                 | 688 ms: 1.42x faster                                                  |
| nbody                    | 93.0 ms                                                | 65.5 ms: 1.42x faster                                                 |
| async_tree_none          | 388 ms                                                 | 278 ms: 1.40x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 68.4 ms: 1.39x faster                                                 |
| thrift                   | 572 us                                                 | 415 us: 1.38x faster                                                  |
| chaos                    | 65.8 ms                                                | 47.8 ms: 1.38x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 33.9 ms: 1.37x faster                                                 |
| hexiom                   | 6.19 ms                                                | 4.58 ms: 1.35x faster                                                 |
| django_template          | 26.4 ms                                                | 19.8 ms: 1.33x faster                                                 |
| logging_format           | 4.83 us                                                | 3.63 us: 1.33x faster                                                 |
| pycparser                | 877 ms                                                 | 660 ms: 1.33x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 485 ms: 1.32x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.37 us: 1.32x faster                                                 |
| pprint_pformat           | 1.30 sec                                               | 988 ms: 1.32x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.30 sec: 1.31x faster                                                |
| async_tree_memoization   | 474 ms                                                 | 363 ms: 1.31x faster                                                  |
| html5lib                 | 42.4 ms                                                | 32.7 ms: 1.30x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 151 us: 1.29x faster                                                  |
| regex_compile            | 95.3 ms                                                | 73.8 ms: 1.29x faster                                                 |
| sqlalchemy_imperative    | 8.86 ms                                                | 6.97 ms: 1.27x faster                                                 |
| float                    | 69.0 ms                                                | 54.4 ms: 1.27x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 514 ms: 1.26x faster                                                  |
| tornado_http             | 86.7 ms                                                | 68.8 ms: 1.26x faster                                                 |
| deepcopy_memo            | 34.7 us                                                | 27.8 us: 1.25x faster                                                 |
| 2to3                     | 192 ms                                                 | 153 ms: 1.25x faster                                                  |
| fannkuch                 | 303 ms                                                 | 244 ms: 1.24x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 28.7 ms: 1.23x faster                                                 |
| sqlalchemy_declarative   | 73.3 ms                                                | 59.5 ms: 1.23x faster                                                 |
| scimark_fft              | 224 ms                                                 | 183 ms: 1.23x faster                                                  |
| coroutines               | 20.7 ms                                                | 17.0 ms: 1.22x faster                                                 |
| mako                     | 9.87 ms                                                | 8.11 ms: 1.22x faster                                                 |
| docutils                 | 1.73 sec                                               | 1.42 sec: 1.22x faster                                                |
| async_generators         | 231 ms                                                 | 191 ms: 1.21x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 711 us: 1.21x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.93 us: 1.21x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 30.4 ms: 1.21x faster                                                 |
| unpack_sequence          | 39.0 ns                                                | 32.7 ns: 1.20x faster                                                 |
| deepcopy                 | 272 us                                                 | 228 us: 1.19x faster                                                  |
| regex_dna                | 174 ms                                                 | 147 ms: 1.19x faster                                                  |
| genshi_text              | 17.3 ms                                                | 14.6 ms: 1.18x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 78.2 ms: 1.18x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.18x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 28.8 ms: 1.17x faster                                                 |
| sqlglot_normalize        | 190 ms                                                 | 163 ms: 1.17x faster                                                  |
| nqueens                  | 63.8 ms                                                | 54.7 ms: 1.17x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.95 ms: 1.16x faster                                                 |
| dask                     | 253 ms                                                 | 219 ms: 1.16x faster                                                  |
| sympy_expand             | 269 ms                                                 | 233 ms: 1.16x faster                                                  |
| sympy_str                | 165 ms                                                 | 143 ms: 1.15x faster                                                  |
| xml_etree_generate       | 53.5 ms                                                | 46.7 ms: 1.14x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 466 us: 1.13x faster                                                  |
| regex_v8                 | 17.1 ms                                                | 15.2 ms: 1.12x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.43 sec: 1.12x faster                                                |
| sqlite_synth             | 1.46 us                                                | 1.31 us: 1.11x faster                                                 |
| aiohttp                  | 1.22 ms                                                | 1.10 ms: 1.11x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.30 ms: 1.11x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 97.2 ms: 1.11x faster                                                 |
| regex_effbot             | 2.46 ms                                                | 2.22 ms: 1.11x faster                                                 |
| pylint                   | 277 ms                                                 | 251 ms: 1.10x faster                                                  |
| json                     | 3.08 ms                                                | 2.79 ms: 1.10x faster                                                 |
| gunicorn                 | 1.30 ms                                                | 1.18 ms: 1.10x faster                                                 |
| telco                    | 3.49 ms                                                | 3.17 ms: 1.10x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 1.14 ms: 1.09x faster                                                 |
| generators               | 32.3 ms                                                | 30.0 ms: 1.08x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 66.9 ms: 1.08x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 72.5 ms: 1.07x faster                                                 |
| json_dumps               | 8.11 ms                                                | 7.58 ms: 1.07x faster                                                 |
| json_loads               | 16.4 us                                                | 15.4 us: 1.07x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.23 us: 1.07x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.2 ms: 1.06x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.59 us: 1.06x faster                                                 |
| pickle_dict              | 17.0 us                                                | 16.1 us: 1.06x faster                                                 |
| asyncio_websockets       | 410 ms                                                 | 407 ms: 1.01x faster                                                  |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| typing_runtime_protocols | 323 us                                                 | 326 us: 1.01x slower                                                  |
| pickle                   | 6.97 us                                                | 7.03 us: 1.01x slower                                                 |
| asyncio_tcp              | 659 ms                                                 | 665 ms: 1.01x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.38 ms: 1.01x slower                                                 |
| comprehensions           | 16.9 us                                                | 17.2 us: 1.01x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.80 us: 1.04x slower                                                 |
| python_startup           | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.74 sec: 1.07x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 41.6 ms: 1.11x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.31 ms: 1.18x slower                                                 |
| coverage                 | 41.5 ms                                                | 72.4 ms: 1.75x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.20x faster                                                          |
Ignored benchmarks (2) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, mypy2
Ignored benchmarks (4) of results/bm-20220530-3.11.0b2-72f00f4/bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.05x