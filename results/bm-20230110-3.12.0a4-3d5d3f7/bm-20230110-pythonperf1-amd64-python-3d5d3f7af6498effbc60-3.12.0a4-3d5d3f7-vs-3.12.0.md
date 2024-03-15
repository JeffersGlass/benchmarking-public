
# Results vs. 3.12.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: windows-amd64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 193 ms: 1.13x faster                                                       |
| chameleon      | 4.98 ms                                                     | 4.39 ms: 1.14x faster                                                      |
| docutils       | 1.66 sec                                                    | 1.48 sec: 1.12x faster                                                     |
| Geometric mean | (ref)                                                       | 1.13x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 465 ms: 1.05x faster                                                       |
| async_tree_none         | 291 ms                                                      | 295 ms: 1.01x slower                                                       |
| async_tree_io           | 731 ms                                                      | 742 ms: 1.01x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.00x faster                                                               |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.5 ms: 1.21x faster                                                      |
| float          | 56.8 ms                                                     | 47.2 ms: 1.20x faster                                                      |
| pidigits       | 152 ms                                                      | 145 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.15x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 78.8 ms: 1.11x faster                                                      |
| regex_dna      | 126 ms                                                      | 120 ms: 1.05x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 13.6 ms: 1.04x faster                                                      |
| regex_effbot   | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                      |
| Geometric mean | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                     | 48.3 ms: 1.16x faster                                                      |
| pickle_pure_python   | 195 us                                                      | 169 us: 1.15x faster                                                       |
| pickle               | 7.43 us                                                     | 6.55 us: 1.13x faster                                                      |
| json_loads           | 13.9 us                                                     | 12.4 us: 1.12x faster                                                      |
| unpickle_pure_python | 133 us                                                      | 119 us: 1.12x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.10 ms: 1.12x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 33.8 ms: 1.12x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 60.1 ms: 1.08x faster                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 86.5 ms: 1.07x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.59 us: 1.06x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 18.2 us: 1.01x faster                                                      |
| pickle_list          | 2.83 us                                                     | 2.81 us: 1.01x faster                                                      |
| unpickle             | 8.18 us                                                     | 8.70 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.08x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.1 ms: 1.07x faster                                                      |
| python_startup_no_site | 16.2 ms                                                     | 15.2 ms: 1.07x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.05 ms: 1.17x faster                                                      |
| django_template | 22.9 ms                                                     | 20.7 ms: 1.11x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.14x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 37.5 ns                                                     | 26.2 ns: 1.43x faster                                                      |
| async_generators        | 239 ms                                                      | 169 ms: 1.42x faster                                                       |
| scimark_sor             | 78.8 ms                                                     | 63.7 ms: 1.24x faster                                                      |
| nbody                   | 71.9 ms                                                     | 59.5 ms: 1.21x faster                                                      |
| float                   | 56.8 ms                                                     | 47.2 ms: 1.20x faster                                                      |
| deepcopy                | 238 us                                                      | 199 us: 1.19x faster                                                       |
| richards                | 28.4 ms                                                     | 24.0 ms: 1.18x faster                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 1.78 us: 1.18x faster                                                      |
| mako                    | 7.09 ms                                                     | 6.05 ms: 1.17x faster                                                      |
| json                    | 3.05 ms                                                     | 2.61 ms: 1.17x faster                                                      |
| deepcopy_memo           | 23.7 us                                                     | 20.4 us: 1.16x faster                                                      |
| xml_etree_generate      | 55.8 ms                                                     | 48.3 ms: 1.16x faster                                                      |
| pickle_pure_python      | 195 us                                                      | 169 us: 1.15x faster                                                       |
| scimark_monte_carlo     | 43.7 ms                                                     | 38.0 ms: 1.15x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.59 ms: 1.15x faster                                                      |
| pprint_safe_repr        | 513 ms                                                      | 448 ms: 1.14x faster                                                       |
| go                      | 91.6 ms                                                     | 80.4 ms: 1.14x faster                                                      |
| pprint_pformat          | 1.05 sec                                                    | 918 ms: 1.14x faster                                                       |
| fannkuch                | 247 ms                                                      | 217 ms: 1.14x faster                                                       |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.25 ms: 1.14x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 661 us: 1.14x faster                                                       |
| chameleon               | 4.98 ms                                                     | 4.39 ms: 1.14x faster                                                      |
| pickle                  | 7.43 us                                                     | 6.55 us: 1.13x faster                                                      |
| bench_mp_pool           | 69.2 ms                                                     | 61.1 ms: 1.13x faster                                                      |
| 2to3                    | 218 ms                                                      | 193 ms: 1.13x faster                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 30.6 ms: 1.13x faster                                                      |
| raytrace                | 192 ms                                                      | 171 ms: 1.12x faster                                                       |
| docutils                | 1.66 sec                                                    | 1.48 sec: 1.12x faster                                                     |
| pyflate                 | 295 ms                                                      | 263 ms: 1.12x faster                                                       |
| json_loads              | 13.9 us                                                     | 12.4 us: 1.12x faster                                                      |
| unpickle_pure_python    | 133 us                                                      | 119 us: 1.12x faster                                                       |
| logging_silent          | 60.5 ns                                                     | 54.2 ns: 1.12x faster                                                      |
| json_dumps              | 5.70 ms                                                     | 5.10 ms: 1.12x faster                                                      |
| xml_etree_process       | 37.7 ms                                                     | 33.8 ms: 1.12x faster                                                      |
| pycparser               | 699 ms                                                      | 628 ms: 1.11x faster                                                       |
| deltablue               | 2.16 ms                                                     | 1.94 ms: 1.11x faster                                                      |
| sqlglot_normalize       | 187 ms                                                      | 168 ms: 1.11x faster                                                       |
| regex_compile           | 87.5 ms                                                     | 78.8 ms: 1.11x faster                                                      |
| django_template         | 22.9 ms                                                     | 20.7 ms: 1.11x faster                                                      |
| scimark_fft             | 184 ms                                                      | 167 ms: 1.11x faster                                                       |
| dulwich_log             | 44.3 ms                                                     | 40.1 ms: 1.10x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 73.2 ms: 1.10x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 67.9 ms: 1.10x faster                                                      |
| nqueens                 | 62.8 ms                                                     | 57.3 ms: 1.10x faster                                                      |
| hexiom                  | 4.10 ms                                                     | 3.77 ms: 1.09x faster                                                      |
| xml_etree_iterparse     | 65.2 ms                                                     | 60.1 ms: 1.08x faster                                                      |
| logging_simple          | 6.28 us                                                     | 5.84 us: 1.08x faster                                                      |
| xml_etree_parse         | 93.0 ms                                                     | 86.5 ms: 1.07x faster                                                      |
| python_startup          | 19.5 ms                                                     | 18.1 ms: 1.07x faster                                                      |
| bench_thread_pool       | 857 us                                                      | 798 us: 1.07x faster                                                       |
| dask                    | 263 ms                                                      | 246 ms: 1.07x faster                                                       |
| python_startup_no_site  | 16.2 ms                                                     | 15.2 ms: 1.07x faster                                                      |
| logging_format          | 6.72 us                                                     | 6.29 us: 1.07x faster                                                      |
| spectral_norm           | 66.9 ms                                                     | 62.8 ms: 1.07x faster                                                      |
| unpickle_list           | 2.75 us                                                     | 2.59 us: 1.06x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.43 ms: 1.06x faster                                                      |
| crypto_pyaes            | 48.5 ms                                                     | 45.9 ms: 1.06x faster                                                      |
| sympy_expand            | 284 ms                                                      | 269 ms: 1.05x faster                                                       |
| async_tree_cpu_io_mixed | 489 ms                                                      | 465 ms: 1.05x faster                                                       |
| regex_dna               | 126 ms                                                      | 120 ms: 1.05x faster                                                       |
| scimark_lu              | 58.9 ms                                                     | 56.0 ms: 1.05x faster                                                      |
| pidigits                | 152 ms                                                      | 145 ms: 1.05x faster                                                       |
| asyncio_tcp             | 487 ms                                                      | 466 ms: 1.04x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 13.6 ms: 1.04x faster                                                      |
| sympy_str               | 175 ms                                                      | 168 ms: 1.04x faster                                                       |
| sympy_integrate         | 13.0 ms                                                     | 12.6 ms: 1.03x faster                                                      |
| chaos                   | 43.3 ms                                                     | 42.1 ms: 1.03x faster                                                      |
| sqlite_synth            | 1.76 us                                                     | 1.72 us: 1.03x faster                                                      |
| coroutines              | 14.3 ms                                                     | 13.9 ms: 1.03x faster                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                      |
| pickle_dict             | 18.4 us                                                     | 18.2 us: 1.01x faster                                                      |
| pickle_list             | 2.83 us                                                     | 2.81 us: 1.01x faster                                                      |
| sympy_sum               | 91.5 ms                                                     | 92.0 ms: 1.01x slower                                                      |
| async_tree_none         | 291 ms                                                      | 295 ms: 1.01x slower                                                       |
| async_tree_io           | 731 ms                                                      | 742 ms: 1.01x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 848 us: 1.05x slower                                                       |
| comprehensions          | 14.1 us                                                     | 15.0 us: 1.06x slower                                                      |
| unpickle                | 8.18 us                                                     | 8.70 us: 1.06x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.51 sec: 1.10x slower                                                     |
| coverage                | 40.8 ms                                                     | 52.5 ms: 1.29x slower                                                      |
| generators              | 22.5 ms                                                     | 33.1 ms: 1.47x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.08x faster                                                               |

Benchmark hidden because not significant (2): sqlglot_transpile, async_tree_memoization
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230110-3.12.0a4-3d5d3f7/bm-20230110-pythonperf1-amd64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown