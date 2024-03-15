
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_cold
- machine: windows-amd64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 223 ms: 1.10x faster                                                     |
| chameleon      | 5.79 ms                                                     | 4.82 ms: 1.20x faster                                                    |
| docutils       | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                   |
| tornado_http   | 108 ms                                                      | 87.3 ms: 1.24x faster                                                    |
| Geometric mean | (ref)                                                       | 1.18x faster                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 264 ms: 1.65x faster                                                     |
| async_tree_memoization  | 526 ms                                                      | 344 ms: 1.53x faster                                                     |
| async_tree_io           | 1.11 sec                                                    | 738 ms: 1.50x faster                                                     |
| async_tree_cpu_io_mixed | 638 ms                                                      | 468 ms: 1.36x faster                                                     |
| Geometric mean          | (ref)                                                       | 1.51x faster                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.8 ms: 1.21x faster                                                    |
| nbody          | 71.3 ms                                                     | 61.9 ms: 1.15x faster                                                    |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                                     |
| Geometric mean | (ref)                                                       | 1.11x faster                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 81.6 ms: 1.30x faster                                                    |
| regex_dna      | 136 ms                                                      | 118 ms: 1.15x faster                                                     |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                    |
| regex_v8       | 15.4 ms                                                     | 17.2 ms: 1.12x slower                                                    |
| Geometric mean | (ref)                                                       | 1.09x faster                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.54 ms: 1.65x faster                                                    |
| pickle_pure_python   | 270 us                                                      | 175 us: 1.54x faster                                                     |
| unpickle_pure_python | 183 us                                                      | 126 us: 1.46x faster                                                     |
| tomli_loads          | 1.67 sec                                                    | 1.32 sec: 1.26x faster                                                   |
| xml_etree_process    | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                    |
| unpickle             | 9.09 us                                                     | 8.82 us: 1.03x faster                                                    |
| xml_etree_parse      | 96.8 ms                                                     | 95.2 ms: 1.02x faster                                                    |
| json_loads           | 14.0 us                                                     | 14.1 us: 1.00x slower                                                    |
| pickle_list          | 2.75 us                                                     | 2.78 us: 1.01x slower                                                    |
| xml_etree_generate   | 55.5 ms                                                     | 56.3 ms: 1.01x slower                                                    |
| unpickle_list        | 2.71 us                                                     | 2.76 us: 1.02x slower                                                    |
| xml_etree_iterparse  | 65.0 ms                                                     | 66.6 ms: 1.02x slower                                                    |
| pickle_dict          | 17.2 us                                                     | 18.0 us: 1.05x slower                                                    |
| pickle               | 6.85 us                                                     | 7.30 us: 1.07x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.12x faster                                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 21.3 ms: 1.03x slower                                                    |
| python_startup_no_site | 15.5 ms                                                     | 19.2 ms: 1.24x slower                                                    |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.68 ms: 1.35x faster                                                    |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 72.1 us: 4.66x faster                                                    |
| deltablue                | 4.19 ms                                                     | 2.14 ms: 1.96x faster                                                    |
| richards_super           | 52.2 ms                                                     | 29.0 ms: 1.80x faster                                                    |
| logging_silent           | 94.6 ns                                                     | 53.2 ns: 1.78x faster                                                    |
| json_dumps               | 9.16 ms                                                     | 5.54 ms: 1.65x faster                                                    |
| richards                 | 42.4 ms                                                     | 25.7 ms: 1.65x faster                                                    |
| async_tree_none          | 435 ms                                                      | 264 ms: 1.65x faster                                                     |
| sqlglot_parse            | 1.22 ms                                                     | 752 us: 1.62x faster                                                     |
| raytrace                 | 273 ms                                                      | 173 ms: 1.58x faster                                                     |
| generators               | 32.4 ms                                                     | 20.8 ms: 1.56x faster                                                    |
| pickle_pure_python       | 270 us                                                      | 175 us: 1.54x faster                                                     |
| async_tree_memoization   | 526 ms                                                      | 344 ms: 1.53x faster                                                     |
| scimark_lu               | 85.8 ms                                                     | 56.0 ms: 1.53x faster                                                    |
| async_tree_io            | 1.11 sec                                                    | 738 ms: 1.50x faster                                                     |
| sqlglot_transpile        | 1.48 ms                                                     | 990 us: 1.49x faster                                                     |
| asyncio_tcp              | 732 ms                                                      | 494 ms: 1.48x faster                                                     |
| unpickle_pure_python     | 183 us                                                      | 126 us: 1.46x faster                                                     |
| scimark_sor              | 106 ms                                                      | 74.4 ms: 1.43x faster                                                    |
| chaos                    | 61.7 ms                                                     | 43.9 ms: 1.41x faster                                                    |
| comprehensions           | 16.5 us                                                     | 11.9 us: 1.39x faster                                                    |
| go                       | 139 ms                                                      | 100 ms: 1.39x faster                                                     |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 468 ms: 1.36x faster                                                     |
| mako                     | 9.03 ms                                                     | 6.68 ms: 1.35x faster                                                    |
| crypto_pyaes             | 62.5 ms                                                     | 47.0 ms: 1.33x faster                                                    |
| deepcopy_memo            | 28.8 us                                                     | 21.6 us: 1.33x faster                                                    |
| pycparser                | 930 ms                                                      | 701 ms: 1.33x faster                                                     |
| pyflate                  | 409 ms                                                      | 313 ms: 1.31x faster                                                     |
| regex_compile            | 106 ms                                                      | 81.6 ms: 1.30x faster                                                    |
| tomli_loads              | 1.67 sec                                                    | 1.32 sec: 1.26x faster                                                   |
| mypy2                    | 555 ms                                                      | 441 ms: 1.26x faster                                                     |
| tornado_http             | 108 ms                                                      | 87.3 ms: 1.24x faster                                                    |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                    |
| sqlite_synth             | 1.91 us                                                     | 1.57 us: 1.21x faster                                                    |
| float                    | 61.7 ms                                                     | 50.8 ms: 1.21x faster                                                    |
| pprint_pformat           | 1.22 sec                                                    | 1.01 sec: 1.20x faster                                                   |
| chameleon                | 5.79 ms                                                     | 4.82 ms: 1.20x faster                                                    |
| docutils                 | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                   |
| dask                     | 313 ms                                                      | 264 ms: 1.19x faster                                                     |
| dulwich_log              | 50.5 ms                                                     | 42.5 ms: 1.19x faster                                                    |
| pprint_safe_repr         | 592 ms                                                      | 499 ms: 1.19x faster                                                     |
| sympy_sum                | 107 ms                                                      | 90.9 ms: 1.18x faster                                                    |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.81 sec: 1.16x faster                                                   |
| xml_etree_process        | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                    |
| deepcopy                 | 255 us                                                      | 221 us: 1.16x faster                                                     |
| regex_dna                | 136 ms                                                      | 118 ms: 1.15x faster                                                     |
| nbody                    | 71.3 ms                                                     | 61.9 ms: 1.15x faster                                                    |
| sympy_str                | 194 ms                                                      | 169 ms: 1.15x faster                                                     |
| deepcopy_reduce          | 2.20 us                                                     | 1.93 us: 1.14x faster                                                    |
| sqlglot_optimize         | 39.8 ms                                                     | 34.8 ms: 1.14x faster                                                    |
| spectral_norm            | 77.3 ms                                                     | 67.7 ms: 1.14x faster                                                    |
| sqlglot_normalize        | 205 ms                                                      | 181 ms: 1.14x faster                                                     |
| sympy_integrate          | 15.3 ms                                                     | 13.5 ms: 1.13x faster                                                    |
| bench_thread_pool        | 958 us                                                      | 855 us: 1.12x faster                                                     |
| nqueens                  | 66.6 ms                                                     | 59.7 ms: 1.12x faster                                                    |
| 2to3                     | 246 ms                                                      | 223 ms: 1.10x faster                                                     |
| create_gc_cycles         | 800 us                                                      | 736 us: 1.09x faster                                                     |
| sympy_expand             | 314 ms                                                      | 290 ms: 1.09x faster                                                     |
| mdp                      | 1.78 sec                                                    | 1.68 sec: 1.06x faster                                                   |
| json                     | 3.14 ms                                                     | 2.96 ms: 1.06x faster                                                    |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                    |
| hexiom                   | 5.74 ms                                                     | 5.52 ms: 1.04x faster                                                    |
| fannkuch                 | 256 ms                                                      | 247 ms: 1.04x faster                                                     |
| logging_simple           | 6.22 us                                                     | 6.03 us: 1.03x faster                                                    |
| unpickle                 | 9.09 us                                                     | 8.82 us: 1.03x faster                                                    |
| logging_format           | 6.76 us                                                     | 6.58 us: 1.03x faster                                                    |
| xml_etree_parse          | 96.8 ms                                                     | 95.2 ms: 1.02x faster                                                    |
| scimark_monte_carlo      | 57.3 ms                                                     | 56.6 ms: 1.01x faster                                                    |
| json_loads               | 14.0 us                                                     | 14.1 us: 1.00x slower                                                    |
| pickle_list              | 2.75 us                                                     | 2.78 us: 1.01x slower                                                    |
| xml_etree_generate       | 55.5 ms                                                     | 56.3 ms: 1.01x slower                                                    |
| unpickle_list            | 2.71 us                                                     | 2.76 us: 1.02x slower                                                    |
| meteor_contest           | 75.9 ms                                                     | 77.5 ms: 1.02x slower                                                    |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                                     |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.79 ms: 1.02x slower                                                    |
| xml_etree_iterparse      | 65.0 ms                                                     | 66.6 ms: 1.02x slower                                                    |
| python_startup           | 20.6 ms                                                     | 21.3 ms: 1.03x slower                                                    |
| pickle_dict              | 17.2 us                                                     | 18.0 us: 1.05x slower                                                    |
| scimark_fft              | 187 ms                                                      | 197 ms: 1.05x slower                                                     |
| pickle                   | 6.85 us                                                     | 7.30 us: 1.07x slower                                                    |
| pathlib                  | 75.7 ms                                                     | 82.0 ms: 1.08x slower                                                    |
| gc_traversal             | 1.41 ms                                                     | 1.55 ms: 1.10x slower                                                    |
| unpack_sequence          | 39.6 ns                                                     | 43.9 ns: 1.11x slower                                                    |
| regex_v8                 | 15.4 ms                                                     | 17.2 ms: 1.12x slower                                                    |
| async_generators         | 222 ms                                                      | 248 ms: 1.12x slower                                                     |
| bench_mp_pool            | 62.0 ms                                                     | 70.0 ms: 1.13x slower                                                    |
| telco                    | 3.94 ms                                                     | 4.57 ms: 1.16x slower                                                    |
| coverage                 | 39.0 ms                                                     | 47.3 ms: 1.21x slower                                                    |
| python_startup_no_site   | 15.5 ms                                                     | 19.2 ms: 1.24x slower                                                    |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                             |
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240202-3.13.0a3+-ad30059-JIT/bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown