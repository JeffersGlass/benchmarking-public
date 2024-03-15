# Results vs. 3.10.4

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: darwin-arm64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 2.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 187 ms: 1.02x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.84 ms: 1.29x faster                                                  |
| docutils       | 1.73 sec                                               | 1.51 sec: 1.14x faster                                                 |
| tornado_http   | 86.7 ms                                                | 69.9 ms: 1.24x faster                                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 252 ms: 1.54x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 328 ms: 1.44x faster                                                   |
| async_tree_io           | 980 ms                                                 | 701 ms: 1.40x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 520 ms: 1.25x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.40x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 70.0 ms: 1.33x faster                                                  |
| float          | 69.0 ms                                                | 52.9 ms: 1.30x faster                                                  |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.20x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 145 ms: 1.20x faster                                                   |
| regex_compile  | 95.3 ms                                                | 87.1 ms: 1.09x faster                                                  |
| regex_v8       | 17.1 ms                                                | 17.1 ms: 1.00x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.58 ms: 1.05x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                   |
| unpickle_pure_python | 194 us                                                 | 152 us: 1.28x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.56 ms: 1.24x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.39 sec: 1.23x faster                                                 |
| xml_etree_process    | 46.5 ms                                                | 40.0 ms: 1.16x faster                                                  |
| json_loads           | 16.4 us                                                | 16.9 us: 1.03x slower                                                  |
| pickle               | 6.97 us                                                | 7.27 us: 1.04x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 75.4 ms: 1.04x slower                                                  |
| unpickle             | 8.80 us                                                | 9.19 us: 1.04x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 56.7 ms: 1.06x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.91 us: 1.06x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 17.7 ms: 1.63x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 16.4 ms: 2.08x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.84x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 6.83 ms: 1.45x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.8 us: 4.50x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.55 ms: 1.93x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 399 ms: 1.65x faster                                                   |
| chaos                    | 65.8 ms                                                | 40.3 ms: 1.63x faster                                                  |
| logging_silent           | 117 ns                                                 | 72.5 ns: 1.62x faster                                                  |
| raytrace                 | 301 ms                                                 | 191 ms: 1.58x faster                                                   |
| async_tree_none          | 388 ms                                                 | 252 ms: 1.54x faster                                                   |
| crypto_pyaes             | 71.8 ms                                                | 47.3 ms: 1.52x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 834 us: 1.49x faster                                                   |
| mako                     | 9.87 ms                                                | 6.83 ms: 1.45x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 328 ms: 1.44x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 46.1 ms: 1.42x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 1.03 ms: 1.41x faster                                                  |
| async_tree_io            | 980 ms                                                 | 701 ms: 1.40x faster                                                   |
| richards_super           | 57.8 ms                                                | 43.4 ms: 1.33x faster                                                  |
| nbody                    | 93.0 ms                                                | 70.0 ms: 1.33x faster                                                  |
| comprehensions           | 16.9 us                                                | 12.9 us: 1.32x faster                                                  |
| float                    | 69.0 ms                                                | 52.9 ms: 1.30x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 26.6 us: 1.30x faster                                                  |
| go                       | 151 ms                                                 | 116 ms: 1.30x faster                                                   |
| chameleon                | 6.26 ms                                                | 4.84 ms: 1.29x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 152 us: 1.28x faster                                                   |
| logging_format           | 4.83 us                                                | 3.77 us: 1.28x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.49 us: 1.28x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 520 ms: 1.25x faster                                                   |
| tornado_http             | 86.7 ms                                                | 69.9 ms: 1.24x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 517 ms: 1.24x faster                                                   |
| json_dumps               | 8.11 ms                                                | 6.56 ms: 1.24x faster                                                  |
| pyflate                  | 427 ms                                                 | 346 ms: 1.23x faster                                                   |
| tomli_loads              | 1.71 sec                                               | 1.39 sec: 1.23x faster                                                 |
| pprint_pformat           | 1.30 sec                                               | 1.06 sec: 1.23x faster                                                 |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.32 sec: 1.22x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 713 us: 1.21x faster                                                   |
| pycparser                | 877 ms                                                 | 727 ms: 1.21x faster                                                   |
| richards                 | 48.7 ms                                                | 40.4 ms: 1.21x faster                                                  |
| regex_dna                | 174 ms                                                 | 145 ms: 1.20x faster                                                   |
| scimark_lu               | 103 ms                                                 | 85.6 ms: 1.20x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 77.1 ms: 1.20x faster                                                  |
| deepcopy                 | 272 us                                                 | 231 us: 1.18x faster                                                   |
| deepcopy_reduce          | 2.33 us                                                | 2.00 us: 1.17x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 40.0 ms: 1.16x faster                                                  |
| hexiom                   | 6.19 ms                                                | 5.33 ms: 1.16x faster                                                  |
| spectral_norm            | 94.8 ms                                                | 81.7 ms: 1.16x faster                                                  |
| dulwich_log              | 35.3 ms                                                | 30.9 ms: 1.15x faster                                                  |
| docutils                 | 1.73 sec                                               | 1.51 sec: 1.14x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                                  |
| sympy_str                | 165 ms                                                 | 145 ms: 1.14x faster                                                   |
| generators               | 32.3 ms                                                | 28.5 ms: 1.14x faster                                                  |
| scimark_fft              | 224 ms                                                 | 199 ms: 1.13x faster                                                   |
| scimark_sor              | 128 ms                                                 | 115 ms: 1.12x faster                                                   |
| coroutines               | 20.7 ms                                                | 18.7 ms: 1.10x faster                                                  |
| regex_compile            | 95.3 ms                                                | 87.1 ms: 1.09x faster                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.14 ms: 1.09x faster                                                  |
| sympy_expand             | 269 ms                                                 | 248 ms: 1.09x faster                                                   |
| meteor_contest           | 77.7 ms                                                | 74.1 ms: 1.05x faster                                                  |
| json                     | 3.08 ms                                                | 2.97 ms: 1.04x faster                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 35.5 ms: 1.04x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 184 ms: 1.03x faster                                                   |
| bench_thread_pool        | 527 us                                                 | 514 us: 1.03x faster                                                   |
| 2to3                     | 192 ms                                                 | 187 ms: 1.02x faster                                                   |
| asyncio_websockets       | 410 ms                                                 | 408 ms: 1.00x faster                                                   |
| regex_v8                 | 17.1 ms                                                | 17.1 ms: 1.00x faster                                                  |
| pidigits                 | 282 ms                                                 | 282 ms: 1.00x faster                                                   |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                  |
| json_loads               | 16.4 us                                                | 16.9 us: 1.03x slower                                                  |
| pathlib                  | 24.5 ms                                                | 25.4 ms: 1.04x slower                                                  |
| pickle                   | 6.97 us                                                | 7.27 us: 1.04x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 75.4 ms: 1.04x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.19 us: 1.04x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.58 ms: 1.05x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 56.7 ms: 1.06x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.91 us: 1.06x slower                                                  |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| fannkuch                 | 303 ms                                                 | 325 ms: 1.07x slower                                                   |
| sqlite_synth             | 1.46 us                                                | 1.61 us: 1.10x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| coverage                 | 41.5 ms                                                | 47.7 ms: 1.15x slower                                                  |
| telco                    | 3.49 ms                                                | 4.48 ms: 1.29x slower                                                  |
| async_generators         | 231 ms                                                 | 311 ms: 1.35x slower                                                   |
| bench_mp_pool            | 37.4 ms                                                | 52.2 ms: 1.40x slower                                                  |
| python_startup           | 10.9 ms                                                | 17.7 ms: 1.63x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 16.4 ms: 2.08x slower                                                  |
| unpack_sequence          | 39.0 ns                                                | 114 ns: 2.91x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.14x faster                                                           |

Benchmark hidden because not significant (4): mypy2, xml_etree_parse, nqueens, mdp
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-f0df35e-JIT/bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 2.07x