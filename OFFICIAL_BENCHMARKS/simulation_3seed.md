# 3-Seed Simulation — K_NEUROSYM

**Seeds:** `82686` · `14023` · `48222`

**Seed method:** `sha256("K_NEUROSYM")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_NEUROSYM`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.0093 | 0.2329 | ±0.4565 |
| throughput_tokens_per_sec | 385.5 | 27.267 | ±53.4433 |
| p50_latency_ms | 46.35 | 3.7246 | ±7.3002 |
| p99_latency_ms | 119.61 | 7.8871 | ±15.4587 |
| ttft_ms | 25.78 | 1.7439 | ±3.418 |
| mmlu_proxy | 0.7252 | 0.0261 | ±0.0512 |
| hellaswag_proxy | 0.7992 | 0.0328 | ±0.0643 |
| truthfulqa_proxy | 0.5613 | 0.0376 | ±0.0737 |
| arc_proxy | 0.6762 | 0.0311 | ±0.061 |
| complexity_cyclomatic | 3.54 | 0.3269 | ±0.6407 |
| maintainability_index | 72.1733 | 4.1484 | ±8.1309 |
| security_issues_high | 0.6667 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 76.5667 | 7.7676 | ±15.2245 |
| test_coverage_pct | 51.5667 | 3.5864 | ±7.0293 |
| doc_coverage_pct | 57.6 | 3.879 | ±7.6028 |
| memory_mb | 1092.4667 | 91.1565 | ±178.6667 |
| gpu_util_pct | 65.9667 | 7.5464 | ±14.7909 |
| openssf_score | 6.7333 | 0.2963 | ±0.5807 |
| eu_ai_act_compliance_pct | 87.3333 | 1.1898 | ±2.332 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 82686 | Seed 14023 | Seed 48222 |
|--------|------------|------------|------------|
| trl_score | 7.033 | 6.713 | 7.282 |
| throughput_tokens_per_sec | 393.6 | 414.1 | 348.8 |
| p50_latency_ms | 50.67 | 46.8 | 41.58 |
| p99_latency_ms | 108.61 | 126.71 | 123.51 |
| ttft_ms | 24.03 | 28.16 | 25.15 |
| mmlu_proxy | 0.6882 | 0.7436 | 0.7437 |
| hellaswag_proxy | 0.827 | 0.8174 | 0.7531 |
| truthfulqa_proxy | 0.5113 | 0.5709 | 0.6018 |
| arc_proxy | 0.7156 | 0.6396 | 0.6733 |
| complexity_cyclomatic | 4.0 | 3.27 | 3.35 |
| maintainability_index | 69.21 | 78.04 | 69.27 |
| security_issues_high | 1 | 1 | 0 |
| dependency_freshness_pct | 87.1 | 74.0 | 68.6 |
| test_coverage_pct | 46.5 | 53.9 | 54.3 |
| doc_coverage_pct | 62.3 | 57.7 | 52.8 |
| memory_mb | 1151.5 | 1162.2 | 963.7 |
| gpu_util_pct | 76.1 | 58.0 | 63.8 |
| openssf_score | 6.68 | 6.4 | 7.12 |
| eu_ai_act_compliance_pct | 85.8 | 88.7 | 87.5 |
| slsa_level | 1 | 1 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._