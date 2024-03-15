# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_arena
- machine: windows-amd64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 223 ms: 1.10x faster                                                      |
| chameleon      | 5.79 ms                                                     | 4.85 ms: 1.19x faster                                                     |
| docutils       | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                    |
| html5lib       | 51.0 ms                                                     | 36.3 ms: 1.40x faster                                                     |
| tornado_http   | 108 ms                                                      | 85.2 ms: 1.27x faster                                                     |
| Geometric mean | (ref)                                                       | 1.23x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 269 ms: 1.62x faster                                                      |
| async_tree_memoization  | 526 ms                                                      | 344 ms: 1.53x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 731 ms: 1.52x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 452 ms: 1.41x faster                                                      |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 49.4 ms: 1.25x faster                                                     |
| nbody          | 71.3 ms                                                     | 57.6 ms: 1.24x faster                                                     |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                       | 1.15x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 77.7 ms: 1.36x faster                                                     |
| regex_dna      | 136 ms                                                      | 125 ms: 1.09x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                     |
| regex_v8       | 15.4 ms                                                     | 15.3 ms: 1.01x faster                                                     |
| Geometric mean | (ref)                                                       | 1.12x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.52 ms: 1.66x faster                                                     |
| pickle_pure_python   | 270 us                                                      | 175 us: 1.54x faster                                                      |
| unpickle_pure_python | 183 us                                                      | 129 us: 1.42x faster                                                      |
| tomli_loads          | 1.67 sec                                                    | 1.18 sec: 1.41x faster                                                    |
| xml_etree_process    | 44.5 ms                                                     | 36.4 ms: 1.22x faster                                                     |
| unpickle             | 9.09 us                                                     | 8.39 us: 1.08x faster                                                     |
| xml_etree_generate   | 55.5 ms                                                     | 52.9 ms: 1.05x faster                                                     |
| xml_etree_parse      | 96.8 ms                                                     | 93.4 ms: 1.04x faster                                                     |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.0 ms: 1.03x faster                                                     |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.03x faster                                                     |
| pickle_dict          | 17.2 us                                                     | 17.4 us: 1.02x slower                                                     |
| pickle               | 6.85 us                                                     | 7.14 us: 1.04x slower                                                     |
| pickle_list          | 2.75 us                                                     | 3.04 us: 1.10x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                              |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 23.4 ms: 1.14x slower                                                     |
| python_startup_no_site | 15.5 ms                                                     | 21.1 ms: 1.36x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.24x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 5.75 ms: 1.57x faster                                                     |
| genshi_text     | 19.8 ms                                                     | 15.2 ms: 1.30x faster                                                     |
| django_template | 28.9 ms                                                     | 22.7 ms: 1.27x faster                                                     |
| genshi_xml      | 41.0 ms                                                     | 34.6 ms: 1.19x faster                                                     |
| Geometric mean  | (ref)                                                       | 1.33x faster                                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 69.5 us: 4.83x faster                                                     |
| deltablue                | 4.19 ms                                                     | 2.09 ms: 2.00x faster                                                     |
| richards_super           | 52.2 ms                                                     | 29.3 ms: 1.78x faster                                                     |
| logging_silent           | 94.6 ns                                                     | 55.9 ns: 1.69x faster                                                     |
| pylint                   | 350 ms                                                      | 210 ms: 1.67x faster                                                      |
| richards                 | 42.4 ms                                                     | 25.5 ms: 1.66x faster                                                     |
| json_dumps               | 9.16 ms                                                     | 5.52 ms: 1.66x faster                                                     |
| async_tree_none          | 435 ms                                                      | 269 ms: 1.62x faster                                                      |
| sqlglot_parse            | 1.22 ms                                                     | 766 us: 1.59x faster                                                      |
| mako                     | 9.03 ms                                                     | 5.75 ms: 1.57x faster                                                     |
| generators               | 32.4 ms                                                     | 20.6 ms: 1.57x faster                                                     |
| comprehensions           | 16.5 us                                                     | 10.5 us: 1.57x faster                                                     |
| chaos                    | 61.7 ms                                                     | 39.4 ms: 1.57x faster                                                     |
| spectral_norm            | 77.3 ms                                                     | 50.0 ms: 1.55x faster                                                     |
| raytrace                 | 273 ms                                                      | 177 ms: 1.54x faster                                                      |
| asyncio_tcp              | 732 ms                                                      | 475 ms: 1.54x faster                                                      |
| pickle_pure_python       | 270 us                                                      | 175 us: 1.54x faster                                                      |
| async_tree_memoization   | 526 ms                                                      | 344 ms: 1.53x faster                                                      |
| async_tree_io            | 1.11 sec                                                    | 731 ms: 1.52x faster                                                      |
| sqlglot_transpile        | 1.48 ms                                                     | 988 us: 1.49x faster                                                      |
| go                       | 139 ms                                                      | 93.9 ms: 1.48x faster                                                     |
| crypto_pyaes             | 62.5 ms                                                     | 42.4 ms: 1.47x faster                                                     |
| pyflate                  | 409 ms                                                      | 280 ms: 1.46x faster                                                      |
| unpickle_pure_python     | 183 us                                                      | 129 us: 1.42x faster                                                      |
| hexiom                   | 5.74 ms                                                     | 4.04 ms: 1.42x faster                                                     |
| tomli_loads              | 1.67 sec                                                    | 1.18 sec: 1.41x faster                                                    |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 452 ms: 1.41x faster                                                      |
| html5lib                 | 51.0 ms                                                     | 36.3 ms: 1.40x faster                                                     |
| scimark_monte_carlo      | 57.3 ms                                                     | 41.4 ms: 1.38x faster                                                     |
| pycparser                | 930 ms                                                      | 673 ms: 1.38x faster                                                      |
| regex_compile            | 106 ms                                                      | 77.7 ms: 1.36x faster                                                     |
| genshi_text              | 19.8 ms                                                     | 15.2 ms: 1.30x faster                                                     |
| mdp                      | 1.78 sec                                                    | 1.38 sec: 1.29x faster                                                    |
| deepcopy_memo            | 28.8 us                                                     | 22.4 us: 1.28x faster                                                     |
| scimark_sor              | 106 ms                                                      | 83.1 ms: 1.28x faster                                                     |
| mypy2                    | 555 ms                                                      | 436 ms: 1.28x faster                                                      |
| django_template          | 28.9 ms                                                     | 22.7 ms: 1.27x faster                                                     |
| tornado_http             | 108 ms                                                      | 85.2 ms: 1.27x faster                                                     |
| pprint_safe_repr         | 592 ms                                                      | 473 ms: 1.25x faster                                                      |
| float                    | 61.7 ms                                                     | 49.4 ms: 1.25x faster                                                     |
| pprint_pformat           | 1.22 sec                                                    | 976 ms: 1.25x faster                                                      |
| nbody                    | 71.3 ms                                                     | 57.6 ms: 1.24x faster                                                     |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.22 ms: 1.23x faster                                                     |
| fannkuch                 | 256 ms                                                      | 209 ms: 1.23x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 36.4 ms: 1.22x faster                                                     |
| docutils                 | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                    |
| dulwich_log              | 50.5 ms                                                     | 41.4 ms: 1.22x faster                                                     |
| sqlite_synth             | 1.91 us                                                     | 1.57 us: 1.22x faster                                                     |
| sympy_sum                | 107 ms                                                      | 88.1 ms: 1.21x faster                                                     |
| coroutines               | 16.0 ms                                                     | 13.2 ms: 1.21x faster                                                     |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.76 sec: 1.20x faster                                                    |
| sympy_str                | 194 ms                                                      | 163 ms: 1.20x faster                                                      |
| chameleon                | 5.79 ms                                                     | 4.85 ms: 1.19x faster                                                     |
| genshi_xml               | 41.0 ms                                                     | 34.6 ms: 1.19x faster                                                     |
| scimark_lu               | 85.8 ms                                                     | 72.7 ms: 1.18x faster                                                     |
| bench_thread_pool        | 958 us                                                      | 825 us: 1.16x faster                                                      |
| sympy_integrate          | 15.3 ms                                                     | 13.2 ms: 1.16x faster                                                     |
| sqlglot_normalize        | 205 ms                                                      | 177 ms: 1.16x faster                                                      |
| deepcopy                 | 255 us                                                      | 221 us: 1.16x faster                                                      |
| sqlglot_optimize         | 39.8 ms                                                     | 34.6 ms: 1.15x faster                                                     |
| sympy_expand             | 314 ms                                                      | 278 ms: 1.13x faster                                                      |
| deepcopy_reduce          | 2.20 us                                                     | 1.95 us: 1.13x faster                                                     |
| scimark_fft              | 187 ms                                                      | 166 ms: 1.13x faster                                                      |
| aiohttp                  | 995 us                                                      | 894 us: 1.11x faster                                                      |
| 2to3                     | 246 ms                                                      | 223 ms: 1.10x faster                                                      |
| regex_dna                | 136 ms                                                      | 125 ms: 1.09x faster                                                      |
| json                     | 3.14 ms                                                     | 2.88 ms: 1.09x faster                                                     |
| unpickle                 | 9.09 us                                                     | 8.39 us: 1.08x faster                                                     |
| nqueens                  | 66.6 ms                                                     | 61.9 ms: 1.08x faster                                                     |
| logging_format           | 6.76 us                                                     | 6.29 us: 1.07x faster                                                     |
| logging_simple           | 6.22 us                                                     | 5.81 us: 1.07x faster                                                     |
| create_gc_cycles         | 800 us                                                      | 748 us: 1.07x faster                                                      |
| unpack_sequence          | 39.6 ns                                                     | 37.7 ns: 1.05x faster                                                     |
| xml_etree_generate       | 55.5 ms                                                     | 52.9 ms: 1.05x faster                                                     |
| regex_effbot             | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                     |
| xml_etree_parse          | 96.8 ms                                                     | 93.4 ms: 1.04x faster                                                     |
| meteor_contest           | 75.9 ms                                                     | 73.6 ms: 1.03x faster                                                     |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.0 ms: 1.03x faster                                                     |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.03x faster                                                     |
| pathlib                  | 75.7 ms                                                     | 74.6 ms: 1.01x faster                                                     |
| regex_v8                 | 15.4 ms                                                     | 15.3 ms: 1.01x faster                                                     |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                                      |
| pickle_dict              | 17.2 us                                                     | 17.4 us: 1.02x slower                                                     |
| pickle                   | 6.85 us                                                     | 7.14 us: 1.04x slower                                                     |
| gc_traversal             | 1.41 ms                                                     | 1.50 ms: 1.06x slower                                                     |
| async_generators         | 222 ms                                                      | 237 ms: 1.07x slower                                                      |
| pickle_list              | 2.75 us                                                     | 3.04 us: 1.10x slower                                                     |
| bench_mp_pool            | 62.0 ms                                                     | 69.2 ms: 1.12x slower                                                     |
| python_startup           | 20.6 ms                                                     | 23.4 ms: 1.14x slower                                                     |
| dask                     | 313 ms                                                      | 363 ms: 1.16x slower                                                      |
| coverage                 | 39.0 ms                                                     | 46.0 ms: 1.18x slower                                                     |
| telco                    | 3.94 ms                                                     | 4.70 ms: 1.19x slower                                                     |
| python_startup_no_site   | 15.5 ms                                                     | 21.1 ms: 1.36x slower                                                     |
| thrift                   | 617 us                                                      | 8.84 ms: 14.31x slower                                                    |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                              |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: unknown