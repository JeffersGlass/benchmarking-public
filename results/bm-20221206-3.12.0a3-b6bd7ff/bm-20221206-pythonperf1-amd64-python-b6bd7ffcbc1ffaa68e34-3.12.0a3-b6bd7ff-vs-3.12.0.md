
# Results vs. 3.12.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: windows-amd64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 196 ms: 1.11x faster                                                       |
| chameleon      | 4.98 ms                                                     | 4.53 ms: 1.10x faster                                                      |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                     |
| Geometric mean | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 501 ms: 1.03x slower                                                       |
| async_tree_io           | 731 ms                                                      | 780 ms: 1.07x slower                                                       |
| async_tree_none         | 291 ms                                                      | 317 ms: 1.09x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 388 ms: 1.15x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.08x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 62.3 ms: 1.15x faster                                                      |
| float          | 56.8 ms                                                     | 50.1 ms: 1.13x faster                                                      |
| pidigits       | 152 ms                                                      | 151 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.10x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 82.5 ms: 1.06x faster                                                      |
| regex_dna      | 126 ms                                                      | 120 ms: 1.06x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.54 ms: 1.05x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 14.0 ms: 1.02x faster                                                      |
| Geometric mean | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                     | 49.7 ms: 1.12x faster                                                      |
| json_dumps           | 5.70 ms                                                     | 5.17 ms: 1.10x faster                                                      |
| unpickle_pure_python | 133 us                                                      | 121 us: 1.10x faster                                                       |
| pickle_pure_python   | 195 us                                                      | 179 us: 1.09x faster                                                       |
| json_loads           | 13.9 us                                                     | 12.9 us: 1.08x faster                                                      |
| pickle               | 7.43 us                                                     | 6.90 us: 1.08x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 35.0 ms: 1.08x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.61 us: 1.05x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 90.5 ms: 1.03x faster                                                      |
| unpickle             | 8.18 us                                                     | 7.99 us: 1.02x faster                                                      |
| pickle_list          | 2.83 us                                                     | 2.85 us: 1.01x slower                                                      |
| pickle_dict          | 18.4 us                                                     | 19.4 us: 1.05x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.5 ms: 1.05x faster                                                      |
| python_startup_no_site | 16.2 ms                                                     | 15.7 ms: 1.03x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.04x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.19 ms: 1.15x faster                                                      |
| django_template | 22.9 ms                                                     | 21.4 ms: 1.07x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.11x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 37.5 ns                                                     | 26.4 ns: 1.42x faster                                                      |
| async_generators        | 239 ms                                                      | 179 ms: 1.34x faster                                                       |
| scimark_sor             | 78.8 ms                                                     | 64.6 ms: 1.22x faster                                                      |
| richards                | 28.4 ms                                                     | 24.5 ms: 1.16x faster                                                      |
| nbody                   | 71.9 ms                                                     | 62.3 ms: 1.15x faster                                                      |
| scimark_monte_carlo     | 43.7 ms                                                     | 38.1 ms: 1.15x faster                                                      |
| mako                    | 7.09 ms                                                     | 6.19 ms: 1.15x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.64 ms: 1.13x faster                                                      |
| float                   | 56.8 ms                                                     | 50.1 ms: 1.13x faster                                                      |
| xml_etree_generate      | 55.8 ms                                                     | 49.7 ms: 1.12x faster                                                      |
| pprint_safe_repr        | 513 ms                                                      | 458 ms: 1.12x faster                                                       |
| deepcopy_memo           | 23.7 us                                                     | 21.2 us: 1.12x faster                                                      |
| pyflate                 | 295 ms                                                      | 264 ms: 1.12x faster                                                       |
| pathlib                 | 80.5 ms                                                     | 72.1 ms: 1.12x faster                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 1.88 us: 1.11x faster                                                      |
| 2to3                    | 218 ms                                                      | 196 ms: 1.11x faster                                                       |
| json                    | 3.05 ms                                                     | 2.74 ms: 1.11x faster                                                      |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.30 ms: 1.11x faster                                                      |
| deepcopy                | 238 us                                                      | 214 us: 1.11x faster                                                       |
| fannkuch                | 247 ms                                                      | 222 ms: 1.11x faster                                                       |
| pprint_pformat          | 1.05 sec                                                    | 947 ms: 1.10x faster                                                       |
| create_gc_cycles        | 752 us                                                      | 682 us: 1.10x faster                                                       |
| json_dumps              | 5.70 ms                                                     | 5.17 ms: 1.10x faster                                                      |
| bench_mp_pool           | 69.2 ms                                                     | 62.8 ms: 1.10x faster                                                      |
| unpickle_pure_python    | 133 us                                                      | 121 us: 1.10x faster                                                       |
| chameleon               | 4.98 ms                                                     | 4.53 ms: 1.10x faster                                                      |
| pickle_pure_python      | 195 us                                                      | 179 us: 1.09x faster                                                       |
| spectral_norm           | 66.9 ms                                                     | 61.4 ms: 1.09x faster                                                      |
| sqlglot_normalize       | 187 ms                                                      | 172 ms: 1.09x faster                                                       |
| nqueens                 | 62.8 ms                                                     | 57.9 ms: 1.09x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 68.8 ms: 1.08x faster                                                      |
| json_loads              | 13.9 us                                                     | 12.9 us: 1.08x faster                                                      |
| go                      | 91.6 ms                                                     | 84.8 ms: 1.08x faster                                                      |
| pickle                  | 7.43 us                                                     | 6.90 us: 1.08x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 32.0 ms: 1.08x faster                                                      |
| xml_etree_process       | 37.7 ms                                                     | 35.0 ms: 1.08x faster                                                      |
| dulwich_log             | 44.3 ms                                                     | 41.2 ms: 1.08x faster                                                      |
| crypto_pyaes            | 48.5 ms                                                     | 45.1 ms: 1.08x faster                                                      |
| raytrace                | 192 ms                                                      | 179 ms: 1.07x faster                                                       |
| scimark_lu              | 58.9 ms                                                     | 54.8 ms: 1.07x faster                                                      |
| django_template         | 22.9 ms                                                     | 21.4 ms: 1.07x faster                                                      |
| docutils                | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                     |
| regex_compile           | 87.5 ms                                                     | 82.5 ms: 1.06x faster                                                      |
| logging_silent          | 60.5 ns                                                     | 57.2 ns: 1.06x faster                                                      |
| regex_dna               | 126 ms                                                      | 120 ms: 1.06x faster                                                       |
| gc_traversal            | 1.52 ms                                                     | 1.44 ms: 1.06x faster                                                      |
| hexiom                  | 4.10 ms                                                     | 3.89 ms: 1.05x faster                                                      |
| python_startup          | 19.5 ms                                                     | 18.5 ms: 1.05x faster                                                      |
| unpickle_list           | 2.75 us                                                     | 2.61 us: 1.05x faster                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.54 ms: 1.05x faster                                                      |
| xml_etree_iterparse     | 65.2 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| scimark_fft             | 184 ms                                                      | 177 ms: 1.04x faster                                                       |
| deltablue               | 2.16 ms                                                     | 2.07 ms: 1.04x faster                                                      |
| python_startup_no_site  | 16.2 ms                                                     | 15.7 ms: 1.03x faster                                                      |
| xml_etree_parse         | 93.0 ms                                                     | 90.5 ms: 1.03x faster                                                      |
| unpickle                | 8.18 us                                                     | 7.99 us: 1.02x faster                                                      |
| bench_thread_pool       | 857 us                                                      | 837 us: 1.02x faster                                                       |
| dask                    | 263 ms                                                      | 258 ms: 1.02x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 14.0 ms: 1.02x faster                                                      |
| sqlite_synth            | 1.76 us                                                     | 1.73 us: 1.02x faster                                                      |
| logging_format          | 6.72 us                                                     | 6.64 us: 1.01x faster                                                      |
| sympy_str               | 175 ms                                                      | 173 ms: 1.01x faster                                                       |
| pidigits                | 152 ms                                                      | 151 ms: 1.01x faster                                                       |
| logging_simple          | 6.28 us                                                     | 6.22 us: 1.01x faster                                                      |
| sympy_expand            | 284 ms                                                      | 286 ms: 1.01x slower                                                       |
| pickle_list             | 2.83 us                                                     | 2.85 us: 1.01x slower                                                      |
| async_tree_cpu_io_mixed | 489 ms                                                      | 501 ms: 1.03x slower                                                       |
| sympy_integrate         | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                      |
| sqlglot_transpile       | 1.02 ms                                                     | 1.06 ms: 1.04x slower                                                      |
| pickle_dict             | 18.4 us                                                     | 19.4 us: 1.05x slower                                                      |
| coroutines              | 14.3 ms                                                     | 15.1 ms: 1.06x slower                                                      |
| async_tree_io           | 731 ms                                                      | 780 ms: 1.07x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 860 us: 1.07x slower                                                       |
| sympy_sum               | 91.5 ms                                                     | 99.0 ms: 1.08x slower                                                      |
| async_tree_none         | 291 ms                                                      | 317 ms: 1.09x slower                                                       |
| comprehensions          | 14.1 us                                                     | 15.5 us: 1.10x slower                                                      |
| async_tree_memoization  | 339 ms                                                      | 388 ms: 1.15x slower                                                       |
| mdp                     | 1.37 sec                                                    | 1.61 sec: 1.17x slower                                                     |
| coverage                | 40.8 ms                                                     | 51.6 ms: 1.26x slower                                                      |
| generators              | 22.5 ms                                                     | 33.9 ms: 1.51x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 735 ms: 1.51x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.04x faster                                                               |

Benchmark hidden because not significant (2): pycparser, chaos
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20221206-3.12.0a3-b6bd7ff/bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown