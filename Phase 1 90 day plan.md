# PHASE 1 — The 90-Day Plan
### 14 July 2026 → 12 October 2026
**Mission:** Break the recursion wall. Build the JS depth. Ship P1.
 
---
 
## The fixed dates
 
| Date | Event |
|---|---|
| **Tue 14 Jul** | Start. Extend Scaler pause today. |
| **Sun 9 Aug** | Self-driven DSA sprint ends. Recursion + Trees dead. |
| **Mon 11 Aug** | **Scaler resumes — DSA 4 live.** Non-negotiable. |
| **Sun 13 Sep** | P1 (Ask My Docs) v1 deployed. |
| **Sun 12 Oct** | **Q1 GATE.** Full review. |
 
---
 
## The daily shape (every single day)
 
| Block | Time | Weekday | Weekend |
|---|---|---|---|
| **1 — DSA** | 1.5 hr | Problems. Always problems. | 2.5 hr |
| **2 — Depth/Build** | 2 hr | JS/TS → later React/Node/AI | 3 hr |
| **3 — Log** | 0.5 hr | Revision + commit + log | 0.5 hr |
 
**Sunday = 1 day off per week.** Take it. Burnout is the failure mode, not laziness.
 
---
 
## THE COPY-PROOF PROTOCOL
*Read this before every DSA session. This is the whole fix.*
 
For each problem:
1. **Timer: 25 min.** Blank file. No editorial, no YouTube, no ChatGPT.
2. Stuck at 25? Write down **what specifically you don't know.** ("I can't see the recursive case." "I don't know how to avoid revisiting nodes.")
3. **Only now** look at the solution. Read it once. Understand it.
4. **Close everything. Wait 10 minutes.** Re-solve from a blank file.
5. If you can't re-solve from blank → **it doesn't count. Not solved.**
6. Log it. Re-solve it again in 3 days, then 7 days, then 21 days.
**Two problems done this way > eight problems copied. Every time.**
 
---
 
# WEEK-BY-WEEK
 
## WEEK 1 · 14–20 Jul — RECURSION FOUNDATIONS
 
**Block 1 — DSA (the wall)**
 
| Day | Date | Topic | Solve |
|---|---|---|---|
| Tue | 14 Jul | Recursion mental model: base case, recursive case, the call stack. **Draw the stack by hand for every problem.** | Factorial, Fibonacci, Sum of N, Reverse a string |
| Wed | 15 Jul | Recursion on arrays | Print 1→N, N→1, Sum of array, Max of array |
| Thu | 16 Jul | Recursion with return values vs void | Check palindrome, Power(x,n), Binary search recursive |
| Fri | 17 Jul | Subsequences & the include/exclude pattern | Print all subsequences, Count subsequences with sum K |
| Sat | 18 Jul | Recursion + choices | Subsets, Subsets II (duplicates) |
| Sun | 19 Jul | **REST** | — |
| Mon | 20 Jul | Consolidation + re-solve Day 1–3 from blank | 4 re-solves |
 
**Rule this week:** for every single problem, **draw the recursion tree on paper.** Not optional. This is how the mental model gets built.
 
**Block 2 — JS Depth: Execution & Closures**
- Execution context, call stack, hoisting, TDZ
- Scope chain, lexical environment
- **Closures — the actual mechanism**
- Build: `counter()`, `once()`, `memoize()`, private state with closures
- Write a `README.md` in your GitHub explaining closures **in your own words.** If you can't explain it, you don't have it.
---
 
## WEEK 2 · 21–27 Jul — BACKTRACKING
 
**Block 1 — DSA**
 
| Day | Date | Topic | Solve |
|---|---|---|---|
| Tue | 21 Jul | Backtracking pattern: choose → explore → **un-choose** | Permutations |
| Wed | 22 Jul | Permutations & combinations | Permutations II, Combination Sum |
| Thu | 23 Jul | Grid backtracking | Rat in a Maze, Word Search |
| Fri | 24 Jul | Constraint backtracking | N-Queens |
| Sat | 25 Jul | Hard backtracking | Sudoku Solver, Palindrome Partitioning |
| Sun | 26 Jul | **REST** | — |
| Mon | 27 Jul | Re-solve N-Queens + Combination Sum from blank | Spaced repetition |
 
**Block 2 — JS Depth: `this`, Prototypes, OOP**
- `this` binding rules, call/apply/bind — **implement your own `bind`**
- Prototype chain, `__proto__` vs `prototype`
- `class` as syntactic sugar — show the desugared version
- Build: `debounce`, `throttle`, `deepClone`, `curry`
---
 
## WEEK 3 · 28 Jul – 3 Aug — LINKED LISTS
 
**Block 1 — DSA**
 
| Day | Date | Topic | Solve |
|---|---|---|---|
| Tue | 28 Jul | Singly LL: build it from scratch, traverse, insert, delete | Reverse a LL (iterative + recursive) |
| Wed | 29 Jul | Two-pointer on LL | Middle of LL, Detect cycle (Floyd's) |
| Thu | 30 Jul | Cycle + intersection | Start of cycle, Intersection of two LLs |
| Fri | 31 Jul | Merging & sorting | Merge two sorted LLs, Merge Sort on LL |
| Sat | 1 Aug | Doubly LL + hard | Remove Nth from end, Palindrome LL, Reorder List |
| Sun | 2 Aug | **REST** | — |
| Mon | 3 Aug | Re-solve: reverse LL, detect cycle, merge sort LL | Spaced repetition |
 
**Block 2 — JS Depth: THE EVENT LOOP** ⭐
*This is the single highest-value week of Block 2 in the whole quarter.*
- Call stack, task queue, **microtask queue**
- Why `Promise.then` runs before `setTimeout(0)`
- Promises: states, chaining, error propagation
- **Implement `Promise` from scratch.** Then `Promise.all`, `Promise.race`, `Promise.allSettled`.
- Write a blog-style README: "How the JS event loop actually works." **This becomes an interview weapon.**
---
 
## WEEK 4 · 4–9 Aug — TREES (the final boss)
 
**Block 1 — DSA**
 
| Day | Date | Topic | Solve |
|---|---|---|---|
| Tue | 4 Aug | Binary tree structure, DFS traversals (pre/in/post) recursive | All 3 traversals, Height of tree |
| Wed | 5 Aug | BFS / level order | Level order, Zigzag, Right side view |
| Thu | 6 Aug | Tree recursion patterns — **return values up the tree** | Diameter, Balanced tree, Max path sum |
| Fri | 7 Aug | BST | Validate BST, Search, Insert, Kth smallest |
| Sat | 8 Aug | LCA + construction | LCA, Build tree from preorder+inorder |
| Sun | 9 Aug | **Self-audit + rest.** Re-solve 5 problems from blank. | — |
 
**Block 2 — async/await, Generators, TypeScript**
- async/await internals (it's generators + promises)
- Generators & iterators
- TS: generics, utility types, discriminated unions
- **Set up P1 repo.** Next.js + TS scaffold. Push it.
---
 
## 🚪 GATE 1 — Sunday 9 August
 
You do not proceed until you can, **from a blank file, without help:**
 
- [ ] Write recursive + iterative reversal of a linked list
- [ ] Solve N-Queens
- [ ] Detect a cycle in a linked list and find its start
- [ ] Do all 3 DFS traversals + level order on a binary tree
- [ ] Find the diameter of a binary tree
- [ ] Implement `Promise` from scratch
- [ ] Explain the event loop out loud for 3 minutes without notes
**Send me this checklist with honest ticks.** If 5+ tick, you're ready for DSA 4.
If fewer — we don't panic and we don't restart. We spend one more week on the gaps. **One. Week.**
 
---
 
## WEEKS 5–9 · 11 Aug – 13 Sep — SCALER RESUMES + P1 BUILD
 
**Block 1 — Scaler DSA 4, live.**
The rules that were absent last time:
- Attend the class. Every class.
- **Assignments done the same day. Not "later."**
- Additional problems done within the same week.
- **Attempt every contest.** A 40/100 you earned beats a 0/100 you skipped. Your dashboard has three 0/100s. Zero more.
- Book the two pending mock interviews. Do them badly. Do them anyway.
**Block 2 — P1: "Ask My Docs"**
 
| Week | Dates | Build |
|---|---|---|
| 5 | 11–17 Aug | Next.js UI + Node/TS BFF skeleton. Auth. Postgres + Prisma. File upload. |
| 6 | 18–24 Aug | FastAPI service. Chunking strategy. Embeddings. pgvector. Ingest pipeline works end-to-end. |
| 7 | 25–31 Aug | Retrieval + LLM answer generation. **Streaming SSE: FastAPI → Node → Next.** Citations in the UI. |
| 8 | 1–7 Sep | **The eval suite.** 30 golden Q&A pairs. Measure retrieval precision/recall + faithfulness. *This is the part 95% of people skip. It's the part that gets you hired.* |
| 9 | 8–13 Sep | Docker. Deploy (Vercel + Railway). README + architecture diagram. **Ship it.** |
 
**Sun 13 Sep — P1 is live on the internet with a public URL.** Not "almost done." Live.
 
---
 
## WEEKS 10–13 · 15 Sep – 12 Oct — REACT/NEXT DEPTH + HARDEN
 
**Block 1 — Scaler DSA 4 continues.** Same rules. No slippage.
 
**Block 2 — Track 2: React & Next.js Internals**
 
| Week | Focus |
|---|---|
| 10 | Reconciliation, Fiber, render vs commit phase, why re-renders happen |
| 11 | Hooks internals (the linked list), `memo`/`useMemo`/`useCallback` and when they're a net loss, Context's re-render problem |
| 12 | Next.js App Router: Server vs Client Components, the caching layers, streaming, Server Actions |
| 13 | Perf: Core Web Vitals, bundle analysis, code splitting. **Apply all of it to P1.** Measure before/after. |
 
Week 13 gives you an interview story: *"I cut LCP from 3.2s to 1.1s on my RAG app by moving X to a Server Component and streaming Y."* That sentence is worth more than 200 LeetCode problems.
 
---
 
# 🚪 Q1 GATE — Sunday 12 October 2026
 
**DSA**
- [ ] Recursion, backtracking, linked lists, trees: solid from blank
- [ ] Scaler DSA 4 attended fully, **all assignments ≥90%**
- [ ] Every contest attempted, **zero 0/100s**
- [ ] Both pending mock interviews completed
- [ ] ~120 problems solved *honestly* (2/day × 60 days)
**Depth**
- [ ] Can implement Promise, debounce, throttle, deepClone, curry, bind, EventEmitter from blank
- [ ] Can explain the event loop, closures, `this`, and prototypes to a skeptic
- [ ] Can explain React reconciliation and Server vs Client Components
**Ship**
- [ ] **P1 deployed, public URL, README, architecture diagram, eval suite with real numbers**
**Meta**
- [ ] 80+ daily logs in the GitHub repo
- [ ] Zero days of disappearing
---
 
# THE QUARTERLY GATES (the whole year)
 
| Gate | Date | What must be true |
|---|---|---|
| **Q1** | 12 Oct 2026 | Recursion/trees dead · JS internals owned · **P1 live** · DSA 4 on track |
| **Q2** | 11 Jan 2027 | DSA 4.2 + Databases/SQL done · LLD 1–2 done · Node/backend depth · **P2 started** · Resume rewritten |
| **Q3** | 12 Apr 2027 | LLD 3 + **High Level Design** done · **P2 live** · Docker/CI-CD · Referral network built · Mock interviews weekly |
| **Q4** | 12 Jul 2027 | **P3 live with real users** · Scaler capstone done · **Interviewing actively, offers in hand** |
 
**Q4 target: 30–45 LPA, product company, senior/SDE-2+ title.** FAANG loops open, and you walk in unafraid.
 
---
 
# TRACKING — Your GitHub
 
**Yes, GitHub. It is your tracker AND your evidence.** A hiring manager who sees 300 days of commits does not care that you were "Associate" at an agency.
 
Create one public repo today: **`ai-fullstack-transformation`**
 
```
ai-fullstack-transformation/
├── README.md              ← the public face: your mission, tracks, live project links
├── logs/
│   └── 2026-07-14.md      ← ONE FILE PER DAY. Non-negotiable.
├── dsa/
│   ├── recursion/         ← your solutions, in Python, with your own comments
│   ├── backtracking/
│   ├── linked-lists/
│   ├── trees/
│   └── spaced-repetition.md   ← problem | first solved | re-solve dates | status
├── notes/
│   ├── javascript/
│   │   ├── event-loop.md      ← written in YOUR words
│   │   ├── closures.md
│   │   └── prototypes.md
│   ├── react/
│   ├── node/
│   └── ai-engineering/
└── projects/
    ├── p1-ask-my-docs/    ← (or separate repo, linked)
    ├── p2-agent/
    └── p3-yours/
```
 
**Daily log template** — `logs/2026-07-14.md`:
```markdown
# 14 Jul 2026 · Day 1
 
## Block 1 — DSA (1.5 hr)
- Solved: Factorial, Fibonacci, Sum of N, Reverse string
- Solved WITHOUT help: 3/4
- Looked at solution for: Reverse string (recursive) — then re-solved from blank ✅
- What I didn't understand: how to see the base case immediately
 
## Block 2 — Depth (2 hr)
- Execution context, hoisting, TDZ
- Built: counter() with closure
 
## Block 3 — Log
- Commits: 4
- Honest self-rating (1–5): 4
- What broke: got frustrated at ~40 min, wanted to look things up
 
## Tomorrow
- Recursion on arrays
```
 
**The commit rule:** every day you study, you commit. **The green squares are the proof that the process defect is fixed.** In 12 months that grid IS your resume.
 
**Send me the log daily.** I'll read it and tell you the truth.
 
---
 
## THE THREE FAILURE MODES (and how each dies)
 
1. **"Let me restart from the beginning first."** → Dead. You start at recursion on 14 July.
2. **"I'll just peek at the solution, I'm short on time."** → Dead. The 25-min timer + re-solve-from-blank rule.
3. **"I'll catch up on the log/assignments this weekend."** → Dead. Same-day or it didn't happen.
Every one of these has ended a previous attempt. Naming them is how they stop being invisible.
 
---
 
*Start Block 1 today. Factorial. Blank file. Draw the stack.*