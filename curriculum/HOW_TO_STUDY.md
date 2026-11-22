# How to Study This Programme

This is an execution guide for turning the roadmap into demonstrated engineering skill. Do not try to study all five priorities in equal depth at the same time.

## The learning loop for every topic
1. **Diagnose:** answer a few questions without notes to expose gaps.
2. **Learn:** study one concept from first principles. Understand the problem it solves, how it works internally and where it fails.
3. **Reconstruct:** explain the concept in your own words or draw its data/control flow without copying.
4. **Implement:** write a small working version or a focused experiment.
5. **Test and break:** add edge cases, inject failures, profile behaviour and inspect logs.
6. **Apply:** connect the concept to a realistic system-design or production scenario.
7. **Demonstrate:** complete an independent assignment and defend trade-offs.
8. **Record:** write a session note, update PROGRESS.md and set the next exact lesson in NEXT_SESSION.md.

A lesson is not complete because you watched a video or understood an explanation. It is complete when you can explain, implement, test and defend the idea independently.

## How to study each priority

### Priority 1 — AI Systems Engineering
Follow the roadmap sequence: LLM internals → inference → RAG → agents → evaluation → reliability/security → optimisation/fine-tuning.
- Start with a mechanism (for example, attention or KV caching), not a framework tutorial.
- Implement a small experiment in Python/PyTorch.
- Measure something: retrieval quality, TTFT, throughput, token cost, task success or failure rate.
- Apply the learning to the Distributed Agent Runtime, Inference Gateway or TraceCheck.
- Write a short design note explaining alternatives and trade-offs.

### Priority 2 — Distributed Systems & System Design
- Learn one primitive at a time: concurrency, queue, transaction, cache, replication, consistency or retry.
- Build a small reproduction (e.g. duplicate message delivery or worker crash recovery).
- Draw the sequence/data-flow diagram.
- Run a failure experiment and explain what guarantees the system does and does not provide.
- Complete one system-design prompt and defend bottlenecks, scaling and operational trade-offs.

### Priority 3 — Data Structures & Algorithms
- Practise consistently, ideally 2 problems/day on 5 days/week when sustainable.
- Attempt independently before reading hints or solutions.
- State brute force first, then derive the optimised pattern.
- Code in Python, test edge cases and explain time/space complexity aloud.
- Keep a mistake log; revisit missed problems after a delay.
- Track independent solves separately from problems solved after hints.

### Priority 4 — ML Fundamentals & PyTorch
- Refresh one concept, then derive or explain its mathematics and assumptions.
- Implement a small model/training loop in PyTorch.
- Track train/validation behaviour and choose suitable evaluation metrics.
- Inspect errors and run one controlled experiment changing a hyperparameter, regulariser or architecture choice.
- Document reproducibility and what the experiment does not prove.

### Priority 5 — Production Infrastructure & MLOps
- Pick one operational capability (Docker, Kubernetes, CI/CD, tracing, monitoring, serving or load testing).
- Deploy a small service or reproduce the capability locally.
- Add health checks, logs, metrics and traces where relevant.
- Test failure, rollback, scaling and security boundaries.
- Record operational evidence, not just configuration screenshots.

## How to use ChatGPT as your tutor
Use one focused conversation per module or substantial topic inside the ChatGPT Project AI Engineering Mastery. Start each new conversation with this prompt:

> Act as my rigorous AI engineering instructor. Continue my AI Engineering Mastery programme. Use the repository files curriculum/ROADMAP.md, curriculum/HOW_TO_STUDY.md, PROGRESS.md and NEXT_SESSION.md as the source of truth. First give me a short retrieval check based on the last completed lesson. Teach only the next incomplete lesson. Follow Diagnose → Explain → Implement → Test/Break → Apply → Demonstrate → Assess. Do not give me the full solution before I attempt the exercise. At the end, provide exact updates for PROGRESS.md and NEXT_SESSION.md, plus the next session prompt.

If the repository is not accessible in that conversation, attach or paste the relevant progress and handoff files rather than assuming the tutor knows your latest state.

## How to use GitHub
- Commit lesson notes, code, tests, design diagrams and benchmark results.
- Keep one folder or branch per substantial project; use pull requests for meaningful changes if helpful.
- Keep PROGRESS.md and NEXT_SESSION.md current after each learning session.
- Use issues for larger assignments and bugs; close them only when acceptance criteria are met.
- Never commit secrets, API keys, employer code, customer data or confidential information.

## What a good weekly output looks like
Each week should produce:
- A set of DSA attempts with a mistake log.
- One topic note written from memory.
- One runnable implementation or experiment with tests.
- One design exercise or architecture decision record.
- A progress update and next-week plan.

## Mastery standard
Use the 0–4 rubric in LEARNING_METHOD.md for conceptual understanding, independent implementation, testing/debugging, trade-off reasoning and interview explanation. Aim for at least 16/20 with no zero; repeat weak areas instead of rushing ahead.
