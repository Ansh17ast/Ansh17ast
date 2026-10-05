# Ansh Singh Thakur

**Software Engineer | Backend & Distributed Systems | Python & Go | Applied AI**  
Sehore, India • [LinkedIn](https://www.linkedin.com/in/ansh-singh-thakur17/) • [Email](mailto:astrusher@gmail.com) • [GitHub](https://github.com/Ansh17ast)

---

### Engineering Profile

Computer Science undergraduate at VIT Bhopal University (Class of 2027) specializing in **backend architectures, distributed systems, and applied AI systems**. Experienced in building fault-tolerant Go systems with Raft consensus, worker leases, and chaos engineering, alongside production Python backend engines featuring hybrid information retrieval, real-time voice telephony webhooks, and deterministic validation pipelines.

---

### Core Technical Competencies

- **Languages:** Go, Python, SQL (SQLite, PostgreSQL fundamentals), C/C++, JavaScript
- **Backend & Distributed Systems:** HashiCorp Raft Consensus, Replicated State Machines (FSM), Worker Leases & Fencing Tokens, DAG Workflow Orchestration, gRPC & Protocol Buffers, FastAPI, RESTful APIs, Concurrency & Goroutines, Webhook Idempotency
- **Data & Applied AI:** Hybrid Information Retrieval (BM25 + Dense Vectors, Reciprocal Rank Fusion), Voice Agent Integration (OmniDimension STT/TTS), SQLite Analytical Querying, Pandas, NumPy, Scikit-learn, OpenCV
- **Reliability & Tooling:** Chaos Engineering (Fault Injection, Network Partitions), Prometheus, OpenTelemetry, Docker, BoltDB, Git, Linux/Bash, Pytest, GitHub Actions CI/CD

---

### Featured Systems & Projects

#### 1. [Distributed Fault-Tolerant Task Scheduler](https://github.com/Ansh17ast/distributed-task-scheduler)
*Go • HashiCorp Raft • BoltDB • gRPC • Protocol Buffers • Prometheus • OpenTelemetry • Chaos Testing*
- High-throughput distributed task scheduler built from scratch around a 3-node Raft consensus cluster ($Q=2$) with persistent BoltDB write logs.
- Worker-pull scheduling engine with clock-independent monotonic leases and dual-token fencing (`SessionID` + `LeaseEpoch`) to eliminate zombie-worker lease collisions.
- Directed Acyclic Graph (DAG) dependency promotion engine alongside Deficit Weighted Round Robin (DWRR) multi-tenant fairness.
- Hardened across 12 adversarial chaos testing scenarios (leader kills, minority network partitions, worker split-brain); benchmarked at **514 µs p95 Raft quorum commit** and **1,152 tasks/sec sustained execution** across 10,000 tasks with zero memory leaks.

#### 2. [Enterprise AI Analytics & Document Intelligence Copilot](https://github.com/Ansh17ast/enterprise-ai-copilot)
*Python • FastAPI • Hybrid RAG • BM25 • Vector Search • Reciprocal Rank Fusion (RRF) • SQLite • Streamlit • Pytest*
- Production-grade enterprise copilot combining hybrid document retrieval with deterministic SQL analytics to eliminate LLM calculation hallucination.
- Dual-channel retrieval engine fusing Okapi BM25 lexical ranking and dense semantic vector search via Reciprocal Rank Fusion ($k=60$), paired with strict refusal guards for out-of-domain queries.
- Read-only SQL analytical engine with AST/regex mutation protection, executing quantitative aggregations directly against structured datasets.
- Accompanied by automated benchmark evaluation suites demonstrating 100% retrieval hit rate @ 3 and sub-25ms local turnaround latency.

#### 3. [Voice E-Commerce AI Agent & Omnichannel Lead Engine](https://github.com/Ansh17ast/voice-ecommerce-ai-agent)
*Python • FastAPI • OmniDimension (STT/TTS) • Green API (WhatsApp) • n8n • Webhooks • Pytest*
- Full-duplex conversational voice outreach agent integrated with real-time omnichannel WhatsApp dispatch for e-commerce website qualification.
- Asynchronous FastAPI webhook ingestion engine processing mid-call intent classification (**HOT / WARM / COLD**) and post-call collateral delivery (architecture flow diagrams and executive summaries).
- Built-in deduplication and idempotency controls with in-flight concurrency locks blocking race conditions across duplicate webhook triggers.
- Deterministic heuristic context normalizer enforcing a zero-hallucination policy by strictly preserving prospect-stated facts and omitting unconfirmed data.

#### 4. [Smart Attendance System](https://github.com/Ansh17ast/Smart-Attendance-System)
*Python • OpenCV • face_recognition (HOG / 128D Embeddings) • SQLite • Pytest*
- Real-time biometric attendance tracker operating over video streams with automatic per-session deduplication.
- Extracts 128-dimensional facial feature vectors using dlib HOG models and performs Euclidean distance matching against enrolled local encodings.
- SQLite transactional database logging attendance events with timestamp records, session constraints, and duplicate-entry prevention.

#### 5. [Skill Gap Analyzer & Career Roadmap Engine](https://github.com/Ansh17ast/skill-gap-ai)
*Python • Flask • REST API • Pytest • HTML5 / Modern CSS*
- Deterministic skill taxonomy evaluation service analyzing user competencies against technical roles (Backend, Frontend, Data Analyst).
- Computes weighted readiness scores, identifies priority missing competencies across core, technical, and tool categories, and generates structured learning sequences.
- Backed by automated Pytest suites verifying role taxonomy validation, scoring bounds, and API contract conformance.

---

### Current Engineering Focus

- Raft log compaction optimizations and zero-downtime consensus cluster state transitions.
- Asynchronous event streaming and webhook idempotency patterns in distributed backend architectures.
- Low-latency hybrid retrieval and multi-agent coordination pipelines.
