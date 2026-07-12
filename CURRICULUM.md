# B.Tech Cyber Security — 4-Year Project Roadmap

A living map of project-based learning across the degree. Every topic is learned by building something real, not by reading theory in isolation. Six tracks run in parallel; each one deepens year over year, and later projects deliberately reuse or rebuild earlier ones rather than starting from zero.

**Stack across all 4 years:** VS Code, WSL (Ubuntu/Linux), Git/GitHub. Languages expand from Python-only in Year 1 to Python + C + Bash + SQL by Year 4.

---

## Track 1: Programming & Scripting → Secure Software Engineering

| Year | Focus | Flagship project |
|---|---|---|
| 1 | Python fundamentals, file I/O, regex, CLI tools | **SecuScan** — regex-based secret scanner ✅ |
| 2 | C basics, memory model, scripting for automation | Rewrite SecuScan's scan engine in C; add multithreaded directory walking |
| 3 | Secure coding practices, static analysis | Extend SecuScan with entropy-based key detection + `.gitignore`-aware skipping; package as a pip-installable CLI |
| 4 | Software security engineering, CI/CD integration | SecuScan as a GitHub Action / pre-commit hook — real pipeline integration, config file support, false-positive tuning |

## Track 2: Engineering Mathematics → Applied Cryptography

| Year | Focus | Flagship project |
|---|---|---|
| 1 | Discrete math, modular arithmetic | Caesar/Vigenère cipher tool from scratch |
| 2 | Number theory, probability | Small RSA key-pair generator + encrypt/decrypt demo |
| 3 | Cryptographic protocols | Implement Diffie-Hellman key exchange; break weak/custom ciphers |
| 4 | Applied crypto in systems | Build a minimal TLS-handshake simulator; audit a real library's crypto usage |

## Track 3: Digital Electronics → Systems & Protocol Security

| Year | Focus | Flagship project |
|---|---|---|
| 1 | Logic gates, binary | Logic gate simulator with a simple circuit description language |
| 2 | Binary/packet structure | Raw binary packet field parser |
| 3 | Network protocol internals | Custom packet sniffer/parser (Scapy or raw sockets) for a specific protocol |
| 4 | Hardware/firmware security | IoT/firmware binary analysis basics; UART/JTAG concepts on an emulator |

## Track 4: Data Structures & OOP → Secure Systems Design

| Year | Focus | Flagship project |
|---|---|---|
| 1 | Stacks, queues, custom classes | Stack-based undo system or queue-based task scheduler |
| 2 | OOP design, access control modeling | Custom file-permission model (RBAC-style class hierarchy) |
| 3 | Secure data structures | Build a rate-limiter / audit-log system with tamper-evident structure |
| 4 | Systems design | Design a small secure microservice (auth, logging, permissions) end to end |

## Track 5: Computer Architecture → Systems & Binary Security

| Year | Focus | Flagship project |
|---|---|---|
| 1 | CPU cache, memory buffers | Cache hit/miss simulator; bounded circular buffer with intentional overflow demo |
| 2 | Memory management, OS internals | Simple heap/stack visualizer; demonstrate a real buffer overflow in a sandboxed C program |
| 3 | Binary exploitation basics | Intro reverse engineering — disassemble and patch a simple binary |
| 4 | Exploit development / mitigation | Build (and then defeat) basic stack canaries / ASLR demo in a controlled environment |

## Track 6: Cyber Security Foundations → Offensive & Defensive Security

| Year | Focus | Flagship project |
|---|---|---|
| 1 | Log analysis, port scanning basics | Log analyzer flagging suspicious login patterns; basic TCP port scanner |
| 2 | Network security, web basics | Web app vulnerability scanner (SQLi/XSS detection on a deliberately vulnerable test app) |
| 3 | Offensive security, forensics | Small pentest toolkit; basic digital forensics (file carving, metadata analysis) |
| 4 | Advanced / capstone | Full red-team-style engagement report OR a defensive SOC-style monitoring dashboard — capstone integrates tools from all 6 tracks |

---

## How this file gets used

- Each entry is a **seed project**, not a fixed assignment — scope adjusts to what's actually being worked on at the time.
- When a project starts, it gets a roadmap in the Problem/Goal/Solution + day-by-day format, same as SecuScan's.
- When a project finishes, its row here gets a ✅ and a link to its repo.
- Later-year projects are expected to reuse earlier code where it makes sense (e.g., Year 2's SecuScan-in-C reuses the Year 1 pattern set) — the point is compounding, not starting over every year.

## Progress log

- ✅ **Year 1, Track 1:** SecuScan (Python secret scanner) — complete
