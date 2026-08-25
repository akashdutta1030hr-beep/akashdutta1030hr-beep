# Akash Dutta

**AI / ML engineer** building retrieval systems, evaluation harnesses, and the production layer in front of LLMs.

I care about the unglamorous half of applied AI: *did the retriever actually improve, and will this still work when the vendor 500s?*

## What to look at

| Repo | Why it exists |
|---|---|
| **[lattice](https://github.com/akashdutta1030hr-beep/lattice)** | Hybrid RAG from first principles — Okapi BM25, dense cosine, Reciprocal Rank Fusion, nDCG/MRR, bootstrap CIs. No LangChain. Tests run offline. |
| **[forge-gateway](https://github.com/akashdutta1030hr-beep/forge-gateway)** | Go edge gateway for OpenAI-compatible APIs: API keys → principals, token-bucket rate limits, circuit breaker, request IDs. |
| **[Dyck_Task](https://github.com/akashdutta1030hr-beep/Dyck_Task)** | Dyck-language dataset generator (structure / reasoning data). |

## Stack

`Python` · `Go` · `NumPy` · information retrieval · LLM eval · HTTP systems · pytest / Go test · GitHub Actions

## How I work

- Measure retrieval **separately** from generation.
- Report **intervals**, not a single accuracy number.
- Prefer small, readable libraries over framework soup.
- Production path: auth, load shedding, and traces before more prompt templates.

## Contact

- GitHub: [akashdutta1030hr-beep](https://github.com/akashdutta1030hr-beep)
- Email: akashdutta1030hr@gmail.com
