
# Results vs. 3.12.0

- fork: python
- ref: 5a7e1e0a92622c605ab2
- machine: windows-amd64
- commit hash: 5a7e1e0
- commit date: 2022-07-11
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.91%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 206 ms: 1.06x faster                                                       |
| chameleon      | 4.98 ms                                                     | 5.14 ms: 1.03x slower                                                      |
| docutils       | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                     |
| tornado_http   | 89.5 ms                                                     | 91.9 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                       | 1.01x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 731 ms                                                      | 753 ms: 1.03x slower                                                       |
| async_tree_cpu_io_mixed | 489 ms                                                      | 508 ms: 1.04x slower                                                       |
| async_tree_none         | 291 ms                                                      | 317 ms: 1.09x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 375 ms: 1.10x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.06x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.9 ms: 1.05x faster                                                      |
| nbody          | 71.9 ms                                                     | 68.7 ms: 1.05x faster                                                      |
| pidigits       | 152 ms                                                      | 146 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 114 ms: 1.10x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                      |
| regex_compile  | 87.5 ms                                                     | 90.8 ms: 1.04x slower                                                      |
| regex_effbot   | 1.62 ms                                                     | 1.70 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.48 us: 1.15x faster                                                      |
| pickle_list          | 2.83 us                                                     | 2.65 us: 1.06x faster                                                      |
| xml_etree_generate   | 55.8 ms                                                     | 53.4 ms: 1.05x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.7 ms: 1.04x faster                                                      |
| json_loads           | 13.9 us                                                     | 14.1 us: 1.01x slower                                                      |
| unpickle_list        | 2.75 us                                                     | 2.80 us: 1.02x slower                                                      |
| unpickle             | 8.18 us                                                     | 8.32 us: 1.02x slower                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 95.1 ms: 1.02x slower                                                      |
| pickle_pure_python   | 195 us                                                      | 204 us: 1.04x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 152 us: 1.14x slower                                                       |
| json_dumps           | 5.70 ms                                                     | 7.78 ms: 1.37x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.02x slower                                                               |

Benchmark hidden because not significant (2): pickle_dict, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                      |
| python_startup_no_site | 16.2 ms                                                     | 15.4 ms: 1.06x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 7.23 ms: 1.02x slower                                                      |
| django_template | 22.9 ms                                                     | 25.0 ms: 1.09x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.05x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 178 ms: 1.35x faster                                                       |
| pickle                  | 7.43 us                                                     | 6.48 us: 1.15x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 664 us: 1.13x faster                                                       |
| bench_mp_pool           | 69.2 ms                                                     | 61.4 ms: 1.13x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 72.4 ms: 1.11x faster                                                      |
| regex_dna               | 126 ms                                                      | 114 ms: 1.10x faster                                                       |
| gc_traversal            | 1.52 ms                                                     | 1.41 ms: 1.08x faster                                                      |
| pickle_list             | 2.83 us                                                     | 2.65 us: 1.06x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                      |
| 2to3                    | 218 ms                                                      | 206 ms: 1.06x faster                                                       |
| python_startup          | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                      |
| python_startup_no_site  | 16.2 ms                                                     | 15.4 ms: 1.06x faster                                                      |
| float                   | 56.8 ms                                                     | 53.9 ms: 1.05x faster                                                      |
| docutils                | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                     |
| nbody                   | 71.9 ms                                                     | 68.7 ms: 1.05x faster                                                      |
| xml_etree_generate      | 55.8 ms                                                     | 53.4 ms: 1.05x faster                                                      |
| pidigits                | 152 ms                                                      | 146 ms: 1.04x faster                                                       |
| xml_etree_iterparse     | 65.2 ms                                                     | 62.7 ms: 1.04x faster                                                      |
| sqlite_synth            | 1.76 us                                                     | 1.70 us: 1.04x faster                                                      |
| aiohttp                 | 884 us                                                      | 860 us: 1.03x faster                                                       |
| telco                   | 4.13 ms                                                     | 4.02 ms: 1.03x faster                                                      |
| sqlalchemy_declarative  | 86.4 ms                                                     | 84.7 ms: 1.02x faster                                                      |
| pprint_safe_repr        | 513 ms                                                      | 515 ms: 1.00x slower                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                      |
| scimark_fft             | 184 ms                                                      | 186 ms: 1.01x slower                                                       |
| pycparser               | 699 ms                                                      | 706 ms: 1.01x slower                                                       |
| json_loads              | 13.9 us                                                     | 14.1 us: 1.01x slower                                                      |
| scimark_monte_carlo     | 43.7 ms                                                     | 44.3 ms: 1.01x slower                                                      |
| unpickle_list           | 2.75 us                                                     | 2.80 us: 1.02x slower                                                      |
| unpickle                | 8.18 us                                                     | 8.32 us: 1.02x slower                                                      |
| fannkuch                | 247 ms                                                      | 251 ms: 1.02x slower                                                       |
| mako                    | 7.09 ms                                                     | 7.23 ms: 1.02x slower                                                      |
| pprint_pformat          | 1.05 sec                                                    | 1.07 sec: 1.02x slower                                                     |
| xml_etree_parse         | 93.0 ms                                                     | 95.1 ms: 1.02x slower                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 2.14 us: 1.02x slower                                                      |
| sqlglot_normalize       | 187 ms                                                      | 192 ms: 1.03x slower                                                       |
| tornado_http            | 89.5 ms                                                     | 91.9 ms: 1.03x slower                                                      |
| sympy_expand            | 284 ms                                                      | 291 ms: 1.03x slower                                                       |
| dask                    | 263 ms                                                      | 270 ms: 1.03x slower                                                       |
| async_tree_io           | 731 ms                                                      | 753 ms: 1.03x slower                                                       |
| chameleon               | 4.98 ms                                                     | 5.14 ms: 1.03x slower                                                      |
| deepcopy                | 238 us                                                      | 246 us: 1.03x slower                                                       |
| coroutines              | 14.3 ms                                                     | 14.8 ms: 1.04x slower                                                      |
| pyflate                 | 295 ms                                                      | 306 ms: 1.04x slower                                                       |
| async_tree_cpu_io_mixed | 489 ms                                                      | 508 ms: 1.04x slower                                                       |
| regex_compile           | 87.5 ms                                                     | 90.8 ms: 1.04x slower                                                      |
| sympy_str               | 175 ms                                                      | 182 ms: 1.04x slower                                                       |
| pickle_pure_python      | 195 us                                                      | 204 us: 1.04x slower                                                       |
| crypto_pyaes            | 48.5 ms                                                     | 50.6 ms: 1.04x slower                                                      |
| sympy_sum               | 91.5 ms                                                     | 95.8 ms: 1.05x slower                                                      |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.68 ms: 1.05x slower                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.70 ms: 1.05x slower                                                      |
| sympy_integrate         | 13.0 ms                                                     | 13.7 ms: 1.06x slower                                                      |
| raytrace                | 192 ms                                                      | 204 ms: 1.06x slower                                                       |
| logging_simple          | 6.28 us                                                     | 6.68 us: 1.06x slower                                                      |
| scimark_lu              | 58.9 ms                                                     | 62.7 ms: 1.07x slower                                                      |
| deepcopy_memo           | 23.7 us                                                     | 25.3 us: 1.07x slower                                                      |
| logging_format          | 6.72 us                                                     | 7.19 us: 1.07x slower                                                      |
| nqueens                 | 62.8 ms                                                     | 67.6 ms: 1.08x slower                                                      |
| go                      | 91.6 ms                                                     | 99.5 ms: 1.09x slower                                                      |
| async_tree_none         | 291 ms                                                      | 317 ms: 1.09x slower                                                       |
| django_template         | 22.9 ms                                                     | 25.0 ms: 1.09x slower                                                      |
| json                    | 3.05 ms                                                     | 3.32 ms: 1.09x slower                                                      |
| spectral_norm           | 66.9 ms                                                     | 73.7 ms: 1.10x slower                                                      |
| async_tree_memoization  | 339 ms                                                      | 375 ms: 1.10x slower                                                       |
| sqlglot_transpile       | 1.02 ms                                                     | 1.13 ms: 1.11x slower                                                      |
| comprehensions          | 14.1 us                                                     | 15.7 us: 1.11x slower                                                      |
| richards                | 28.4 ms                                                     | 31.7 ms: 1.12x slower                                                      |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.4 ms: 1.12x slower                                                      |
| hexiom                  | 4.10 ms                                                     | 4.61 ms: 1.12x slower                                                      |
| chaos                   | 43.3 ms                                                     | 48.7 ms: 1.12x slower                                                      |
| unpickle_pure_python    | 133 us                                                      | 152 us: 1.14x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 936 us: 1.16x slower                                                       |
| logging_silent          | 60.5 ns                                                     | 72.4 ns: 1.20x slower                                                      |
| unpack_sequence         | 37.5 ns                                                     | 45.4 ns: 1.21x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.67 sec: 1.22x slower                                                     |
| deltablue               | 2.16 ms                                                     | 2.66 ms: 1.23x slower                                                      |
| coverage                | 40.8 ms                                                     | 54.1 ms: 1.32x slower                                                      |
| json_dumps              | 5.70 ms                                                     | 7.78 ms: 1.37x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 675 ms: 1.38x slower                                                       |
| generators              | 22.5 ms                                                     | 33.9 ms: 1.51x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.04x slower                                                               |

Benchmark hidden because not significant (6): scimark_sor, dulwich_log, pickle_dict, xml_etree_process, bench_thread_pool, meteor_contest
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220711-3.11.0b4-5a7e1e0/bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.91% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown