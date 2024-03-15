
# Results vs. 3.10.4

- fork: python
- ref: 2e91dba437fe5c56c6f8
- machine: darwin-arm64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.15x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 155 ms: 1.23x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.65 ms: 1.34x faster                                                 |
| docutils       | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                |
| html5lib       | 42.4 ms                                                | 33.6 ms: 1.26x faster                                                 |
| tornado_http   | 86.7 ms                                                | 76.9 ms: 1.13x faster                                                 |
| Geometric mean | (ref)                                                  | 1.23x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 288 ms: 1.35x faster                                                  |
| async_tree_memoization  | 474 ms                                                 | 374 ms: 1.27x faster                                                  |
| async_tree_io           | 980 ms                                                 | 816 ms: 1.20x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 558 ms: 1.16x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.24x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 64.4 ms: 1.45x faster                                                 |
| float          | 69.0 ms                                                | 51.6 ms: 1.34x faster                                                 |
| Geometric mean | (ref)                                                  | 1.25x faster                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 72.7 ms: 1.31x faster                                                 |
| regex_v8       | 17.1 ms                                                | 16.6 ms: 1.03x faster                                                 |
| regex_dna      | 174 ms                                                 | 173 ms: 1.01x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.45 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 203 us: 1.38x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 35.1 ms: 1.32x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.36 sec: 1.26x faster                                                |
| unpickle_pure_python | 194 us                                                 | 158 us: 1.23x faster                                                  |
| xml_etree_generate   | 53.5 ms                                                | 47.3 ms: 1.13x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 96.7 ms: 1.11x faster                                                 |
| json_dumps           | 8.11 ms                                                | 7.46 ms: 1.09x faster                                                 |
| json_loads           | 16.4 us                                                | 15.3 us: 1.08x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 69.6 ms: 1.04x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.67 us: 1.03x faster                                                 |
| unpickle             | 8.80 us                                                | 8.57 us: 1.03x faster                                                 |
| pickle_dict          | 17.0 us                                                | 16.8 us: 1.01x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| pickle               | 6.97 us                                                | 7.39 us: 1.06x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 7.91 ms                                                | 9.02 ms: 1.14x slower                                                 |
| python_startup         | 10.9 ms                                                | 14.9 ms: 1.37x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 26.4 ms                                                | 20.8 ms: 1.27x faster                                                 |
| mako            | 9.87 ms                                                | 8.07 ms: 1.22x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.8 ms: 1.17x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 29.4 ms: 1.15x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.20x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.96 ms: 1.66x faster                                                 |
| logging_silent           | 117 ns                                                 | 74.3 ns: 1.58x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 43.2 ms: 1.52x faster                                                 |
| scimark_sor              | 128 ms                                                 | 85.3 ms: 1.50x faster                                                 |
| richards                 | 48.7 ms                                                | 33.2 ms: 1.46x faster                                                 |
| nbody                    | 93.0 ms                                                | 64.4 ms: 1.45x faster                                                 |
| scimark_lu               | 103 ms                                                 | 71.4 ms: 1.44x faster                                                 |
| chaos                    | 65.8 ms                                                | 46.4 ms: 1.42x faster                                                 |
| hexiom                   | 6.19 ms                                                | 4.41 ms: 1.41x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.19 us: 1.40x faster                                                 |
| logging_format           | 4.83 us                                                | 3.49 us: 1.38x faster                                                 |
| pickle_pure_python       | 281 us                                                 | 203 us: 1.38x faster                                                  |
| raytrace                 | 301 ms                                                 | 218 ms: 1.38x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 465 ms: 1.38x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 952 ms: 1.37x faster                                                  |
| richards_super           | 57.8 ms                                                | 42.7 ms: 1.35x faster                                                 |
| async_tree_none          | 388 ms                                                 | 288 ms: 1.35x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.65 ms: 1.34x faster                                                 |
| float                    | 69.0 ms                                                | 51.6 ms: 1.34x faster                                                 |
| deepcopy_memo            | 34.7 us                                                | 26.0 us: 1.33x faster                                                 |
| go                       | 151 ms                                                 | 113 ms: 1.33x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 35.1 ms: 1.32x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 71.6 ms: 1.32x faster                                                 |
| pyflate                  | 427 ms                                                 | 322 ms: 1.32x faster                                                  |
| regex_compile            | 95.3 ms                                                | 72.7 ms: 1.31x faster                                                 |
| thrift                   | 572 us                                                 | 440 us: 1.30x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 56.0 ms: 1.28x faster                                                 |
| django_template          | 26.4 ms                                                | 20.8 ms: 1.27x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 374 ms: 1.27x faster                                                  |
| html5lib                 | 42.4 ms                                                | 33.6 ms: 1.26x faster                                                 |
| unpack_sequence          | 39.0 ns                                                | 31.0 ns: 1.26x faster                                                 |
| tomli_loads              | 1.71 sec                                               | 1.36 sec: 1.26x faster                                                |
| pycparser                | 877 ms                                                 | 702 ms: 1.25x faster                                                  |
| 2to3                     | 192 ms                                                 | 155 ms: 1.23x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.89 us: 1.23x faster                                                 |
| unpickle_pure_python     | 194 us                                                 | 158 us: 1.23x faster                                                  |
| mako                     | 9.87 ms                                                | 8.07 ms: 1.22x faster                                                 |
| fannkuch                 | 303 ms                                                 | 247 ms: 1.22x faster                                                  |
| coroutines               | 20.7 ms                                                | 16.9 ms: 1.22x faster                                                 |
| generators               | 32.3 ms                                                | 26.6 ms: 1.22x faster                                                 |
| scimark_fft              | 224 ms                                                 | 184 ms: 1.22x faster                                                  |
| async_generators         | 231 ms                                                 | 191 ms: 1.21x faster                                                  |
| deepcopy                 | 272 us                                                 | 224 us: 1.21x faster                                                  |
| async_tree_io            | 980 ms                                                 | 816 ms: 1.20x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 29.6 ms: 1.19x faster                                                 |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.43 ms: 1.19x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 729 us: 1.18x faster                                                  |
| genshi_text              | 17.3 ms                                                | 14.8 ms: 1.17x faster                                                 |
| docutils                 | 1.73 sec                                               | 1.48 sec: 1.17x faster                                                |
| sqlalchemy_declarative   | 73.3 ms                                                | 62.6 ms: 1.17x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 31.6 ms: 1.16x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 558 ms: 1.16x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.3 ms: 1.16x faster                                                 |
| sqlglot_normalize        | 190 ms                                                 | 164 ms: 1.16x faster                                                  |
| genshi_xml               | 33.8 ms                                                | 29.4 ms: 1.15x faster                                                 |
| pylint                   | 277 ms                                                 | 241 ms: 1.15x faster                                                  |
| nqueens                  | 63.8 ms                                                | 55.5 ms: 1.15x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.01 ms: 1.14x faster                                                 |
| xml_etree_generate       | 53.5 ms                                                | 47.3 ms: 1.13x faster                                                 |
| tornado_http             | 86.7 ms                                                | 76.9 ms: 1.13x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 82.2 ms: 1.12x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 96.7 ms: 1.11x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.32 us: 1.11x faster                                                 |
| sympy_expand             | 269 ms                                                 | 244 ms: 1.10x faster                                                  |
| sympy_str                | 165 ms                                                 | 151 ms: 1.10x faster                                                  |
| flaskblogging            | 2.65 ms                                                | 2.43 ms: 1.09x faster                                                 |
| json_dumps               | 8.11 ms                                                | 7.46 ms: 1.09x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 71.7 ms: 1.08x faster                                                 |
| json                     | 3.08 ms                                                | 2.86 ms: 1.08x faster                                                 |
| json_loads               | 16.4 us                                                | 15.3 us: 1.08x faster                                                 |
| sqlglot_transpile        | 1.44 ms                                                | 1.35 ms: 1.07x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 498 us: 1.06x faster                                                  |
| gunicorn                 | 1.30 ms                                                | 1.23 ms: 1.06x faster                                                 |
| telco                    | 3.49 ms                                                | 3.31 ms: 1.05x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.3 ms: 1.05x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 1.19 ms: 1.05x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 69.6 ms: 1.04x faster                                                 |
| regex_v8                 | 17.1 ms                                                | 16.6 ms: 1.03x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.67 us: 1.03x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.57 us: 1.03x faster                                                 |
| comprehensions           | 16.9 us                                                | 16.5 us: 1.02x faster                                                 |
| pickle_dict              | 17.0 us                                                | 16.8 us: 1.01x faster                                                 |
| regex_dna                | 174 ms                                                 | 173 ms: 1.01x faster                                                  |
| regex_effbot             | 2.46 ms                                                | 2.45 ms: 1.00x faster                                                 |
| typing_runtime_protocols | 323 us                                                 | 325 us: 1.00x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.01x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.75 us: 1.02x slower                                                 |
| pickle                   | 6.97 us                                                | 7.39 us: 1.06x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.76 sec: 1.08x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 41.4 ms: 1.11x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.02 ms: 1.14x slower                                                 |
| dask                     | 253 ms                                                 | 302 ms: 1.19x slower                                                  |
| python_startup           | 10.9 ms                                                | 14.9 ms: 1.37x slower                                                 |
| coverage                 | 41.5 ms                                                | 303 ms: 7.30x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.15x faster                                                          |

Benchmark hidden because not significant (1): pidigits
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.09x