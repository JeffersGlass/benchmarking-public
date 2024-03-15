
# Results vs. 3.10.4

- fork: python
- ref: 2e49bd06c5ffab7d1540
- machine: darwin-arm64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.17x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 156 ms: 1.23x faster                                                  |
| chameleon      | 6.26 ms                                                | 4.32 ms: 1.45x faster                                                 |
| docutils       | 1.73 sec                                               | 1.40 sec: 1.24x faster                                                |
| html5lib       | 42.4 ms                                                | 32.3 ms: 1.31x faster                                                 |
| tornado_http   | 86.7 ms                                                | 70.6 ms: 1.23x faster                                                 |
| Geometric mean | (ref)                                                  | 1.29x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_io           | 980 ms                                                 | 693 ms: 1.41x faster                                                  |
| async_tree_none         | 388 ms                                                 | 277 ms: 1.40x faster                                                  |
| async_tree_memoization  | 474 ms                                                 | 361 ms: 1.31x faster                                                  |
| async_tree_cpu_io_mixed | 649 ms                                                 | 516 ms: 1.26x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.34x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 69.0 ms                                                | 49.9 ms: 1.38x faster                                                 |
| nbody          | 93.0 ms                                                | 67.4 ms: 1.38x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.24x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.7 ms: 1.29x faster                                                 |
| regex_effbot   | 2.46 ms                                                | 2.07 ms: 1.19x faster                                                 |
| regex_dna      | 174 ms                                                 | 175 ms: 1.00x slower                                                  |
| regex_v8       | 17.1 ms                                                | 19.3 ms: 1.13x slower                                                 |
| Geometric mean | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 190 us: 1.48x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 34.6 ms: 1.35x faster                                                 |
| unpickle_pure_python | 194 us                                                 | 149 us: 1.31x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.36 sec: 1.25x faster                                                |
| xml_etree_generate   | 53.5 ms                                                | 47.0 ms: 1.14x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 97.0 ms: 1.11x faster                                                 |
| json_loads           | 16.4 us                                                | 14.9 us: 1.10x faster                                                 |
| xml_etree_iterparse  | 72.1 ms                                                | 67.4 ms: 1.07x faster                                                 |
| json_dumps           | 8.11 ms                                                | 7.58 ms: 1.07x faster                                                 |
| unpickle             | 8.80 us                                                | 8.31 us: 1.06x faster                                                 |
| pickle_list          | 2.74 us                                                | 2.66 us: 1.03x faster                                                 |
| pickle_dict          | 17.0 us                                                | 17.4 us: 1.02x slower                                                 |
| pickle               | 6.97 us                                                | 7.19 us: 1.03x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.80 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| python_startup_no_site | 7.91 ms                                                | 9.19 ms: 1.16x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.10x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 9.87 ms                                                | 7.05 ms: 1.40x faster                                                 |
| django_template | 26.4 ms                                                | 20.0 ms: 1.32x faster                                                 |
| genshi_text     | 17.3 ms                                                | 14.0 ms: 1.24x faster                                                 |
| genshi_xml      | 33.8 ms                                                | 29.7 ms: 1.14x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.27x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue               | 4.91 ms                                                | 2.69 ms: 1.83x faster                                                 |
| logging_silent          | 117 ns                                                 | 70.1 ns: 1.67x faster                                                 |
| richards                | 48.7 ms                                                | 31.3 ms: 1.55x faster                                                 |
| scimark_sor             | 128 ms                                                 | 82.8 ms: 1.55x faster                                                 |
| richards_super          | 57.8 ms                                                | 37.9 ms: 1.52x faster                                                 |
| pickle_pure_python      | 281 us                                                 | 190 us: 1.48x faster                                                  |
| scimark_monte_carlo     | 65.6 ms                                                | 44.6 ms: 1.47x faster                                                 |
| raytrace                | 301 ms                                                 | 207 ms: 1.46x faster                                                  |
| chameleon               | 6.26 ms                                                | 4.32 ms: 1.45x faster                                                 |
| scimark_lu              | 103 ms                                                 | 71.2 ms: 1.44x faster                                                 |
| go                      | 151 ms                                                 | 105 ms: 1.44x faster                                                  |
| pyflate                 | 427 ms                                                 | 297 ms: 1.44x faster                                                  |
| async_tree_io           | 980 ms                                                 | 693 ms: 1.41x faster                                                  |
| mako                    | 9.87 ms                                                | 7.05 ms: 1.40x faster                                                 |
| async_tree_none         | 388 ms                                                 | 277 ms: 1.40x faster                                                  |
| deepcopy_memo           | 34.7 us                                                | 24.8 us: 1.40x faster                                                 |
| float                   | 69.0 ms                                                | 49.9 ms: 1.38x faster                                                 |
| nbody                   | 93.0 ms                                                | 67.4 ms: 1.38x faster                                                 |
| thrift                  | 572 us                                                 | 421 us: 1.36x faster                                                  |
| chaos                   | 65.8 ms                                                | 48.7 ms: 1.35x faster                                                 |
| logging_format          | 4.83 us                                                | 3.58 us: 1.35x faster                                                 |
| crypto_pyaes            | 71.8 ms                                                | 53.4 ms: 1.35x faster                                                 |
| xml_etree_process       | 46.5 ms                                                | 34.6 ms: 1.35x faster                                                 |
| spectral_norm           | 94.8 ms                                                | 70.9 ms: 1.34x faster                                                 |
| logging_simple          | 4.45 us                                                | 3.35 us: 1.33x faster                                                 |
| django_template         | 26.4 ms                                                | 20.0 ms: 1.32x faster                                                 |
| html5lib                | 42.4 ms                                                | 32.3 ms: 1.31x faster                                                 |
| async_tree_memoization  | 474 ms                                                 | 361 ms: 1.31x faster                                                  |
| unpickle_pure_python    | 194 us                                                 | 149 us: 1.31x faster                                                  |
| pprint_safe_repr        | 641 ms                                                 | 492 ms: 1.30x faster                                                  |
| pprint_pformat          | 1.30 sec                                               | 1.00 sec: 1.30x faster                                                |
| regex_compile           | 95.3 ms                                                | 73.7 ms: 1.29x faster                                                 |
| pycparser               | 877 ms                                                 | 684 ms: 1.28x faster                                                  |
| deepcopy                | 272 us                                                 | 212 us: 1.28x faster                                                  |
| hexiom                  | 6.19 ms                                                | 4.85 ms: 1.28x faster                                                 |
| deepcopy_reduce         | 2.33 us                                                | 1.83 us: 1.27x faster                                                 |
| async_tree_cpu_io_mixed | 649 ms                                                 | 516 ms: 1.26x faster                                                  |
| tomli_loads             | 1.71 sec                                               | 1.36 sec: 1.25x faster                                                |
| docutils                | 1.73 sec                                               | 1.40 sec: 1.24x faster                                                |
| genshi_text             | 17.3 ms                                                | 14.0 ms: 1.24x faster                                                 |
| 2to3                    | 192 ms                                                 | 156 ms: 1.23x faster                                                  |
| tornado_http            | 86.7 ms                                                | 70.6 ms: 1.23x faster                                                 |
| async_generators        | 231 ms                                                 | 189 ms: 1.22x faster                                                  |
| dulwich_log             | 35.3 ms                                                | 28.9 ms: 1.22x faster                                                 |
| create_gc_cycles        | 860 us                                                 | 706 us: 1.22x faster                                                  |
| sqlalchemy_imperative   | 8.86 ms                                                | 7.31 ms: 1.21x faster                                                 |
| sqlalchemy_declarative  | 73.3 ms                                                | 60.7 ms: 1.21x faster                                                 |
| scimark_fft             | 224 ms                                                 | 187 ms: 1.20x faster                                                  |
| sqlglot_optimize        | 36.8 ms                                                | 30.7 ms: 1.20x faster                                                 |
| fannkuch                | 303 ms                                                 | 254 ms: 1.19x faster                                                  |
| regex_effbot            | 2.46 ms                                                | 2.07 ms: 1.19x faster                                                 |
| sympy_sum               | 92.2 ms                                                | 78.2 ms: 1.18x faster                                                 |
| sympy_integrate         | 13.1 ms                                                | 11.2 ms: 1.18x faster                                                 |
| unpack_sequence         | 39.0 ns                                                | 33.7 ns: 1.16x faster                                                 |
| sqlite_synth            | 1.46 us                                                | 1.26 us: 1.15x faster                                                 |
| coroutines              | 20.7 ms                                                | 17.9 ms: 1.15x faster                                                 |
| sympy_str               | 165 ms                                                 | 144 ms: 1.15x faster                                                  |
| sympy_expand            | 269 ms                                                 | 234 ms: 1.15x faster                                                  |
| sqlglot_normalize       | 190 ms                                                 | 166 ms: 1.15x faster                                                  |
| nqueens                 | 63.8 ms                                                | 55.8 ms: 1.14x faster                                                 |
| genshi_xml              | 33.8 ms                                                | 29.7 ms: 1.14x faster                                                 |
| xml_etree_generate      | 53.5 ms                                                | 47.0 ms: 1.14x faster                                                 |
| scimark_sparse_mat_mult | 3.42 ms                                                | 3.04 ms: 1.13x faster                                                 |
| json                    | 3.08 ms                                                | 2.75 ms: 1.12x faster                                                 |
| asyncio_tcp_ssl         | 1.60 sec                                               | 1.43 sec: 1.12x faster                                                |
| aiohttp                 | 1.22 ms                                                | 1.09 ms: 1.12x faster                                                 |
| sqlglot_transpile       | 1.44 ms                                                | 1.30 ms: 1.11x faster                                                 |
| xml_etree_parse         | 108 ms                                                 | 97.0 ms: 1.11x faster                                                 |
| pylint                  | 277 ms                                                 | 249 ms: 1.11x faster                                                  |
| flaskblogging           | 2.65 ms                                                | 2.39 ms: 1.11x faster                                                 |
| telco                   | 3.49 ms                                                | 3.15 ms: 1.11x faster                                                 |
| gunicorn                | 1.30 ms                                                | 1.18 ms: 1.11x faster                                                 |
| json_loads              | 16.4 us                                                | 14.9 us: 1.10x faster                                                 |
| sqlglot_parse           | 1.24 ms                                                | 1.15 ms: 1.08x faster                                                 |
| bench_thread_pool       | 527 us                                                 | 487 us: 1.08x faster                                                  |
| generators              | 32.3 ms                                                | 30.1 ms: 1.07x faster                                                 |
| xml_etree_iterparse     | 72.1 ms                                                | 67.4 ms: 1.07x faster                                                 |
| json_dumps              | 8.11 ms                                                | 7.58 ms: 1.07x faster                                                 |
| pathlib                 | 24.5 ms                                                | 23.1 ms: 1.06x faster                                                 |
| unpickle                | 8.80 us                                                | 8.31 us: 1.06x faster                                                 |
| meteor_contest          | 77.7 ms                                                | 73.9 ms: 1.05x faster                                                 |
| comprehensions          | 16.9 us                                                | 16.3 us: 1.04x faster                                                 |
| pickle_list             | 2.74 us                                                | 2.66 us: 1.03x faster                                                 |
| pidigits                | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| asyncio_websockets      | 410 ms                                                 | 407 ms: 1.01x faster                                                  |
| regex_dna               | 174 ms                                                 | 175 ms: 1.00x slower                                                  |
| asyncio_tcp             | 659 ms                                                 | 663 ms: 1.01x slower                                                  |
| gc_traversal            | 2.36 ms                                                | 2.38 ms: 1.01x slower                                                 |
| pickle_dict             | 17.0 us                                                | 17.4 us: 1.02x slower                                                 |
| pickle                  | 6.97 us                                                | 7.19 us: 1.03x slower                                                 |
| unpickle_list           | 2.69 us                                                | 2.80 us: 1.04x slower                                                 |
| python_startup          | 10.9 ms                                                | 11.4 ms: 1.05x slower                                                 |
| mdp                     | 1.63 sec                                               | 1.76 sec: 1.08x slower                                                |
| bench_mp_pool           | 37.4 ms                                                | 41.5 ms: 1.11x slower                                                 |
| regex_v8                | 17.1 ms                                                | 19.3 ms: 1.13x slower                                                 |
| python_startup_no_site  | 7.91 ms                                                | 9.19 ms: 1.16x slower                                                 |
| coverage                | 41.5 ms                                                | 392 ms: 9.45x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.17x faster                                                          |

Benchmark hidden because not significant (1): typing_runtime_protocols
Ignored benchmarks (2) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: dask, mypy2
Ignored benchmarks (4) of results/bm-20220405-3.11.0a7-2e49bd0/bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.09x