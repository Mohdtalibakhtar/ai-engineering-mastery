# Six-Month Curriculum

This programme develops a Senior AI Engineer / AI Systems Engineer profile for top technology companies. The intended specialisation is **AI Systems Engineering**, supported by strong software engineering and distributed-systems fundamentals.

## Preparation allocation

| Priority | Track | Time allocation | Why it matters |
|---|---|---:|---|
| 1 | AI Systems Engineering | 30% | Primary differentiator and specialisation |
| 2 | Distributed Systems & System Design | 25% | Biggest identified engineering-depth gap |
| 3 | Data Structures & Algorithms | 20% | Coding-interview critical |
| 4 | ML Fundamentals & PyTorch | 15% | Preserve model and training depth |
| 5 | Production Infrastructure & MLOps | 10% | Operate systems reliably in production |

These percentages are allocations of preparation time, not estimates of how companies weight interviews. DSA is practised continuously.

## Priority 1 — AI Systems Engineering (30%)
**Outcome:** Engineer the full AI execution lifecycle, not merely integrate model APIs.

### 1. LLM internals
- Tokenisation and context windows.
- Embeddings and positional information.
- Transformer architecture, self-attention (Q/K/V), masking and multi-head attention.
- Transformer blocks, residual connections, normalisation and next-token prediction.
- Implement a small attention/Transformer component in PyTorch.

### 2. Inference engineering — a key differentiator
- Prefill vs decode and autoregressive generation.
- KV cache and GPU memory utilisation.
- Batching and continuous batching.
- Time-to-first-token (TTFT), inter-token latency, throughput and tail latency.
- Quantisation, speculative decoding and model serving.
- Multi-model serving and efficient routing.
- Benchmark workloads and explain quality/latency/cost trade-offs.
- Understand inference architecture first; CUDA kernel engineering is not an initial prerequisite.

### 3. Advanced RAG
- Ingestion, parsing, chunking and metadata design.
- Dense, sparse and hybrid retrieval; BM25.
- Query rewriting, filters, reranking and context assembly.
- Graph RAG and knowledge-graph retrieval.
- Retrieval evaluation: recall@k, precision@k, MRR/nDCG; answer quality and faithfulness.

### 4. Agent systems
- Planning, tool calling and orchestration.
- State, memory and context management.
- Workflow graphs vs open-ended agents.
- Durable execution, checkpoints and recovery.
- Permissions, human-in-the-loop approvals and multi-agent coordination.
- Retries, idempotency and safe tool execution.

### 5. Evaluation engineering
- Dataset management and test-case design.
- Offline and online evaluations.
- Task, step and trajectory evaluation.
- Graders, benchmarks and LLM-as-a-judge limitations.
- Human spot checks, regression suites and experiment tracking.
- Cost, latency and failure analysis.

### 6. Reliability and safety
- Timeouts, bounded retries, backoff, circuit breakers and fallbacks.
- Partial failures and recovery.
- Hallucination measurement and guardrails.
- Prompt injection, data exfiltration and tool authorization.
- Tenant isolation, audit trails and observability.

### 7. Optimisation and fine-tuning
- Latency, throughput, token-cost optimisation and caching.
- Model routing, context budgets and capacity planning.
- Supervised fine-tuning (SFT).
- LoRA and QLoRA.
- Preference optimisation concepts and evaluation of fine-tuned models.

## Priority 2 — Distributed Systems & System Design (25%)
**Outcome:** Design systems that remain correct and available under concurrency, load and partial failure. This is a major identified development area.

Learn in this order:
1. Concurrency vs parallelism; processes and threads.
2. Async programming, event loops and non-blocking I/O.
3. Networking, HTTP/RPC and connection management.
4. Message queues: Kafka and RabbitMQ.
5. Delivery semantics, ordering, partitions, consumer groups and backpressure.
6. Redis and distributed caching.
7. Database indexing, transactions and isolation.
8. Replication, partitioning and consistency.
9. Horizontal scaling and load balancing.
10. Distributed locks, leases and coordination.
11. Fault tolerance, circuit breakers, retries and idempotency.
12. Observability and performance engineering.

### System-design exercises
For every design, explain architecture, APIs, data model, bottlenecks, trade-offs, failure scenarios, scaling strategies and operational metrics.
- Design ChatGPT.
- Design a distributed task execution engine.
- Design an LLM inference gateway.
- Design a multi-tenant RAG platform.
- Design an agent orchestration platform.
- Design a real-time streaming AI system.
- Design a distributed rate limiter.

## Priority 3 — Data Structures & Algorithms (20%)
**Outcome:** Solve coding interview problems independently under time pressure and explain complexity.

| Topic | Target |
|---|---|
| Arrays and strings | Strong |
| Hash maps and sets | Strong |
| Two pointers and sliding window | Strong |
| Binary search | Strong |
| Stacks, queues and linked lists | Strong |
| Trees and heaps / priority queues | Strong |
| Graphs, BFS and DFS | Strong |
| Dynamic programming | Intermediate to strong |

Practice:
- Start with easy problems, then progress to medium.
- Aim for 2 problems per day, 5 days per week when sustainable.
- Target 150–180 well-understood problems over six months, not a rushed problem count.
- Prioritise patterns over memorised solutions.
- Explain the approach and time/space complexity aloud.
- Use Python initially; there is no need to learn several languages for this plan.
- Keep a mistake log and revisit previously difficult patterns.

## Priority 4 — Machine Learning Fundamentals & PyTorch (15%)
**Outcome:** Retain enough ML depth to make informed modelling and engineering decisions; this is not a research-scientist track.

Revisit:
- Supervised and unsupervised learning.
- Bias-variance trade-off and regularisation.
- Gradient descent, backpropagation and loss functions.
- Embeddings and representation learning.
- CNNs, RNNs and Transformers.
- Model evaluation and experimentation.
- PyTorch model implementation.

**Required practical outcome:** Implement a small model in PyTorch, train it, evaluate it, inspect errors and optimise at least one aspect of the training or inference process.

## Priority 5 — Production Infrastructure & MLOps (10%)
**Outcome:** Deploy, observe, scale and operate AI services reliably.

Deepen:
- Linux and runtime fundamentals.
- Docker and containerisation.
- Kubernetes.
- CI/CD and deployment strategies.
- Distributed tracing.
- Prometheus, Grafana and OpenTelemetry.
- Model serving with vLLM.
- Autoscaling and load testing.
- Security, governance and operational reliability.

Learn through implementation, not certification collection.

## Six-month sequence

| Month | Main emphasis | Parallel practice |
|---|---|---|
| 1 | Transformer/LLM fundamentals; concurrency and async | DSA; ML refresh; start Agent Runtime |
| 2 | Inference; queues; database fundamentals | DSA; PyTorch implementation |
| 3 | RAG; reliability; Kafka/Redis; Docker/CI | DSA; system-design exercises |
| 4 | Agent runtime; evaluation; Kubernetes | DSA; fine-tuning concepts |
| 5 | Optimisation; observability; inference gateway | DSA; capstone benchmarks |
| 6 | Production architecture; portfolio and interviews | DSA mocks; project hardening |

Recalibrate this sequence after the baseline assessment. Do not attempt to master all five tracks simultaneously at equal depth.
