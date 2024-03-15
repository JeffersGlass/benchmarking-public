# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_arena
- machine: linux-x86_64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.12x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 307 ms: 1.08x slower                                                       |
| chameleon      | 7.23 ms                                                      | 7.60 ms: 1.05x slower                                                      |
| docutils       | 2.87 sec                                                     | 2.91 sec: 1.01x slower                                                     |
| tornado_http   | 121 ms                                                       | 125 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 445 ms: 1.01x faster                                                       |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 710 ms: 1.02x slower                                                       |
| async_tree_memoization     | 544 ms                                                       | 559 ms: 1.03x slower                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 447 ms: 1.04x slower                                                       |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                     |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                     |
| async_tree_memoization_tg  | 540 ms                                                       | 572 ms: 1.06x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 261 ms: 1.01x faster                                                       |
| float          | 76.6 ms                                                      | 78.1 ms: 1.02x slower                                                      |
| nbody          | 88.0 ms                                                      | 98.5 ms: 1.12x slower                                                      |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.56 ms: 1.00x faster                                                      |
| regex_compile  | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| regex_v8       | 23.6 ms                                                      | 25.2 ms: 1.07x slower                                                      |
| Geometric mean | (ref)                                                        | 1.02x slower                                                               |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.0 us: 1.05x faster                                                      |
| xml_etree_generate   | 86.1 ms                                                      | 83.2 ms: 1.04x faster                                                      |
| pickle_pure_python   | 318 us                                                       | 308 us: 1.03x faster                                                       |
| pickle_list          | 4.43 us                                                      | 4.30 us: 1.03x faster                                                      |
| pickle               | 10.5 us                                                      | 10.3 us: 1.02x faster                                                      |
| xml_etree_process    | 58.4 ms                                                      | 57.7 ms: 1.01x faster                                                      |
| xml_etree_iterparse  | 103 ms                                                       | 102 ms: 1.01x faster                                                       |
| xml_etree_parse      | 144 ms                                                       | 143 ms: 1.01x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.64 us: 1.00x faster                                                      |
| tomli_loads          | 2.16 sec                                                     | 2.17 sec: 1.01x slower                                                     |
| json_loads           | 24.4 us                                                      | 24.8 us: 1.02x slower                                                      |
| unpickle             | 14.8 us                                                      | 15.1 us: 1.02x slower                                                      |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                      |
| unpickle_pure_python | 210 us                                                       | 230 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 15.4 ms: 1.32x slower                                                      |
| python_startup_no_site | 8.64 ms                                                      | 13.9 ms: 1.60x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.46x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 9.85 ms: 1.02x faster                                                      |
| django_template | 38.2 ms                                                      | 38.9 ms: 1.02x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.00x slower                                                               |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 118 us: 1.28x faster                                                       |
| comprehensions             | 21.9 us                                                      | 18.7 us: 1.17x faster                                                      |
| generators                 | 37.4 ms                                                      | 33.0 ms: 1.13x faster                                                      |
| pickle_dict                | 32.5 us                                                      | 31.0 us: 1.05x faster                                                      |
| logging_format             | 7.48 us                                                      | 7.12 us: 1.05x faster                                                      |
| crypto_pyaes               | 80.3 ms                                                      | 76.7 ms: 1.05x faster                                                      |
| logging_simple             | 6.71 us                                                      | 6.42 us: 1.04x faster                                                      |
| xml_etree_generate         | 86.1 ms                                                      | 83.2 ms: 1.04x faster                                                      |
| pickle_pure_python         | 318 us                                                       | 308 us: 1.03x faster                                                       |
| sqlite_synth               | 2.77 us                                                      | 2.69 us: 1.03x faster                                                      |
| pickle_list                | 4.43 us                                                      | 4.30 us: 1.03x faster                                                      |
| coroutines                 | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                      |
| create_gc_cycles           | 1.59 ms                                                      | 1.55 ms: 1.03x faster                                                      |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.02x faster                                                      |
| asyncio_tcp                | 378 ms                                                       | 371 ms: 1.02x faster                                                       |
| mako                       | 10.0 ms                                                      | 9.85 ms: 1.02x faster                                                      |
| sympy_sum                  | 162 ms                                                       | 160 ms: 1.01x faster                                                       |
| async_tree_none            | 452 ms                                                       | 445 ms: 1.01x faster                                                       |
| pidigits                   | 265 ms                                                       | 261 ms: 1.01x faster                                                       |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.16 ms: 1.01x faster                                                      |
| xml_etree_process          | 58.4 ms                                                      | 57.7 ms: 1.01x faster                                                      |
| deepcopy_reduce            | 3.37 us                                                      | 3.34 us: 1.01x faster                                                      |
| xml_etree_iterparse        | 103 ms                                                       | 102 ms: 1.01x faster                                                       |
| xml_etree_parse            | 144 ms                                                       | 143 ms: 1.01x faster                                                       |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                                     |
| unpickle_list              | 4.66 us                                                      | 4.64 us: 1.00x faster                                                      |
| regex_effbot               | 3.57 ms                                                      | 3.56 ms: 1.00x faster                                                      |
| async_generators           | 390 ms                                                       | 389 ms: 1.00x faster                                                       |
| mdp                        | 2.57 sec                                                     | 2.58 sec: 1.00x slower                                                     |
| tomli_loads                | 2.16 sec                                                     | 2.17 sec: 1.01x slower                                                     |
| spectral_norm              | 91.6 ms                                                      | 92.6 ms: 1.01x slower                                                      |
| regex_compile              | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| docutils                   | 2.87 sec                                                     | 2.91 sec: 1.01x slower                                                     |
| sqlglot_parse              | 1.38 ms                                                      | 1.40 ms: 1.01x slower                                                      |
| deepcopy_memo              | 36.8 us                                                      | 37.4 us: 1.02x slower                                                      |
| json_loads                 | 24.4 us                                                      | 24.8 us: 1.02x slower                                                      |
| deepcopy                   | 368 us                                                       | 375 us: 1.02x slower                                                       |
| float                      | 76.6 ms                                                      | 78.1 ms: 1.02x slower                                                      |
| django_template            | 38.2 ms                                                      | 38.9 ms: 1.02x slower                                                      |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                      |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 710 ms: 1.02x slower                                                       |
| raytrace                   | 298 ms                                                       | 304 ms: 1.02x slower                                                       |
| unpickle                   | 14.8 us                                                      | 15.1 us: 1.02x slower                                                      |
| sympy_integrate            | 23.9 ms                                                      | 24.5 ms: 1.02x slower                                                      |
| async_tree_memoization     | 544 ms                                                       | 559 ms: 1.03x slower                                                       |
| meteor_contest             | 128 ms                                                       | 132 ms: 1.03x slower                                                       |
| logging_silent             | 94.4 ns                                                      | 97.0 ns: 1.03x slower                                                      |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                       |
| tornado_http               | 121 ms                                                       | 125 ms: 1.03x slower                                                       |
| sqlglot_transpile          | 1.78 ms                                                      | 1.83 ms: 1.03x slower                                                      |
| sqlglot_normalize          | 116 ms                                                       | 120 ms: 1.03x slower                                                       |
| pprint_safe_repr           | 807 ms                                                       | 835 ms: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 447 ms: 1.04x slower                                                       |
| pprint_pformat             | 1.65 sec                                                     | 1.72 sec: 1.04x slower                                                     |
| pycparser                  | 1.23 sec                                                     | 1.28 sec: 1.04x slower                                                     |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                     |
| chaos                      | 64.0 ms                                                      | 66.8 ms: 1.04x slower                                                      |
| bench_thread_pool          | 950 us                                                       | 991 us: 1.04x slower                                                       |
| json                       | 5.12 ms                                                      | 5.35 ms: 1.04x slower                                                      |
| dulwich_log                | 65.4 ms                                                      | 68.3 ms: 1.05x slower                                                      |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                     |
| chameleon                  | 7.23 ms                                                      | 7.60 ms: 1.05x slower                                                      |
| json_dumps                 | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                      |
| scimark_fft                | 301 ms                                                       | 318 ms: 1.06x slower                                                       |
| sympy_expand               | 484 ms                                                       | 512 ms: 1.06x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 572 ms: 1.06x slower                                                       |
| regex_v8                   | 23.6 ms                                                      | 25.2 ms: 1.07x slower                                                      |
| 2to3                       | 285 ms                                                       | 307 ms: 1.08x slower                                                       |
| gunicorn                   | 1.00 ms                                                      | 1.08 ms: 1.08x slower                                                      |
| richards                   | 45.7 ms                                                      | 49.6 ms: 1.08x slower                                                      |
| aiohttp                    | 1.02 ms                                                      | 1.10 ms: 1.08x slower                                                      |
| mypy2                      | 830 ms                                                       | 910 ms: 1.10x slower                                                       |
| sqlglot_optimize           | 57.5 ms                                                      | 63.0 ms: 1.10x slower                                                      |
| unpickle_pure_python       | 210 us                                                       | 230 us: 1.10x slower                                                       |
| fannkuch                   | 350 ms                                                       | 386 ms: 1.10x slower                                                       |
| richards_super             | 51.3 ms                                                      | 56.7 ms: 1.10x slower                                                      |
| scimark_monte_carlo        | 69.0 ms                                                      | 76.6 ms: 1.11x slower                                                      |
| nbody                      | 88.0 ms                                                      | 98.5 ms: 1.12x slower                                                      |
| nqueens                    | 89.9 ms                                                      | 101 ms: 1.13x slower                                                       |
| unpack_sequence            | 53.2 ns                                                      | 60.5 ns: 1.14x slower                                                      |
| telco                      | 6.96 ms                                                      | 7.99 ms: 1.15x slower                                                      |
| go                         | 150 ms                                                       | 172 ms: 1.15x slower                                                       |
| deltablue                  | 3.24 ms                                                      | 3.81 ms: 1.18x slower                                                      |
| scimark_lu                 | 98.8 ms                                                      | 117 ms: 1.19x slower                                                       |
| coverage                   | 66.7 ms                                                      | 81.4 ms: 1.22x slower                                                      |
| hexiom                     | 5.96 ms                                                      | 7.30 ms: 1.23x slower                                                      |
| pyflate                    | 439 ms                                                       | 538 ms: 1.23x slower                                                       |
| python_startup             | 11.6 ms                                                      | 15.4 ms: 1.32x slower                                                      |
| scimark_sor                | 109 ms                                                       | 151 ms: 1.39x slower                                                       |
| bench_mp_pool              | 4.76 ms                                                      | 7.08 ms: 1.49x slower                                                      |
| dask                       | 392 ms                                                       | 588 ms: 1.50x slower                                                       |
| python_startup_no_site     | 8.64 ms                                                      | 13.9 ms: 1.60x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.05x slower                                                               |

Benchmark hidden because not significant (4): sympy_str, gc_traversal, asyncio_websockets, regex_dna
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.12x