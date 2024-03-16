# Faster CPython Benchmark Infrastructure

🔒 [▶️ START A BENCHMARK RUN](../../actions/workflows/benchmark.yml)

## Results

Here are some recent and important revisions. 👉 [Complete list of results](RESULTS.md).

**Key:** 📄: table, 📈: time plot, 🧠: memory plot

<!-- START table -->
[Most recent pystats on main (8c094c3)](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS/bm-20240313-azure-x86_64-python-main-3.13.0a5%2B-8c094c3-pystats.md)

## linux x86_64 (linux)
| date | fork/ref | hash/flags | vs. 3.10.4: | vs. 3.11.0: | vs. 3.12.0: | vs. base: |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| [2024-03-16](results/bm-20240316-3.13.0a5%2B-f486338-JIT) | jeffersglass/justin_supernodes_on | f486338 (JIT) | 1.33x ↑<br>[📄](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.10.4.md)[📈](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.10.4.png) | 1.04x ↑<br>[📄](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.11.0.md)[📈](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.11.0.png) | 1.02x ↑<br>[📄](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.12.0.md)[📈](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-3.12.0.png) | 1.01x ↑<br>[📄](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-base.md)[📈](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-base.png)[🧠](results/bm-20240316-3.13.0a5%2B-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5%2B-f486338-vs-base-mem.png) |
| [2024-03-15](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT) | faster-cpython/hot_cold_with_fixes | 22ff3c3 (JIT) | 1.29x ↑<br>[📄](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-3.10.4.md)[📈](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-3.11.0.md)[📈](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-3.12.0.md)[📈](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-3.12.0.png) | 1.00x ↑<br>[📄](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-base.md)[📈](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-base.png)[🧠](results/bm-20240315-3.13.0a5%2B-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%252dcpython-hot_cold_with_fixes-3.13.0a5%2B-22ff3c3-vs-base-mem.png) |
| [2024-03-15](results/bm-20240315-3.13.0a5%2B-1904f0a-JIT) | python/1904f0a2245f500aa85f | 1904f0a (JIT) | 1.31x ↑<br>[📄](results/bm-20240315-3.13.0a5%2B-1904f0a-JIT/bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.10.4.md)[📈](results/bm-20240315-3.13.0a5%2B-1904f0a-JIT/bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.10.4.png) | 1.03x ↑<br>[📄](results/bm-20240315-3.13.0a5%2B-1904f0a-JIT/bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.11.0.md)[📈](results/bm-20240315-3.13.0a5%2B-1904f0a-JIT/bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.11.0.png) | 1.01x ↑<br>[📄](results/bm-20240315-3.13.0a5%2B-1904f0a-JIT/bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.12.0.md)[📈](results/bm-20240315-3.13.0a5%2B-1904f0a-JIT/bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5%2B-1904f0a-vs-3.12.0.png) |  |
| [2024-03-14](results/bm-20240314-3.13.0a5%2B-78b2070-JIT) | brandtbucher/justin_relax_absolut | 78b2070 (JIT) | 1.29x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.10.4.md)[📈](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.11.0.md)[📈](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.12.0.md)[📈](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-3.12.0.png) | 1.00x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-base.md)[📈](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-base.png)[🧠](results/bm-20240314-3.13.0a5%2B-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-78b2070-vs-base-mem.png) |
| [2024-03-14](results/bm-20240314-3.13.0a5%2B-61e54bf-JIT) | python/61e54bfcee9f08a8e09a | 61e54bf (JIT) | 1.29x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5%2B-61e54bf-vs-3.10.4.md)[📈](results/bm-20240314-3.13.0a5%2B-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5%2B-61e54bf-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5%2B-61e54bf-vs-3.11.0.md)[📈](results/bm-20240314-3.13.0a5%2B-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5%2B-61e54bf-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240314-3.13.0a5%2B-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5%2B-61e54bf-vs-3.12.0.md)[📈](results/bm-20240314-3.13.0a5%2B-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5%2B-61e54bf-vs-3.12.0.png) |  |
| [2024-03-14](results/bm-20240314-3.13.0a5%2B-89ade43-JIT) | brandtbucher/justin_relax_absolut | 89ade43 (JIT) | 1.29x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-3.10.4.md)[📈](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-3.11.0.md)[📈](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-3.12.0.md)[📈](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-3.12.0.png) | 1.00x ↓<br>[📄](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-base.md)[📈](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-base.png)[🧠](results/bm-20240314-3.13.0a5%2B-89ade43-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5%2B-89ade43-vs-base-mem.png) |
| [2024-03-14](results/bm-20240314-3.13.0a5%2B-2a54c4b-JIT) | python/2a54c4b25e05e30c50b9 | 2a54c4b (JIT) | 1.30x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-2a54c4b-JIT/bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.10.4.md)[📈](results/bm-20240314-3.13.0a5%2B-2a54c4b-JIT/bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-2a54c4b-JIT/bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.11.0.md)[📈](results/bm-20240314-3.13.0a5%2B-2a54c4b-JIT/bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240314-3.13.0a5%2B-2a54c4b-JIT/bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.12.0.md)[📈](results/bm-20240314-3.13.0a5%2B-2a54c4b-JIT/bm-20240314-linux-x86_64-python-2a54c4b25e05e30c50b9-3.13.0a5%2B-2a54c4b-vs-3.12.0.png) |  |
| [2024-03-14](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT) | mdboom/estimate_too_short | c3a9b5a (JIT) | 1.30x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.10.4.md)[📈](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.10.4.png) | 1.03x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.11.0.md)[📈](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.11.0.png) | 1.00x ↓<br>[📄](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.12.0.md)[📈](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-3.12.0.png) | 1.00x ↑<br>[📄](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-base.md)[📈](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-base.png)[🧠](results/bm-20240314-3.13.0a5%2B-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5%2B-c3a9b5a-vs-base-mem.png) |
| [2024-03-13](results/bm-20240313-3.13.0a5%2B-8c094c3-JIT) | python/8c094c3095feb4de2efe | 8c094c3 (JIT) | 1.29x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5%2B-8c094c3-vs-3.10.4.md)[📈](results/bm-20240313-3.13.0a5%2B-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5%2B-8c094c3-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5%2B-8c094c3-vs-3.11.0.md)[📈](results/bm-20240313-3.13.0a5%2B-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5%2B-8c094c3-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240313-3.13.0a5%2B-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5%2B-8c094c3-vs-3.12.0.md)[📈](results/bm-20240313-3.13.0a5%2B-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5%2B-8c094c3-vs-3.12.0.png) |  |
| [2024-03-13](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS) | python/main | 8c094c3 ️(T2) | 1.22x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5%2B-8c094c3-vs-3.10.4.md)[📈](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5%2B-8c094c3-vs-3.10.4.png) | 1.04x ↓<br>[📄](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5%2B-8c094c3-vs-3.11.0.md)[📈](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5%2B-8c094c3-vs-3.11.0.png) | 1.06x ↓<br>[📄](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5%2B-8c094c3-vs-3.12.0.md)[📈](results/bm-20240313-3.13.0a5%2B-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5%2B-8c094c3-vs-3.12.0.png) |  |
| [2024-03-13](results/bm-20240313-3.13.0a5%2B-313165e-JIT) | mdboom/too_short_3 | 313165e (JIT) | 1.30x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-3.10.4.md)[📈](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-3.11.0.md)[📈](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-3.12.0.md)[📈](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-3.12.0.png) | 1.00x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-base.md)[📈](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-base.png)[🧠](results/bm-20240313-3.13.0a5%2B-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5%2B-313165e-vs-base-mem.png) |
| [2024-03-13](results/bm-20240313-3.13.0a5%2B-61ce027-JIT) | mdboom/too_short_7 | 61ce027 (JIT) | 1.30x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-3.10.4.md)[📈](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-3.11.0.md)[📈](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-3.11.0.png) | 1.00x ↓<br>[📄](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-3.12.0.md)[📈](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-3.12.0.png) | 1.00x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-base.md)[📈](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-base.png)[🧠](results/bm-20240313-3.13.0a5%2B-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5%2B-61ce027-vs-base-mem.png) |
| [2024-03-13](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT) | mdboom/dont_getenv | cb999fb (JIT) | 1.30x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.10.4.md)[📈](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.11.0.md)[📈](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.12.0.md)[📈](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-3.12.0.png) | 1.00x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-base.md)[📈](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-base.png)[🧠](results/bm-20240313-3.13.0a5%2B-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5%2B-cb999fb-vs-base-mem.png) |
| [2024-03-13](results/bm-20240313-3.13.0a5%2B-61733a2-JIT) | python/61733a2fb9dc36d2246d | 61733a2 (JIT) | 1.29x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-61733a2-JIT/bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5%2B-61733a2-vs-3.10.4.md)[📈](results/bm-20240313-3.13.0a5%2B-61733a2-JIT/bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5%2B-61733a2-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240313-3.13.0a5%2B-61733a2-JIT/bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5%2B-61733a2-vs-3.11.0.md)[📈](results/bm-20240313-3.13.0a5%2B-61733a2-JIT/bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5%2B-61733a2-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240313-3.13.0a5%2B-61733a2-JIT/bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5%2B-61733a2-vs-3.12.0.md)[📈](results/bm-20240313-3.13.0a5%2B-61733a2-JIT/bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5%2B-61733a2-vs-3.12.0.png) |  |

## linux x86_64 (pythonperf2)
| date | fork/ref | hash/flags | vs. 3.10.4: | vs. 3.11.0: | vs. 3.12.0: | vs. base: |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf) | python/17d31bf3843c38487399 | 17d31bf | 1.28x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.06x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.01x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) |  |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS) | python/17d31bf3843c38487399 | 17d31bf ️(T2) | 1.14x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.06x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.14x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.13x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)[🧠](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png) |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT) | python/17d31bf3843c38487399 | 17d31bf (JIT) | 1.24x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.02x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.05x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.04x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)[🧠](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf2-x86_64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png) |

## windows amd64 (pythonperf1)
| date | fork/ref | hash/flags | vs. 3.10.4: | vs. 3.11.0: | vs. 3.12.0: | vs. base: |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf) | python/17d31bf3843c38487399 | 17d31bf | 1.21x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.08x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.05x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) |  |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS) | python/17d31bf3843c38487399 | 17d31bf ️(T2) | 1.11x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.00x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.03x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.08x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png) |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT) | python/17d31bf3843c38487399 | 17d31bf (JIT) | 1.20x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.07x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.04x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.01x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1-amd64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png) |

## windows x86 (pythonperf1_win32)
| date | fork/ref | hash/flags | vs. 3.10.4: | vs. 3.11.0: | vs. 3.12.0: | vs. base: |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf) | python/17d31bf3843c38487399 | 17d31bf | 1.17x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.28x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.20x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) |  |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS) | python/17d31bf3843c38487399 | 17d31bf ️(T2) | 1.12x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.23x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.16x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.04x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png) |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT) | python/17d31bf3843c38487399 | 17d31bf (JIT) | 1.06x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.16x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.10x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.10x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-pythonperf1_win32-x86-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png) |

