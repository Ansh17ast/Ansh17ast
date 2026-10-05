# Ansh Singh Thakur

**Software Engineer | Backend & Distributed Systems | Python & Go | Applied AI**  
Sehore, India • [LinkedIn](https://www.linkedin.com/in/ansh-singh-thakur17/) • [Email](mailto:astrusher@gmail.com) • [GitHub](https://github.com/Ansh17ast)

---

### Engineering Profile

Computer Science undergraduate at VIT Bhopal University (Class of 2027) focused on **backend architectures, distributed consensus, and systems reliability**. Experienced in engineering fault-tolerant Go systems using Raft consensus, worker leases, and chaos engineering, as well as production-ready Python backend pipelines with strict data validation, automated testing, and observability.

---

### Core Technical Competencies

- **Languages:** Go, Python, SQL (SQLite), C/C++, JavaScript
- **Distributed Systems & Backend:** HashiCorp Raft Consensus, Replicated State Machines (FSM), Worker Leases & Fencing Tokens, DAG Workflow Orchestration, gRPC & Protocol Buffers, RESTful APIs, Concurrency & Goroutines
- **Data & Applied AI:** Hybrid Information Retrieval (BM25 + Dense Vectors), OpenCV & Computer Vision Pipelines (128D Face Embeddings), SQLite, Scikit-learn, Pandas, NumPy
- **Reliability & Tooling:** Chaos Engineering (Fault Injection, Network Partitions), Prometheus, OpenTelemetry, Docker, BoltDB, Git, Linux/Bash, Pytest, GitHub Actions CI/CD

---

### Featured Systems & Projects

#### 1. [Distributed Fault-Tolerant Task Scheduler](https://github.com/Ansh17ast/distributed-task-scheduler)
*Go • HashiCorp Raft • BoltDB • gRPC • Protocol Buffers • Prometheus • OpenTelemetry • Chaos Testing*
- High-throughput distributed task scheduler built from scratch around a 3-node Raft consensus cluster ($Q=2$) with persistent BoltDB write logs.
- Worker-pull scheduling engine with clock-independent monotonic leases and dual-token fencing (`SessionID` + `LeaseEpoch`) to eliminate zombie-worker lease collisions.
- Directed Acyclic Graph (DAG) dependency promotion engine alongside Deficit Weighted Round Robin (DWRR) multi-tenant fairness.
- Hardened across 12 adversarial chaos testing scenarios (leader kills, minority network partitions, worker split-brain); benchmarked at **514 µs p95 Raft quorum commit** and **1,152 tasks/sec sustained execution** across 10,000 tasks with zero memory leaks.

#### 2. [Smart Attendance System](https://github.com/Ansh17ast/Smart-Attendance-System)
*Python • OpenCV • face_recognition (HOG / 128D Embeddings) • SQLite • Pytest*
- Real-time biometric attendance tracker operating over webcam video streams with automatic per-session deduplication.
- Extracts 128-dimensional facial feature vectors using dlib HOG models and performs Euclidean distance matching against enrolled local encodings.
- SQLite transactional database logging attendance events with timestamp records, session constraints, and duplicate-entry prevention.

#### 3. [Skill Gap Analyzer & Career Roadmap Engine](https://github.com/Ansh17ast/skill-gap-ai)
*Python • Flask • REST API • Pytest • HTML5 / Modern CSS*
- Deterministic skill taxonomy evaluation service analyzing user competencies against technical roles (Backend, Frontend, Data Analyst).
- Computes weighted readiness scores, identifies priority missing competencies across core, technical, and tool categories, and generates structured learning sequences.
- Backed by automated Pytest suites verifying role taxonomy validation, scoring bounds, and API contract conformance.

---

### Current Engineering Focus

- Raft log compaction optimizations and zero-downtime consensus cluster state transitions.
- Asynchronous event streaming and webhook idempotency patterns in distributed backend architectures.
