# Anticloud × NEUROSYM
> Neuro-symbolic reasoning under cryptographic audit.

**Part of:** World / Neuro / Embodied · Anticloud FZ LLE · 0-1.gg
**Upstream:** upstream/neurosym (Apache-2.0)
**License:** Apache-2.0 OR LicenseRef-Anticommons-Enterprise-1.0
**IP:** USPTO pending · Lois-Kleinner Alpasan · 2026

Combine LLM reasoning with symbolic logic (Prolog, Z3). Verify outputs mathematically.

```python
from neurosym_anticloud import NeuroSymbolic

ns = NeuroSymbolic(
    llm_backend="pax-one-27b",
    symbolic_engines=["z3", "prolog"],
    ledger_path="./neurosym_ledger.aioss",
)

# LLM proposes → symbolic engine verifies → ledger-tracked proof
answer = ns.query("If A > B and B > C, then A > C. Verify for A=10, B=5, C=2")
# Returns: {answer: "True", proof_hash: "k5:...", verified: true}
```

**Plays well with:** L-KASTERAN (reasoning engine), K-AIOSS (ledger), PAX_SEMANTIC_ENGINE (structured output)
