
# Results vs. 3.10.4

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: darwin-arm64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.09x faster
- HPT reliability: 99.95%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 181 ms: 1.06x faster                                                   |
| chameleon      | 6.26 ms                                                | 5.34 ms: 1.17x faster                                                  |
| docutils       | 1.73 sec                                               | 1.56 sec: 1.11x faster                                                 |
| tornado_http   | 86.7 ms                                                | 74.9 ms: 1.16x faster                                                  |
| Geometric mean | (ref)                                                  | 1.13x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 264 ms: 1.47x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 341 ms: 1.39x faster                                                   |
| async_tree_io           | 980 ms                                                 | 722 ms: 1.36x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 536 ms: 1.21x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 90.1 ms: 1.03x faster                                                  |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| float          | 69.0 ms                                                | 70.9 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 153 ms: 1.14x faster                                                   |
| regex_compile  | 95.3 ms                                                | 87.5 ms: 1.09x faster                                                  |
| regex_v8       | 17.1 ms                                                | 17.8 ms: 1.04x slower                                                  |
| regex_effbot   | 2.46 ms                                                | 2.72 ms: 1.10x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 206 us: 1.36x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.69 ms: 1.21x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 174 us: 1.12x faster                                                   |
| xml_etree_process    | 46.5 ms                                                | 42.7 ms: 1.09x faster                                                  |
| xml_etree_parse      | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| tomli_loads          | 1.71 sec                                               | 1.70 sec: 1.00x faster                                                 |
| unpickle             | 8.80 us                                                | 9.16 us: 1.04x slower                                                  |
| json_loads           | 16.4 us                                                | 17.3 us: 1.05x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.0 us: 1.06x slower                                                  |
| pickle               | 6.97 us                                                | 7.46 us: 1.07x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.94 us: 1.07x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 81.1 ms: 1.12x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 62.3 ms: 1.16x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.2 ms: 1.21x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.7 ms: 1.48x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.34x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.93 ms: 1.01x slower                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 78.1 us: 4.13x faster                                                  |
| logging_silent           | 117 ns                                                 | 75.0 ns: 1.56x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 432 ms: 1.53x faster                                                   |
| raytrace                 | 301 ms                                                 | 199 ms: 1.51x faster                                                   |
| richards_super           | 57.8 ms                                                | 38.5 ms: 1.50x faster                                                  |
| async_tree_none          | 388 ms                                                 | 264 ms: 1.47x faster                                                   |
| richards                 | 48.7 ms                                                | 34.6 ms: 1.41x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 886 us: 1.40x faster                                                   |
| async_tree_memoization   | 474 ms                                                 | 341 ms: 1.39x faster                                                   |
| chaos                    | 65.8 ms                                                | 48.2 ms: 1.36x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 206 us: 1.36x faster                                                   |
| async_tree_io            | 980 ms                                                 | 722 ms: 1.36x faster                                                   |
| unpack_sequence          | 39.0 ns                                                | 28.9 ns: 1.35x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 1.08 ms: 1.34x faster                                                  |
| deltablue                | 4.91 ms                                                | 3.68 ms: 1.34x faster                                                  |
| go                       | 151 ms                                                 | 115 ms: 1.31x faster                                                   |
| scimark_lu               | 103 ms                                                 | 78.7 ms: 1.31x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 55.9 ms: 1.29x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 27.3 us: 1.27x faster                                                  |
| generators               | 32.3 ms                                                | 25.6 ms: 1.26x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.23x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 704 us: 1.22x faster                                                   |
| pycparser                | 877 ms                                                 | 721 ms: 1.22x faster                                                   |
| json_dumps               | 8.11 ms                                                | 6.69 ms: 1.21x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 536 ms: 1.21x faster                                                   |
| logging_format           | 4.83 us                                                | 4.02 us: 1.20x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.72 us: 1.19x faster                                                  |
| chameleon                | 6.26 ms                                                | 5.34 ms: 1.17x faster                                                  |
| scimark_sor              | 128 ms                                                 | 110 ms: 1.17x faster                                                   |
| tornado_http             | 86.7 ms                                                | 74.9 ms: 1.16x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 30.6 ms: 1.15x faster                                                  |
| deepcopy                 | 272 us                                                 | 239 us: 1.14x faster                                                   |
| regex_dna                | 174 ms                                                 | 153 ms: 1.14x faster                                                   |
| pyflate                  | 427 ms                                                 | 377 ms: 1.13x faster                                                   |
| unpickle_pure_python     | 194 us                                                 | 174 us: 1.12x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.56 sec: 1.11x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 59.3 ms: 1.11x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 83.4 ms: 1.10x faster                                                  |
| coroutines               | 20.7 ms                                                | 18.8 ms: 1.10x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 2.12 us: 1.10x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 42.7 ms: 1.09x faster                                                  |
| regex_compile            | 95.3 ms                                                | 87.5 ms: 1.09x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 12.1 ms: 1.08x faster                                                  |
| dask                     | 253 ms                                                 | 234 ms: 1.08x faster                                                   |
| pprint_safe_repr         | 641 ms                                                 | 594 ms: 1.08x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.22 sec: 1.07x faster                                                 |
| 2to3                     | 192 ms                                                 | 181 ms: 1.06x faster                                                   |
| sympy_str                | 165 ms                                                 | 158 ms: 1.05x faster                                                   |
| comprehensions           | 16.9 us                                                | 16.3 us: 1.04x faster                                                  |
| nbody                    | 93.0 ms                                                | 90.1 ms: 1.03x faster                                                  |
| sympy_expand             | 269 ms                                                 | 262 ms: 1.03x faster                                                   |
| json                     | 3.08 ms                                                | 3.01 ms: 1.03x faster                                                  |
| hexiom                   | 6.19 ms                                                | 6.08 ms: 1.02x faster                                                  |
| xml_etree_parse          | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| tomli_loads              | 1.71 sec                                               | 1.70 sec: 1.00x faster                                                 |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                   |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| bench_thread_pool        | 527 us                                                 | 530 us: 1.01x slower                                                   |
| mako                     | 9.87 ms                                                | 9.93 ms: 1.01x slower                                                  |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                  |
| float                    | 69.0 ms                                                | 70.9 ms: 1.03x slower                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 37.8 ms: 1.03x slower                                                  |
| pathlib                  | 24.5 ms                                                | 25.2 ms: 1.03x slower                                                  |
| meteor_contest           | 77.7 ms                                                | 80.3 ms: 1.03x slower                                                  |
| regex_v8                 | 17.1 ms                                                | 17.8 ms: 1.04x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.16 us: 1.04x slower                                                  |
| mdp                      | 1.63 sec                                               | 1.71 sec: 1.05x slower                                                 |
| json_loads               | 16.4 us                                                | 17.3 us: 1.05x slower                                                  |
| sqlglot_normalize        | 190 ms                                                 | 200 ms: 1.05x slower                                                   |
| pickle_dict              | 17.0 us                                                | 18.0 us: 1.06x slower                                                  |
| pickle                   | 6.97 us                                                | 7.46 us: 1.07x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.94 us: 1.07x slower                                                  |
| nqueens                  | 63.8 ms                                                | 69.7 ms: 1.09x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.72 ms: 1.10x slower                                                  |
| spectral_norm            | 94.8 ms                                                | 106 ms: 1.12x slower                                                   |
| xml_etree_iterparse      | 72.1 ms                                                | 81.1 ms: 1.12x slower                                                  |
| fannkuch                 | 303 ms                                                 | 341 ms: 1.13x slower                                                   |
| scimark_fft              | 224 ms                                                 | 253 ms: 1.13x slower                                                   |
| xml_etree_generate       | 53.5 ms                                                | 62.3 ms: 1.16x slower                                                  |
| coverage                 | 41.5 ms                                                | 48.4 ms: 1.17x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.72 us: 1.18x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.2 ms: 1.21x slower                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 4.21 ms: 1.23x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 46.1 ms: 1.23x slower                                                  |
| async_generators         | 231 ms                                                 | 309 ms: 1.33x slower                                                   |
| telco                    | 3.49 ms                                                | 4.83 ms: 1.39x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.7 ms: 1.48x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.09x faster                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.95% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.10x