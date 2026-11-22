# Six-Month Curriculum — AI Systems Engineer Track

This programme prepares the learner for Senior AI Engineer / AI Systems Engineer roles, with a specialisation in production AI systems, LLM infrastructure, agentic systems, evaluation and reliability. The longer-term progression is toward Staff / Principal engineering.

## Target engineering profile

An AI Systems Engineer can:
- Explain how modern LLMs work, including the mechanics and constraints of inference.
- Design end-to-end AI applications and platforms, not just prompts or API integrations.
- Build reliable RAG and agentic systems with durable execution, evaluation and security.
- Reason about distributed systems, data, queues, concurrency, latency and failure.
- Measure quality, reliability, cost and performance using defensible engineering methods.
- Operate production AI services and communicate architecture trade-offs clearly.

## Preparation allocation

| Priority | Track | Time allocation | Role in the programme |
|---|---|---:|---|
| 1 | AI Systems Engineering | 40% | Core specialisation and primary differentiator |
| 2 | Distributed Systems & System Design | 25% | Foundations for correctness, scale and resilience |
| 3 | Production Infrastructure & MLOps | 15% | Deploy, observe and operate AI systems |
| 4 | Data Structures & Algorithms | 10% | Targeted coding-interview readiness |
| 5 | ML Fundamentals & PyTorch | 10% | Model literacy and implementation depth |

These are preparation allocations, not estimates of interview weighting. Coding remains important, but basic syntax drills are not the centre of the programme. Use coding to prove concepts, build systems, test hypotheses and prepare for relevant interviews.

## Priority 1 — AI Systems Engineering (40%)

**Outcome:** Design and operate the full AI execution lifecycle, from model request to measurable production outcome.

### 1. LLM foundations and internals
- Tokenisation, token IDs, context windows and token budgets.
- Embeddings, positional information and representation spaces.
- Transformer architecture: attention, Q/K/V, masking and multi-head attention.
- Transformer blocks, residual connections, normalisation and feed-forward layers.
- Next-token prediction, decoding strategies and model behaviour.
- Understand tensor shapes and the data flow through a Transformer.
- Implement or inspect a small attention/Transformer component when it helps validate understanding.

### 2. Inference engineering
- Request lifecycle: tokenisation, prefill, decode and detokenisation.
- Autoregressive generation and why decode is sequential.
- KV cache mechanics, memory growth and cache trade-offs.
- GPU memory: weights, activations, KV cache and temporary buffers.
- Compute-bound vs memory-bandwidth-bound workloads.
- Batching, continuous batching, scheduling and admission control.
- TTFT, inter-token latency, throughput, queueing delay and tail latency.
- Quantisation, speculative decoding, prefix caching and model serving.
- Serving architectures, multi-model routing and capacity planning.
- Benchmark workloads and explain quality/latency/cost trade-offs.
- CUDA kernel engineering is optional enrichment, not an initial prerequisite.

### 3. RAG and knowledge systems
- Ingestion architecture, parsing, normalisation, chunking and metadata.
- Dense, sparse and hybrid retrieval; BM25 and embedding search.
- Query rewriting, filters, reranking, context assembly and citations.
- Graph RAG and knowledge-graph retrieval; when graph structure adds value.
- Retrieval vs generation failure diagnosis.
- Retrieval evaluation: recall@k, precision@k, MRR and nDCG.
- Answer relevance, faithfulness, groundedness and task success.
- Freshness, access control, tenant isolation and data lifecycle.

### 4. Agentic systems and orchestration
- Tool calling, planning, routing and control flow.
- Workflows vs autonomous/open-ended agents.
- State, memory, context management and conversation compaction.
- Agent runtime architecture and execution state machines.
- Durable execution, checkpoints, recovery and replay.
- Queues, worker pools, concurrency limits and scheduling.
- Retries, idempotency, timeouts, cancellation and compensation.
- Tool permissions, human approval and safe side effects.
- Multi-agent coordination, delegation and shared-state hazards.
- Streaming, interruption and long-running tasks.

### 5. Evaluation engineering
- Define task success and operational quality before selecting metrics.
- Dataset design, coverage, versioning and representative test cases.
- Retrieval, answer, tool-call, step and trajectory evaluation.
- Deterministic assertions, programmatic graders and LLM-as-judge.
- Judge calibration, bias, variance and limitations.
- Human review and adjudication.
- Offline evaluation, online monitoring, canaries and regression gates.
- Trace analysis, error taxonomies and root-cause diagnosis.
- Cost, latency, reliability and quality measurement together.

### 6. Reliability, security and governance
- Timeouts, bounded retries, exponential backoff, jitter and circuit breakers.
- Partial failures, fallbacks, bulkheads and graceful degradation.
- Prompt injection, indirect injection and untrusted retrieved content.
- Tool authorisation, least privilege and approval boundaries.
- Data exfiltration, secrets handling and sensitive-data controls.
- Tenant isolation, audit trails and policy enforcement.
- Observability across model, retrieval, tools, orchestration and infrastructure.
- SLOs, error budgets and incident response for AI applications.

