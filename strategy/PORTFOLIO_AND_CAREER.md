# Portfolio and Career Positioning

## Target identity
**Senior AI Systems Engineer** — specialisation in Applied AI, Distributed Systems and LLM Infrastructure.

Target senior-level roles first:
- Applied AI Engineer
- AI Software Engineer
- Machine Learning Engineer (with deeper ML preparation)
- AI Platform Engineer (after infrastructure preparation)
- LLM Systems Engineer

Staff / Principal AI Engineer or AI Systems Architect is a longer-term trajectory. Research Scientist is not the recommended immediate target.

## Three coherent engineering projects

### 1. Distributed Agent Runtime — highest priority
Build a platform where multiple agents can execute tasks concurrently.
- Durable task execution.
- Queue-based orchestration.
- State persistence.
- Retries and failure recovery.
- Tool execution and permissions.
- Distributed tracing.

**Evidence:** architecture and design decisions, duplicate-delivery tests, worker-crash recovery, concurrency tests, load-test results and a working demonstration.

### 2. LLM Inference Gateway
Build an intelligent model-serving layer.
- Multiple model providers.
- Request routing.
- Semantic caching.
- Rate limiting.
- Token and cost tracking.
- Load testing.
- Latency and throughput benchmarking.

**Evidence:** reproducible workload, p50/p95 latency, throughput, error rate, cost comparisons and documented routing trade-offs.

### 3. AI Evaluation Platform — evolve TraceCheck
Do not create a disconnected evaluation project from scratch. Evolve the existing TraceCheck project.
- Dataset management.
- Retrieval evaluation.
- Agent trajectory evaluation.
- LLM-as-a-judge with limitations and human spot checks.
- Regression testing.
- Cost and latency analysis.
- Experiment tracking.

**Evidence:** reproducible evaluation report, a detected regression, judge-quality analysis and CI integration.

## Use existing professional experience as evidence

### Zavmo — AI platform engineering
Potential case-study themes, subject to confidentiality and permission:
- Multi-agent architecture and orchestration.
- RAG and knowledge graphs.
- Real-time voice AI.
- Learning adaptation and personalisation.
- Automated evaluation.
- Engineering a complex AI product from architecture through production.

### Enterprise AI workflow engineering
Potential case-study themes, subject to confidentiality and permission:
- Unstructured data processing.
- Semantic product matching.
- Enterprise integrations.
- AI-powered estimation workflows.
- Human-in-the-loop architecture.
- Business-process automation.

## Metrics to collect
Never invent results. Establish baselines and measure improvements.

| Dimension | Example measurement |
|---|---|
| Accuracy | Product-matching accuracy |
| Performance | Average processing latency |
| Efficiency | Time saved per quotation |
| Reliability | Successful workflow completion rate |
| Cost | Cost per AI workflow |
| Adoption | Active users and workflow usage |

## Interview narrative
For every project or professional case study, be prepared to explain:
1. The user or business problem.
2. Requirements and constraints.
3. Architecture and alternatives considered.
4. Your personal contribution.
5. Failure modes and operational decisions.
6. Evidence and measured impact.
7. What you would change at 10× scale.
