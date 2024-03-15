
# Results vs. 3.10.4

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: darwin-arm64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.15x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 178 ms: 1.07x faster                                                   |
| chameleon      | 6.26 ms                                                | 5.19 ms: 1.21x faster                                                  |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                 |
| tornado_http   | 86.7 ms                                                | 71.8 ms: 1.21x faster                                                  |
| Geometric mean | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 256 ms: 1.52x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 332 ms: 1.42x faster                                                   |
| async_tree_io           | 980 ms                                                 | 711 ms: 1.38x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 528 ms: 1.23x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 61.0 ms: 1.13x faster                                                  |
| nbody          | 93.0 ms                                                | 82.4 ms: 1.13x faster                                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 76.9 ms: 1.24x faster                                                  |
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                   |
| regex_v8       | 17.1 ms                                                | 17.7 ms: 1.03x slower                                                  |
| regex_effbot   | 2.46 ms                                                | 2.72 ms: 1.10x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 208 us: 1.35x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.66 ms: 1.22x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 167 us: 1.17x faster                                                   |
| xml_etree_process    | 46.5 ms                                                | 41.2 ms: 1.13x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.61 sec: 1.06x faster                                                 |
| unpickle             | 8.80 us                                                | 9.17 us: 1.04x slower                                                  |
| json_loads           | 16.4 us                                                | 17.2 us: 1.05x slower                                                  |
| pickle_dict          | 17.0 us                                                | 17.9 us: 1.06x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 76.6 ms: 1.06x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.91 us: 1.06x slower                                                  |
| pickle               | 6.97 us                                                | 7.44 us: 1.07x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 58.2 ms: 1.09x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.11 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.1 ms: 1.20x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.6 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.99 ms: 1.24x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 75.0 us: 4.31x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.54 ms: 1.94x faster                                                  |
| raytrace                 | 301 ms                                                 | 183 ms: 1.65x faster                                                   |
| logging_silent           | 117 ns                                                 | 72.8 ns: 1.61x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 416 ms: 1.58x faster                                                   |
| chaos                    | 65.8 ms                                                | 42.0 ms: 1.57x faster                                                  |
| async_tree_none          | 388 ms                                                 | 256 ms: 1.52x faster                                                   |
| richards_super           | 57.8 ms                                                | 39.8 ms: 1.45x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 50.2 ms: 1.43x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 869 us: 1.43x faster                                                   |
| async_tree_memoization   | 474 ms                                                 | 332 ms: 1.42x faster                                                   |
| go                       | 151 ms                                                 | 109 ms: 1.38x faster                                                   |
| async_tree_io            | 980 ms                                                 | 711 ms: 1.38x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 1.05 ms: 1.37x faster                                                  |
| richards                 | 48.7 ms                                                | 35.7 ms: 1.36x faster                                                  |
| pickle_pure_python       | 281 us                                                 | 208 us: 1.35x faster                                                   |
| comprehensions           | 16.9 us                                                | 12.7 us: 1.34x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 26.3 us: 1.32x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 49.8 ms: 1.32x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.71 ms: 1.31x faster                                                  |
| scimark_lu               | 103 ms                                                 | 78.3 ms: 1.31x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 30.3 ns: 1.29x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 76.1 ms: 1.25x faster                                                  |
| regex_compile            | 95.3 ms                                                | 76.9 ms: 1.24x faster                                                  |
| mako                     | 9.87 ms                                                | 7.99 ms: 1.24x faster                                                  |
| generators               | 32.3 ms                                                | 26.2 ms: 1.24x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.30 sec: 1.23x faster                                                 |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 528 ms: 1.23x faster                                                   |
| pyflate                  | 427 ms                                                 | 350 ms: 1.22x faster                                                   |
| create_gc_cycles         | 860 us                                                 | 705 us: 1.22x faster                                                   |
| logging_simple           | 4.45 us                                                | 3.65 us: 1.22x faster                                                  |
| json_dumps               | 8.11 ms                                                | 6.66 ms: 1.22x faster                                                  |
| pycparser                | 877 ms                                                 | 720 ms: 1.22x faster                                                   |
| logging_format           | 4.83 us                                                | 3.99 us: 1.21x faster                                                  |
| tornado_http             | 86.7 ms                                                | 71.8 ms: 1.21x faster                                                  |
| chameleon                | 6.26 ms                                                | 5.19 ms: 1.21x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 76.7 ms: 1.20x faster                                                  |
| pprint_pformat           | 1.30 sec                                               | 1.09 sec: 1.19x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 539 ms: 1.19x faster                                                   |
| scimark_sor              | 128 ms                                                 | 108 ms: 1.18x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 30.2 ms: 1.17x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 11.2 ms: 1.17x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 167 us: 1.17x faster                                                   |
| deepcopy                 | 272 us                                                 | 235 us: 1.16x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.15x faster                                                 |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                   |
| mypy2                    | 607 ms                                                 | 531 ms: 1.14x faster                                                   |
| float                    | 69.0 ms                                                | 61.0 ms: 1.13x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 41.2 ms: 1.13x faster                                                  |
| nbody                    | 93.0 ms                                                | 82.4 ms: 1.13x faster                                                  |
| sympy_str                | 165 ms                                                 | 149 ms: 1.11x faster                                                   |
| deepcopy_reduce          | 2.33 us                                                | 2.11 us: 1.11x faster                                                  |
| dask                     | 253 ms                                                 | 229 ms: 1.10x faster                                                   |
| 2to3                     | 192 ms                                                 | 178 ms: 1.07x faster                                                   |
| coroutines               | 20.7 ms                                                | 19.3 ms: 1.07x faster                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.20 ms: 1.07x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.61 sec: 1.06x faster                                                 |
| scimark_fft              | 224 ms                                                 | 211 ms: 1.06x faster                                                   |
| sympy_expand             | 269 ms                                                 | 257 ms: 1.05x faster                                                   |
| meteor_contest           | 77.7 ms                                                | 74.5 ms: 1.04x faster                                                  |
| fannkuch                 | 303 ms                                                 | 293 ms: 1.03x faster                                                   |
| sqlglot_optimize         | 36.8 ms                                                | 35.8 ms: 1.03x faster                                                  |
| nqueens                  | 63.8 ms                                                | 62.8 ms: 1.02x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 519 us: 1.02x faster                                                   |
| json                     | 3.08 ms                                                | 3.04 ms: 1.01x faster                                                  |
| mdp                      | 1.63 sec                                               | 1.64 sec: 1.01x slower                                                 |
| sqlglot_normalize        | 190 ms                                                 | 193 ms: 1.01x slower                                                   |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                  |
| pathlib                  | 24.5 ms                                                | 24.9 ms: 1.02x slower                                                  |
| regex_v8                 | 17.1 ms                                                | 17.7 ms: 1.03x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.17 us: 1.04x slower                                                  |
| json_loads               | 16.4 us                                                | 17.2 us: 1.05x slower                                                  |
| pickle_dict              | 17.0 us                                                | 17.9 us: 1.06x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 76.6 ms: 1.06x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.91 us: 1.06x slower                                                  |
| pickle                   | 6.97 us                                                | 7.44 us: 1.07x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 58.2 ms: 1.09x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.72 ms: 1.10x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.65 us: 1.13x slower                                                  |
| coverage                 | 41.5 ms                                                | 47.8 ms: 1.15x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.11 us: 1.15x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.1 ms: 1.20x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 45.7 ms: 1.22x slower                                                  |
| async_generators         | 231 ms                                                 | 306 ms: 1.32x slower                                                   |
| telco                    | 3.49 ms                                                | 4.62 ms: 1.32x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.6 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.15x faster                                                           |

Benchmark hidden because not significant (3): xml_etree_parse, asyncio_websockets, pidigits
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-2feec0f-JIT/bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: 1.10x