## darwin arm64 (darwin)
| date | fork/ref | hash/flags | vs. 3.10.4: | vs. 3.11.0: | vs. 3.12.0: | vs. base: |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf) | python/17d31bf3843c38487399 | 17d31bf | 1.17x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.05x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.02x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) |  |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS) | python/17d31bf3843c38487399 | 17d31bf ️(T2) | 1.09x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.12x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.09x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.07x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)[🧠](results/bm-20240309-3.13.0a4%2B-17d31bf-PYTHON_UOPS/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png) |
| [2024-03-09](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT) | python/17d31bf3843c38487399 | 17d31bf (JIT) | 1.14x ↑<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.10.4.png) | 1.08x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.11.0.png) | 1.05x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-3.12.0.png) | 1.03x ↓<br>[📄](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.md)[📈](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base.png)[🧠](results/bm-20240309-3.13.0a4%2B-17d31bf-JIT/bm-20240309-darwin-arm64-python-17d31bf3843c38487399-3.13.0a4%2B-17d31bf-vs-base-mem.png) |


<!-- END table -->

`*` indicates that the exact same versions of pyperformance was not used.

For the results above, the "faster/slower" result is a geometric mean of each of the benchmarks. The "reliability (rel)" number is the likelihood that the change is faster or slower based on the [Heirarchical Performance Testing (HPT)](#hpt) method.  For more details, visit each individual result's README.md.

## Longitudinal results

Below are longitudinal timing results. There are also [🧠 longitudinal memory results](memory.md).

![Longitudinal speed improvement](/longitudinal.png)

![Effect of different configurations](/configs.png)

Improvement of the HPT score of key merged benchmarks, computed with `pyperf compare`.
The results have a resolution of 0.01 (1%).

- linux: Intel® Xeon® W-2255 CPU @ 3.70GHz, running Ubuntu 20.04 LTS, gcc 9.4.0
- linux2: 12th Gen Intel® Core™ i9-12900 @ 2.40 GHz, running Ubuntu 22.04 LTS, gcc 11.3.0
- macos: M1 arm64 Mac® Mini, running macOS 13.2.1, clang 1400.0.29.202
- windows: 12th Gen Intel® Core™ i9-12900 @ 2.40 GHz, running Windows 11 Pro (21H2, 22000.1696), MSVC v143

## Documentation

### Running benchmarks from the GitHub web UI

Visit the 🔒 [benchmark action](../../actions/workflows/benchmark.yml) and click the "Run Workflow" button.

The available parameters are:

- `fork`: The fork of CPython to benchmark.
  If benchmarking a pull request, this would normally be your GitHub username.
- `ref`: The branch, tag or commit SHA to benchmark.
  If a SHA, it must be the full SHA, since finding it by a prefix is not supported.
- `machine`: The machine to run on.
  One of `linux-amd64` (default), `windows-amd64`, `darwin-arm64` or `all`.
- `benchmark_base`: If checked, the base of the selected branch will also be benchmarked.
  The base is determined by running `git merge-base upstream/main $ref`.
- `pystats`: If checked, collect the pystats from running the benchmarks.

To watch the progress of the benchmark, select it from the 🔒 [benchmark action page](../../actions/workflows/benchmark.yml).
It may be canceled from there as well.
To show only your benchmark workflows, select your GitHub ID from the "Actor" dropdown.

When the benchmarking is complete, the results are published to this repository and will appear in the [master table](RESULTS.md).
Each set of benchmarks will have:

- The raw `.json` results from pyperformance.
- Comparisons against important reference releases, as well as the merge base of the branch if `benchmark_base` was selected.  These include
  - A markdown table produced by `pyperf compare_to`.
  - A set of "violin" plots showing the distribution of results for each benchmark.
  - A set of plots showing the memory change for each benchmark (for immediate bases only, on non-Windows platforms).

The most convenient way to get results locally is to clone this repo and `git pull` from it.

### Running benchmarks from the GitHub CLI

To automate benchmarking runs, it may be more convenient to use the [GitHub CLI](https://cli.github.com/).
Once you have `gh` installed and configured, you can run benchmarks by cloning this repository and then from inside it:

```bash
$ gh workflow run benchmark.yml -f fork=me -f ref=my_branch
```

Any of the parameters described above are available at the commandline using the `-f key=value` syntax.

### Collecting Linux perf profiling data

To collect Linux perf sampling profile data for a benchmarking run, run the `_benchmark` action and check the `perf` checkbox.

### Developer docs

The infrastructure to make all of this work is the [bench_runner
project](https://github.com/faster-cpython/bench_runner).  Look there for more
detailed developer docs.

### Details about how results are collected

The easiest way to reproduce what is here is to use the [bench_runner
project](https://github.com/faster-cpython/bench_runner) library directly, but
if you want to run parts of it in a different context or better understand how the
numbers are calculated, this section describes some of the things that the
benchmarking infrastructure does.

#### Benchmarks from pyperformance and python-macrobenchmarks

These results combine benchmarks that live in the
[pyperformance](https://github.com/python/pyperformance) and
[pyston/python-macrobenchmarks](https://github.com/pyston/python-macrobenchmarks)
projects, so running the default set from `pyperformance` will definitely
produce different results. To combine these benchmarks in the same run, clone
both repos side-by-side in the same directory and [use a manifest
file](https://github.com/faster-cpython/bench_runner/blob/main/bench_runner/templates/benchmarks.manifest)
to combine them.  This file should be passed to `pyperformance run`:

```
pyperformance run --manifest benchmarks.manifest
```

#### Different configurations

Benchmarks and stats collection can happen in three different configurations.
Here "configuration" may be a combination of both build-time and run-time flags:

- Default: A PGO build of CPython (`./configure --enable-optimizations
  --with-lto=yes`).
- Tier 2: The same build as above, but with the `PYTHON_UOPS` environment
  variable set at runtime to use the Tier 2 interpreter.
- JIT: A JIT and PGO build of CPython (`./configure --enable-optimizations
  --with-lto=yes --enable-experimental-jit`).

Information about the configuration of the run is in the `README.md` at the root
of each run directory.  The directory name will also include `PYTHON_UOPS` for
Tier 2 and `JIT` for JIT.

To reduce the number of unknown variables when comparing results, runs are
always compared against runs of the same configuration. Be aware that sometimes
the base commit on main may predate the configuration becoming available, for
example, before the JIT compiler was merged into main.  (An exception to this
rule are the weekly benchmarks of upstream main, there Tier 2 and JIT
configurations are compared against default configurations of the same commit,
but that isn't relevant for the common case of testing a pull request).

An additional sharp edge is that, by default, `pyperformance` does not pass
environment variables to the child process that actually does the work.
Therefore for a Tier 2 configuration, the `--inherit-environ=PYTHON_UOPS` flag
must be passed to `pyperformance run` when running benchmarks.

For detailed information, see how configurations affect [build time flags in the
Github Actions
configuration.](https://github.com/faster-cpython/bench_runner/blob/main/bench_runner/templates/_benchmark.src.yml).

#### Timing benchmarks

Timing benchmarks are notoriously noisy.  There are a few techniques to reduce this:

- Where available (on Linux), we use [`pyperf
  tune`](https://pyperf.readthedocs.io/en/latest/system.html) to set CPU
  affinity and other things that make the benchmarks more reproducible.  For
  this reason, we know that the benchmarks are more predictable on Linux than on
  the other platforms.
- `pyperf` has the concept of "warmup" runs, while caches are warming up and
  other things about the system are still stabilizing. These runs are excluded
  from the timing results. This is generally effective at reducing variability,
  but also may exclude real work done during optimization, for example.
- We use the Hierarchical Performance Testing (HPT) method (see below) to
  statistically reduce the effect of benchmarks that have more variability.
  This is a different method than the simple geometric mean that `pyperf` uses
  by default.  We provide both numbers in our results.

#### pystats

`pystats` are a set of counters in CPython that measure things like the number
of times each bytecode instruction is executed.  (Detailed documentation of all
of the counters should be added to CPython in the future).

Collecting `pystats` requires a special build of CPython with `pystats` enabled:
(`./configure --enable-pystats`).

`pystats` must also be enabled at runtime, either using the `-Xpystats` command
line argument or `sys._stats_on()`. `pyperformance`/`pyperf` handles this step
automatically when running on a pystats-enabled build.  Stats collection is
enabled during actual benchmarking code, and disabled while running the
"benchmarking harness" code in `pyperf` itself.  `pyperf` has the concept of
"warmup" runs, which allow things like cache lines to warmup before actually
timing benchmarks. While they aren't included in the timing benchmarks, these
warmup runs are included in pystats collection since often Tier 2/JIT traces are
created during warmup, and we don't want the stats to appear as if the traces
ran but were not created.

Any statistics collected are then dumped at exit to the `/tmp/py_stats`
directory with a random filename. Lastly, the `Tools/scripts/summarize_stats.py`
script (in the CPython repo) is used to read all of the files from
`/tmp/py_stats` and produce a human-readable markdown summary and a JSON file
with aggregate data.  Because of this design, it is imperative that:

- The `/tmp/py_stats` directory is cleared before data collection.
- No other Python processes are run that could also produce pystats data.
  Especially, this means benchmarks can not run in parallel.

For more information, see the actual code to [collect
pystats](https://github.com/faster-cpython/bench_runner/blob/main/bench_runner/templates/_pystats.src.yml).

### HPT

Heirarchical performance testing (HPT) is a method introduced in this paper:

> T. Chen, Y. Chen, Q. Guo, O. Temam, Y. Wu and W. Hu,
"Statistical performance comparisons of computers,"
IEEE International Symposium on High-Performance Comp Architecture,
New Orleans, LA, USA, 2012, pp. 1-12,
doi: 10.1109/HPCA.2012.6169043.

From the abstract:

> In traditional performance comparisons, the impact of performance variability
is usually ignored (i.e., the means of performance measurements are compared
regardless of the variability), or in the few cases where it is factored in
using parametric confidence techniques, the confidence is either erroneously
computed based on the distribution of performance measurements (with the
implicit assumption that it obeys the normal law), instead of the distribution
of sample mean of performance measurements, or too few measurements are
considered for the distribution of sample mean to be normal. …  We propose a
non-parametric Hierarchical Performance Testing (HPT) framework for
performance comparison, which is significantly more practical than standard
parametric techniques because it does not require to collect a large number of
measurements in order to achieve a normal distribution of the sample mean.

For each result, we compute a reliability score, as well as the estimated
speedup at the 90th, 95th and 99th percentile.

**The inclusion of HPT scores is considered experimental as we learn about their
usefulness for decision-making.**
