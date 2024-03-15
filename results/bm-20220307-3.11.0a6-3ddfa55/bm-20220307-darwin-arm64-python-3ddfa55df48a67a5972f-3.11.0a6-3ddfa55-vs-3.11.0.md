
# Results vs. 3.11.0

- fork: python
- ref: 3ddfa55df48a67a5972f
- machine: darwin-arm64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.11x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 164 ms: 1.06x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.55 ms: 1.06x slower                                                 |
| docutils       | 1.43 sec                                               | 1.47 sec: 1.02x slower                                                |
| html5lib       | 33.0 ms                                                | 33.5 ms: 1.02x slower                                                 |
| tornado_http   | 69.1 ms                                                | 73.8 ms: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_io              | 697 ms                                                 | 704 ms: 1.01x slower                                                  |
| async_tree_none            | 282 ms                                                 | 287 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 533 ms: 1.03x slower                                                  |
| async_tree_io_tg           | 724 ms                                                 | 761 ms: 1.05x slower                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 624 ms: 1.13x slower                                                  |
| async_tree_none_tg         | 276 ms                                                 | 350 ms: 1.27x slower                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 449 ms: 1.27x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.10x slower                                                          |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 281 ms: 1.00x slower                                                  |
| float          | 50.8 ms                                                | 54.8 ms: 1.08x slower                                                 |
| nbody          | 61.7 ms                                                | 74.1 ms: 1.20x slower                                                 |
| Geometric mean | (ref)                                                  | 1.09x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| regex_compile  | 72.8 ms                                                | 76.7 ms: 1.05x slower                                                 |
| regex_v8       | 15.1 ms                                                | 17.5 ms: 1.16x slower                                                 |
| regex_dna      | 148 ms                                                 | 177 ms: 1.19x slower                                                  |
| Geometric mean | (ref)                                                  | 1.10x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_list          | 2.70 us                                                | 2.61 us: 1.03x faster                                                 |
| json_loads           | 15.3 us                                                | 14.9 us: 1.03x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 97.5 ms: 1.03x faster                                                 |
| pickle_dict          | 17.1 us                                                | 17.3 us: 1.01x slower                                                 |
| json_dumps           | 7.53 ms                                                | 7.66 ms: 1.02x slower                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 69.4 ms: 1.02x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.74 us: 1.02x slower                                                 |
| pickle               | 6.98 us                                                | 7.21 us: 1.03x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 48.7 ms: 1.06x slower                                                 |
| xml_etree_process    | 33.6 ms                                                | 36.5 ms: 1.09x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 214 us: 1.12x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 167 us: 1.12x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.44 sec: 1.13x slower                                                |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                          |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 8.57 ms                                                | 9.28 ms: 1.08x slower                                                 |
| python_startup         | 10.8 ms                                                | 14.8 ms: 1.38x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.22x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.33 ms: 1.08x faster                                                 |
| genshi_text     | 14.4 ms                                                | 15.2 ms: 1.06x slower                                                 |
| django_template | 20.1 ms                                                | 21.6 ms: 1.07x slower                                                 |
| genshi_xml      | 28.5 ms                                                | 31.4 ms: 1.10x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako                       | 7.93 ms                                                | 7.33 ms: 1.08x faster                                                 |
| logging_format             | 3.67 us                                                | 3.43 us: 1.07x faster                                                 |
| logging_simple             | 3.41 us                                                | 3.21 us: 1.06x faster                                                 |
| pickle_list                | 2.70 us                                                | 2.61 us: 1.03x faster                                                 |
| json_loads                 | 15.3 us                                                | 14.9 us: 1.03x faster                                                 |
| xml_etree_parse            | 100 ms                                                 | 97.5 ms: 1.03x faster                                                 |
| pylint                     | 253 ms                                                 | 247 ms: 1.02x faster                                                  |
| json                       | 2.75 ms                                                | 2.71 ms: 1.01x faster                                                 |
| sqlite_synth               | 1.26 us                                                | 1.25 us: 1.01x faster                                                 |
| chaos                      | 47.4 ms                                                | 47.2 ms: 1.00x faster                                                 |
| pidigits                   | 280 ms                                                 | 281 ms: 1.00x slower                                                  |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.00x slower                                                 |
| async_tree_io              | 697 ms                                                 | 704 ms: 1.01x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.45 ms: 1.01x slower                                                 |
| pickle_dict                | 17.1 us                                                | 17.3 us: 1.01x slower                                                 |
| async_generators           | 192 ms                                                 | 194 ms: 1.01x slower                                                  |
| create_gc_cycles           | 711 us                                                 | 720 us: 1.01x slower                                                  |
| generators                 | 30.3 ms                                                | 30.8 ms: 1.02x slower                                                 |
| html5lib                   | 33.0 ms                                                | 33.5 ms: 1.02x slower                                                 |
| json_dumps                 | 7.53 ms                                                | 7.66 ms: 1.02x slower                                                 |
| xml_etree_iterparse        | 68.3 ms                                                | 69.4 ms: 1.02x slower                                                 |
| async_tree_none            | 282 ms                                                 | 287 ms: 1.02x slower                                                  |
| unpickle_list              | 2.69 us                                                | 2.74 us: 1.02x slower                                                 |
| sympy_sum                  | 80.2 ms                                                | 82.0 ms: 1.02x slower                                                 |
| scimark_monte_carlo        | 43.5 ms                                                | 44.6 ms: 1.02x slower                                                 |
| docutils                   | 1.43 sec                                               | 1.47 sec: 1.02x slower                                                |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 533 ms: 1.03x slower                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.44 sec: 1.03x slower                                                |
| asyncio_tcp                | 643 ms                                                 | 663 ms: 1.03x slower                                                  |
| pickle                     | 6.98 us                                                | 7.21 us: 1.03x slower                                                 |
| flaskblogging              | 2.35 ms                                                | 2.43 ms: 1.03x slower                                                 |
| raytrace                   | 206 ms                                                 | 214 ms: 1.04x slower                                                  |
| sympy_integrate            | 11.3 ms                                                | 11.7 ms: 1.04x slower                                                 |
| meteor_contest             | 71.1 ms                                                | 74.1 ms: 1.04x slower                                                 |
| hexiom                     | 4.58 ms                                                | 4.78 ms: 1.04x slower                                                 |
| sympy_str                  | 144 ms                                                 | 150 ms: 1.04x slower                                                  |
| bench_mp_pool              | 41.0 ms                                                | 42.8 ms: 1.05x slower                                                 |
| nqueens                    | 55.9 ms                                                | 58.5 ms: 1.05x slower                                                 |
| dulwich_log                | 28.6 ms                                                | 30.0 ms: 1.05x slower                                                 |
| sqlglot_normalize          | 162 ms                                                 | 170 ms: 1.05x slower                                                  |
| async_tree_io_tg           | 724 ms                                                 | 761 ms: 1.05x slower                                                  |
| coroutines                 | 17.2 ms                                                | 18.1 ms: 1.05x slower                                                 |
| regex_compile              | 72.8 ms                                                | 76.7 ms: 1.05x slower                                                 |
| telco                      | 3.17 ms                                                | 3.34 ms: 1.05x slower                                                 |
| thrift                     | 410 us                                                 | 433 us: 1.05x slower                                                  |
| genshi_text                | 14.4 ms                                                | 15.2 ms: 1.06x slower                                                 |
| chameleon                  | 4.30 ms                                                | 4.55 ms: 1.06x slower                                                 |
| go                         | 105 ms                                                 | 112 ms: 1.06x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 48.7 ms: 1.06x slower                                                 |
| deepcopy                   | 215 us                                                 | 229 us: 1.06x slower                                                  |
| 2to3                       | 154 ms                                                 | 164 ms: 1.06x slower                                                  |
| deepcopy_memo              | 25.7 us                                                | 27.5 us: 1.07x slower                                                 |
| tornado_http               | 69.1 ms                                                | 73.8 ms: 1.07x slower                                                 |
| django_template            | 20.1 ms                                                | 21.6 ms: 1.07x slower                                                 |
| sympy_expand               | 229 ms                                                 | 247 ms: 1.08x slower                                                  |
| sqlalchemy_declarative     | 59.3 ms                                                | 63.8 ms: 1.08x slower                                                 |
| float                      | 50.8 ms                                                | 54.8 ms: 1.08x slower                                                 |
| pycparser                  | 659 ms                                                 | 711 ms: 1.08x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 9.28 ms: 1.08x slower                                                 |
| sqlglot_optimize           | 29.6 ms                                                | 32.2 ms: 1.09x slower                                                 |
| xml_etree_process          | 33.6 ms                                                | 36.5 ms: 1.09x slower                                                 |
| deepcopy_reduce            | 1.79 us                                                | 1.95 us: 1.09x slower                                                 |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.07 ms: 1.09x slower                                                 |
| aiohttp                    | 1.02 ms                                                | 1.12 ms: 1.09x slower                                                 |
| bench_thread_pool          | 465 us                                                 | 510 us: 1.10x slower                                                  |
| typing_runtime_protocols   | 301 us                                                 | 330 us: 1.10x slower                                                  |
| genshi_xml                 | 28.5 ms                                                | 31.4 ms: 1.10x slower                                                 |
| fannkuch                   | 240 ms                                                 | 264 ms: 1.10x slower                                                  |
| deltablue                  | 2.75 ms                                                | 3.03 ms: 1.10x slower                                                 |
| gunicorn                   | 1.10 ms                                                | 1.21 ms: 1.11x slower                                                 |
| sqlalchemy_imperative      | 6.98 ms                                                | 7.72 ms: 1.11x slower                                                 |
| scimark_lu                 | 67.7 ms                                                | 75.5 ms: 1.11x slower                                                 |
| pyflate                    | 284 ms                                                 | 316 ms: 1.11x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 214 us: 1.12x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 88.7 ms: 1.12x slower                                                 |
| scimark_fft                | 173 ms                                                 | 194 ms: 1.12x slower                                                  |
| richards                   | 31.1 ms                                                | 34.9 ms: 1.12x slower                                                 |
| pprint_safe_repr           | 478 ms                                                 | 538 ms: 1.12x slower                                                  |
| richards_super             | 37.3 ms                                                | 41.9 ms: 1.12x slower                                                 |
| unpickle_pure_python       | 149 us                                                 | 167 us: 1.12x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 1.10 sec: 1.13x slower                                                |
| tomli_loads                | 1.27 sec                                               | 1.44 sec: 1.13x slower                                                |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 624 ms: 1.13x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 75.5 ms: 1.15x slower                                                 |
| regex_v8                   | 15.1 ms                                                | 17.5 ms: 1.16x slower                                                 |
| crypto_pyaes               | 47.5 ms                                                | 55.4 ms: 1.17x slower                                                 |
| comprehensions             | 14.4 us                                                | 17.1 us: 1.18x slower                                                 |
| regex_dna                  | 148 ms                                                 | 177 ms: 1.19x slower                                                  |
| nbody                      | 61.7 ms                                                | 74.1 ms: 1.20x slower                                                 |
| logging_silent             | 66.5 ns                                                | 80.3 ns: 1.21x slower                                                 |
| mdp                        | 1.48 sec                                               | 1.80 sec: 1.21x slower                                                |
| async_tree_none_tg         | 276 ms                                                 | 350 ms: 1.27x slower                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 449 ms: 1.27x slower                                                  |
| sqlglot_transpile          | 1.05 ms                                                | 1.40 ms: 1.33x slower                                                 |
| python_startup             | 10.8 ms                                                | 14.8 ms: 1.38x slower                                                 |
| sqlglot_parse              | 890 us                                                 | 1.23 ms: 1.38x slower                                                 |
| dask                       | 219 ms                                                 | 308 ms: 1.41x slower                                                  |
| unpack_sequence            | 33.6 ns                                                | 93.6 ns: 2.78x slower                                                 |
| coverage                   | 43.9 ms                                                | 328 ms: 7.47x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.11x slower                                                          |

Benchmark hidden because not significant (3): pathlib, unpickle, async_tree_memoization
Ignored benchmarks (2) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: asyncio_websockets, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.04x