# The Mentor Curriculum
### The half Scaler doesn't teach you
**Owner:** You · **Duration:** 12 months · **Daily budget:** 2 hrs (Block 2)
 
---
 
## The division of labour
 
| | Owns | Time |
|---|---|---|
| **Scaler** | DSA · LLD · HLD · Databases/SQL · Mock interviews | Block 1 — 1.5 hr/day |
| **This curriculum** | JS/TS/Node/React depth · AI Engineering · Portfolio · Positioning | Block 2 — 2 hr/day |
| **Revision** | Spaced repetition + daily log | Block 3 — 0.5 hr/day |
 
Scaler makes you **interviewable**. This makes you **worth hiring**.
Neither works alone. Scaler grads with no depth get filtered at the design round. Deep engineers with no DSA never reach it.
 
---
 
## The 5 Tracks
 
### TRACK 1 — JavaScript & TypeScript Depth
*The thing you've used for 8 years and never opened up.*
 
**Why:** Every senior frontend/full-stack interview probes this. It's also the fastest depth win you have, because you already have the muscle memory — you're just missing the model underneath.
 
- Execution context, call stack, hoisting, TDZ
- Closures — the real mechanism, not the interview cliché
- `this` binding, call/apply/bind, arrow function semantics
- Prototypes, prototype chain, `class` as sugar
- **The Event Loop** — macrotask vs microtask, why `Promise.then` beats `setTimeout(0)`
- Promises from scratch — implement one
- async/await internals, error propagation
- Generators & iterators
- Memory: references, GC, leaks, WeakMap/WeakRef
- **TypeScript:** generics, conditional types, mapped types, `infer`, discriminated unions, type-level thinking
**Proof of mastery:** You can implement `Promise`, `debounce`, `throttle`, `deepClone`, `curry`, and `EventEmitter` from a blank file, and explain the event loop to a skeptical interviewer.
 
---
 
### TRACK 2 — React & Next.js Internals
*Your paycheck. This is where you become genuinely excellent, not just competent.*
 
**React:**
- Reconciliation & the diffing algorithm — actually how it works
- Fiber architecture, why it exists, time slicing
- Render vs commit phase
- Why re-renders happen; `memo` / `useMemo` / `useCallback` — and when they're a net loss
- Hooks internals — the linked-list of hooks, rules of hooks and *why*
- Context and its re-render problem
- Concurrent features: `useTransition`, `useDeferredValue`, Suspense
- State management: when Zustand vs Context vs server state (TanStack Query)
**Next.js:**
- App Router: **Server Components vs Client Components** — the actual boundary
- Rendering: SSR / SSG / ISR / PPR — pick correctly, defend the choice
- The caching layers (this is where everyone gets confused; you won't)
- Streaming & Suspense boundaries
- Server Actions
- Edge vs Node runtime, middleware
- Perf: Core Web Vitals, bundle analysis, code splitting, image/font optimization
**Proof of mastery:** You can look at any page and say *"this should be a Server Component, streamed, with these three things client-side, cached this way — here's why."* That sentence is what a senior sounds like.
 
---
 
### TRACK 3 — Node.js & Backend (TypeScript)
*Turning "I've used Node unofficially" into "I own the backend."*
 
- Node's event loop (**different from the browser's** — phases, libuv, thread pool)
- Streams & backpressure
- Cluster, worker threads, when to actually reach for them
- Express/Fastify or NestJS — pick one, go deep
- Auth done properly: JWT, sessions, refresh tokens, OAuth, RBAC
- API design: REST maturity, validation (Zod), error contracts, versioning
- **Postgres:** schema design, indexes, EXPLAIN, N+1, transactions, connection pooling
- Prisma / Drizzle
- Redis: caching, rate limiting, queues (BullMQ)
- Testing: Vitest/Jest, integration tests, Playwright
- Observability: structured logging, tracing, error tracking
**Proof of mastery:** You can design and ship a production backend that handles auth, rate limits, background jobs, and doesn't fall over — and explain every choice.
 
---
 
### TRACK 4 — AI Engineering (Python + FastAPI)
*Your differentiator. Almost nobody has this AND real frontend depth.*
 
**The architecture we're building toward:**
```
Next.js (UI)  →  Node/TS BFF (auth, business logic, Postgres)  →  FastAPI (AI service)
                                                                    ├─ LLM calls
                                                                    ├─ RAG / vector DB
                                                                    ├─ Agents & tools
                                                                    └─ Evals & tracing
```
 
