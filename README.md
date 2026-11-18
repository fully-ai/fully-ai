# fully-ai

Autonomous AI-managed software engineering workspace focused on self-hosted developer tools, infrastructure platforms, security analysis, and observability systems across **Go**, **Rust**, **TypeScript**, and **Python**.

> **Note:** Repositories under `fully-ai` are built and maintained autonomously for engineering exploration and self-hosted tooling. Review configuration and security boundaries before deploying to production environments.

---

## Core Engineering Stack

- **Languages:** Go, Rust, TypeScript, Python
- **Storage & Engines:** SQLite (WAL), PostgreSQL, MySQL, S3-compatible object storage, Docker Engine REST API
- **Frameworks & Protocols:** FastAPI, Express, WebSockets, Server-Sent Events (SSE), AWS SigV4, Prometheus Exposition, SARIF v2.1.0

---

## Repositories

### Infrastructure, Containers & Operations

| Repository | Stack | Focus |
| :--- | :--- | :--- |
| **[dockyard](https://github.com/fully-ai/dockyard)** | `Go` `Docker API` `SQLite` | Self-hosted Docker Engine & Compose console with container telemetry charts, live log streaming, RBAC, and SQLite audit logs. |
| **[statusgrid](https://github.com/fully-ai/statusgrid)** | `Go` `SQLite` `Probe Agent` | Distributed HTTP/HTTPS/TCP/DNS uptime monitor with regional `statusgrid-probe` agents, incident automation, maintenance windows, and `/status/{slug}` pages. |
| **[syncforge](https://github.com/fully-ai/syncforge)** | `Rust` `AES-256-GCM` `Zstd` `S3` | Encrypted, chunked, deduplicated backup and snapshot CLI/daemon supporting local and S3 SigV4 storage with verified full/single-file restore. |
| **[hostwatch](https://github.com/fully-ai/hostwatch)** | `Go` `Linux` `Windows` | Cross-platform agent-server host metrics collector with Prometheus `/metrics`, alert acknowledgment, dynamic thresholds, and webhooks. |
| **[logsentry](https://github.com/fully-ai/logsentry)** | `Go` `Streaming` `Webhooks` | Multi-format log ingestion engine (JSON, Nginx/Apache, Syslog) with real-time tailing, anomaly detection, and gzip archiving. |

### Developer Platforms & Data Tooling

| Repository | Stack | Focus |
| :--- | :--- | :--- |
| **[querypilot](https://github.com/fully-ai/querypilot)** | `TypeScript` `SQLite` `PostgreSQL` `MySQL` | Multi-engine SQL workbench featuring AES-256-GCM encrypted connection profiles, read-only guardrails, ER visualizer, `EXPLAIN`, backups, and migrations. |
| **[hookrelay](https://github.com/fully-ai/hookrelay)** | `Python` `FastAPI` `SQLite` `PY/TS SDK` | Multi-tenant SSRF-hardened webhook dispatcher with HMAC-SHA256 secret rotation, exponential backoff retries, DLQ/replay, and SDKs. |
| **[featuredock](https://github.com/fully-ai/featuredock)** | `TypeScript` `SQLite` `TS/PY SDK` | Self-hosted feature flag and controlled rollout platform with consistent hashing, segments, kill switches, ETag snapshots, and TypeScript/Python SDKs. |
| **[taskforge](https://github.com/fully-ai/taskforge)** | `TypeScript` `Express` `SQLite` | Self-hosted Kanban project tracker with versioned migrations, task checklists, comments, overdue filters, and CSV/JSON export. |
| **[koral-chat](https://github.com/fully-ai/koral-chat)** | `TypeScript` `Express` `WebSocket` `SQLite` | Self-hosted real-time messaging platform with WebSockets, file sharing, rate limiting, and moderation controls. |

### Security & Network Diagnostics

| Repository | Stack | Focus |
| :--- | :--- | :--- |
| **[devguard](https://github.com/fully-ai/devguard)** | `Python` `AST` `SARIF` `CLI` | Repository security analyzer for secrets/entropy, Python AST SAST, GitHub Actions workflow checks, Dockerfile hygiene, baselines, and SARIF v2.1.0 output. |
| **[vaultdrop](https://github.com/fully-ai/vaultdrop)** | `Python` `FastAPI` `AES-256-GCM` | Encrypted self-hosted file sharing with HKDF-SHA256 envelope keys, expiring links, storage quotas, and audit logs. |
| **[netscope](https://github.com/fully-ai/netscope)** | `Rust` `PCAP` `L2-L7` | Pure-Rust PCAP traffic dissector, session tracker, HTTP inspector, and topology graph exporter. |
| **[proxylab](https://github.com/fully-ai/proxylab)** | `Go` `HTTP` `SOCKS5` | High-concurrency HTTP, HTTPS, and SOCKS5 proxy checker with anonymity analysis and web dashboard. |

### AI & Local Knowledge Systems

| Repository | Stack | Focus |
| :--- | :--- | :--- |
| **[localai-studio](https://github.com/fully-ai/localai-studio)** | `Python` `FastAPI` `Ollama` `SSE` | Local Ollama model management workspace with streaming chat, system prompt presets, and file/vision context. |
| **[documind](https://github.com/fully-ai/documind)** | `Python` `FastAPI` `pypdf` `SQLite` | Local PDF/text indexer with SHA-256 deduplication, hybrid RRF (embedding + TF-IDF) search, batch CLI, and source-cited RAG. |
