
# Results vs. 3.10.4

- fork: python
- ref: 3ddfa55df48a67a5972f
- machine: darwin-arm64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 164 ms: 1.17x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.55 ms: 1.38x faster                                                 |
| docutils       | 1.73 sec                                               | 1.47 sec: 1.18x faster                                                |
| html5lib       | 42.4 ms                                                | 33.5 ms: 1.26x faster                                                 |
| tornado_http   | 86.7 ms                                                | 73.8 ms: 1.17x faster                                                 |
| Geometric mean | (ref)                                                  | 1.23x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_io           | 980 ms                                                 | 704 ms: 1.39x faster                                                  |
| async_tree_memoization  | 474 ms                                                 | 347 ms: 1.37x faster                                                  |
| async_tree_none         | 388 ms                                                 | 287 ms: 1.35x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 533 ms: 1.22x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.33x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 54.8 ms: 1.26x faster                                                 |
| nbody          | 93.0 ms                                                | 74.1 ms: 1.26x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 76.7 ms: 1.24x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.45 ms: 1.00x faster                                                 |
| regex_dna      | 174 ms                                                 | 177 ms: 1.01x slower                                                  |
| regex_v8       | 17.1 ms                                                | 17.5 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 214 us: 1.31x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 36.5 ms: 1.27x faster                                                 |
| tomli_loads          | 1.71 sec                                               | 1.44 sec: 1.19x faster                                                |
| unpickle_pure_python | 194 us                                                 | 167 us: 1.16x faster                                                  |
| xml_etree_parse      | 108 ms                                                 | 97.5 ms: 1.11x faster                                                 |
| json_loads           | 16.4 us                                                | 14.9 us: 1.10x faster                                                 |
| xml_etree_generate   | 53.5 ms                                                | 48.7 ms: 1.10x faster                                                 |
| unpickle             | 8.80 us                                                | 8.29 us: 1.06x faster                                                 |
| json_dumps           | 8.11 ms                                                | 7.66 ms: 1.06x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.61 us: 1.05x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 69.4 ms: 1.04x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.74 us: 1.02x slower                                                 |
| pickle_dict          | 17.0 us                                                | 17.3 us: 1.02x slower                                                 |
| pickle               | 6.97 us                                                | 7.21 us: 1.03x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.09x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 7.91 ms                                                | 9.28 ms: 1.17x slower                                                 |
| python_startup         | 10.9 ms                                                | 14.8 ms: 1.36x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.27x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.33 ms: 1.35x faster                                                 |
| django_template | 26.4 ms                                                | 21.6 ms: 1.22x faster                                                 |
| genshi_text     | 17.3 ms                                                | 15.2 ms: 1.14x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 31.4 ms: 1.08x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.19x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue                | 4.91 ms                                                | 3.03 ms: 1.62x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 44.6 ms: 1.47x faster                                                 |
| logging_silent           | 117 ns                                                 | 80.3 ns: 1.46x faster                                                 |
| scimark_sor              | 128 ms                                                 | 88.7 ms: 1.45x faster                                                 |
| raytrace                 | 301 ms                                                 | 214 ms: 1.41x faster                                                  |
| logging_format           | 4.83 us                                                | 3.43 us: 1.41x faster                                                 |
| richards                 | 48.7 ms                                                | 34.9 ms: 1.39x faster                                                 |
| chaos                    | 65.8 ms                                                | 47.2 ms: 1.39x faster                                                 |
| async_tree_io            | 980 ms                                                 | 704 ms: 1.39x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.21 us: 1.39x faster                                                 |
| richards_super           | 57.8 ms                                                | 41.9 ms: 1.38x faster                                                 |
| chameleon                | 6.26 ms                                                | 4.55 ms: 1.38x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 347 ms: 1.37x faster                                                  |
| scimark_lu               | 103 ms                                                 | 75.5 ms: 1.36x faster                                                 |
| async_tree_none          | 388 ms                                                 | 287 ms: 1.35x faster                                                  |
| pyflate                  | 427 ms                                                 | 316 ms: 1.35x faster                                                  |
| go                       | 151 ms                                                 | 112 ms: 1.35x faster                                                  |
| mako                     | 9.87 ms                                                | 7.33 ms: 1.35x faster                                                 |
| thrift                   | 572 us                                                 | 433 us: 1.32x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 214 us: 1.31x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 55.4 ms: 1.30x faster                                                 |
| hexiom                   | 6.19 ms                                                | 4.78 ms: 1.30x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 36.5 ms: 1.27x faster                                                 |
| html5lib                 | 42.4 ms                                                | 33.5 ms: 1.26x faster                                                 |
| deepcopy_memo            | 34.7 us                                                | 27.5 us: 1.26x faster                                                 |
| float                    | 69.0 ms                                                | 54.8 ms: 1.26x faster                                                 |
| nbody                    | 93.0 ms                                                | 74.1 ms: 1.26x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 75.5 ms: 1.25x faster                                                 |
| regex_compile            | 95.3 ms                                                | 76.7 ms: 1.24x faster                                                 |
| pycparser                | 877 ms                                                 | 711 ms: 1.23x faster                                                  |
| django_template          | 26.4 ms                                                | 21.6 ms: 1.22x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 533 ms: 1.22x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 720 us: 1.19x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.95 us: 1.19x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 538 ms: 1.19x faster                                                  |
| async_generators         | 231 ms                                                 | 194 ms: 1.19x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.44 sec: 1.19x faster                                                |
| deepcopy                 | 272 us                                                 | 229 us: 1.18x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.10 sec: 1.18x faster                                                |
| docutils                 | 1.73 sec                                               | 1.47 sec: 1.18x faster                                                |
| dulwich_log              | 35.3 ms                                                | 30.0 ms: 1.18x faster                                                 |
| tornado_http             | 86.7 ms                                                | 73.8 ms: 1.17x faster                                                 |
| sqlite_synth             | 1.46 us                                                | 1.25 us: 1.17x faster                                                 |
| 2to3                     | 192 ms                                                 | 164 ms: 1.17x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 167 us: 1.16x faster                                                  |
| scimark_fft              | 224 ms                                                 | 194 ms: 1.16x faster                                                  |
| fannkuch                 | 303 ms                                                 | 264 ms: 1.15x faster                                                  |
| sqlalchemy_declarative   | 73.3 ms                                                | 63.8 ms: 1.15x faster                                                 |
| sqlalchemy_imperative    | 8.86 ms                                                | 7.72 ms: 1.15x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.1 ms: 1.15x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 32.2 ms: 1.14x faster                                                 |
| genshi_text              | 17.3 ms                                                | 15.2 ms: 1.14x faster                                                 |
| json                     | 3.08 ms                                                | 2.71 ms: 1.14x faster                                                 |
| sympy_sum                | 92.2 ms                                                | 82.0 ms: 1.12x faster                                                 |
| pylint                   | 277 ms                                                 | 247 ms: 1.12x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.7 ms: 1.12x faster                                                 |
| sqlglot_normalize        | 190 ms                                                 | 170 ms: 1.12x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.44 sec: 1.12x faster                                                |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.07 ms: 1.11x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 97.5 ms: 1.11x faster                                                 |
| json_loads               | 16.4 us                                                | 14.9 us: 1.10x faster                                                 |
| sympy_str                | 165 ms                                                 | 150 ms: 1.10x faster                                                  |
| xml_etree_generate       | 53.5 ms                                                | 48.7 ms: 1.10x faster                                                 |
| aiohttp                  | 1.22 ms                                                | 1.12 ms: 1.09x faster                                                 |
| sympy_expand             | 269 ms                                                 | 247 ms: 1.09x faster                                                  |
| nqueens                  | 63.8 ms                                                | 58.5 ms: 1.09x faster                                                 |
| flaskblogging            | 2.65 ms                                                | 2.43 ms: 1.09x faster                                                 |
| genshi_xml               | 33.8 ms                                                | 31.4 ms: 1.08x faster                                                 |
| gunicorn                 | 1.30 ms                                                | 1.21 ms: 1.07x faster                                                 |
| unpickle                 | 8.80 us                                                | 8.29 us: 1.06x faster                                                 |
| pathlib                  | 24.5 ms                                                | 23.1 ms: 1.06x faster                                                 |
| json_dumps               | 8.11 ms                                                | 7.66 ms: 1.06x faster                                                 |
| generators               | 32.3 ms                                                | 30.8 ms: 1.05x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 74.1 ms: 1.05x faster                                                 |
| pickle_list              | 2.74 us                                                | 2.61 us: 1.05x faster                                                 |
| telco                    | 3.49 ms                                                | 3.34 ms: 1.05x faster                                                 |
| xml_etree_iterparse      | 72.1 ms                                                | 69.4 ms: 1.04x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 510 us: 1.03x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 1.40 ms: 1.03x faster                                                 |
| sqlglot_parse            | 1.24 ms                                                | 1.23 ms: 1.01x faster                                                 |
| pidigits                 | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| regex_effbot             | 2.46 ms                                                | 2.45 ms: 1.00x faster                                                 |
| asyncio_tcp              | 659 ms                                                 | 663 ms: 1.01x slower                                                  |
| comprehensions           | 16.9 us                                                | 17.1 us: 1.01x slower                                                 |
| regex_dna                | 174 ms                                                 | 177 ms: 1.01x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.01x slower                                                 |
| unpickle_list            | 2.69 us                                                | 2.74 us: 1.02x slower                                                 |
| pickle_dict              | 17.0 us                                                | 17.3 us: 1.02x slower                                                 |
| regex_v8                 | 17.1 ms                                                | 17.5 ms: 1.02x slower                                                 |
| typing_runtime_protocols | 323 us                                                 | 330 us: 1.02x slower                                                  |
| pickle                   | 6.97 us                                                | 7.21 us: 1.03x slower                                                 |
| mdp                      | 1.63 sec                                               | 1.80 sec: 1.10x slower                                                |
| bench_mp_pool            | 37.4 ms                                                | 42.8 ms: 1.15x slower                                                 |
| python_startup_no_site   | 7.91 ms                                                | 9.28 ms: 1.17x slower                                                 |
| dask                     | 253 ms                                                 | 308 ms: 1.22x slower                                                  |
| python_startup           | 10.9 ms                                                | 14.8 ms: 1.36x slower                                                 |
| unpack_sequence          | 39.0 ns                                                | 93.6 ns: 2.40x slower                                                 |
| coverage                 | 41.5 ms                                                | 328 ms: 7.90x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.12x faster                                                          |
Ignored benchmarks (2) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: asyncio_websockets, mypy2
Ignored benchmarks (4) of results/bm-20220307-3.11.0a6-3ddfa55/bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.10x