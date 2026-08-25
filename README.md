<div align="center">

# Akash Dutta

### Senior AI / ML Engineer · Retrieval Systems · LLM Infrastructure

[![Email](https://img.shields.io/badge/email-akashdutta1030hr%40gmail.com-555?logo=gmail&logoColor=white)](mailto:akashdutta1030hr@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-akashdutta1030hr--beep-181717?logo=github)](https://github.com/akashdutta1030hr-beep)
[![Hireable](https://img.shields.io/badge/open_to-work-yes-2ea44f)](https://github.com/akashdutta1030hr-beep)

</div>

---

I build the **unsexy half of applied AI** — the parts that decide whether a system ships or dies in production:

- Did hybrid retrieval actually beat BM25, or was it noise on 40 queries?
- When OpenAI 500s, does your app retry-storm the vendor or fail fast?
- Can you explain every line of your eval harness in a staff interview?

Framework demos are easy. **Measurable retrieval + production LLM edges** are what senior loops test.

## Featured projects

| Project | One-liner | Stack |
|---------|-----------|-------|
| **[lattice](https://github.com/akashdutta1030hr-beep/lattice)** | Hybrid RAG from first principles — BM25, dense cosine, RRF, nDCG/MRR, bootstrap CIs. Zero API keys in CI. | Python · NumPy · pytest |
| **[forge-gateway](https://github.com/akashdutta1030hr-beep/forge-gateway)** | OpenAI-compatible edge: API keys → principals, token buckets, circuit breaker, request IDs. | Go · stdlib HTTP |
| **[Dyck_Task](https://github.com/akashdutta1030hr-beep/Dyck_Task)** | Dyck-language generator + LoRA fine-tune with reasoning traces. | Python · Unsloth |
| **[Fine-tuning](https://github.com/akashdutta1030hr-beep/Fine-tuning)** | PEFT comparison — LoRA, QLoRA, prefix & prompt tuning on Qwen3-0.6B. | Jupyter · PEFT |

```text
Query ──► BM25 ──┐
                 ├── RRF ──► Grounded prompt ──► LLM
Query ──► Dense ─┘              ▲
                                │
                     EvalRunner (nDCG + 95% CI)
```

**Lattice** — retrieval quality measured *before* generation. **Forge** — the gateway layer when LLM traffic hits production.

## How I work

| Principle | In practice |
|-----------|-------------|
| **Separate retrieval from generation** | Eval the retriever on labeled queries without calling an LLM |
| **Intervals, not point estimates** | Bootstrap CIs and paired tests on the same query set |
| **Small, readable libraries** | BM25 IDF and RRF implemented in-repo — interview-readable |
| **Production before prompts** | Auth, rate limits, circuit breakers, traces |

## Stack

`Python` · `Go` · `Java` · `JavaScript` · NumPy · information retrieval · LLM eval · HTTP systems · Docker · GitHub Actions · pytest · `go test`

## 60-second demo

```bash
# Hybrid retrieval eval (offline, no API keys)
git clone https://github.com/akashdutta1030hr-beep/lattice && cd lattice
pip install -e ".[dev]" && pytest -q && python examples/run_eval.py

# LLM gateway (mock upstream included)
git clone https://github.com/akashdutta1030hr-beep/forge-gateway && cd forge-gateway
docker compose up --build
curl -s localhost:8080/healthz
```

## Contact

- **Email:** [akashdutta1030hr@gmail.com](mailto:akashdutta1030hr@gmail.com)
- **GitHub:** [akashdutta1030hr-beep](https://github.com/akashdutta1030hr-beep)

---

<sub>Pin **lattice** and **forge-gateway** on my profile · MIT licensed flagship repos · CI green on every push</sub>
