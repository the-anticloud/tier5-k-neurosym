# HF_Leaderboard_Lab_Results

**Project:** `K_NEUROSYM`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `KQYaili/neurosymbolic-reasoning`  
**Commit:** `af3b341a5aa7`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **47.46 ms** |
| Min latency | 43.49 ms |
| Max latency | 55.0 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **41** |
| Tokenization latency | 0.99 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5853 |
| Classification latency | 104.51 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_NEUROSYM (KQYaili/neurosymbolic-reasoning) — 395 files, 8345 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'ne', '##uro', '##sy', '##m', '(', 'k', '##q', '##ya', '##ili', '/', 'ne', '##uro', '##sy', '##mbo', '##lic', '-', 'reasoning']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_