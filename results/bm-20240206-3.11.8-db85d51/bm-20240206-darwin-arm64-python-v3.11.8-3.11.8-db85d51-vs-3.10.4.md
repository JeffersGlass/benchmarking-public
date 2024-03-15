
# Results vs. 3.10.4

- fork: python
- ref: v3.11.8
- machine: darwin-arm64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.22x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 151 ms: 1.27x faster                                   |
| chameleon      | 6.26 ms                                                | 4.32 ms: 1.45x faster                                  |
| docutils       | 1.73 sec                                               | 1.42 sec: 1.22x faster                                 |
| html5lib       | 42.4 ms                                                | 33.2 ms: 1.27x faster                                  |
| tornado_http   | 86.7 ms                                                | 69.4 ms: 1.25x faster                                  |
| Geometric mean | (ref)                                                  | 1.29x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 321 ms: 1.48x faster                                   |
| async_tree_io           | 980 ms                                                 | 693 ms: 1.41x faster                                   |
| async_tree_none         | 388 ms                                                 | 280 ms: 1.39x faster                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 520 ms: 1.25x faster                                   |
| Geometric mean          | (ref)                                                  | 1.38x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 68.5 ms: 1.36x faster                                  |
| float          | 69.0 ms                                                | 53.4 ms: 1.29x faster                                  |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                   |
| Geometric mean | (ref)                                                  | 1.21x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 70.9 ms: 1.34x faster                                  |
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                   |
| regex_v8       | 17.1 ms                                                | 16.3 ms: 1.05x faster                                  |
| regex_effbot   | 2.46 ms                                                | 2.64 ms: 1.07x slower                                  |
| Geometric mean | (ref)                                                  | 1.11x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.44x faster                                   |
| xml_etree_process    | 46.5 ms                                                | 33.2 ms: 1.40x faster                                  |
| unpickle_pure_python | 194 us                                                 | 145 us: 1.34x faster                                   |
| tomli_loads          | 1.71 sec                                               | 1.29 sec: 1.32x faster                                 |
| xml_etree_generate   | 53.5 ms                                                | 45.1 ms: 1.19x faster                                  |
| json_loads           | 16.4 us                                                | 15.3 us: 1.08x faster                                  |
| json_dumps           | 8.11 ms                                                | 7.55 ms: 1.07x faster                                  |
| unpickle             | 8.80 us                                                | 8.21 us: 1.07x faster                                  |
| xml_etree_parse      | 108 ms                                                 | 101 ms: 1.07x faster                                   |
| xml_etree_iterparse  | 72.1 ms                                                | 68.0 ms: 1.06x faster                                  |
| pickle_list          | 2.74 us                                                | 2.64 us: 1.04x faster                                  |
| unpickle_list        | 2.69 us                                                | 2.64 us: 1.02x faster                                  |
| pickle_dict          | 17.0 us                                                | 17.3 us: 1.02x slower                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                           |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.6 ms: 1.07x slower                                  |
| python_startup_no_site | 7.91 ms                                                | 9.53 ms: 1.21x slower                                  |
| Geometric mean         | (ref)                                                  | 1.13x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 26.4 ms                                                | 19.6 ms: 1.34x faster                                  |
| mako            | 9.87 ms                                                | 7.97 ms: 1.24x faster                                  |
| genshi_text     | 17.3 ms                                                | 14.2 ms: 1.22x faster                                  |
| genshi_xml      | 33.8 ms                                                | 28.3 ms: 1.20x faster                                  |
| Geometric mean  | (ref)                                                  | 1.25x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 2.62 ms: 1.88x faster                                  |
| logging_silent           | 117 ns                                                 | 66.0 ns: 1.77x faster                                  |
| scimark_sor              | 128 ms                                                 | 81.0 ms: 1.58x faster                                  |
| richards                 | 48.7 ms                                                | 31.3 ms: 1.55x faster                                  |
| richards_super           | 57.8 ms                                                | 37.8 ms: 1.53x faster                                  |
| scimark_lu               | 103 ms                                                 | 67.6 ms: 1.52x faster                                  |
| crypto_pyaes             | 71.8 ms                                                | 47.3 ms: 1.52x faster                                  |
| raytrace                 | 301 ms                                                 | 203 ms: 1.48x faster                                   |
| pyflate                  | 427 ms                                                 | 289 ms: 1.48x faster                                   |
| async_tree_memoization   | 474 ms                                                 | 321 ms: 1.48x faster                                   |
| go                       | 151 ms                                                 | 103 ms: 1.46x faster                                   |
| chameleon                | 6.26 ms                                                | 4.32 ms: 1.45x faster                                  |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.44x faster                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 46.2 ms: 1.42x faster                                  |
| async_tree_io            | 980 ms                                                 | 693 ms: 1.41x faster                                   |
| xml_etree_process        | 46.5 ms                                                | 33.2 ms: 1.40x faster                                  |
| sqlglot_parse            | 1.24 ms                                                | 889 us: 1.40x faster                                   |
| deepcopy_memo            | 34.7 us                                                | 24.9 us: 1.39x faster                                  |
| thrift                   | 572 us                                                 | 411 us: 1.39x faster                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.04 ms: 1.39x faster                                  |
| async_tree_none          | 388 ms                                                 | 280 ms: 1.39x faster                                   |
| chaos                    | 65.8 ms                                                | 48.1 ms: 1.37x faster                                  |
| hexiom                   | 6.19 ms                                                | 4.53 ms: 1.37x faster                                  |
| nbody                    | 93.0 ms                                                | 68.5 ms: 1.36x faster                                  |
| spectral_norm            | 94.8 ms                                                | 70.0 ms: 1.35x faster                                  |
| django_template          | 26.4 ms                                                | 19.6 ms: 1.34x faster                                  |
| regex_compile            | 95.3 ms                                                | 70.9 ms: 1.34x faster                                  |
| pprint_safe_repr         | 641 ms                                                 | 478 ms: 1.34x faster                                   |
| unpickle_pure_python     | 194 us                                                 | 145 us: 1.34x faster                                   |
| pprint_pformat           | 1.30 sec                                               | 976 ms: 1.34x faster                                   |
| pycparser                | 877 ms                                                 | 657 ms: 1.33x faster                                   |
| deepcopy                 | 272 us                                                 | 204 us: 1.33x faster                                   |
| deepcopy_reduce          | 2.33 us                                                | 1.76 us: 1.33x faster                                  |
| tomli_loads              | 1.71 sec                                               | 1.29 sec: 1.32x faster                                 |
| logging_format           | 4.83 us                                                | 3.67 us: 1.32x faster                                  |
| logging_simple           | 4.45 us                                                | 3.39 us: 1.31x faster                                  |
| float                    | 69.0 ms                                                | 53.4 ms: 1.29x faster                                  |
| html5lib                 | 42.4 ms                                                | 33.2 ms: 1.27x faster                                  |
| 2to3                     | 192 ms                                                 | 151 ms: 1.27x faster                                   |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.03 ms: 1.26x faster                                  |
| tornado_http             | 86.7 ms                                                | 69.4 ms: 1.25x faster                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 520 ms: 1.25x faster                                   |
| sqlglot_optimize         | 36.8 ms                                                | 29.5 ms: 1.25x faster                                  |
| mako                     | 9.87 ms                                                | 7.97 ms: 1.24x faster                                  |
| async_generators         | 231 ms                                                 | 187 ms: 1.24x faster                                   |
| dulwich_log              | 35.3 ms                                                | 28.6 ms: 1.23x faster                                  |
| fannkuch                 | 303 ms                                                 | 246 ms: 1.23x faster                                   |
| sqlalchemy_declarative   | 73.3 ms                                                | 59.6 ms: 1.23x faster                                  |
| coroutines               | 20.7 ms                                                | 16.9 ms: 1.23x faster                                  |
| genshi_text              | 17.3 ms                                                | 14.2 ms: 1.22x faster                                  |
| comprehensions           | 16.9 us                                                | 13.9 us: 1.22x faster                                  |
| docutils                 | 1.73 sec                                               | 1.42 sec: 1.22x faster                                 |
| create_gc_cycles         | 860 us                                                 | 712 us: 1.21x faster                                   |
| scimark_fft              | 224 ms                                                 | 186 ms: 1.21x faster                                   |
| genshi_xml               | 33.8 ms                                                | 28.3 ms: 1.20x faster                                  |
| sympy_integrate          | 13.1 ms                                                | 11.1 ms: 1.19x faster                                  |
| sqlglot_normalize        | 190 ms                                                 | 160 ms: 1.19x faster                                   |
| xml_etree_generate       | 53.5 ms                                                | 45.1 ms: 1.19x faster                                  |
| sympy_expand             | 269 ms                                                 | 227 ms: 1.19x faster                                   |
| sympy_str                | 165 ms                                                 | 140 ms: 1.18x faster                                   |
| sympy_sum                | 92.2 ms                                                | 78.5 ms: 1.17x faster                                  |
| dask                     | 253 ms                                                 | 218 ms: 1.16x faster                                   |
| sqlite_synth             | 1.46 us                                                | 1.26 us: 1.16x faster                                  |
| unpack_sequence          | 39.0 ns                                                | 33.8 ns: 1.16x faster                                  |
| nqueens                  | 63.8 ms                                                | 55.3 ms: 1.15x faster                                  |
| aiohttp                  | 1.22 ms                                                | 1.06 ms: 1.15x faster                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 2.98 ms: 1.15x faster                                  |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                   |
| bench_thread_pool        | 527 us                                                 | 461 us: 1.14x faster                                   |
| flaskblogging            | 2.65 ms                                                | 2.33 ms: 1.14x faster                                  |
| gunicorn                 | 1.30 ms                                                | 1.15 ms: 1.13x faster                                  |
| json                     | 3.08 ms                                                | 2.74 ms: 1.13x faster                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.43 sec: 1.12x faster                                 |
| telco                    | 3.49 ms                                                | 3.15 ms: 1.11x faster                                  |
| pylint                   | 277 ms                                                 | 250 ms: 1.11x faster                                   |
| mdp                      | 1.63 sec                                               | 1.48 sec: 1.11x faster                                 |
| generators               | 32.3 ms                                                | 29.4 ms: 1.10x faster                                  |
| meteor_contest           | 77.7 ms                                                | 71.1 ms: 1.09x faster                                  |
| json_loads               | 16.4 us                                                | 15.3 us: 1.08x faster                                  |
| json_dumps               | 8.11 ms                                                | 7.55 ms: 1.07x faster                                  |
| unpickle                 | 8.80 us                                                | 8.21 us: 1.07x faster                                  |
| xml_etree_parse          | 108 ms                                                 | 101 ms: 1.07x faster                                   |
| typing_runtime_protocols | 323 us                                                 | 303 us: 1.07x faster                                   |
| xml_etree_iterparse      | 72.1 ms                                                | 68.0 ms: 1.06x faster                                  |
| pathlib                  | 24.5 ms                                                | 23.2 ms: 1.05x faster                                  |
| regex_v8                 | 17.1 ms                                                | 16.3 ms: 1.05x faster                                  |
| pickle_list              | 2.74 us                                                | 2.64 us: 1.04x faster                                  |
| unpickle_list            | 2.69 us                                                | 2.64 us: 1.02x faster                                  |
| asyncio_websockets       | 410 ms                                                 | 407 ms: 1.01x faster                                   |
| pidigits                 | 282 ms                                                 | 280 ms: 1.01x faster                                   |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                  |
| pickle_dict              | 17.0 us                                                | 17.3 us: 1.02x slower                                  |
| coverage                 | 41.5 ms                                                | 43.4 ms: 1.05x slower                                  |
| python_startup           | 10.9 ms                                                | 11.6 ms: 1.07x slower                                  |
| regex_effbot             | 2.46 ms                                                | 2.64 ms: 1.07x slower                                  |
| bench_mp_pool            | 37.4 ms                                                | 41.2 ms: 1.10x slower                                  |
| python_startup_no_site   | 7.91 ms                                                | 9.53 ms: 1.21x slower                                  |
| Geometric mean           | (ref)                                                  | 1.22x faster                                           |

Benchmark hidden because not significant (3): mypy2, asyncio_tcp, pickle
Ignored benchmarks (4) of results/bm-20240206-3.11.8-db85d51/bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.07x