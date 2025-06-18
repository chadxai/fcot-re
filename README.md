# FCoT-RE — Formal Chain-of-Thought Reasoning Engine

```bash
pip install fcot-re~=0.9
```

```python
from fcot_re import Engine

solver = Engine(llm="gpt-4o", max_depth=32, temperature=0.2)
result, trace = solver.solve("John sold some apples …")

print(result)
print(trace.to_markdown(max_steps=5))
```

Need proofs or deep-dive docs? See [`docs/whitepaper.md`](docs/whitepaper.md).
