# Developer Cookbook — K_NEUROSYM
**Stack:** Python 3.11, PAX 27B, Prolog (pyswip), SPARQL, networkx, AIOSS_FORMAT
**Domain:** NeuroSymbolic: neural-symbolic integration layer for PAX 27B structured reasoning

## Neural-symbolic query
```python
from k_neurosym import NeuroSymPipeline

ns = NeuroSymPipeline(
    pax_model="./pax-27b-q4.gguf",
    kb_ttl="./anticloud_graph.ttl",
    prolog_rules="./anticloud_rules.pl",
    aioss_chain="./neurosym.aioss"
)

result = ns.query(
    "Which TIER_7 projects require IRB approval for human subject EEG data?"
)
print(f"Answer: {result.answer}")
print(f"Prolog proof: {result.proof}")
print(f"Chain: {result.chain_hash}")
```

## Add symbolic rules
```python
ns.add_rule("requires_irb(X) :- project(X), uses_human_eeg(X), tier(X, tier7).")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
