# L5 Narrow / L2 General Classification — K_NEUROSYM
**Platform:** Anticloud | **Tier:** TIER_5_WORLD_NEURO_EMBODIED | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
K_NEUROSYM provides the neural-symbolic integration infrastructure for Anticloud: PAX 27B's neural reasoning feeds into Prolog/SPARQL symbolic inference, and symbolic constraints feed back into PAX's generation. Narrow scope: Anticloud domain knowledge graphs and logical constraints.

## L2 General
L2 General: K_NEUROSYM improves reasoning correctness across all tiers where logical constraints apply. TIER_6 security policy reasoning and TIER_7 clinical decision support both benefit from neural-symbolic integration.

## PAX 27B Integration
PAX 27B handles the neural part: natural language understanding, entity extraction, free-form generation. K_NEUROSYM feeds PAX outputs to Prolog/SPARQL for formal verification and constraint checking.

## AIOSS Audit Chain
Every neuro-symbolic cycle (neural output hash + symbolic query hash + constraints satisfied + final answer hash) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
ISO/IEC 42001 (explainable hybrid AI). NIST AI RMF 1.0 (reliable AI).
