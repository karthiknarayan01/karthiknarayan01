# Karthik Narayan

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/C++17-00599C?style=flat&logo=cplusplus&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Ollama-000000?style=flat&logo=ollama&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" height="22"/>
</p>

---

Software engineer working on AI agents and distributed systems. I build agents from the
ground up, measure them with evals, and care about what happens under the hood: inference,
storage, and how systems stay correct when parts of them fail.

---

### What I work on

**AI agents, built and measured.** I write the agent loop myself, without a framework, and
judge it against an eval set.

**Inference.** Why one model call takes a second and another takes thirty. Prefill, KV caches,
batching, and getting open models to run well on everyday hardware.

**Distributed systems and storage.** Replication, gossip, CRDTs, append-only logs,
crash recovery, and database internals: how a planner picks a plan, and how a system keeps its
data correct when a node dies halfway through a write.

---

### Selected projects

**[AskVisa](https://github.com/karthiknarayan01/AskVisa)**
An AI assistant for US immigration questions, from visas and status to green cards. It checks
the regulations, Department of Labor data and your dates before it answers, shows every lookup
it makes, and runs free on your own computer. Comes with eval suites for tool choice, date math
and reasoning.

**[Shellmate](https://github.com/karthiknarayan01/Shellmate)**
A crash-safe agent runtime written from scratch in Python. Every step goes into an append-only
SQLite log, so a session killed mid-turn resumes without repeating a tool's side effects.
Approvals for risky tools, context compaction, and Claude, DeepSeek or local Qwen models.

**[flyio_distributed_systems_challenges](https://github.com/karthiknarayan01/flyio_distributed_systems_challenges)**
Fly.io's Gossip Glomers in Go, tested against the Maelstrom cluster simulator: unique IDs,
gossip broadcast, a CRDT counter, a replicated Kafka-style log, and transactions that stay
available through network partitions.

**[mnist-neural-network](https://github.com/karthiknarayan01/mnist-neural-network)**
A handwritten-digit recognizer built from scratch in NumPy, with no ML framework: backprop,
SGD, convolutions and pooling written out by hand. 99.35% test accuracy, with the architecture
chosen by screening candidates rather than guessing.

**[mnist-digit-recognizer](https://github.com/karthiknarayan01/mnist-digit-recognizer)**
Draw a digit and watch that network recognize it, live in your browser. The forward pass is
reimplemented in plain TypeScript, with no backend.
[Try it](https://mnist-digit-recognizer-coral.vercel.app).
