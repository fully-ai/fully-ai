# fully-ai

Software engineering workspace focused on self-hosted infrastructure, security tooling, network diagnostics, and local AI systems across Python, Go, TypeScript, and Rust.

## Technical Focus

- Self-hosted web applications and real-time communication services
- Network traffic dissection, proxy diagnostics, and cross-platform host observability
- Applied cryptography, repository security auditing, and CI/CD automation
- Local LLM orchestration and offline/hybrid document retrieval

## Projects

### AI & Knowledge Tooling
- **[localai-studio](https://github.com/fully-ai/localai-studio)** — Self-hosted web workspace and FastAPI/SSE gateway for Ollama model management, system prompt presets, conversation history, and text/vision attachments. (`Python`, `FastAPI`, `SQLite`)
- **[documind](https://github.com/fully-ai/documind)** — Local PDF and text document indexer with collections, query history, hybrid Ollama embedding + TF-IDF cosine search, and source-cited RAG. (`Python`, `FastAPI`, `pypdf`, `SQLite`)

### Security & Networking
- **[vaultdrop](https://github.com/fully-ai/vaultdrop)** — Encrypted file sharing platform using HKDF-SHA256 + AES-256-GCM envelope encryption, expiring/passcode share links, quotas, and download audit logs. (`Python`, `cryptography`, `FastAPI`)
- **[devguard](https://github.com/fully-ai/devguard)** — Extensible repository security analyzer performing secret/entropy detection, Python AST SAST, container/config audits, and manifest hygiene checks. (`Python`, `AST`, `CLI`)
- **[netscope](https://github.com/fully-ai/netscope)** — Pure-Rust PCAP traffic analyzer, L2–L7 dissector (802.1Q, ARP, IPv4/v6, TCP, UDP, ICMP, DNS), session tracker, HTTP explorer, and DOT/HTML/JSON/CSV exporter. (`Rust`)
- **[proxylab](https://github.com/fully-ai/proxylab)** — Concurrent HTTP, HTTPS, and SOCKS5 proxy verifier with token-bucket rate limiting, built-in echo judge, anonymity classification, and web dashboard. (`Go`)

### Infrastructure, Real-Time & Productivity
- **[hostwatch](https://github.com/fully-ai/hostwatch)** — Cross-platform Linux and Windows agent-server system monitor with rolling history, JSON state persistence, threshold/service alerts, and SVG sparklines. (`Go`)
- **[logsentry](https://github.com/fully-ai/logsentry)** — Multi-format log engine (JSON, Nginx/Apache, Syslog, generic) with real-time file tailing, z-score anomaly detection, webhook alerts, and gzip archiving. (`Go`)
- **[koral-chat](https://github.com/fully-ai/koral-chat)** — Self-hosted real-time chat platform over WebSockets with scrypt/JWT auth, rate limiting, file sharing, structured logging, and admin moderation. (`TypeScript`, `Express`, `WebSocket`, `SQLite`)
- **[taskforge](https://github.com/fully-ai/taskforge)** — Self-hosted Kanban project and task tracker featuring versioned SQLite migrations, labels, priorities, due dates, activity logs, and notifications. (`TypeScript`, `Express`, `SQLite`)