### 7. Optimisation and adaptation
- Latency, throughput, token-cost and quality optimisation.
- Caching boundaries: semantic, response, prompt/prefix and retrieval caches.
- Model routing, context budgets and capacity planning.
- Prompt optimisation vs retrieval changes vs model changes.
- SFT, LoRA and QLoRA: use cases, constraints and evaluation.
- Preference optimisation concepts and when fine-tuning is justified.

## Priority 2 — Distributed Systems & System Design (25%)

**Outcome:** Design systems that remain correct under concurrency, load, retries and partial failure.

Learn in this order:
1. Processes, threads, concurrency, parallelism and scheduling.
2. Async runtimes, event loops, blocking I/O and cancellation.
3. Networking, HTTP/RPC, connection pools and timeouts.
4. Queues and event streaming: Kafka and RabbitMQ.
5. Delivery semantics, duplicate delivery, ordering, partitions and consumer groups.
6. Backpressure, load shedding and admission control.
7. Redis, caching, consistency and distributed coordination.
8. Database indexes, transactions, isolation and connection management.
9. Replication, partitioning, consistency and data ownership.
10. Idempotency, deduplication, outbox/inbox patterns and sagas.
11. Horizontal scaling, load balancing and capacity estimation.
12. Fault tolerance, observability and performance engineering.

### System-design exercises
For every design, explain requirements, APIs, data model, architecture, bottlenecks, failure scenarios, scaling, security, operational metrics and trade-offs.
- Design a ChatGPT-like serving platform.
- Design a distributed task execution engine.
- Design an LLM inference gateway.
- Design a multi-tenant RAG platform.
- Design a durable agent orchestration platform.
- Design a real-time streaming AI system.
- Design a distributed rate limiter.

## Priority 3 — Production Infrastructure & MLOps (15%)

**Outcome:** Deploy, observe, scale and operate AI services reliably.

- Linux processes, memory, filesystems, networking and resource limits.
- Containers, Docker images, networking and storage.
- Kubernetes primitives, scheduling, probes, autoscaling and deployments.
- CI/CD, release strategies, canaries and rollback.
- Distributed tracing with OpenTelemetry.
- Metrics and dashboards with Prometheus/Grafana.
- Structured logs, correlation IDs and trace context propagation.
- Model serving with vLLM or comparable serving systems.
- Load testing, capacity planning and performance diagnosis.
- Secrets, IAM, network boundaries and production governance.

## Priority 4 — Data Structures & Algorithms (10%)

**Outcome:** Maintain practical coding-interview readiness without displacing core systems learning.

Focus on reusable patterns:
- Arrays, strings, hash maps and sets.
- Two pointers, sliding window and binary search.
- Stacks, queues and linked lists.
- Trees, heaps and priority queues.
- Graph traversal: BFS and DFS.
- Dynamic programming fundamentals.
- Time/space complexity and clear problem explanation.

Practice consistently, typically 3–5 focused problems per week initially, increasing when interviews require it. Prioritise understanding, independent implementation and review of mistakes over raw problem count. Use Python.

## Priority 5 — ML Fundamentals & PyTorch (10%)

**Outcome:** Understand model behaviour and make sound decisions about model use, evaluation and adaptation.

- Supervised/unsupervised learning and representation learning.
- Bias-variance, regularisation, loss functions and optimisation.
- Gradient descent and backpropagation at a conceptual and mathematical level.
- Embeddings and neural network building blocks.
- CNNs, RNNs and Transformers at an architectural level.
- Model evaluation, calibration and dataset quality.
- PyTorch tensors, autograd, training and inference.
- Fine-tuning concepts and evaluation of adapted models.

Required practical outcome: implement or adapt a small model, train/evaluate it, inspect errors and explain the operational implications.

## Six-month sequence

| Month | Primary emphasis | Applied outcome |
|---|---|---|
| 1 | LLM/Transformer internals; AI system architecture; async and concurrency foundations | Explain end-to-end LLM request flow; architecture brief for an AI application |
| 2 | Inference engineering; GPU/KV-cache constraints; serving and queueing | Inference benchmark and performance analysis |
| 3 | Advanced RAG; retrieval evaluation; data and access-control design | Measured RAG pipeline with versioned evaluation dataset |
| 4 | Agent runtime; durable execution; distributed reliability and security | Working Distributed Agent Runtime with failure recovery |
| 5 | Evaluation engineering; observability; optimisation and model routing | TraceCheck evaluation platform improvements and LLM gateway |
| 6 | Production hardening; system design; portfolio and interview preparation | End-to-end capstone, architecture defence and interview simulations |

Distributed systems and infrastructure are threaded through all six months rather than postponed until their dedicated modules. DSA and ML are maintained as supporting tracks.

## Learning and assessment standard

For every major concept:
1. State the problem it solves and the assumptions it makes.
2. Explain the internal mechanism and relevant mathematics.
3. Trace data/control flow through the architecture.
4. Compare alternatives and articulate trade-offs.
5. Analyse failure modes, security and operational behaviour.
6. Implement a focused proof or production-relevant component where useful.
7. Test, measure and explain observed behaviour.
8. Defend the design verbally, as in a senior engineering review.

A concept is not mastered by recognising terminology or using a framework. Evidence must show independent explanation, reasoning, implementation where appropriate, and diagnosis under realistic constraints.
