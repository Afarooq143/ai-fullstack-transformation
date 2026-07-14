# AI Full-Stack Engineer — 12 Month Transformation
 
**Started:** 14 July 2026 · **Target:** 14 July 2027
**Stack:** TypeScript · React · Next.js · Node.js · Python · FastAPI · Postgres
**Focus:** Deep fundamentals + production AI engineering
 
---
 
## What this is
 
A public, daily-logged record of a structured 12-month program to go from frontend engineer to **senior full-stack engineer who ships AI-powered products.**
 
Everything here is built or solved from scratch. Every day is committed. Nothing is decorative.
 
**Two parallel tracks, 4 hours daily:**
 
| Track | Time | Content |
|---|---|---|
| **Interview readiness** | 1.5 hr/day | DSA · Low-Level Design · High-Level Design · Databases |
| **Engineering depth** | 2 hr/day | JS/TS internals · React/Next internals · Node · AI Engineering · Projects |
| **Revision** | 0.5 hr/day | Spaced repetition · daily log |
 
---
 
## Progress
 
### Current phase
**Phase 1 — Foundations** (14 Jul → 12 Oct 2026)
 
```
Recursion & Backtracking   [          ]  0%
Linked Lists               [          ]  0%
Trees                      [          ]  0%
JS Internals               [          ]  0%
React/Next Internals       [          ]  0%
P1 — Ask My Docs           [          ]  0%
```
 
### Quarterly gates
 
| Gate | Date | Target | Status |
|---|---|---|---|
| **Q1** | 12 Oct 2026 | Recursion/Trees solid · JS internals owned · **P1 deployed** | 🔵 In progress |
| **Q2** | 11 Jan 2027 | Databases/SQL · LLD · Node depth · **P2 started** | ⚪ Pending |
| **Q3** | 12 Apr 2027 | High-Level Design · **P2 deployed** · Docker/CI-CD | ⚪ Pending |
| **Q4** | 12 Jul 2027 | **P3 live with real users** · Interviewing | ⚪ Pending |
 
---
 
## The Projects
 
Three projects. Deployed, documented, measured. Not tutorials.
 
### P1 — Ask My Docs *(Aug–Sep 2026)*
Production-grade RAG system.
`Next.js → Node/TS BFF → FastAPI AI service → pgvector`
 
Document ingestion, chunking, hybrid retrieval, re-ranking, streamed answers with citations — **shipped with an evaluation suite that measures retrieval precision, recall, and faithfulness.**
 
> *Building AI that works is one skill. Proving it works is a different one.*
 
**Status:** Not started · **Repo:** _coming_ · **Live:** _coming_
 
### P2 — Agentic Workflow Tool *(Nov 2026 – Feb 2027)*
Multi-step agent with real tools. Auth, background jobs, retries, cost ceilings, full tracing. Production-shaped, not a demo.
 
**Status:** Not started
 
### P3 — TBD *(Apr–Jun 2027)*
Real product. Real users. Real monitoring.
 
**Status:** Not started
 
---
 
## The Architecture
 
The pattern every project is built on:
 
```
┌─────────────┐     ┌──────────────────┐     ┌─────────────────┐
│  Next.js    │────▶│  Node/TS BFF     │────▶│  FastAPI        │
│  (UI)       │◀────│  auth · logic    │◀────│  (AI service)   │
│             │ SSE │  Postgres        │ SSE │                 │
└─────────────┘     └──────────────────┘     ├─ LLM calls      │
                                              ├─ RAG / vectors  │
                                              ├─ Agents & tools │
                                              └─ Evals & traces │
```
 
**Why two backends?** Node owns the product surface — auth, business logic, data. Python owns the AI layer, because that's where the ecosystem lives. Separate services, separate scaling, separate failure domains.
 
---
 
## Repo Structure
 
```
├── logs/           # Daily log. One file per day. The proof.
├── dsa/            # Solutions in Python — recursion, trees, graphs, DP
│   └── spaced-repetition.md
├── notes/          # Concepts written in my own words
│   ├── javascript/
│   ├── react/
│   ├── node/
│   └── ai-engineering/
└── projects/       # P1, P2, P3
```
 
---
 
## Notes Index
 
Concepts I've written up from scratch. If it's listed here, I can explain it without notes.
 
### JavaScript
- [ ] Execution context, hoisting & the TDZ
- [ ] Closures — the actual mechanism
- [ ] `this`, call/apply/bind
- [ ] Prototypes & the prototype chain
- [ ] **The Event Loop** — macrotasks vs microtasks
- [ ] Promises (implemented from scratch)
- [ ] async/await internals
- [ ] Generators & iterators
- [ ] Memory, GC & leaks
### React & Next.js
- [ ] Reconciliation & the diffing algorithm
- [ ] Fiber architecture
- [ ] Hooks internals
- [ ] Server Components vs Client Components
- [ ] The Next.js caching layers
- [ ] Streaming & Suspense
### Node.js
- [ ] Node's event loop (and how it differs from the browser's)
- [ ] Streams & backpressure
- [ ] Worker threads & clustering
### AI Engineering
- [ ] Chunking strategies — and why naive chunking fails
- [ ] Embeddings & vector search
- [ ] Hybrid retrieval & re-ranking
- [ ] Evaluating RAG: precision, recall, faithfulness
- [ ] Agents: tool use, ReAct, guardrails
- [ ] Streaming LLM responses through a BFF
---
 
## The Rules
 
1. **No copied solutions.** 25 minutes of honest effort, then look — then close it and re-solve from a blank file. If I can't re-solve it, it isn't solved.
2. **Two real problems beat eight copied ones.**
3. **Ship > study.** A deployed imperfect project beats a perfect unfinished one.
4. **Commit daily.** The log is not optional.
5. **Measure outputs, not hours.**
---
 
## Log
 
| Date | Day | DSA | Depth | Committed |
|---|---|---|---|---|
| 14 Jul 2026 | 001 | Recursion — foundations | Execution context & closures | ✅ |
 
<sub>Full logs in [`/logs`](./logs)</sub>
 
---
 
*Depth is finite. The list above is ~40 concepts, not infinite. That's why it's beatable.*
 
