# Baseline Technical Assessment — AI Systems Engineer

This is a diagnostic, not a judgement. It is concept-first and interactive. Ask one question at a time, wait for the learner's attempt, and probe the same concept before moving on. Do not require coding syntax as the first test.

## A. AI systems architecture and LLM internals
1. Trace an LLM request from user input through tokenisation, model execution and generated response.
2. Explain the Transformer attention mechanism and the roles of Q, K and V.
3. Explain prefill, decode and KV cache, including the main performance constraints.
4. Distinguish model limitations from application/system design failures.

## B. RAG and knowledge systems
1. Design a RAG pipeline from source ingestion to grounded answer.
2. Diagnose retrieval failure versus generation failure.
3. Select retrieval and answer-quality metrics for a production use case.
4. Explain freshness, access control and tenant isolation.

## C. Agentic systems and evaluation
1. Compare a deterministic workflow with an open-ended agent.
2. Design durable execution and recovery after a worker crash.
3. Explain tool-call safety, idempotency and approval boundaries.
4. Design an evaluation strategy for multi-step agent tasks.

## D. Distributed systems and reliability
1. Explain concurrency, parallelism, async execution and blocking I/O conceptually.
2. Explain duplicate message delivery and idempotent processing.
3. Analyse a timeout where a downstream side effect may have succeeded.
4. Explain backpressure, retries, circuit breakers and graceful degradation.

## E. Production infrastructure and observability
1. Explain the request lifecycle across an AI service, retrieval store, tool service and model provider.
2. Design tracing and metrics to diagnose p95/p99 latency.
3. Explain safe deployment, rollback and capacity management.
4. Identify key security risks in a tool-using RAG/agent system.

## F. Supporting engineering foundations
1. Discuss a suitable data model and transaction boundary for a multi-step task.
2. Solve a representative DSA problem and explain complexity.
3. Explain a relevant ML concept and its effect on model/system behaviour.
4. Demonstrate practical Python/PyTorch implementation depth where required.

## Scoring
Score each area 0–4 based on evidence: 0 unable; 1 partial familiarity; 2 sound basics but weak depth/trade-offs; 3 independent, technically sound reasoning; 4 rigorous first-principles explanation, sound architecture, failure analysis and implementation evidence where appropriate. Record demonstrated evidence and remediation in PROGRESS.md. Do not infer capability from confidence alone.
