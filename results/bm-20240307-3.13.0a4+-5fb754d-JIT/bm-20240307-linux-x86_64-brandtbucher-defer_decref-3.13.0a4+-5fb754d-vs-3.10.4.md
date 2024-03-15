# Results vs. 3.10.4

- fork: brandtbucher
- ref: defer_decref
- machine: linux-x86_64
- commit hash: 5fb754d
- commit date: 2024-03-07
- overall geometric mean: 1.22x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.34x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 301 ms: 1.16x faster                                                 |
| chameleon      | 9.68 ms                                                | 7.48 ms: 1.30x faster                                                |
| docutils       | 3.30 sec                                               | 2.90 sec: 1.14x faster                                               |
| html5lib       | 88.9 ms                                                | 71.7 ms: 1.24x faster                                                |
| tornado_http   | 136 ms                                                 | 107 ms: 1.27x faster                                                 |
| Geometric mean | (ref)                                                  | 1.22x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 459 ms: 1.59x faster                                                 |
| async_tree_memoization  | 870 ms                                                 | 591 ms: 1.47x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.23 sec: 1.43x faster                                               |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 744 ms: 1.37x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.46x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 107 ms: 1.43x faster                                                 |
| float          | 117 ms                                                 | 84.6 ms: 1.38x faster                                                |
| pidigits       | 191 ms                                                 | 192 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.25x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 156 ms: 1.20x faster                                                 |
| regex_v8       | 27.8 ms                                                | 25.8 ms: 1.08x faster                                                |
| regex_dna      | 227 ms                                                 | 224 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.07x faster                                                         |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 336 us: 1.44x faster                                                 |
| tomli_loads          | 3.14 sec                                               | 2.35 sec: 1.33x faster                                               |
| json_dumps           | 14.2 ms                                                | 10.9 ms: 1.30x faster                                                |
| unpickle_pure_python | 331 us                                                 | 259 us: 1.27x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 64.1 ms: 1.23x faster                                                |
| json_loads           | 31.2 us                                                | 27.9 us: 1.12x faster                                                |
| xml_etree_generate   | 99.4 ms                                                | 90.2 ms: 1.10x faster                                                |
| xml_etree_parse      | 168 ms                                                 | 160 ms: 1.05x faster                                                 |
| unpickle_list        | 5.20 us                                                | 5.03 us: 1.03x faster                                                |
| xml_etree_iterparse  | 115 ms                                                 | 113 ms: 1.02x faster                                                 |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.02x faster                                                |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                                |
| pickle               | 10.7 us                                                | 11.7 us: 1.09x slower                                                |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.17x slower                                                |
| Geometric mean       | (ref)                                                  | 1.10x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 13.4 ms: 1.09x faster                                                |
| python_startup_no_site | 5.93 ms                                                | 11.9 ms: 2.00x slower                                                |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 12.4 ms: 1.32x faster                                                |
| django_template | 48.2 ms                                                | 38.0 ms: 1.27x faster                                                |
| genshi_text     | 31.8 ms                                                | 26.4 ms: 1.21x faster                                                |
| genshi_xml      | 66.0 ms                                                | 58.3 ms: 1.13x faster                                                |
| Geometric mean  | (ref)                                                  | 1.23x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 119 us: 4.56x faster                                                 |
| generators               | 80.1 ms                                                | 30.7 ms: 2.61x faster                                                |
| deltablue                | 7.91 ms                                                | 3.90 ms: 2.03x faster                                                |
| asyncio_tcp              | 922 ms                                                 | 513 ms: 1.80x faster                                                 |
| logging_silent           | 190 ns                                                 | 107 ns: 1.77x faster                                                 |
| richards_super           | 94.7 ms                                                | 57.7 ms: 1.64x faster                                                |
| chaos                    | 115 ms                                                 | 71.3 ms: 1.62x faster                                                |
| async_tree_none          | 728 ms                                                 | 459 ms: 1.59x faster                                                 |
| pylint                   | 551 ms                                                 | 348 ms: 1.59x faster                                                 |
| raytrace                 | 507 ms                                                 | 323 ms: 1.57x faster                                                 |
| richards                 | 79.3 ms                                                | 51.8 ms: 1.53x faster                                                |
| scimark_monte_carlo      | 118 ms                                                 | 77.5 ms: 1.53x faster                                                |
| crypto_pyaes             | 128 ms                                                 | 84.6 ms: 1.51x faster                                                |
| sqlglot_parse            | 2.17 ms                                                | 1.45 ms: 1.50x faster                                                |
| comprehensions           | 28.8 us                                                | 19.3 us: 1.49x faster                                                |
| async_tree_memoization   | 870 ms                                                 | 591 ms: 1.47x faster                                                 |
| pickle_pure_python       | 484 us                                                 | 336 us: 1.44x faster                                                 |
| async_tree_io            | 1.77 sec                                               | 1.23 sec: 1.43x faster                                               |
| nbody                    | 154 ms                                                 | 107 ms: 1.43x faster                                                 |
| sqlglot_transpile        | 2.57 ms                                                | 1.81 ms: 1.42x faster                                                |
| scimark_sor              | 220 ms                                                 | 154 ms: 1.42x faster                                                 |
| deepcopy_memo            | 58.5 us                                                | 42.1 us: 1.39x faster                                                |
| float                    | 117 ms                                                 | 84.6 ms: 1.38x faster                                                |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.86 sec: 1.38x faster                                               |
| go                       | 240 ms                                                 | 175 ms: 1.38x faster                                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 744 ms: 1.37x faster                                                 |
| spectral_norm            | 170 ms                                                 | 124 ms: 1.37x faster                                                 |
| coroutines               | 35.1 ms                                                | 26.0 ms: 1.35x faster                                                |
| tomli_loads              | 3.14 sec                                               | 2.35 sec: 1.33x faster                                               |
| mako                     | 16.3 ms                                                | 12.4 ms: 1.32x faster                                                |
| hexiom                   | 10.4 ms                                                | 7.90 ms: 1.32x faster                                                |
| logging_simple           | 8.30 us                                                | 6.34 us: 1.31x faster                                                |
| pyflate                  | 716 ms                                                 | 548 ms: 1.31x faster                                                 |
| logging_format           | 9.09 us                                                | 6.97 us: 1.30x faster                                                |
| json_dumps               | 14.2 ms                                                | 10.9 ms: 1.30x faster                                                |
| chameleon                | 9.68 ms                                                | 7.48 ms: 1.30x faster                                                |
| thrift                   | 1.07 ms                                                | 831 us: 1.29x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 259 us: 1.27x faster                                                 |
| tornado_http             | 136 ms                                                 | 107 ms: 1.27x faster                                                 |
| deepcopy                 | 479 us                                                 | 378 us: 1.27x faster                                                 |
| django_template          | 48.2 ms                                                | 38.0 ms: 1.27x faster                                                |
| pprint_pformat           | 2.10 sec                                               | 1.67 sec: 1.26x faster                                               |
| deepcopy_reduce          | 4.17 us                                                | 3.32 us: 1.26x faster                                                |
| sqlglot_normalize        | 143 ms                                                 | 115 ms: 1.25x faster                                                 |
| scimark_lu               | 176 ms                                                 | 142 ms: 1.24x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 821 ms: 1.24x faster                                                 |
| html5lib                 | 88.9 ms                                                | 71.7 ms: 1.24x faster                                                |
| scimark_fft              | 466 ms                                                 | 376 ms: 1.24x faster                                                 |
| xml_etree_process        | 79.1 ms                                                | 64.1 ms: 1.23x faster                                                |
| genshi_text              | 31.8 ms                                                | 26.4 ms: 1.21x faster                                                |
| regex_compile            | 188 ms                                                 | 156 ms: 1.20x faster                                                 |
| pycparser                | 1.58 sec                                               | 1.32 sec: 1.20x faster                                               |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.49 ms: 1.18x faster                                                |
| djangocms                | 38.4 us                                                | 32.7 us: 1.18x faster                                                |
| dulwich_log              | 84.3 ms                                                | 72.3 ms: 1.17x faster                                                |
| 2to3                     | 348 ms                                                 | 301 ms: 1.16x faster                                                 |
| sqlglot_optimize         | 69.2 ms                                                | 60.0 ms: 1.15x faster                                                |
| docutils                 | 3.30 sec                                               | 2.90 sec: 1.14x faster                                               |
| genshi_xml               | 66.0 ms                                                | 58.3 ms: 1.13x faster                                                |
| sympy_sum                | 196 ms                                                 | 173 ms: 1.13x faster                                                 |
| sympy_str                | 346 ms                                                 | 307 ms: 1.13x faster                                                 |
| sympy_integrate          | 25.8 ms                                                | 23.0 ms: 1.12x faster                                                |
| json_loads               | 31.2 us                                                | 27.9 us: 1.12x faster                                                |
| aiohttp                  | 1.44 ms                                                | 1.29 ms: 1.12x faster                                                |
| sympy_expand             | 566 ms                                                 | 512 ms: 1.10x faster                                                 |
| xml_etree_generate       | 99.4 ms                                                | 90.2 ms: 1.10x faster                                                |
| gunicorn                 | 1.53 ms                                                | 1.39 ms: 1.10x faster                                                |
| python_startup           | 14.6 ms                                                | 13.4 ms: 1.09x faster                                                |
| regex_v8                 | 27.8 ms                                                | 25.8 ms: 1.08x faster                                                |
| json                     | 5.69 ms                                                | 5.30 ms: 1.07x faster                                                |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.07x faster                                                |
| pathlib                  | 20.5 ms                                                | 19.3 ms: 1.06x faster                                                |
| xml_etree_parse          | 168 ms                                                 | 160 ms: 1.05x faster                                                 |
| fannkuch                 | 532 ms                                                 | 508 ms: 1.05x faster                                                 |
| nqueens                  | 106 ms                                                 | 101 ms: 1.05x faster                                                 |
| unpickle_list            | 5.20 us                                                | 5.03 us: 1.03x faster                                                |
| sqlite_synth             | 3.02 us                                                | 2.95 us: 1.03x faster                                                |
| xml_etree_iterparse      | 115 ms                                                 | 113 ms: 1.02x faster                                                 |
| pickle_list              | 5.08 us                                                | 5.00 us: 1.02x faster                                                |
| regex_dna                | 227 ms                                                 | 224 ms: 1.01x faster                                                 |
| meteor_contest           | 120 ms                                                 | 119 ms: 1.00x faster                                                 |
| pidigits                 | 191 ms                                                 | 192 ms: 1.01x slower                                                 |
| mdp                      | 2.85 sec                                               | 2.90 sec: 1.02x slower                                               |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                                |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                                |
| pickle                   | 10.7 us                                                | 11.7 us: 1.09x slower                                                |
| async_generators         | 444 ms                                                 | 496 ms: 1.12x slower                                                 |
| bench_mp_pool            | 24.0 ms                                                | 28.1 ms: 1.17x slower                                                |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.17x slower                                                |
| telco                    | 7.27 ms                                                | 8.91 ms: 1.23x slower                                                |
| coverage                 | 79.4 ms                                                | 101 ms: 1.27x slower                                                 |
| bench_thread_pool        | 986 us                                                 | 1.58 ms: 1.60x slower                                                |
| python_startup_no_site   | 5.93 ms                                                | 11.9 ms: 2.00x slower                                                |
| Geometric mean           | (ref)                                                  | 1.22x faster                                                         |

Benchmark hidden because not significant (3): asyncio_websockets, regex_effbot, mypy2
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: dask, flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative, unpack_sequence
Ignored benchmarks (4) of results/bm-20240307-3.13.0a4+-5fb754d-JIT/bm-20240307-linux-x86_64-brandtbucher-defer_decref-3.13.0a4+-5fb754d.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.34x