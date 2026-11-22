# Six-Month Curriculum

Five parallel tracks. AI Systems Engineering is the primary specialisation; DSA runs continuously.

## Priority 1 — AI Systems Engineering
**Outcome:** Design, implement and operate production AI systems, not merely call model APIs.
1. **Transformer and LLM internals:** tokenisation, embeddings, positional information, self-attention (Q/K/V), masking, multi-head attention, transformer blocks, residuals, normalisation, next-token prediction. Build a small language-model component in PyTorch.
2. **Inference engineering:** prefill vs decode, autoregressive generation, KV cache, batching and continuous batching, throughput/latency, quantisation, speculative decoding and model serving. Benchmark TTFT, inter-token latency and throughput.
3. **Advanced RAG:** ingestion, parsing, chunking, metadata, sparse/dense/hybrid retrieval, BM25, query rewriting, filtering, reranking, context assembly, graph retrieval. Measure recall@k, precision@k, MRR/nDCG and answer faithfulness.
4. **Agent architecture:** tool calling, planning, state/context management, workflow graphs vs open-ended agents, durable execution, checkpoints, human approval, permissions, idempotency, retries and multi-agent coordination.
5. **Evaluation engineering:** datasets, task success, step/trajectory evaluation, graders, LLM-as-judge limitations, human spot checks, offline/online evaluation, regression suites, trace-level cost and latency.
6. **Reliability and security:** timeouts, bounded retries, backoff, circuit breakers, fallbacks, partial failure/recovery, prompt injection, data exfiltration, tool authorization, tenant isolation, audit trails, logs/metrics/traces.
7. **Optimisation:** model routing, quality/cost/latency trade-offs, exact and semantic caching, token budgets, context compression, load testing and capacity planning.
8. **Production AI architecture:** multi-tenant design, APIs/service boundaries, deployment/versioning, observability, governance, SLOs, rollbacks and operational ownership.

## Priority 2 — Distributed Systems & System Design
**Outcome:** Design systems that remain correct and available under concurrency, load and partial failure.
1. Processes, threads, async I/O; concurrency vs parallelism.
2. Networking, HTTP/RPC, API design and connection management.
3. Timeouts, retries, backoff, idempotency and rate limiting.
4. Queues and event-driven systems; Kafka/RabbitMQ concepts.
5. Delivery semantics, ordering, partitions, consumer groups and backpressure.
6. Redis, caching strategies, invalidation and stampede prevention.
7. Relational database internals: indexes, transactions and isolation.
8. Replication, partitioning, consistency and coordination.
9. Distributed locks, leases, sagas and transactional outbox.
10. Load balancing, circuit breakers, bulkheads and graceful degradation.
11. Observability, capacity planning and failure analysis.
12. Design exercises: task queue, notification service, chat service, inference gateway and RAG platform.

## Priority 3 — Data Structures & Algorithms
**Outcome:** Solve coding interview problems accurately under time constraints and explain complexity. Run 4–5 days/week throughout.
1. Complexity, arrays, strings, hash maps and sets.
2. Two pointers, sliding window and prefix sums.
3. Stacks, queues, linked lists and binary search.
4. Trees, heaps, priority queues and tries.
5. Graphs: BFS, DFS, topological sort and union-find.
6. Intervals, greedy algorithms and backtracking.
7. Dynamic programming: state, transitions, memoisation and tabulation.
8. Timed mixed practice, code quality and mock interviews.

Target 150–180 well-understood problems as a guide, not a vanity metric. Maintain a mistake log and revisit patterns.

## Priority 4 — Machine Learning & PyTorch
1. Supervised/unsupervised learning, train/validation/test and data leakage.
2. Bias-variance, regularisation, loss functions and optimisation.
3. Metrics, calibration, imbalanced data and error analysis.
4. Neural networks, backpropagation and gradient descent.
5. PyTorch tensors, autograd, modules, dataloaders and training loops.
6. Embeddings, representation learning and sequence models.
7. Transformer implementation and fine-tuning concepts.
8. SFT, LoRA/QLoRA and experiment design.
9. Reproducibility, evaluation and model comparison.

## Priority 5 — Production Infrastructure & MLOps
1. Linux, shell, processes, networking and environment management.
2. Docker images, containers, volumes, networks and Compose.
3. Testing, CI/CD, canaries, deployment and rollback.
4. Cloud fundamentals: identity, networking, compute, storage and secrets.
5. Kubernetes: pods, deployments, services, config, probes and autoscaling.
6. Model serving, GPU-aware deployment and resource scheduling.
7. OpenTelemetry, structured logs, metrics and distributed traces.
8. Prometheus/Grafana, load testing, SLOs and incident response.
9. Security, supply-chain hygiene and cost management.

## Suggested six-month sequence
| Month | Primary emphasis | Parallel practice |
|---|---|---|
| 1 | Transformer/LLM fundamentals; async/concurrency | DSA; ML refresh |
| 2 | Inference; queues and databases | DSA; PyTorch implementation |
| 3 | RAG; reliability; Docker/CI | DSA; distributed system design |
| 4 | Agent runtime; evaluation; Kubernetes | DSA; fine-tuning concepts |
| 5 | Optimisation; observability; system design | DSA; capstone benchmarks |
| 6 | Production architecture; portfolio/interviews | DSA mocks; project hardening |

Adjust after baseline assessment and actual weekly capacity.
