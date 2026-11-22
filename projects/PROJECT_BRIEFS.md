# Engineering Project Briefs

Build progressively; prioritise measurable milestones over broad feature lists.

## 1. Distributed Agent Runtime
**Goal:** Durable execution platform for multi-step tool-using tasks.
- API to submit and inspect tasks.
- Persistent task state and queue-backed workers.
- Timeouts, bounded retries and failure classification.
- Idempotency and duplicate-delivery handling.
- Checkpointing and recovery after worker/process failure.
- Tool permissions and human approval boundaries.
- Trace IDs, structured logs and metrics.
- Failure-injection and concurrency tests.

**Evidence:** architecture diagram/decision records; duplicate-delivery and crash-recovery tests; load-test throughput, p95 latency and queue delay; failure report and demo.

## 2. LLM Inference Gateway
**Goal:** Gateway routing requests across model providers or local serving backends.
- Unified request/response schema and provider adapters.
- Model routing policy with explicit fallback conditions.
- Per-user rate limits and token budgets.
- Timeouts, bounded retries and circuit breaking.
- Cost, latency, token and error telemetry.
- Load tests using documented workload profiles.
- Optional caching with correctness and privacy boundaries.

**Evidence:** p50/p95 latency, throughput, error rate and cost per workload; routing trade-off analysis; tenant isolation/security notes.

## 3. TraceCheck Evaluation Platform
**Goal:** Evolve existing TraceCheck rather than create a duplicate.
- Versioned evaluation datasets and test cases.
- Step-level and trajectory-level assertions.
- Retrieval metrics where relevant.
- LLM judge rubric with human spot checks and limitations.
- Regression comparison across versions.
- Cost, latency and failure analysis.
- CI integration and reproducible runs.

**Evidence:** reproducible evaluation report; a real regression detected; judge reliability analysis and known limitations.

## Portfolio safety
Do not publish employer code, customer information, credentials, internal prompts or confidential architecture. Reimplement generic patterns independently and disclose only authorised information.
