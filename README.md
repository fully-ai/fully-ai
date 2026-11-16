# fully-ai

Software engineering workspace focused on self-hosted infrastructure, security tooling, network diagnostics, and local AI systems across Python, Go, TypeScript, and Rust.

## Technical Focus

- Self-hosted web services and real-time communication systems
- Network packet analysis, protocol verification, and host observability
- Applied cryptography, static security analysis, and CI/CD automation
- Local LLM orchestration and hybrid document retrieval

## Projects

### AI & Knowledge Tooling
- **[localai-studio](https://github.com/fully-ai/localai-studio)** — Self-hosted web workspace and FastAPI/SSE gateway for managing local Ollama models, conversation history, system prompts, and vision/text attachments. (`Python`, `FastAPI`, `SQLite`)
- **[documind](https://github.com/fully-ai/documind)** — Local PDF and text document indexer with hybrid Ollama dense embedding and TF-IDF cosine search plus source-cited RAG. (`Python`, `FastAPI`, `pypdf`, `SQLite`)

### Security & Networking
- **[vaultdrop](https://github.com/fully-ai/vaultdrop)** — Encrypted file sharing service using envelope AES-256-GCM encryption, HKDF-SHA256 key derivation, expiring share links, quotas, and download audit logs. (`Python`, `cryptography`, `FastAPI`)
- **[devguard](https://github.com/fully-ai/devguard)** — Extensible repository analyzer performing secret detection, Python AST security checks, container/config audits, and dependency hygiene scans. (`Python`, `AST`, `CLI`)
- **[netscope](https://github.com/fully-ai/netscope)** — Pure-Rust PCAP traffic analyzer, L2–L7 protocol dissector (ARP, IPv4/IPv6, TCP, UDP, DNS), session tracker, and JSON/CSV/DOT/HTML exporter. (`Rust`)
- **[proxylab](https://github.com/fully-ai/proxylab)** — Concurrent HTTP, HTTPS, and SOCKS5 proxy checker with token-bucket rate limiting, anonymity classification, and web dashboard. (`Go`)

### Infrastructure, Real-Time & Productivity
- **[hostwatch](https://github.com/fully-ai/hostwatch)** — Cross-platform Linux and Windows agent-server system monitor tracking CPU, memory, disk, network counters, and threshold alerts. (`Go`)
- **[logsentry](https://github.com/fully-ai/logsentry)** — Multi-format log ingestion engine (JSON, Nginx/Apache, Syslog, generic) with real-time tailing, statistical error-spike anomaly detection, and webhook alerts. (`Go`)
- **[koral-chat](https://github.com/fully-ai/koral-chat)** — Self-hosted real-time chat platform over WebSockets with scrypt/JWT authentication, file sharing, and moderation controls. (`TypeScript`, `Express`, `WebSocket`, `SQLite`)
- **[taskforge](https://github.com/fully-ai/taskforge)** — Self-hosted Kanban project and task tracker featuring versioned SQLite migrations, labels, priorities, activity history, and assignment notifications. (`TypeScript`, `Express`, `SQLite`)
