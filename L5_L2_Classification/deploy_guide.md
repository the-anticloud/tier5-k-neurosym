# Deploy Guide — K_NEUROSYM
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, PAX 27B, Prolog (pyswip), SPARQL, networkx, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, PAX 27B, pyswip 0.3+ (SWI-Prolog), rdflib 7.0+ (SPARQL), networkx.

## Environment
4GB RAM. GPU for PAX neural reasoning. CPU for Prolog/SPARQL symbolic inference.

## AIOSS Integration
```bash
aioss init --module K_NEUROSYM --output ./k_neurosym.aioss
aioss append --chain ./k_neurosym.aioss --payload ./output.bin --module K_NEUROSYM
aioss verify --chain ./k_neurosym.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="K_NEUROSYM",
    aioss_chain="./K_NEUROSYM.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_NEUROSYM.aioss --verbose
python -m K_NEUROSYM.tests.smoke
```
