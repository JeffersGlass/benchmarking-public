
# Results vs. 3.10.4

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: darwin-arm64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.16x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 175 ms: 1.10x faster                                                   |
| chameleon      | 6.26 ms                                                | 5.13 ms: 1.22x faster                                                  |
| docutils       | 1.73 sec                                               | 1.50 sec: 1.16x faster                                                 |
| tornado_http   | 86.7 ms                                                | 71.9 ms: 1.21x faster                                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 256 ms: 1.52x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 331 ms: 1.43x faster                                                   |
| async_tree_io           | 980 ms                                                 | 706 ms: 1.39x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 526 ms: 1.23x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.39x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 58.0 ms: 1.19x faster                                                  |
| nbody          | 93.0 ms                                                | 82.1 ms: 1.13x faster                                                  |
| Geometric mean | (ref)                                                  | 1.10x faster                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 79.3 ms: 1.20x faster                                                  |
| regex_dna      | 174 ms                                                 | 149 ms: 1.17x faster                                                   |
| regex_v8       | 17.1 ms                                                | 16.9 ms: 1.01x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.57 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 208 us: 1.35x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.59 ms: 1.23x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 165 us: 1.18x faster                                                   |
| xml_etree_process    | 46.5 ms                                                | 40.7 ms: 1.14x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.61 sec: 1.06x faster                                                 |
| unpickle             | 8.80 us                                                | 9.07 us: 1.03x slower                                                  |
| json_loads           | 16.4 us                                                | 17.2 us: 1.05x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.88 us: 1.05x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 76.1 ms: 1.05x slower                                                  |
| pickle_dict          | 17.0 us                                                | 17.9 us: 1.06x slower                                                  |
| pickle               | 6.97 us                                                | 7.47 us: 1.07x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 58.4 ms: 1.09x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.14 us: 1.17x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.2 ms: 1.21x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.34x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.78 ms: 1.27x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 77.5 us: 4.17x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.45 ms: 2.01x faster                                                  |
| logging_silent           | 117 ns                                                 | 71.0 ns: 1.65x faster                                                  |
| raytrace                 | 301 ms                                                 | 184 ms: 1.64x faster                                                   |
| asyncio_tcp              | 659 ms                                                 | 412 ms: 1.60x faster                                                   |
| chaos                    | 65.8 ms                                                | 43.2 ms: 1.52x faster                                                  |
| async_tree_none          | 388 ms                                                 | 256 ms: 1.52x faster                                                   |
| sqlglot_parse            | 1.24 ms                                                | 829 us: 1.50x faster                                                   |
| richards_super           | 57.8 ms                                                | 38.9 ms: 1.49x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 48.9 ms: 1.47x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 331 ms: 1.43x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.01 ms: 1.43x faster                                                  |
| go                       | 151 ms                                                 | 106 ms: 1.42x faster                                                   |
| async_tree_io            | 980 ms                                                 | 706 ms: 1.39x faster                                                   |
| richards                 | 48.7 ms                                                | 35.2 ms: 1.38x faster                                                  |
| scimark_lu               | 103 ms                                                 | 75.9 ms: 1.36x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 48.5 ms: 1.35x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 208 us: 1.35x faster                                                   |
| unpack_sequence          | 39.0 ns                                                | 29.0 ns: 1.34x faster                                                  |
| comprehensions           | 16.9 us                                                | 12.7 us: 1.34x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 26.0 us: 1.34x faster                                                  |
| mako                     | 9.87 ms                                                | 7.78 ms: 1.27x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 75.1 ms: 1.26x faster                                                  |
| pyflate                  | 427 ms                                                 | 344 ms: 1.24x faster                                                   |
| generators               | 32.3 ms                                                | 26.1 ms: 1.24x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 526 ms: 1.23x faster                                                   |
| pycparser                | 877 ms                                                 | 710 ms: 1.23x faster                                                   |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                                 |
| hexiom                   | 6.19 ms                                                | 5.02 ms: 1.23x faster                                                  |
| json_dumps               | 8.11 ms                                                | 6.59 ms: 1.23x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.63 us: 1.23x faster                                                  |
| logging_format           | 4.83 us                                                | 3.95 us: 1.22x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 703 us: 1.22x faster                                                   |
| chameleon                | 6.26 ms                                                | 5.13 ms: 1.22x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 75.9 ms: 1.21x faster                                                  |
| tornado_http             | 86.7 ms                                                | 71.9 ms: 1.21x faster                                                  |
| regex_compile            | 95.3 ms                                                | 79.3 ms: 1.20x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.09 sec: 1.20x faster                                                 |
| scimark_sor              | 128 ms                                                 | 107 ms: 1.20x faster                                                   |
| pprint_safe_repr         | 641 ms                                                 | 536 ms: 1.20x faster                                                   |
| float                    | 69.0 ms                                                | 58.0 ms: 1.19x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 165 us: 1.18x faster                                                   |
| sympy_integrate          | 13.1 ms                                                | 11.2 ms: 1.17x faster                                                  |
| regex_dna                | 174 ms                                                 | 149 ms: 1.17x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 30.2 ms: 1.17x faster                                                  |
| deepcopy                 | 272 us                                                 | 232 us: 1.17x faster                                                   |
| mypy2                    | 607 ms                                                 | 525 ms: 1.16x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.50 sec: 1.16x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 40.7 ms: 1.14x faster                                                  |
| nbody                    | 93.0 ms                                                | 82.1 ms: 1.13x faster                                                  |
| sympy_str                | 165 ms                                                 | 147 ms: 1.13x faster                                                   |
| deepcopy_reduce          | 2.33 us                                                | 2.07 us: 1.12x faster                                                  |
| dask                     | 253 ms                                                 | 229 ms: 1.10x faster                                                   |
| 2to3                     | 192 ms                                                 | 175 ms: 1.10x faster                                                   |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.17 ms: 1.08x faster                                                  |
| coroutines               | 20.7 ms                                                | 19.3 ms: 1.07x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.61 sec: 1.06x faster                                                 |
| sympy_expand             | 269 ms                                                 | 254 ms: 1.06x faster                                                   |
| scimark_fft              | 224 ms                                                 | 212 ms: 1.06x faster                                                   |
| fannkuch                 | 303 ms                                                 | 289 ms: 1.05x faster                                                   |
| meteor_contest           | 77.7 ms                                                | 75.3 ms: 1.03x faster                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 35.8 ms: 1.03x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 516 us: 1.02x faster                                                   |
| regex_v8                 | 17.1 ms                                                | 16.9 ms: 1.01x faster                                                  |
| json                     | 3.08 ms                                                | 3.04 ms: 1.01x faster                                                  |
| nqueens                  | 63.8 ms                                                | 63.0 ms: 1.01x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 192 ms: 1.01x slower                                                   |
| mdp                      | 1.63 sec                                               | 1.66 sec: 1.02x slower                                                 |
| unpickle                 | 8.80 us                                                | 9.07 us: 1.03x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.57 ms: 1.04x slower                                                  |
| json_loads               | 16.4 us                                                | 17.2 us: 1.05x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.88 us: 1.05x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 76.1 ms: 1.05x slower                                                  |
| pickle_dict              | 17.0 us                                                | 17.9 us: 1.06x slower                                                  |
| pickle                   | 6.97 us                                                | 7.47 us: 1.07x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.54 ms: 1.07x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 58.4 ms: 1.09x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.65 us: 1.13x slower                                                  |
| coverage                 | 41.5 ms                                                | 48.0 ms: 1.16x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.14 us: 1.17x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.2 ms: 1.21x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 45.3 ms: 1.21x slower                                                  |
| async_generators         | 231 ms                                                 | 305 ms: 1.32x slower                                                   |
| telco                    | 3.49 ms                                                | 4.72 ms: 1.35x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.16x faster                                                           |

Benchmark hidden because not significant (4): asyncio_websockets, pidigits, xml_etree_parse, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: 1.10x