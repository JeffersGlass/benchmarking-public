
# Results vs. 3.12.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: windows-amd64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 193 ms: 1.13x faster                                                       |
| chameleon      | 4.98 ms                                                     | 4.59 ms: 1.08x faster                                                      |
| docutils       | 1.66 sec                                                    | 1.52 sec: 1.09x faster                                                     |
| Geometric mean | (ref)                                                       | 1.08x faster                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 507 ms: 1.04x slower                                                       |
| async_tree_io           | 731 ms                                                      | 783 ms: 1.07x slower                                                       |
| async_tree_none         | 291 ms                                                      | 325 ms: 1.12x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 386 ms: 1.14x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.09x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 48.7 ms: 1.17x faster                                                      |
| nbody          | 71.9 ms                                                     | 62.3 ms: 1.15x faster                                                      |
| pidigits       | 152 ms                                                      | 146 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 82.3 ms: 1.06x faster                                                      |
| regex_dna      | 126 ms                                                      | 120 ms: 1.05x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                                      |
| regex_effbot   | 1.62 ms                                                     | 1.70 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                     | 49.0 ms: 1.14x faster                                                      |
| pickle               | 7.43 us                                                     | 6.57 us: 1.13x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 33.9 ms: 1.11x faster                                                      |
| json_dumps           | 5.70 ms                                                     | 5.12 ms: 1.11x faster                                                      |
| pickle_pure_python   | 195 us                                                      | 180 us: 1.09x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.62 us: 1.08x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 87.6 ms: 1.06x faster                                                      |
| json_loads           | 13.9 us                                                     | 13.3 us: 1.05x faster                                                      |
| unpickle_pure_python | 133 us                                                      | 130 us: 1.02x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.3 us: 1.01x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.79 us: 1.01x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.06x faster                                                               |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| python_startup_no_site | 16.2 ms                                                     | 15.4 ms: 1.05x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.25 ms: 1.13x faster                                                      |
| django_template | 22.9 ms                                                     | 21.6 ms: 1.06x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.10x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 173 ms: 1.38x faster                                                       |
| unpack_sequence         | 37.5 ns                                                     | 30.8 ns: 1.22x faster                                                      |
| float                   | 56.8 ms                                                     | 48.7 ms: 1.17x faster                                                      |
| nbody                   | 71.9 ms                                                     | 62.3 ms: 1.15x faster                                                      |
| xml_etree_generate      | 55.8 ms                                                     | 49.0 ms: 1.14x faster                                                      |
| scimark_sor             | 78.8 ms                                                     | 69.2 ms: 1.14x faster                                                      |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.25 ms: 1.14x faster                                                      |
| mako                    | 7.09 ms                                                     | 6.25 ms: 1.13x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 665 us: 1.13x faster                                                       |
| pickle                  | 7.43 us                                                     | 6.57 us: 1.13x faster                                                      |
| bench_mp_pool           | 69.2 ms                                                     | 61.2 ms: 1.13x faster                                                      |
| 2to3                    | 218 ms                                                      | 193 ms: 1.13x faster                                                       |
| pprint_safe_repr        | 513 ms                                                      | 458 ms: 1.12x faster                                                       |
| pprint_pformat          | 1.05 sec                                                    | 934 ms: 1.12x faster                                                       |
| deepcopy_reduce         | 2.09 us                                                     | 1.87 us: 1.12x faster                                                      |
| xml_etree_process       | 37.7 ms                                                     | 33.9 ms: 1.11x faster                                                      |
| json_dumps              | 5.70 ms                                                     | 5.12 ms: 1.11x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 72.6 ms: 1.11x faster                                                      |
| json                    | 3.05 ms                                                     | 2.75 ms: 1.11x faster                                                      |
| scimark_monte_carlo     | 43.7 ms                                                     | 39.8 ms: 1.10x faster                                                      |
| deepcopy                | 238 us                                                      | 217 us: 1.10x faster                                                       |
| docutils                | 1.66 sec                                                    | 1.52 sec: 1.09x faster                                                     |
| nqueens                 | 62.8 ms                                                     | 57.5 ms: 1.09x faster                                                      |
| go                      | 91.6 ms                                                     | 84.0 ms: 1.09x faster                                                      |
| fannkuch                | 247 ms                                                      | 227 ms: 1.09x faster                                                       |
| scimark_fft             | 184 ms                                                      | 170 ms: 1.09x faster                                                       |
| pickle_pure_python      | 195 us                                                      | 180 us: 1.09x faster                                                       |
| chameleon               | 4.98 ms                                                     | 4.59 ms: 1.08x faster                                                      |
| pyflate                 | 295 ms                                                      | 272 ms: 1.08x faster                                                       |
| pickle_list             | 2.83 us                                                     | 2.62 us: 1.08x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 69.3 ms: 1.08x faster                                                      |
| pycparser               | 699 ms                                                      | 650 ms: 1.07x faster                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 32.1 ms: 1.07x faster                                                      |
| sqlglot_normalize       | 187 ms                                                      | 174 ms: 1.07x faster                                                       |
| crypto_pyaes            | 48.5 ms                                                     | 45.4 ms: 1.07x faster                                                      |
| deepcopy_memo           | 23.7 us                                                     | 22.2 us: 1.07x faster                                                      |
| python_startup          | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| xml_etree_iterparse     | 65.2 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| regex_compile           | 87.5 ms                                                     | 82.3 ms: 1.06x faster                                                      |
| xml_etree_parse         | 93.0 ms                                                     | 87.6 ms: 1.06x faster                                                      |
| richards                | 28.4 ms                                                     | 26.7 ms: 1.06x faster                                                      |
| django_template         | 22.9 ms                                                     | 21.6 ms: 1.06x faster                                                      |
| spectral_norm           | 66.9 ms                                                     | 63.1 ms: 1.06x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.44 ms: 1.06x faster                                                      |
| python_startup_no_site  | 16.2 ms                                                     | 15.4 ms: 1.05x faster                                                      |
| regex_dna               | 126 ms                                                      | 120 ms: 1.05x faster                                                       |
| json_loads              | 13.9 us                                                     | 13.3 us: 1.05x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.95 ms: 1.05x faster                                                      |
| raytrace                | 192 ms                                                      | 184 ms: 1.04x faster                                                       |
| pidigits                | 152 ms                                                      | 146 ms: 1.04x faster                                                       |
| scimark_lu              | 58.9 ms                                                     | 56.9 ms: 1.03x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                                      |
| sqlite_synth            | 1.76 us                                                     | 1.71 us: 1.03x faster                                                      |
| dulwich_log             | 44.3 ms                                                     | 43.1 ms: 1.03x faster                                                      |
| bench_thread_pool       | 857 us                                                      | 835 us: 1.03x faster                                                       |
| hexiom                  | 4.10 ms                                                     | 4.00 ms: 1.03x faster                                                      |
| logging_format          | 6.72 us                                                     | 6.56 us: 1.02x faster                                                      |
| unpickle_pure_python    | 133 us                                                      | 130 us: 1.02x faster                                                       |
| dask                    | 263 ms                                                      | 258 ms: 1.02x faster                                                       |
| logging_silent          | 60.5 ns                                                     | 59.9 ns: 1.01x faster                                                      |
| pickle_dict             | 18.4 us                                                     | 18.3 us: 1.01x faster                                                      |
| sympy_expand            | 284 ms                                                      | 282 ms: 1.01x faster                                                       |
| sympy_integrate         | 13.0 ms                                                     | 12.9 ms: 1.01x faster                                                      |
| chaos                   | 43.3 ms                                                     | 43.1 ms: 1.00x faster                                                      |
| logging_simple          | 6.28 us                                                     | 6.31 us: 1.01x slower                                                      |
| unpickle_list           | 2.75 us                                                     | 2.79 us: 1.01x slower                                                      |
| async_tree_cpu_io_mixed | 489 ms                                                      | 507 ms: 1.04x slower                                                       |
| deltablue               | 2.16 ms                                                     | 2.24 ms: 1.04x slower                                                      |
| sqlglot_transpile       | 1.02 ms                                                     | 1.06 ms: 1.04x slower                                                      |
| sympy_sum               | 91.5 ms                                                     | 96.1 ms: 1.05x slower                                                      |
| coroutines              | 14.3 ms                                                     | 15.0 ms: 1.05x slower                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.70 ms: 1.05x slower                                                      |
| async_tree_io           | 731 ms                                                      | 783 ms: 1.07x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 865 us: 1.08x slower                                                       |
| comprehensions          | 14.1 us                                                     | 15.4 us: 1.09x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.53 sec: 1.11x slower                                                     |
| async_tree_none         | 291 ms                                                      | 325 ms: 1.12x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 386 ms: 1.14x slower                                                       |
| coverage                | 40.8 ms                                                     | 52.0 ms: 1.27x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 708 ms: 1.45x slower                                                       |
| generators              | 22.5 ms                                                     | 35.7 ms: 1.58x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.04x faster                                                               |

Benchmark hidden because not significant (3): sympy_str, tornado_http, unpickle
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20221114-3.12.0a2-3b9d793/bm-20221114-pythonperf1-amd64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown