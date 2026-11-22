# Baseline Technical Assessment

Complete without AI coding assistance. This is diagnostic, not a judgement. Record time, confidence and mistakes.

## A. Python and coding
1. Implement an LRU cache with O(1) average get/put.
2. Explain concurrency vs parallelism in Python.
3. Explain what happens when an async function calls blocking I/O.

## B. DSA
1. Solve one medium array/hash-map problem.
2. Solve one tree traversal problem.
3. Explain time and space complexity for both.

## C. Distributed systems
1. What can go wrong if a worker processes the same queue message twice?
2. Explain idempotency and how you would implement it for a payment-like operation.
3. What happens when a service times out but the downstream operation actually succeeded?

## D. AI systems
1. Explain a Transformer block and the role of Q, K and V.
2. Explain prefill, decode and KV cache.
3. Design a RAG evaluation dataset and choose metrics.
4. Explain how to recover a multi-step agent after a worker crash.

## E. ML fundamentals
1. Explain backpropagation and gradient descent.
2. Describe overfitting and three ways to address it.
3. Choose metrics for an imbalanced classification task and justify them.

## F. Production infrastructure
1. Explain the difference between a process, container and Kubernetes pod.
2. Describe how to observe p95 latency across a multi-service AI request.
3. Describe a safe deployment and rollback strategy.

## Scoring
Score each section 0–4: 0 unable; 1 partial familiarity; 2 basic explanation but weak implementation/trade-offs; 3 independently competent; 4 rigorous explanation, implementation and edge-case reasoning. Record evidence and remediation in PROGRESS.md.