**Foundations**
- LLM APIs: completions, streaming, tool/function calling, structured output
- Prompt engineering that survives production (not blog-post prompting)
- Token economics: cost, latency, context windows, caching
**RAG — done properly, not the toy version**
- Chunking strategies and why naive chunking fails
- Embeddings, vector DBs (pgvector / Qdrant)
- Hybrid search, re-ranking
- **Evaluation:** retrieval precision/recall, faithfulness, groundedness
- Why your RAG returns garbage, and how to *measure* that it does
**Agents**
- Tool use, ReAct loops, planning
- Multi-step workflows, state, failure handling
- Guardrails, retries, cost ceilings
**Production AI**
- Streaming LLM responses through Node → Next (SSE)
- Evals & regression testing for non-deterministic systems
- Observability: LangSmith / Langfuse, tracing
- Caching, fallbacks, graceful degradation
**FastAPI**
- Async Python, Pydantic, dependency injection
- Background tasks, streaming responses
- Containerizing and deploying the AI service
**Proof of mastery:** You can defend, in an interview, why you split Node and Python — and describe how you measured whether your RAG was actually any good.
 
---
 
### TRACK 5 — Deployment, Positioning & The Job
*The 10% that converts the other 90% into money.*
 
**Infra**
- Docker & docker-compose
- CI/CD (GitHub Actions)
- Deploy: Vercel (frontend) + Railway/Fly/AWS (services)
- Monitoring, alerts, cost control
**Positioning** *(this is where your Publicis/agency problem gets solved)*
- Resume rewritten around **impact and ownership**, not tasks
- Title framing — you are a Senior/Full-Stack engineer; the "Associate" label is your employer's ladder, not your level
- GitHub as evidence: clean READMEs, architecture diagrams, live demos
- LinkedIn positioned for **product companies**, not agencies
- Referrals — the single highest-ROI activity in Indian tech hiring
- Behavioral: 6–8 STAR stories on scope, conflict, failure, ownership
- Salary negotiation — you have never done this properly and it is worth lakhs
---
 
## The Portfolio: 3 projects, not 20
 
Tutorials are not portfolio. These three, built well, tell one coherent story:
 
**P1 — "Ask My Docs" (Months 2–4)**
Full RAG system. Next.js + Node BFF + FastAPI. Document upload, chunking, pgvector, hybrid retrieval, streaming answers with citations. **Ships with an eval suite that proves retrieval quality.**
→ *Proves: you can build AI that actually works, and you can measure it.*
 
**P2 — Agentic Workflow Tool (Months 5–8)**
Multi-step agent with real tools (search, DB, external API). Auth, background jobs, retries, cost ceilings, full tracing. Production-shaped.
→ *Proves: you can build systems, not demos.*
 
**P3 — Your Choice, Your Domain (Months 8–11)**
Something you actually care about. Real users, even ten of them. Real deployment. Real monitoring.
→ *Proves: ownership. This is the one you'll talk about in interviews.*
 
**Rule:** deployed, documented, with an architecture diagram, or it doesn't count.
 
---
 
## Timeline
 
| Phase | Months | Scaler (Block 1) | This curriculum (Block 2) |
|---|---|---|---|
| **1. Break the wall** | 1–3 | Recursion → Trees → resume DSA 4 | Track 1 (JS/TS) → start Track 4 → **P1** |
| **2. Unlock** | 4–6 | DSA 4.2 · Databases/SQL · LLD 1–2 | Track 2 (React/Next) · Track 3 (Node) · **P1 done** |
| **3. Design** | 7–9 | LLD 3 · High Level Design · Capstone | Track 4 deep · Track 5 infra · **P2** |
| **4. Convert** | 10–12 | DSA back to 2 hr/day · Mocks weekly | Track 5 positioning · **P3** · Apply in waves |
 
---
 
## The rules (these matter more than the content)
 
1. **No copying. Ever.** 25 minutes of honest struggle before you look. After you look, close it and re-solve from blank.
2. **Two real problems beat eight copied ones.** Always.
3. **Ship > study.** A deployed ugly project beats a beautiful unfinished one.
4. **Log daily.** What you studied, what you solved, what broke. Send it to me.
5. **When it hurts, say so.** Don't disappear. Disappearing is the only thing that has ever actually stopped you.
6. **Depth is finite.** The list above is ~40 concepts. Not infinite. That's why this is beatable.
---
 
*"You don't have a talent ceiling. You have a process defect. Process defects are fixable."*