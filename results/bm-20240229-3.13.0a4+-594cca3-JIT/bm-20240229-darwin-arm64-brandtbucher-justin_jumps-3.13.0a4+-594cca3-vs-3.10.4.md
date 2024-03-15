# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_jumps
- machine: darwin-arm64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: 2.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 188 ms: 1.02x faster                                                 |
| chameleon      | 6.26 ms                                                | 4.85 ms: 1.29x faster                                                |
| docutils       | 1.73 sec                                               | 1.53 sec: 1.14x faster                                               |
| tornado_http   | 86.7 ms                                                | 70.3 ms: 1.23x faster                                                |
| Geometric mean | (ref)                                                  | 1.17x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 251 ms: 1.55x faster                                                 |
| async_tree_memoization  | 474 ms                                                 | 327 ms: 1.45x faster                                                 |
| async_tree_io           | 980 ms                                                 | 701 ms: 1.40x faster                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 521 ms: 1.25x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.41x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 70.6 ms: 1.32x faster                                                |
| float          | 69.0 ms                                                | 53.0 ms: 1.30x faster                                                |
| Geometric mean | (ref)                                                  | 1.20x faster                                                         |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 174 ms                                                 | 152 ms: 1.14x faster                                                 |
| regex_compile  | 95.3 ms                                                | 86.7 ms: 1.10x faster                                                |
| regex_v8       | 17.1 ms                                                | 17.2 ms: 1.00x slower                                                |
| regex_effbot   | 2.46 ms                                                | 2.63 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                  | 1.04x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.43x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 152 us: 1.28x faster                                                 |
| json_dumps           | 8.11 ms                                                | 6.54 ms: 1.24x faster                                                |
| tomli_loads          | 1.71 sec                                               | 1.38 sec: 1.24x faster                                               |
| xml_etree_process    | 46.5 ms                                                | 39.0 ms: 1.19x faster                                                |
| json_loads           | 16.4 us                                                | 16.9 us: 1.03x slower                                                |
| xml_etree_iterparse  | 72.1 ms                                                | 75.0 ms: 1.04x slower                                                |
| pickle               | 6.97 us                                                | 7.25 us: 1.04x slower                                                |
| unpickle             | 8.80 us                                                | 9.15 us: 1.04x slower                                                |
| pickle_dict          | 17.0 us                                                | 18.3 us: 1.08x slower                                                |
| pickle_list          | 2.74 us                                                | 2.96 us: 1.08x slower                                                |
| xml_etree_generate   | 53.5 ms                                                | 57.8 ms: 1.08x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                         |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 17.3 ms: 1.59x slower                                                |
| python_startup_no_site | 7.91 ms                                                | 15.9 ms: 2.01x slower                                                |
| Geometric mean         | (ref)                                                  | 1.79x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 6.85 ms: 1.44x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 72.1 us: 4.48x faster                                                |
| deltablue                | 4.91 ms                                                | 2.54 ms: 1.93x faster                                                |
| chaos                    | 65.8 ms                                                | 40.4 ms: 1.63x faster                                                |
| asyncio_tcp              | 659 ms                                                 | 407 ms: 1.62x faster                                                 |
| logging_silent           | 117 ns                                                 | 72.6 ns: 1.61x faster                                                |
| raytrace                 | 301 ms                                                 | 192 ms: 1.57x faster                                                 |
| async_tree_none          | 388 ms                                                 | 251 ms: 1.55x faster                                                 |
| crypto_pyaes             | 71.8 ms                                                | 47.4 ms: 1.52x faster                                                |
| sqlglot_parse            | 1.24 ms                                                | 836 us: 1.49x faster                                                 |
| async_tree_memoization   | 474 ms                                                 | 327 ms: 1.45x faster                                                 |
| mako                     | 9.87 ms                                                | 6.85 ms: 1.44x faster                                                |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.43x faster                                                 |
| scimark_monte_carlo      | 65.6 ms                                                | 46.0 ms: 1.43x faster                                                |
| sqlglot_transpile        | 1.44 ms                                                | 1.03 ms: 1.41x faster                                                |
| async_tree_io            | 980 ms                                                 | 701 ms: 1.40x faster                                                 |
| richards_super           | 57.8 ms                                                | 43.8 ms: 1.32x faster                                                |
| nbody                    | 93.0 ms                                                | 70.6 ms: 1.32x faster                                                |
| comprehensions           | 16.9 us                                                | 13.0 us: 1.31x faster                                                |
| deepcopy_memo            | 34.7 us                                                | 26.6 us: 1.31x faster                                                |
| float                    | 69.0 ms                                                | 53.0 ms: 1.30x faster                                                |
| go                       | 151 ms                                                 | 116 ms: 1.30x faster                                                 |
| chameleon                | 6.26 ms                                                | 4.85 ms: 1.29x faster                                                |
| unpickle_pure_python     | 194 us                                                 | 152 us: 1.28x faster                                                 |
| logging_format           | 4.83 us                                                | 3.79 us: 1.27x faster                                                |
| logging_simple           | 4.45 us                                                | 3.49 us: 1.27x faster                                                |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 521 ms: 1.25x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 517 ms: 1.24x faster                                                 |
| json_dumps               | 8.11 ms                                                | 6.54 ms: 1.24x faster                                                |
| tomli_loads              | 1.71 sec                                               | 1.38 sec: 1.24x faster                                               |
| pyflate                  | 427 ms                                                 | 346 ms: 1.23x faster                                                 |
| tornado_http             | 86.7 ms                                                | 70.3 ms: 1.23x faster                                                |
| pprint_pformat           | 1.30 sec                                               | 1.06 sec: 1.23x faster                                               |
| richards                 | 48.7 ms                                                | 39.8 ms: 1.22x faster                                                |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.22x faster                                               |
| pycparser                | 877 ms                                                 | 724 ms: 1.21x faster                                                 |
| create_gc_cycles         | 860 us                                                 | 712 us: 1.21x faster                                                 |
| scimark_lu               | 103 ms                                                 | 85.7 ms: 1.20x faster                                                |
| xml_etree_process        | 46.5 ms                                                | 39.0 ms: 1.19x faster                                                |
| sympy_sum                | 92.2 ms                                                | 77.4 ms: 1.19x faster                                                |
| deepcopy                 | 272 us                                                 | 228 us: 1.19x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 80.2 ms: 1.18x faster                                                |
| hexiom                   | 6.19 ms                                                | 5.32 ms: 1.16x faster                                                |
| deepcopy_reduce          | 2.33 us                                                | 2.00 us: 1.16x faster                                                |
| regex_dna                | 174 ms                                                 | 152 ms: 1.14x faster                                                 |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                                |
| generators               | 32.3 ms                                                | 28.4 ms: 1.14x faster                                                |
| dulwich_log              | 35.3 ms                                                | 31.1 ms: 1.14x faster                                                |
| docutils                 | 1.73 sec                                               | 1.53 sec: 1.14x faster                                               |
| sympy_str                | 165 ms                                                 | 146 ms: 1.13x faster                                                 |
| scimark_fft              | 224 ms                                                 | 201 ms: 1.12x faster                                                 |
| coroutines               | 20.7 ms                                                | 18.6 ms: 1.11x faster                                                |
| scimark_sor              | 128 ms                                                 | 116 ms: 1.11x faster                                                 |
| regex_compile            | 95.3 ms                                                | 86.7 ms: 1.10x faster                                                |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.14 ms: 1.09x faster                                                |
| sympy_expand             | 269 ms                                                 | 247 ms: 1.09x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 74.5 ms: 1.04x faster                                                |
| json                     | 3.08 ms                                                | 2.96 ms: 1.04x faster                                                |
| sqlglot_normalize        | 190 ms                                                 | 184 ms: 1.04x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 510 us: 1.03x faster                                                 |
| sqlglot_optimize         | 36.8 ms                                                | 35.6 ms: 1.03x faster                                                |
| 2to3                     | 192 ms                                                 | 188 ms: 1.02x faster                                                 |
| regex_v8                 | 17.1 ms                                                | 17.2 ms: 1.00x slower                                                |
| mdp                      | 1.63 sec                                               | 1.64 sec: 1.00x slower                                               |
| gc_traversal             | 2.36 ms                                                | 2.41 ms: 1.02x slower                                                |
| nqueens                  | 63.8 ms                                                | 65.0 ms: 1.02x slower                                                |
| pathlib                  | 24.5 ms                                                | 25.2 ms: 1.03x slower                                                |
| json_loads               | 16.4 us                                                | 16.9 us: 1.03x slower                                                |
| xml_etree_iterparse      | 72.1 ms                                                | 75.0 ms: 1.04x slower                                                |
| pickle                   | 6.97 us                                                | 7.25 us: 1.04x slower                                                |
| unpickle                 | 8.80 us                                                | 9.15 us: 1.04x slower                                                |
| fannkuch                 | 303 ms                                                 | 316 ms: 1.04x slower                                                 |
| regex_effbot             | 2.46 ms                                                | 2.63 ms: 1.07x slower                                                |
| pickle_dict              | 17.0 us                                                | 18.3 us: 1.08x slower                                                |
| pickle_list              | 2.74 us                                                | 2.96 us: 1.08x slower                                                |
| xml_etree_generate       | 53.5 ms                                                | 57.8 ms: 1.08x slower                                                |
| sqlite_synth             | 1.46 us                                                | 1.59 us: 1.09x slower                                                |
| unpickle_list            | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| coverage                 | 41.5 ms                                                | 48.5 ms: 1.17x slower                                                |
| telco                    | 3.49 ms                                                | 4.48 ms: 1.28x slower                                                |
| async_generators         | 231 ms                                                 | 309 ms: 1.33x slower                                                 |
| bench_mp_pool            | 37.4 ms                                                | 52.0 ms: 1.39x slower                                                |
| python_startup           | 10.9 ms                                                | 17.3 ms: 1.59x slower                                                |
| python_startup_no_site   | 7.91 ms                                                | 15.9 ms: 2.01x slower                                                |
| unpack_sequence          | 39.0 ns                                                | 113 ns: 2.90x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                         |

Benchmark hidden because not significant (4): mypy2, xml_etree_parse, asyncio_websockets, pidigits
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-594cca3-JIT/bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: 2.08x