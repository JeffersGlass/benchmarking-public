
# Results vs. 3.10.4

- fork: python
- ref: v3.12.2
- machine: darwin-arm64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 168 ms: 1.14x faster                                   |
| chameleon      | 6.26 ms                                                | 4.68 ms: 1.34x faster                                  |
| docutils       | 1.73 sec                                               | 1.49 sec: 1.16x faster                                 |
| tornado_http   | 86.7 ms                                                | 70.1 ms: 1.24x faster                                  |
| Geometric mean | (ref)                                                  | 1.22x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 474 ms                                                 | 311 ms: 1.52x faster                                   |
| async_tree_io           | 980 ms                                                 | 665 ms: 1.47x faster                                   |
| async_tree_none         | 388 ms                                                 | 264 ms: 1.47x faster                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 525 ms: 1.24x faster                                   |
| Geometric mean          | (ref)                                                  | 1.42x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 68.5 ms: 1.36x faster                                  |
| float          | 69.0 ms                                                | 56.0 ms: 1.23x faster                                  |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.19x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 75.8 ms: 1.26x faster                                  |
| regex_dna      | 174 ms                                                 | 158 ms: 1.11x faster                                   |
| regex_v8       | 17.1 ms                                                | 16.9 ms: 1.02x faster                                  |
| regex_effbot   | 2.46 ms                                                | 2.83 ms: 1.15x slower                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 200 us: 1.40x faster                                   |
| unpickle_pure_python | 194 us                                                 | 149 us: 1.30x faster                                   |
| json_dumps           | 8.11 ms                                                | 6.24 ms: 1.30x faster                                  |
| tomli_loads          | 1.71 sec                                               | 1.39 sec: 1.23x faster                                 |
| xml_etree_process    | 46.5 ms                                                | 39.3 ms: 1.18x faster                                  |
| xml_etree_parse      | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| xml_etree_iterparse  | 72.1 ms                                                | 73.8 ms: 1.02x slower                                  |
| xml_etree_generate   | 53.5 ms                                                | 55.4 ms: 1.04x slower                                  |
| unpickle             | 8.80 us                                                | 9.13 us: 1.04x slower                                  |
| json_loads           | 16.4 us                                                | 17.1 us: 1.04x slower                                  |
| pickle               | 6.97 us                                                | 7.28 us: 1.04x slower                                  |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                  |
| pickle_list          | 2.74 us                                                | 2.93 us: 1.07x slower                                  |
| unpickle_list        | 2.69 us                                                | 3.08 us: 1.14x slower                                  |
| Geometric mean       | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.1 ms: 1.12x slower                                  |
| python_startup_no_site | 7.91 ms                                                | 10.1 ms: 1.28x slower                                  |
| Geometric mean         | (ref)                                                  | 1.20x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.73 ms: 1.28x faster                                  |
| django_template | 26.4 ms                                                | 22.4 ms: 1.18x faster                                  |
| Geometric mean  | (ref)                                                  | 1.23x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 74.1 us: 4.36x faster                                  |
| deltablue                | 4.91 ms                                                | 2.71 ms: 1.81x faster                                  |
| richards_super           | 57.8 ms                                                | 36.4 ms: 1.59x faster                                  |
| asyncio_tcp              | 659 ms                                                 | 418 ms: 1.58x faster                                   |
| chaos                    | 65.8 ms                                                | 42.9 ms: 1.53x faster                                  |
| logging_silent           | 117 ns                                                 | 77.0 ns: 1.52x faster                                  |
| async_tree_memoization   | 474 ms                                                 | 311 ms: 1.52x faster                                   |
| richards                 | 48.7 ms                                                | 32.5 ms: 1.50x faster                                  |
| go                       | 151 ms                                                 | 102 ms: 1.48x faster                                   |
| async_tree_io            | 980 ms                                                 | 665 ms: 1.47x faster                                   |
| async_tree_none          | 388 ms                                                 | 264 ms: 1.47x faster                                   |
| sqlglot_parse            | 1.24 ms                                                | 847 us: 1.47x faster                                   |
| scimark_sor              | 128 ms                                                 | 88.1 ms: 1.46x faster                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 45.1 ms: 1.45x faster                                  |
| raytrace                 | 301 ms                                                 | 212 ms: 1.42x faster                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.02 ms: 1.41x faster                                  |
| pickle_pure_python       | 281 us                                                 | 200 us: 1.40x faster                                   |
| crypto_pyaes             | 71.8 ms                                                | 51.8 ms: 1.39x faster                                  |
| hexiom                   | 6.19 ms                                                | 4.51 ms: 1.37x faster                                  |
| nbody                    | 93.0 ms                                                | 68.5 ms: 1.36x faster                                  |
| scimark_lu               | 103 ms                                                 | 76.0 ms: 1.35x faster                                  |
| pyflate                  | 427 ms                                                 | 316 ms: 1.35x faster                                   |
| chameleon                | 6.26 ms                                                | 4.68 ms: 1.34x faster                                  |
| sqlalchemy_imperative    | 8.86 ms                                                | 6.65 ms: 1.33x faster                                  |
| unpickle_pure_python     | 194 us                                                 | 149 us: 1.30x faster                                   |
| pycparser                | 877 ms                                                 | 674 ms: 1.30x faster                                   |
| json_dumps               | 8.11 ms                                                | 6.24 ms: 1.30x faster                                  |
| mypy2                    | 607 ms                                                 | 470 ms: 1.29x faster                                   |
| pprint_safe_repr         | 641 ms                                                 | 499 ms: 1.28x faster                                   |
| pprint_pformat           | 1.30 sec                                               | 1.02 sec: 1.28x faster                                 |
| mako                     | 9.87 ms                                                | 7.73 ms: 1.28x faster                                  |
| regex_compile            | 95.3 ms                                                | 75.8 ms: 1.26x faster                                  |
| deepcopy_memo            | 34.7 us                                                | 27.9 us: 1.25x faster                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 525 ms: 1.24x faster                                   |
| tornado_http             | 86.7 ms                                                | 70.1 ms: 1.24x faster                                  |
| create_gc_cycles         | 860 us                                                 | 696 us: 1.24x faster                                   |
| spectral_norm            | 94.8 ms                                                | 76.8 ms: 1.23x faster                                  |
| float                    | 69.0 ms                                                | 56.0 ms: 1.23x faster                                  |
| tomli_loads              | 1.71 sec                                               | 1.39 sec: 1.23x faster                                 |
| unpack_sequence          | 39.0 ns                                                | 31.9 ns: 1.22x faster                                  |
| fannkuch                 | 303 ms                                                 | 248 ms: 1.22x faster                                   |
| logging_format           | 4.83 us                                                | 4.00 us: 1.21x faster                                  |
| logging_simple           | 4.45 us                                                | 3.69 us: 1.20x faster                                  |
| sympy_sum                | 92.2 ms                                                | 76.6 ms: 1.20x faster                                  |
| dulwich_log              | 35.3 ms                                                | 29.4 ms: 1.20x faster                                  |
| xml_etree_process        | 46.5 ms                                                | 39.3 ms: 1.18x faster                                  |
| django_template          | 26.4 ms                                                | 22.4 ms: 1.18x faster                                  |
| sqlalchemy_declarative   | 73.3 ms                                                | 62.2 ms: 1.18x faster                                  |
| comprehensions           | 16.9 us                                                | 14.4 us: 1.18x faster                                  |
| sympy_integrate          | 13.1 ms                                                | 11.2 ms: 1.17x faster                                  |
| deepcopy                 | 272 us                                                 | 233 us: 1.17x faster                                   |
| docutils                 | 1.73 sec                                               | 1.49 sec: 1.16x faster                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.39 sec: 1.16x faster                                 |
| dask                     | 253 ms                                                 | 220 ms: 1.15x faster                                   |
| scimark_fft              | 224 ms                                                 | 196 ms: 1.14x faster                                   |
| 2to3                     | 192 ms                                                 | 168 ms: 1.14x faster                                   |
| sympy_str                | 165 ms                                                 | 146 ms: 1.13x faster                                   |
| deepcopy_reduce          | 2.33 us                                                | 2.08 us: 1.12x faster                                  |
| sympy_expand             | 269 ms                                                 | 240 ms: 1.12x faster                                   |
| regex_dna                | 174 ms                                                 | 158 ms: 1.11x faster                                   |
| aiohttp                  | 1.22 ms                                                | 1.11 ms: 1.10x faster                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.14 ms: 1.09x faster                                  |
| coroutines               | 20.7 ms                                                | 19.1 ms: 1.08x faster                                  |
| gunicorn                 | 1.30 ms                                                | 1.20 ms: 1.08x faster                                  |
| meteor_contest           | 77.7 ms                                                | 72.0 ms: 1.08x faster                                  |
| sqlglot_optimize         | 36.8 ms                                                | 34.1 ms: 1.08x faster                                  |
| coverage                 | 41.5 ms                                                | 38.6 ms: 1.07x faster                                  |
| bench_thread_pool        | 527 us                                                 | 498 us: 1.06x faster                                   |
| generators               | 32.3 ms                                                | 31.3 ms: 1.03x faster                                  |
| nqueens                  | 63.8 ms                                                | 61.9 ms: 1.03x faster                                  |
| mdp                      | 1.63 sec                                               | 1.58 sec: 1.03x faster                                 |
| sqlglot_normalize        | 190 ms                                                 | 186 ms: 1.02x faster                                   |
| pathlib                  | 24.5 ms                                                | 24.1 ms: 1.02x faster                                  |
| regex_v8                 | 17.1 ms                                                | 16.9 ms: 1.02x faster                                  |
| xml_etree_parse          | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| json                     | 3.08 ms                                                | 3.04 ms: 1.01x faster                                  |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                   |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x faster                                   |
| gc_traversal             | 2.36 ms                                                | 2.39 ms: 1.01x slower                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 73.8 ms: 1.02x slower                                  |
| xml_etree_generate       | 53.5 ms                                                | 55.4 ms: 1.04x slower                                  |
| unpickle                 | 8.80 us                                                | 9.13 us: 1.04x slower                                  |
| json_loads               | 16.4 us                                                | 17.1 us: 1.04x slower                                  |
| pickle                   | 6.97 us                                                | 7.28 us: 1.04x slower                                  |
| telco                    | 3.49 ms                                                | 3.69 ms: 1.06x slower                                  |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                  |
| pickle_list              | 2.74 us                                                | 2.93 us: 1.07x slower                                  |
| sqlite_synth             | 1.46 us                                                | 1.58 us: 1.08x slower                                  |
| python_startup           | 10.9 ms                                                | 12.1 ms: 1.12x slower                                  |
| unpickle_list            | 2.69 us                                                | 3.08 us: 1.14x slower                                  |
| regex_effbot             | 2.46 ms                                                | 2.83 ms: 1.15x slower                                  |
| bench_mp_pool            | 37.4 ms                                                | 44.5 ms: 1.19x slower                                  |
| python_startup_no_site   | 7.91 ms                                                | 10.1 ms: 1.28x slower                                  |
| async_generators         | 231 ms                                                 | 300 ms: 1.30x slower                                   |
| Geometric mean           | (ref)                                                  | 1.19x faster                                           |
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20240206-3.12.2-6abddd9/bm-20240206-darwin-arm64-python-v3.12.2-3.12.2-6abddd9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.08x